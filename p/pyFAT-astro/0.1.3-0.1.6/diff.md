# Comparing `tmp/pyFAT_astro-0.1.3.tar.gz` & `tmp/pyFAT_astro-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFAT_astro-0.1.3.tar", last modified: Tue Nov 14 14:46:07 2023, max compression
+gzip compressed data, was "pyFAT_astro-0.1.6.tar", last modified: Mon Apr  8 08:56:39 2024, max compression
```

## Comparing `pyFAT_astro-0.1.3.tar` & `pyFAT_astro-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35202 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      498 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9854 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.826499 pyFAT_astro-0.1.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/bin/pyFAT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.826499 pyFAT_astro-0.1.3/pyFAT_astro/
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/FAT_Galaxy_Loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.830499 pyFAT_astro-0.1.3/pyFAT_astro/Installation_Check/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7143 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Installation_Check/ModelInput.def
--rwxr-xr-x   0 runner    (1001) docker     (127)  2825280 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Installation_Check/NGC_2903.fits
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Installation_Check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/pyFAT_astro/Support/
--rwxr-xr-x   0 runner    (1001) docker     (127)        1 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28260 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/clean_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      547 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    48081 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/development_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1101 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/fat_errors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37013 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/fits_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   159007 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/modify_template.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    60419 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/read_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    66093 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/run_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   153457 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/support_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15189 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/tirshaker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    72226 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Support/write_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/pyFAT_astro/Templates/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Templates/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Templates/sofia_template.par
--rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/Templates/template.def
--rwxr-xr-x   0 runner    (1001) docker     (127)     1896 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/pyFAT_astro/config/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/config/FAT_Input_Catalogue.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6462 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/config/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14442 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/pyFAT_astro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:46:07.826499 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-14 14:46:07.000000 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-11-14 14:46:07.000000 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:46:07.000000 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-14 14:46:07.000000 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-14 14:46:07.000000 pyFAT_astro-0.1.3/pyFAT_astro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 14:46:07.834499 pyFAT_astro-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1501 2023-11-14 14:45:57.000000 pyFAT_astro-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35202 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9854 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.561919 pyFAT_astro-0.1.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/bin/pyFAT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.561919 pyFAT_astro-0.1.6/pyFAT_astro/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15683 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/FAT_Galaxy_Loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.565919 pyFAT_astro-0.1.6/pyFAT_astro/Installation_Check/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8970 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Installation_Check/ModelInput.def
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2825280 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Installation_Check/NGC_2903.fits
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Installation_Check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/pyFAT_astro/Support/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        1 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31101 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/clean_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      528 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48081 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/development_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/fat_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28150 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/fits_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15455 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/log_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179156 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/modify_template.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64569 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/read_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    69603 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/run_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   155884 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/support_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    80090 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Support/write_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/pyFAT_astro/Templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Templates/TRM_errors_FAT.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Templates/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3082 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Templates/sofia_template.par
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/Templates/template.def
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2023 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/pyFAT_astro/config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/config/FAT_Input_Catalogue.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7117 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/config/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14593 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/pyFAT_astro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 08:56:39.000000 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-08 08:56:39.000000 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:56:39.000000 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 08:56:39.000000 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 08:56:39.000000 pyFAT_astro-0.1.6/pyFAT_astro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:56:39.569919 pyFAT_astro-0.1.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2024-04-08 08:56:34.000000 pyFAT_astro-0.1.6/setup.py
```

### Comparing `pyFAT_astro-0.1.3/LICENSE` & `pyFAT_astro-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/PKG-INFO` & `pyFAT_astro-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFAT_astro
-Version: 0.1.3
+Version: 0.1.6
 Summary: Development Status :: 4 - Beta
 Home-page: https://github.com/PeterKamphuis/pyFAT
 Author: P. Kamphuis
 Author-email: peterkamphuisastronomy@gmail.com
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -18,8 +18,11 @@
 Requires-Dist: numpy>=1.14
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: omegaconf>=2.2.2
 Requires-Dist: matplotlib
 Requires-Dist: future-fstrings
 Requires-Dist: psutil
+Requires-Dist: make-moments>=1.0.6
 Requires-Dist: importlib_resources>=3.3.0
+Requires-Dist: importlib_metadata
+Requires-Dist: TRM_errors>=0.0.5
```

### Comparing `pyFAT_astro-0.1.3/README.md` & `pyFAT_astro-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/FAT_Galaxy_Loop.py` & `pyFAT_astro-0.1.6/pyFAT_astro/FAT_Galaxy_Loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,44 +12,47 @@
 import pyFAT_astro.Support.read_functions as rf
 import pyFAT_astro.Support.run_functions as runf
 import pyFAT_astro.Support.support_functions as sf
 import pyFAT_astro.Support.write_functions as wf
 
 from datetime import datetime
 from pyFAT_astro.Support.fat_errors import BadCatalogueError
+from pyFAT_astro.Support.log_functions import print_log,write_config,update_statistics
 
 def FAT_Galaxy_Loop(Configuration):
 
     try:
 
         registered_exception = None
         current_run = 'Not Initialized'
         Fits_Files = initialize_loop(Configuration)
         loop_sofia(Configuration,Fits_Files)
 
         # If you add any make sure that the fitstage  starts with 'Fit_'
         if Configuration['USED_FITTING']:
             # Process the found source in sofia to set up the proper fitting and make sure source can be fitted
+
             Initial_Parameters = runf.check_source(
-                Configuration, Fits_Files)
+                    Configuration, Fits_Files)
+
             #sf.sofia_output_exists(Configuration,Fits_Files)
-            sf.print_log(f'''FAT_GALAXY_LOOPS: The source is well defined and we will now setup the initial tirific file
+            print_log(f'''FAT_GALAXY_LOOPS: The source is well defined and we will now setup the initial tirific file
 ''', Configuration)
             #Add your personal fitting types here
             if Configuration['DEBUG']:
-                sf.write_config(
+                write_config(
                     f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Fitting.txt', Configuration)
         # then we want to read the template
-        Tirific_Template = sf.tirific_template()
+      
 
-        if 'fit_tirific_osc' in Configuration['FITTING_STAGES']:
-            current_run = runf.fitting_osc(
-                Configuration, Fits_Files, Tirific_Template, Initial_Parameters)
+        if 'fit_tirific_osc' in Configuration['FITTING_STAGES']: 
+            current_run,Tirific_Template = runf.fitting_osc(
+                Configuration, Fits_Files,  Initial_Parameters)
         elif 'fit_make_your_own' in Configuration['FITTING_STAGES']:
-            sf.print_log(f'''FAT_GALAXY_LOOPS: If you add any fitting routine make sure that the fit stage  starts with Fit_
+            print_log(f'''FAT_GALAXY_LOOPS: If you add any fitting routine make sure that the fit stage  starts with Fit_
 ''',Configuration)
             sf.create_directory(Configuration['USED_FITTING'],Configuration['FITTING_DIR'])
             Configuration['FINAL_COMMENT'] = 'This example does not work'
             catalogue_line = cf.finish_galaxy(Configuration)
             return catalogue_line
         else:
             Configuration['FINAL_COMMENT'] = 'You have chosen not to do any fitting'
@@ -57,15 +60,15 @@
             return catalogue_line
 
         #if all the fitting has gone properly we create nice errors
 
         if Configuration['OUTPUT_QUANTITY'] != 5:
             if 'tirshaker' in Configuration['FITTING_STAGES']:
                 runf.tirshaker_call(
-                    Configuration)
+                    Configuration,Fits_Files)
 
             Configuration['FINAL_COMMENT'] = 'The fit has converged succesfully'
 
 
         catalogue_line = cf.finish_galaxy(Configuration, current_run=current_run,
                          Fits_Files=Fits_Files,exiting=registered_exception)
         if Configuration['OUTPUT_QUANTITY'] != 5:
@@ -74,25 +77,33 @@
             Totflux = rf.get_totflux(
                 Configuration, f"/Finalmodel/Finalmodel_mom0.fits")
             wf.basicinfo(Configuration, template=Tirific_Template, Tot_Flux=Totflux, DHI=[
                          DHI, Configuration['BEAM'][0]*Configuration['RING_SIZE']])
             if Configuration['INSTALLATION_CHECK']:
                 cf.installation_check(
                     Configuration)
+        print_log(f'''FAT_GALAXY_LOOP: This galaxy has succesfully ran through all parts of the fitting
+''', Configuration)
     except Exception as e:
         if e.__class__.__name__ in Configuration['STOP_INDIVIDUAL_ERRORS']:
             Configuration['OUTPUT_QUANTITY'] = 5
         else:
             Configuration['OUTPUT_QUANTITY'] = 'error'
         registered_exception = e
         Configuration['FINAL_COMMENT'] = e
         Configuration['OUTPUT_QUANTITY'] = 'error'
+        try:
+            tmp=Fits_Files
+        except:
+            Fits_Files= None
+        
         catalogue_line = cf.finish_galaxy(Configuration,
                           current_run=current_run,Fits_Files=Fits_Files,
                           exiting=registered_exception)
+       
     return catalogue_line
 
 
 def initialize_loop(Configuration):
     Configuration['INITIALIZATION_TIME'][0] = datetime.now()
     # First check the starttime
     if Configuration['FITTING_DIR'][-2:] == '//':
@@ -130,32 +141,34 @@
             Configuration['OUTPUTLOG'], f"{os.path.splitext(Configuration['OUTPUTLOG'])[0]}_Prev.txt")
 
     with open(Configuration['OUTPUTLOG'], 'w') as log:
         log.write(log_statement)
 
 
     #if we skip the create_fat _cube stage peaople could give the fat cube itself
-
+  
     if Fits_Files['ORIGINAL_CUBE'][-9:] == '_FAT.fits':
         if 'create_fat_cube' in Configuration['FITTING_STAGES']:
-            sf.print_log(f'''FAT_GALAXY_LOOPS: Your input cube ends in _FAT.fits indicating it is a FAT processed cube.
+            print_log(f'''FAT_GALAXY_LOOPS: Your input cube ends in _FAT.fits indicating it is a FAT processed cube.
 Therefore we remove the Create_FAT_Cube stages from the loop.
 ''', Configuration)
             Configuration['FITTING_STAGES'].remove('create_fat_cube')
         fat_ext = ''
     else:
         fat_ext = '_FAT'
     stripped_file_name = os.path.splitext(Configuration['INPUT_CUBE'])[0]
+    
     Fits_Files['FITTING_CUBE'] = f"{stripped_file_name}{fat_ext}.fits"
     Fits_Files['OPTIMIZED_CUBE'] = f"{stripped_file_name}{fat_ext}_opt.fits"
     Fits_Files['MOMENT0'] = f"Sofia_Output/{Configuration['BASE_NAME']}_mom0.fits"
     Fits_Files['MOMENT1'] = f"Sofia_Output/{Configuration['BASE_NAME']}_mom1.fits"
     Fits_Files['MOMENT2'] = f"Sofia_Output/{Configuration['BASE_NAME']}_mom2.fits"
     Fits_Files['MASK'] = f"Sofia_Output/{Configuration['BASE_NAME']}_mask.fits"
     Fits_Files['CHANNEL_MAP'] = f"Sofia_Output/{Configuration['BASE_NAME']}_chan.fits"
+    Fits_Files['TIR_RUN_CUBE'] = copy.deepcopy(Fits_Files['FITTING_CUBE'])
     if 'create_fat_cube' in Configuration['FITTING_STAGES']:
         if not os.path.exists(f"{Configuration['FITTING_DIR']}/{Fits_Files['ORIGINAL_CUBE']}"):
             raise BadCatalogueError(
                 f'''We can not find the file {Fits_Files['ORIGINAL_CUBE']}. This is likely to be due to a typo in your catalog {Configuration['CATALOGUE']}.''')
     else:
         if not os.path.exists(f"{Configuration['FITTING_DIR']}/{Fits_Files['FITTING_CUBE']}"):
             raise BadCatalogueError(
@@ -170,46 +183,47 @@
         from scipy import __version__ as spversion
         from astropy import __version__ as apversion
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             from matplotlib import __version__ as mpversion
         #from subprocess import __version__ as subversion
 
-        sf.print_log(f'''FAT_GALAXY_LOOPS: We are using the following versions
+        print_log(f'''FAT_GALAXY_LOOPS: We are using the following versions
 {'':8s}NumPy {npversion}
 {'':8s}SciPy {spversion}
 {'':8s}AstroPy {apversion}
 {'':8s}Matplotlib {mpversion}
 ''', Configuration)
 
     log_statement = f'''We are starting the catalogue entry {Configuration['ID']} in the directory {Configuration['SUB_DIR']}.\n'''
-    sf.print_log(
+    print_log(
         log_statement, Configuration)
 
     if Configuration['TIMING']:
         Configuration['FAT_PSUPROCESS'] = psu.Process(
             Configuration['FAT_PID'])
-        sf.update_statistic(
+        update_statistics(
             Configuration, message="Creating a CPU RAM Log for analysis.")
 
 
     # Let's see if our base cube exists, Note that cleanup removes it if we want to start from the original dir so no need to check start_point
     if not os.path.exists(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}"):
-        ff.create_fat_cube(Configuration, Fits_Files)
+        ff.create_fat_cube(Configuration, Fits_Files = Fits_Files)
     # Get a bunch of info from the cube
     rf.read_cube(
         Configuration, Fits_Files['FITTING_CUBE'])
     Configuration['INITIALIZATION_TIME'][1] = datetime.now()
     return Fits_Files
 
 def loop_sofia(Configuration,Fits_Files):
+     
     Configuration['SOFIA_TIME'][0] = datetime.now()
     #If we have Sofia Preprocessed Output request make sure it all exists
     if Configuration['DEBUG']:
-        sf.write_config(
+        write_config(
             f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Sofia.txt', Configuration)
 
     if 'external_sofia' in Configuration['FITTING_STAGES']:
         sf.copy_homemade_sofia(
             Configuration)
     elif 'run_sofia' in Configuration['FITTING_STAGES']:
         runf.sofia(Configuration, Fits_Files)
@@ -227,15 +241,15 @@
     Fits_Files = {}
     try:
         Fits_Files = initialize_loop(Configuration)
         loop_sofia(Configuration,Fits_Files)
         if Configuration['USED_FITTING']:
             Initial_Parameters = runf.check_source(Configuration, Fits_Files)
             succes =True
-            sf.print_log(f'''FAT_GALAXY_LOOPS: The source is well defined and we will now setup the initial tirific file
+            print_log(f'''FAT_GALAXY_LOOPS: The source is well defined and we will now setup the initial tirific file
 ''', Configuration)
         else:
             catalogue_line = cf.finish_galaxy(Configuration,
                           current_run=current_run,Fits_Files=Fits_Files,
                           timing_lock=timing_lock, catalogue_lock = catalogue_lock,
                           exiting=registered_exception)
     except Exception as e:
@@ -248,47 +262,50 @@
         registered_exception = e
         Configuration['FINAL_COMMENT'] = e
         catalogue_line = cf.finish_galaxy(Configuration,
                           current_run=current_run,Fits_Files=Fits_Files,
                           timing_lock=timing_lock, catalogue_lock = catalogue_lock,
                           exiting=registered_exception)
 
-    Configuration['FAT_PSUPROCESS'] = None
+   
     sofia_output = {'Succes': succes, 'Configuration': Configuration,
                       'catalogue_line': catalogue_line, 'Fits_Files':Fits_Files,
                       'Size': Configuration['SIZE_IN_BEAMS'],
                       'Initial_Parameters': Initial_Parameters}
-
-
+    
+    update_statistics(
+            Configuration, message="Pause at")  
+    Configuration['FAT_PSUPROCESS'] = None
     return sofia_output
 
 
 def MP_Fitting_Loop(input,timing_lock,catalogue_lock):
     try:
+       
         Configuration = input['Configuration']
         Configuration['FAT_PSUPROCESS'] = psu.Process(
             Configuration['FAT_PID'])
+        update_statistics(
+            Configuration, message="Start fitting loop")  
         Initial_Parameters = input['Initial_Parameters']
         Fits_Files = input['Fits_Files']
         registered_exception = None
         current_run = 'Not Initialized'
-        # then we want to read the template
-        Tirific_Template = sf.tirific_template()
-
+       
             # If you add any make sure that the fitstage  starts with 'Fit_'
 
         if Configuration['DEBUG']:
-            sf.write_config(
+            write_config(
                 f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Fitting.txt', Configuration)
 
-        if 'fit_tirific_osc' in Configuration['FITTING_STAGES']:
-            current_run = runf.fitting_osc(
-                Configuration, Fits_Files, Tirific_Template, Initial_Parameters)
+        if 'fit_tirific_osc' in Configuration['FITTING_STAGES']:   
+            current_run,Tirific_Template = runf.fitting_osc(
+                Configuration, Fits_Files, Initial_Parameters)
         elif 'fit_make_your_own' in Configuration['FITTING_STAGES']:
-            sf.print_log(f'''FAT_GALAXY_LOOPS: If you add any fitting routine make sure that the fit stage  starts with Fit_
+            print_log(f'''FAT_GALAXY_LOOPS: If you add any fitting routine make sure that the fit stage  starts with Fit_
 ''',Configuration)
             sf.create_directory(Configuration['USED_FITTING'],Configuration['FITTING_DIR'])
             Configuration['FINAL_COMMENT'] = 'This example does not work'
             catalogue_line = cf.finish_galaxy(Configuration)
             return catalogue_line
         else:
             Configuration['FINAL_COMMENT'] = 'You have chosen not to do any fitting'
@@ -296,15 +313,15 @@
             return catalogue_line
 
         #if all the fitting has gone properly we create nice errors
 
         if Configuration['OUTPUT_QUANTITY'] != 5:
             if 'tirshaker' in Configuration['FITTING_STAGES']:
                 runf.tirshaker_call(
-                    Configuration)
+                    Configuration,Fits_Files)
 
             Configuration['FINAL_COMMENT'] = 'The fit has converged succesfully'
 
     #Only
         catalogue_line = cf.finish_galaxy(Configuration, current_run=current_run,
                          Fits_Files=Fits_Files,timing_lock=timing_lock,
                          catalogue_lock = catalogue_lock,
@@ -315,14 +332,16 @@
             Totflux = rf.get_totflux(
                 Configuration, f"/Finalmodel/Finalmodel_mom0.fits")
             wf.basicinfo(Configuration, template=Tirific_Template, Tot_Flux=Totflux,\
                 DHI=[DHI, Configuration['BEAM'][0]*Configuration['RING_SIZE']])
             if Configuration['INSTALLATION_CHECK']:
                 cf.installation_check(
                     Configuration)
+        print_log(f'''FAT_GALAXY_LOOP: This galaxy has succesfully ran through all parts of the fitting
+''', Configuration)
     except Exception as e:
         if e.__class__.__name__ in Configuration['STOP_INDIVIDUAL_ERRORS']:
             Configuration['OUTPUT_QUANTITY'] = 5
         else:
             Configuration['OUTPUT_QUANTITY'] = 'error'
         registered_exception = e
         Configuration['FINAL_COMMENT'] = e
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Installation_Check/NGC_2903.fits` & `pyFAT_astro-0.1.6/pyFAT_astro/Installation_Check/NGC_2903.fits`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/clean_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/clean_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in several different Python scripts in the Database.
 
-import pyFAT_astro
-import os,signal,sys
+
+import os,sys
 import numpy as np
 import traceback
-from datetime import datetime
 
-from pyFAT_astro.Support.fits_functions import make_moments
-from pyFAT_astro.Support.modify_template import get_error
+from datetime import datetime
+from astropy.io import fits
+from make_moments.functions import moments
+from pyFAT_astro.Support.modify_template import get_error,\
+    set_fitting_parameters,get_ring_weights
 from pyFAT_astro.Support.write_functions import make_overview_plot,plot_usage_stats,tirific
-from pyFAT_astro.Support.fat_errors import SofiaMissingError
+from pyFAT_astro.Support.log_functions import print_log,write_config
 import pyFAT_astro.Support.support_functions as sf
-import pyFAT_astro
+
 
 class DummyLock():
     def __enter__(self):
         pass
 
     def __exit__(self, *args):
         pass
 
 def check_legitimacy_osc(Configuration):
-    sf.print_log(f'''CHECK_LEGITIMACY_OSC: Start.
+    print_log(f'''CHECK_LEGITIMACY_OSC: Start.
 ''',Configuration,case=['debug_start'])
     if Configuration['OUTPUT_QUANTITY'] == 'error':
-        sf.print_log(f'''CHECK_LEGITIMACY_OSC: An unspecified error is registered. The final message should reflect this.
+        print_log(f'''CHECK_LEGITIMACY_OSC: An unspecified error is registered. The final message should reflect this.
 ''',Configuration)
         return
     elif Configuration['OUTPUT_QUANTITY'] == 5:
-        sf.print_log(f'''CHECK_LEGITIMACY_OSC: A FAT specific error is registered. The final message should reflect this.
+        print_log(f'''CHECK_LEGITIMACY_OSC: A FAT specific error is registered. The final message should reflect this.
 ''',Configuration)
         return
     else:
         fit_check=[True if 'fit_' in x.lower() else False for x in Configuration['FITTING_STAGES']]
         if any(fit_check):
             outfile = f"{Configuration['FITTING_DIR']}/{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def"
     inclination = sf.load_tirific(Configuration,outfile,Variables=['INCL'],array=True)
 
     if float(inclination[0]) < Configuration['UNRELIABLE_INCLINATION']:
         Configuration['ACCEPTED'] = False
         Configuration['FINAL_COMMENT'] = f"The final inclination is below {Configuration['UNRELIABLE_INCLINATION']}. FAT is not neccesarily reliable in this range."
-        sf.print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved inclination {float(inclination[0])} is below {Configuration['UNRELIABLE_INCLINATION']} thus the fit is not accepted.
+        print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved inclination {float(inclination[0])} is below {Configuration['UNRELIABLE_INCLINATION']} thus the fit is not accepted.
 ''',Configuration)
     if np.sum(Configuration['SIZE_IN_BEAMS']) < Configuration['UNRELIABLE_SIZE']:
         Configuration['ACCEPTED'] = False
         Configuration['FINAL_COMMENT'] = f"The final size is below {Configuration['UNRELIABLE_SIZE']}. FAT is not neccesarily reliable in this range."
-        sf.print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved size {np.sum(Configuration['SIZE_IN_BEAMS'])} is below {Configuration['UNRELIABLE_SIZE']} thus the fit is not accepted.
+        print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved size {np.sum(Configuration['SIZE_IN_BEAMS'])} is below {Configuration['UNRELIABLE_SIZE']} thus the fit is not accepted.
 ''',Configuration)
     return
 
 check_legitimacy_osc.__doc__ =f'''
  NAME:
     check_legitimacy_osc
 
@@ -75,15 +77,15 @@
 
  NOTE:
     !!!!!!! Until release these are set ridiculously low for testing purposes.
 '''
 
 def clean_before_sofia(Configuration):
 
-    sf.print_log(f'''CLEAN_BEFORE_SOFIA: Starting.
+    print_log(f'''CLEAN_BEFORE_SOFIA: Starting.
 ''',Configuration,case = ['debug_start'])
     files =['_mask.fits','_mom0.fits','_mom1.fits','_chan.fits','_mom2.fits','_cat.txt']
 
     for file in files:
         try:
             os.remove(Configuration['BASE_NAME']+file)
         except FileNotFoundError:
@@ -124,15 +126,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def clean_after_sofia(Configuration):
-    sf.print_log(f'''CLEAN_AFTER_SOFIA: Starting clean
+    print_log(f'''CLEAN_AFTER_SOFIA: Starting clean
 ''',Configuration,case = ['debug_start'])
     files =['_mask.fits','_chan.fits','_cat.txt']
 
     for file in files:
         try:
             os.rename(Configuration['BASE_NAME']+file,'Sofia_Output/'+Configuration['BASE_NAME']+file )
         except FileNotFoundError:
@@ -166,29 +168,29 @@
     Unspecified
 
  NOTE:
 '''
 
 # cleanup dirty files before starting fitting
 def cleanup(Configuration,Fits_Files):
-    sf.print_log(f'''CLEANUP: Starting clean
+    print_log(f'''CLEANUP: Starting clean
 ''',Configuration,case = ['debug_start'])
         #Move any existing output to the Log directory
     if os.path.exists(f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf"):
         if os.path.exists(f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf"):
             os.remove(f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf")
         os.rename( f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf",f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf")
     #Move any existing Overview.png to the Log directory well
     if os.path.exists(f"{Configuration['FITTING_DIR']}Overview.png"):
         if os.path.exists(f"{Configuration['LOG_DIRECTORY']}Overview_prev.png"):
             os.remove(f"{Configuration['LOG_DIRECTORY']}Overview_prev.png")
-            sf.print_log(f'''CLEANUP: Removing an old Overview_prev.png from {Configuration['LOG_DIRECTORY']}
+            print_log(f'''CLEANUP: Removing an old Overview_prev.png from {Configuration['LOG_DIRECTORY']}
 ''',Configuration,case = ['debug_add'])
         os.rename( f"{Configuration['FITTING_DIR']}Overview.png",f"{Configuration['LOG_DIRECTORY']}Overview_prev.png")
-        sf.print_log(f'''CLEANUP: We moved an old Overview.png to {Configuration['LOG_DIRECTORY']}Overview_prev.png
+        print_log(f'''CLEANUP: We moved an old Overview.png to {Configuration['LOG_DIRECTORY']}Overview_prev.png
 ''',Configuration,case = ['debug_add'])
     #clean the log directory of all files except those named Prev_ and not the Log as it is already moved if existing
     files_in_log = ['restart_One_Step_Convergence.txt','restart_Centre_Convergence.txt',f"restart_{Configuration['USED_FITTING']}.txt",\
                     'restart_Extent_Convergence.txt','Usage_Statistics.txt', 'clean_map_0.fits','clean_map_1.fits','clean_map.fits',\
                     'dep_map_0.fits','minimum_map_0.fits','rot_map_0.fits','dep_map.fits','minimum_map.fits','rot_map.fits',\
                     'dep_map_1.fits','minimum_map_1.fits','rot_map_1.fits','Convolved_Cube_FAT_opt.fits']
 
@@ -232,15 +234,15 @@
 
     if 'create_fat_cube' in Configuration['FITTING_STAGES']:
         files.append(Fits_Files['FITTING_CUBE'])
 
     if 'run_sofia' in Configuration['FITTING_STAGES'] or 'external_sofia' in Configuration['FITTING_STAGES']:
         dir =f'{Configuration["FITTING_DIR"]}Sofia_Output/'
         file_ext=['_mask.fits','_mom0.fits','_mom1.fits','_mom2.fits','_chan.fits','_cat.txt','_sofia_xv.fits']
-        sf.print_log(f'''CLEANUP: We are cleaning the following files in the directory {dir}:
+        print_log(f'''CLEANUP: We are cleaning the following files in the directory {dir}:
 {"":8s}CLEANUP: sofia_input.par,{','.join([f'{Configuration["SOFIA_BASENAME"]}{x}' for x in file_ext])}
 ''',Configuration,case = ['verbose'])
         for extension in file_ext:
             try:
                 os.remove(f'{dir}{Configuration["BASE_NAME"]}{extension}')
             except FileNotFoundError:
                 pass
@@ -251,15 +253,15 @@
     if 'tirshaker' in Configuration['FITTING_STAGES']:
         directories.append('Error_Shaker')
     # Existing_Sofia
 
 
 
     if directories:
-        sf.print_log(f'''CLEANUP: We are cleaning the following directories:
+        print_log(f'''CLEANUP: We are cleaning the following directories:
 {"":8s}CLEANUP: {','.join(directories)}
 {"":8s}CLEANUP: and the following files:
 {"":8s}CLEANUP: {','.join(files)}
 ''',Configuration, case=['verbose'])
 
 
         ext=['.fits','_Prev.fits','.log','.ps','.def']
@@ -274,28 +276,34 @@
 
                 for fe in ext:
                     if dir == 'Finalmodel' and fe in ['.fits','.def']:
                         try:
                             os.unlink(f'{Configuration["FITTING_DIR"]}{dir}/{dir}{fe}')
                         except FileNotFoundError:
                             pass
+
                     elif dir == Configuration['USED_FITTING'] and fe in ['.def']:
                         target = sf.get_system_string(f"{Configuration['FITTING_DIR']}{dir}/{dir}*{fe}")
                         os.system(f'rm -f {target}')
                     else:
                         try:
                             os.remove(f'{Configuration["FITTING_DIR"]}{dir}/{dir}{fe}')
                         except FileNotFoundError:
                             pass
 
                 for mom in moments:
                     try:
                         os.remove(f'{Configuration["FITTING_DIR"]}{dir}/{dir}_{mom}.fits')
                     except FileNotFoundError:
                         pass
+                if dir == 'Finalmodel':
+                    try:
+                        os.remove(f'{Configuration["FITTING_DIR"]}{dir}/{Configuration["BASE_NAME"]}_final_xv.fits')
+                    except FileNotFoundError:
+                        pass
 
 
     for file in files:
         try:
             os.remove(f'{Configuration["FITTING_DIR"]}{file}')
         except FileNotFoundError:
             pass
@@ -324,15 +332,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def cleanup_final(Configuration,Fits_Files):
-    sf.print_log(f'''CLEANUP_FINAL: Starting the final cleanup of the directory.
+    print_log(f'''CLEANUP_FINAL: Starting the final cleanup of the directory.
 {'':8s} The request is {Configuration['OUTPUT_QUANTITY']}
 ''',Configuration,case = ['debug_start','verbose'] )
 
     if Configuration['USED_FITTING'] == 'Fit_Tirific_OSC':
         clean_files = [Fits_Files['OPTIMIZED_CUBE'],f"{Configuration['USED_FITTING']}_In.def",\
                         "clean_map_0.fits","dep_map_0.fits","minimum_map_0.fits","rot_map_0.fits",\
                         "clean_map_1.fits","dep_map_1.fits","minimum_map_1.fits","rot_map_1.fits",
@@ -430,56 +438,56 @@
 '''
 
 
 
 
 
 def installation_check(Configuration):
-    sf.print_log(f'''INSTALLATION_CHECK: Starting to compare the output to what is expected.
+    print_log(f'''INSTALLATION_CHECK: Starting to compare the output to what is expected.
 ''',Configuration, case = ['debug_start', 'main'])
 
     Model = sf.tirific_template(filename = 'Installation_Check')
     Variables_to_Compare = ['VROT','INCL','PA','SBR','SDIS','Z0','XPOS','YPOS','VSYS']
     Model_values = sf.load_tirific(Configuration,Model,\
         Variables = Variables_to_Compare,array=True)
     #Then the fitted file
     Fitted_values =sf.load_tirific(Configuration,\
         f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",\
         Variables = Variables_to_Compare,array = True)
     succes = False
     diff = np.abs(Model_values-Fitted_values)
 
-    sf.print_log(f'''INSTALLATION_CHECK: the found differences
+    print_log(f'''INSTALLATION_CHECK: the found differences
 {'':8s}{diff}
 ''',Configuration, case = ['verbose'])
     too_much = np.array(np.where(diff > 1e-3),dtype=bool)
 
-    sf.print_log(f'''INSTALLATION_CHECK: at the locations
+    print_log(f'''INSTALLATION_CHECK: at the locations
 {'':8s}{too_much}{np.where(diff > 1e-3)}
 {'':8s}{too_much.size}
 ''',Configuration, case = ['verbose'])
 
     if too_much.size == 0.:
         succes = True
 
 
     if succes:
-        sf.print_log(f'''
+        print_log(f'''
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!! All parameters are fitted within the expected variance. !!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!!        We think pyFAT is installed succesfully          !!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 ''',Configuration, case = ['main','screen'])
     else:
-        sf.print_log(f'''
+        print_log(f'''
 !!!!---------------------------------------------!!!!!
 !!!! FAT ran through the fitting process but the !!!!!
 !!!! fitted values differ too much from their    !!!!!
 !!!! expectations. Please update SoFiA and other !!!!!
-!!!! dependencies. I f you have done so and this !!!!!
+!!!! dependencies. If you have done so and this !!!!!
 !!!! message remains, the check is likely out of !!!!!
 !!!! date. If you are unable to resolve the issue!!!!!
 !!!! please file a bug report at:                !!!!!
 !!!!                                             !!!!!
 !!!! https://github.com/PeterKamphuis/pyFAT/issues !!!!!
 !!!!                                             !!!!!
 !!!! Please add the Log.txt file in the directory!!!!!
@@ -514,22 +522,34 @@
  NOTE:
 '''
 
 def finish_galaxy(Configuration,current_run = 'Not initialized',\
         timing_lock= DummyLock(), catalogue_lock = DummyLock(),
         Fits_Files= {'ORIGINAL_CUBE': "Unset.fits"},exiting = None):
     Configuration['FULL_TIME'][1] = datetime.now()
-    sf.print_log(f'''FINISH_GALAXY: These fits files are used:
+    print_log(f'''FINISH_GALAXY: These fits files are used:
 {'':8s} {Fits_Files}
 ''',Configuration,case = ['debug_start','verbose'])
     if Configuration['DEBUG']:
-        sf.write_config(f'{Configuration["LOG_DIRECTORY"]}CFG_At_Finish.txt',Configuration)
+        write_config(f'{Configuration["LOG_DIRECTORY"]}CFG_At_Finish.txt',Configuration)
 
     #make sure we are not leaving stuff
     sf.finish_current_run(Configuration,current_run)
+    # And place the correct velocity frame
+    if Configuration['HDR_VELOCITY'] != 'VELO':
+        print_log(f'''
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+{"":8s}Your velocity frame is not suitable for Tirific it is CTYPE3 = {Configuration['HDR_VELOCITY']} and should be VELO, FELO or FREQ 
+{"":8s}If you want to continue to fit with tirific please use the cube marked _tirific , we have kept the correct conversion in the FAT cube
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+''',Configuration, case = ['main','screen'])
+        
+
+
+
     # We need to check if the final output is legit
     if Configuration['USED_FITTING'] == 'Fit_Tirific_OSC':
         check_legitimacy_osc(Configuration)
 
 
     if Configuration['OUTPUT_QUANTITY'] == 'error':
         error_message = '''
@@ -541,61 +561,71 @@
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 {"":8s}FAT did not run the full fitting routines for catalog entry {Configuration['ID']}.
 {"":8s}Which is the galaxy in directory {Configuration['FITTING_DIR']}.
 {"":8s}Please check this log and output_catalogue carefully for what went wrong.
 {"":8s}The detected exit reason is: "{Configuration['FINAL_COMMENT']}".
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 '''
-        sf.print_log(log_statement,Configuration, case = ['main','screen'])
-        sf.print_log(error_message,Configuration, case = ['main','screen'])
+        print_log(log_statement,Configuration, case = ['main','screen'])
+        print_log(error_message,Configuration, case = ['main','screen'])
 
-        if exiting:
+        if exiting != None:
             with open(Configuration['OUTPUTLOG'],'a') as log_file:
                 traceback.print_exception(type(exiting),exiting,exiting.__traceback__,file=log_file)
             traceback.print_exception(type(exiting),exiting,exiting.__traceback__)
+        
         if Configuration['MULTIPROCESSING']:
             Configuration['ACCEPTED'] = False
             Configuration['FINAL_COMMENT'] = f"The code crashed while fitting this galaxy please check it's log."
             Configuration['OUTPUT_QUANTITY'] = 5
         else:
-            if exiting:
+            if exiting != None:
                 sys.exit(1)
             else:
                 Configuration['ACCEPTED'] = False
                 Configuration['FINAL_COMMENT'] = f"The code crashed while fitting this galaxy please check it's log."
                 Configuration['OUTPUT_QUANTITY'] = 5
     elif Configuration['OUTPUT_QUANTITY'] == 5:
-        sf.print_log(f'''
+        print_log(f'''
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 {"":8s}FAT could not find an acceptable model for the galaxy in directory {Configuration['FITTING_DIR']}.
 {"":8s}Please check the log in {Configuration['LOG_DIRECTORY']} and the output_catalogue carefully for more information.
 {"":8s}The detected exit reason is: "{Configuration['FINAL_COMMENT']}".
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 ''',Configuration, case = ['main','screen'])
 
     elif Configuration['OUTPUT_QUANTITY'] < 4:
-        sf.print_log( f'''Producing final output in {Configuration['FITTING_DIR']}.
+        print_log( f'''Producing final output in {Configuration['FITTING_DIR']}.
 ''',Configuration)
         # We need to produce a FinalModel Directory with moment maps and an XV-Diagram of the model.
         if any([True if 'fit_' in x else False for x in Configuration['FITTING_STAGES']]):
             if not 'Fit_Make_Your_Own' in  Configuration['USED_FITTING']:
                 sf.create_directory('Finalmodel',Configuration['FITTING_DIR'])
-                if 'tirshaker' not in Configuration['FITTING_STAGES'] and not Configuration['INSTALLATION_CHECK']:
+                if 'tirshaker' not in Configuration['FITTING_STAGES']:
                     transfer_errors(Configuration,fit_type=Configuration['USED_FITTING'])
+                    #Also transfer the last fitting settings
+                    transfer_fitting_parameters(Configuration)    
                 linkname = f"../{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}"
                 os.symlink(f"{linkname}.fits",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits")
                 os.symlink(f"{linkname}.def",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.def")
 
                 # We need to produce a FinalModel Directory with moment maps and an XV-Diagram of the model.
                 if Fits_Files and os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits"):
-                    make_moments(Configuration,Fits_Files,fit_type = 'Generic_Final',vel_unit = 'm/s')
+                    # we do not mask the model as it is also important where the model extends and there is no data.  
+                    messages = moments(filename =  f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits",\
+                            overwrite = True, cube_velocity_unit='m/s',map_velocity_unit= 'km/s',\
+                            debug = Configuration['DEBUG'], log=True, level = 0.25*Configuration['NOISE'],\
+                            output_directory = f"{Configuration['FITTING_DIR']}/Finalmodel/",\
+                            output_name = 'Finalmodel')
+                    print_log(messages,Configuration,case=['verbose'])
+                    #make_moments(Configuration,Fits_Files,fit_type = 'Generic_Final',vel_unit = 'm/s')
                     make_overview_plot(Configuration,Fits_Files)
+    
 
-
-    sf.print_log(f'''Finished the fitting in {Configuration['FITTING_DIR']}.
+    print_log(f'''Finished the fitting in {Configuration['FITTING_DIR']}.
 ''',Configuration, case = ['main','screen'])
     # Need to organize the fitting output orderly
     # Need to write date and Time to timing log
     if Configuration['TIMING']:
         plot_usage_stats(Configuration)
         with timing_lock:
             with open(Configuration['MAIN_DIRECTORY']+'/Timing_Result.txt','a') as timing_result:
@@ -611,26 +641,24 @@
 
             #    timing_result.write(f'''The galaxy in directory {Configuration['FITTING_DIR']} started at {Configuration['START_TIME']}.
 #Finished preparations at {Configuration['PREP_END_TIME']}.
 #Converged to a galaxy size at {Configuration['END_TIME']}.
 #It finished the whole process at {datetime.now()}.
 #''')
 
-        sf.print_log(f'''Finished timing statistics for the galaxy in {Configuration['FITTING_DIR']}.
+        print_log(f'''Finished timing statistics for the galaxy in {Configuration['FITTING_DIR']}.
 ''',Configuration)
 
     cleanup_final(Configuration,Fits_Files)
     # Need to write to results catalog
     catalogue_line = f"{Configuration['FITTING_DIR'].split('/')[-2]:{Configuration['MAXIMUM_DIRECTORY_LENGTH']}s} {str(Configuration['ACCEPTED']):>6s} {Configuration['FINAL_COMMENT']} \n"
-
     if Configuration['OUTPUT_CATALOGUE']:
         with catalogue_lock:
             with open(Configuration['OUTPUT_CATALOGUE'],'a') as output_catalogue:
                 output_catalogue.write(catalogue_line)
-
     return catalogue_line
 
 finish_galaxy.__doc__ =f'''
  NAME:
     finish_galaxy
 
  PURPOSE:
@@ -653,45 +681,65 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This function should always be followed by a continue statement
 '''
 
+def mod_vrot_incl_err(profile,errors,incl,incl_errors):
+    '''Error up and down have to be exactly the same'''
+    vobs_up = np.sin(np.radians(incl+incl_errors))*\
+                (profile+errors)
+    errors = vobs_up/np.sin(np.radians(incl))-profile
+    return errors
+
 def transfer_errors(Configuration,fit_type='Undefined'):
-    sf.print_log(f'''TRANSFER_ERROR: Start.
+    print_log(f'''TRANSFER_ERROR: Start.
 ''',Configuration, case = ['debug_start'])
     # Load the final file
     Tirific_Template = sf.tirific_template(filename = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def")
     variables = ['INCL','PA','VROT','SDIS','SBR','VSYS','XPOS','YPOS','Z0']
-    weights = sf.get_ring_weights(Configuration,Tirific_Template)
+    weights = get_ring_weights(Configuration,Tirific_Template)
+    incl_error = None
+    incl = None
     for parameter in variables:
-        sf.print_log(f'''TRANSFER_ERROR: Creating errors for {parameter}.
+        print_log(f'''TRANSFER_ERROR: Creating errors for {parameter}.
 ''',Configuration, case = ['debug_add'])
-        profile = sf.load_tirific(Configuration,Tirific_Template,\
+        reg_profile = sf.load_tirific(Configuration,Tirific_Template,\
             [parameter,f"{parameter}_2"],array=True)
-        sm_profile = sf.load_tirific(Configuration,\
+        profile = sf.load_tirific(Configuration,\
             f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def",\
             Variables=[parameter,f"{parameter}_2"],array=True)
+        
+        # As we can cut rings away during the smoothing we have to ensure the profiles have the same length
+        if len(profile[0,:]) != len(reg_profile[0,:]):
+            tmp = [[],[]]    
+            for i in [0,1]:
+                tmp[i] = profile[i,:len(reg_profile[i,:]-1)]
+            profile=np.array(tmp,dtype=float)
             #it is possible that the last iteration of the fitted smooth check
             #Crashes and is rerun with
         if parameter == 'VROT':
             apply_max= False
         else:
             apply_max = True
-        errors = get_error(Configuration,sm_profile,profile,parameter,\
+        errors = get_error(Configuration,profile,reg_profile,parameter,\
             min_error=Configuration['MIN_ERROR'][parameter],\
             apply_max_error = apply_max,weights = weights)
+        if parameter == 'VROT':
+            errors = mod_vrot_incl_err(reg_profile,errors,incl,incl_error)   
+        if parameter == 'INCL':
+            incl_error=errors
+            incl = reg_profile
+
         format = sf.set_format(parameter)
         Tirific_Template.insert(parameter,f"# {parameter}_ERR",f"{' '.join([f'{x:{format}}' for x in errors[0]])}")
         Tirific_Template.insert(f"{parameter}_2",f"# {parameter}_2_ERR",f"{' '.join([f'{x:{format}}' for x in errors[1]])}")
 
-    Tirific_Template['GR_CONT']=' '
-    Tirific_Template.insert('GR_CONT','RESTARTID','0')
-    Tirific_Template.insert('MINDELTA','DISTANCE',Configuration['DISTANCE'])
+
     # write back to the File
     tirific(Configuration,Tirific_Template, name = f"{fit_type}/{fit_type}.def")
 
 transfer_errors.__doc__ =f'''
  NAME:
     transfer_errors
 
@@ -710,7 +758,22 @@
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 '''
+
+def transfer_fitting_parameters(Configuration):
+    fit_type = Configuration['USED_FITTING']
+    # first read the Final file
+    print_log(f'''TRANSFER_FITTING_PARAMETERS: Start.
+''',Configuration, case = ['debug_start'])
+    # Load the final file
+    Tirific_Template = sf.tirific_template(filename = \
+        f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def")
+    
+    set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os')
+   
+    # write back to the File
+    tirific(Configuration,Tirific_Template, name = f"{fit_type}/{fit_type}.def")
+
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/constants.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: future_fstrings -*-
-import pyFAT_astro
 #def initialize():
 global H_0
 H_0 = 69.7 #km/s/Mpc
 global c
 c=299792458                  #light speed in m/s
 global pc
 pc=3.086e+18                  #parsec in cm
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/development_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/development_functions.py`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/fat_errors.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/fat_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: future_fstrings -*-
-import pyFAT_astro
 #Define some errors
 class BadCatalogueError(Exception):
     pass
 class BadConfigurationError(Exception):
     pass
 class BadCubeError(Exception):
     pass
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/fits_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/fits_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,115 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in several different Python scripts in the Database.
 from astropy.io import fits
 from astropy.wcs import WCS
 from datetime import datetime
 from shutil import copyfile
-from pyFAT_astro.Support.fat_errors import FunctionCallError,BadHeaderError,\
-                                        BadCubeError,BadMaskError
+from pyFAT_astro.Support.fat_errors import FunctionCallError,BadCubeError\
+    ,BadMaskError,InputError
+from pyFAT_astro.Support.log_functions import print_log
 import pyFAT_astro.Support.support_functions as sf
 
+
+from make_moments.functions import moments
+
 #from pyFAT_astro.Support.read_functions import obtain_border_pix
-import pyFAT_astro
 from scipy import ndimage
 import numpy as np
 import copy
-import shutil
 import warnings
 import os
 
 #Check that the mask only contains the selected sources
-def check_mask(Configuration,id,Fits_Files):
-    sf.print_log(f'''CHECK_MASK: Checking the mask to contain only the correct source.
+def check_mask(Configuration,id,Fits_Files,SNR= 5.):
+    print_log(f'''CHECK_MASK: Checking the mask to contain only the correct source.
+and to have decent signal noise
 ''',Configuration, case =['debug_start','verbose'])
     if Configuration['DEBUG']:
         copyfile(f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}",f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_Original_Mask.fits")
     mask = fits.open(f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+    mask = check_mask_sources(Configuration,id,mask)
+
+    if SNR < 3.:
+        mask = smooth_mask(Configuration,mask)
+    fits.writeto(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",mask[0].data,\
+            mask[0].header, overwrite = True)
+    # to ensure compatible units and calculations with th models we make the maps ourselves
+    del mask[0].header['C*3']
+    chan_map = np.array(np.nansum(mask[0].data,axis=0),dtype =float)
+    fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_chan.fits",\
+        chan_map,header=mask[0].header,overwrite = True)
+    mask.close()
+    if Configuration['SOFIA_RAN']:
+        print_log('CHECK_MASK: Creating Sofia Moments',Configuration,case=['verbose'])
+        messages = moments(filename =  f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}",\
+                        mask =  f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}",\
+                        overwrite = True, map_velocity_unit= 'km/s',\
+                        debug = Configuration['DEBUG'], log=True,\
+                        output_directory =   f"{Configuration['FITTING_DIR']}/Sofia_Output",\
+                        output_name = f"{Configuration['BASE_NAME']}")
+        print_log(messages,Configuration,case=['verbose'])
+        
+    
+    #moments()
+        #make_moments(Configuration, Fits_Files,fit_type='Generic_Initialize',vel_unit = 'm/s')
+
+check_mask.__doc__ =f'''
+ NAME:
+    check_mask
+
+ PURPOSE:
+    Check that the mask only contains the source we want and if that source
+    has low SNR that it is smoothed with a beam
+
+ CATEGORY:
+    fits_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    id = the SoFiA ID of the source we are interested in
+    Fits_Files = Standard FAT dictionary with filenames
+    Tirific_Template = Standard FAT Tirific Template
+
+ OPTIONAL INPUTS:
+    fit_type = 'Undefined'
+
+ OUTPUTS:
+    moment maps and the channel map
+
+ OPTIONAL OUTPUTS:
+    a cleaned mask
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
 
+def check_mask_sources(Configuration,id,mask):
     if float(id) not in mask[0].data:
-        sf.print_log(f'''CHECK_MASK: We cannot find the selected source in the mask. This will lead to errors. Aborting the fit.
-''',Configuration,case=['main','screen'])
+        print_log(f'''CHECK_MASK: We cannot find the selected source in the mask. This will lead to errors. Aborting the fit.
+    ''',Configuration,case=['main','screen'])
         BadMaskError(f" We can not find the sofia source id in the mask.")
     else:
         data = copy.deepcopy(mask[0].data)
         data[data != float(id)] = 0.
         diff = data-mask[0].data
         neg_index = np.where(diff < 0.)[0]
         if len(neg_index) != 0:
-            sf.print_log(f'''CHECK_MASK: The initial mask had more than a single source. redoing the mask.
-''',Configuration, case = ['verbose'])
+            print_log(f'''CHECK_MASK: The initial mask had more than a single source. redoing the mask.
+    ''',Configuration, case = ['verbose'])
             mask[0].data = data
-            fits.writeto(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",mask[0].data,mask[0].header, overwrite = True)
-# to ensure compatible units and calculations with th models we make the maps ourselves
-    del mask[0].header['C*3']
+
+
     mask[0].data[mask[0].data> 0.5] = 1.
-    chan_map = np.array(np.nansum(mask[0].data,axis=0),dtype =float)
+
     mask[0].header['BITPIX'] = -32
-    fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_chan.fits",chan_map,header=mask[0].header,overwrite = True)
-    mask.close()
-    if Configuration['SOFIA_RAN']:
-        make_moments(Configuration, Fits_Files,fit_type='Generic_Initialize',vel_unit = 'm/s')
-check_mask.__doc__ =f'''
+    return mask
+check_mask_sources.__doc__ =f'''
  NAME:
     check_mask
 
  PURPOSE:
     Check that the mask only contains the source we want and not parts of other nearby sources.
     Subsequently make the channel_map and the moment maps.
 
@@ -75,20 +132,16 @@
     a cleaned mask
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-
-
-
-
 # Create a cube suitable for FAT
-def create_fat_cube(Configuration, Fits_Files,sofia_catalogue=False,\
+def create_fat_cube(Configuration, Fits_Files = None,sofia_catalogue=False,\
         id='No default',name='No default'):
     Configuration['PREPARATION_TIME'][0] = datetime.now()
     #First get the cubes
     if sofia_catalogue:
         Cube = fits.open(f"{Configuration['SOFIA_DIR']}{name}_{id}_cube.fits",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     else:
@@ -101,25 +154,34 @@
         del hdr['NAXIS4']
         hdr['NAXIS'] = 3
     # clean the header
     hdr = sf.clean_header(Configuration,hdr)
     data = prep_cube(Configuration,hdr,data)
     # and write our new cube
 
-    sf.print_log(f'''CREATE_FAT_CUBE: We are writing a FAT modified cube to be used for the fitting. This cube is called {Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE']}
-''',Configuration)
+  
     if sofia_catalogue:
-        fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{name}_FAT_cubelets/{name}_{id}/{name}_{id}_FAT.fits",data,hdr)
+        print_log(f'''CREATE_FAT_CUBE: We are writing a FAT modified cube to be used for the fitting. This cube is called {name}_{id}/{name}_{id}_FAT.fits
+''',Configuration)
+        try:
+            fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{name}_FAT_cubelets/{name}_{id}/{name}_{id}_FAT.fits",data,hdr,overwrite=Configuration['SOFIA_OVERWRITE'])
+        except OSError:
+            raise InputError('pyFAT has already setup this directory, if you want to overwrite the bcubelets please set advanced.sofia_overwrite to True in the configuration')
+
     else:
+        print_log(f'''CREATE_FAT_CUBE: We are writing a FAT modified cube to be used for the fitting. This cube is called {Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE']}
+''',Configuration)
         fits.writeto(Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE'],data,hdr)
     # Release the arrays
 
     Cube.close()
 
     data = []
+    if sofia_catalogue:
+        return hdr
     hdr = []
     Configuration['PREPARATION_TIME'][1] = datetime.now()
 
 create_fat_cube.__doc__ =f'''
  NAME:
     create_fat_cube
 
@@ -147,15 +209,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def cut_cubes(Configuration, Fits_Files, galaxy_box):
-    sf.print_log(f'''CUT_CUBES: Starting to cut the cube_size.
+    print_log(f'''CUT_CUBES: Starting to cut the cube_size.
 ''', Configuration, case= ['debug_start'])
     cube_edge= [6.,5.*round(Configuration['BEAM_IN_PIXELS'][0]),5.*round(Configuration['BEAM_IN_PIXELS'][0])]
     cube_size= []
     new_cube = []
     for i in [2,1,0]:
         cube_size.append(Configuration['NAXES'][i])
         new_cube.append([0,Configuration['NAXES'][i]])
@@ -177,23 +239,23 @@
         files_to_cut = [Fits_Files['FITTING_CUBE'],Fits_Files['MASK'],\
                         Fits_Files['MOMENT0'],\
                         Fits_Files['MOMENT1'],\
                         Fits_Files['MOMENT2'],\
                         Fits_Files['CHANNEL_MAP'],\
                         ]
     if cut:
-        sf.print_log(f'''CUT_CUBES: Your input cube is significantly larger than the detected source.
+        print_log(f'''CUT_CUBES: Your input cube is significantly larger than the detected source.
 {"":8s}CUT_CUBES: we will cut to x-axis = [{new_cube[2,0]},{new_cube[2,1]}] y-axis = [{new_cube[1,0]},{new_cube[1,1]}]
 {"":8s}CUT_CUBES: z-axis = [{new_cube[2,0]},{new_cube[2,1]}].
 {"":8s}CUT_CUBES: We will cut the following files:
 {"":8s}CUT_CUBES: {', '.join(files_to_cut)}
 ''', Configuration)
 
         for file in files_to_cut:
-            sf.print_log(f'''CUT_CUBES: We are cutting the file {file}
+            print_log(f'''CUT_CUBES: We are cutting the file {file}
 ''', Configuration)
             if os.path.exists(f"{Configuration['FITTING_DIR']}{file}"):
                 cutout_cube(Configuration,file,new_cube)
             else:
                 if file == Fits_Files['CHANNEL_MAP']:
                     pass
                 else:
@@ -297,191 +359,29 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-# Extract a PV-Diagrams
-def extract_pv(Configuration,cube_in,angle,center= None,finalsize=None,convert=-1):
-    if center is None:
-        center=[-1,-1,-1]
-    if finalsize is None:
-        finalsize=[-1,-1]
-    sf.print_log(f'''EXTRACT_PV: We are the extraction of a PV-Diagram
-{'':8s} PA = {angle}
-{'':8s} center = {center}
-{'':8s} finalsize = {finalsize}
-{'':8s} convert = {convert}
-''', Configuration, case = ['debug_start'])
-
-
-    cube = copy.deepcopy(cube_in)
-    hdr = copy.deepcopy(cube[0].header)
-    TwoD_hdr= copy.deepcopy(cube[0].header)
-    data = copy.deepcopy(cube[0].data)
-    #Because astro py is even dumber than Python
-    try:
-        if hdr['CUNIT3'].lower() == 'km/s':
-            hdr['CUNIT3'] = 'm/s'
-            hdr['CDELT3'] = hdr['CDELT3']*1000.
-            hdr['CRVAL3'] = hdr['CRVAL3']*1000.
-        elif hdr['CUNIT3'].lower() == 'm/s':
-            hdr['CUNIT3'] = 'm/s'
-    except KeyError:
-        hdr['CUNIT3'] = 'm/s'
-    if center[0] == -1:
-        center = [hdr['CRVAL1'],hdr['CRVAL2'],hdr['CRVAL3']]
-        xcenter,ycenter,zcenter = hdr['CRPIX1'],hdr['CRPIX2'],hdr['CRPIX3']
-    else:
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            coordinate_frame = WCS(hdr)
-        xcenter,ycenter,zcenter = coordinate_frame.wcs_world2pix(center[0], center[1], center[2], 1.)
-
-    nz, ny, nx = data.shape
-    if finalsize[0] != -1:
-        if finalsize[1] >nz:
-            finalsize[1] = nz
-        if finalsize[0] > nx:
-            finalsize[0] = nx
-    # if the center is not set assume the crval values
-
-    sf.print_log(f'''EXTRACT_PV: The shape of the output
-{'':8s} nz = {nz}
-{'':8s} ny = {ny}
-{'':8s} nx = {nx}
-''', Configuration,case=['verbose'])
-    x1,x2,y1,y2 = sf.obtain_border_pix(Configuration,angle,[xcenter,ycenter])
-    linex,liney,linez = np.linspace(x1,x2,nx), np.linspace(y1,y2,nx), np.linspace(0,nz-1,nz)
-    #This only works when ny == nx hence nx is used in liney
-    new_coordinates = np.array([(z,y,x)
-                        for z in linez
-                        for y,x in zip(liney,linex)
-                        ],dtype=float).transpose().reshape((-1,nz,nx))
-    #spatial_resolution = abs((abs(x2-x1)/nx)*np.sin(np.radians(angle)))+abs(abs(y2-y1)/ny*np.cos(np.radians(angle)))
-    PV = ndimage.map_coordinates(data, new_coordinates,order=1)
-    if hdr['CDELT1'] < 0:
-        PV = PV[:,::-1]
-
-    if finalsize[0] == -1:
-        # then lets update the header
-        # As python is stupid making a simple copy will mean that these changes are still applied to hudulist
-        TwoD_hdr['NAXIS2'] = nz
-        TwoD_hdr['NAXIS1'] = nx
-
-        TwoD_hdr['CRPIX2'] = hdr['CRPIX3']
-        TwoD_hdr['CRPIX1'] = xcenter+1
-    else:
-        zstart = sf.set_limits(int(zcenter-finalsize[1]/2.),0,int(nz))
-        zend = sf.set_limits(int(zcenter+finalsize[1]/2.),0,int(nz))
-        xstart = sf.set_limits(int(xcenter-finalsize[0]/2.),0,int(nx))
-        xend = sf.set_limits(int(xcenter+finalsize[0]/2.),0,int(nx))
-
-        PV =  PV[zstart:zend, xstart:xend]
-        TwoD_hdr['NAXIS2'] = int(finalsize[1])
-        TwoD_hdr['NAXIS1'] = int(finalsize[0])
-        TwoD_hdr['CRPIX2'] = hdr['CRPIX3']-int(nz/2.-finalsize[1]/2.)
-        TwoD_hdr['CRPIX1'] = int(finalsize[0]/2.)+1
-
-    if convert !=-1:
-        TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/convert
-        TwoD_hdr['CDELT2'] = hdr['CDELT3']/convert
-    else:
-        TwoD_hdr['CRVAL2'] = hdr['CRVAL3']
-        TwoD_hdr['CDELT2'] = hdr['CDELT3']
-    TwoD_hdr['CTYPE2'] = hdr['CTYPE3']
-    try:
-        if hdr['CUNIT3'].lower() == 'm/s' and convert == 1000. :
-            TwoD_hdr['CDELT2'] = hdr['CDELT3']/1000.
-            TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/1000.
-            TwoD_hdr['CUNIT2'] = 'km/s'
-            del (TwoD_hdr['CUNIT3'])
-        elif  convert != -1:
-            del (TwoD_hdr['CUNIT3'])
-            try:
-                del (TwoD_hdr['CUNIT2'])
-            except KeyError:
-                pass
-        else:
-            TwoD_hdr['CUNIT2'] = hdr['CUNIT3']
-            del (TwoD_hdr['CUNIT3'])
-    except KeyError:
-        sf.print_log(f'''EXTRACT_PV: We could not find units in the header for the 3rd axis.
-''', Configuration)
-    del (TwoD_hdr['CRPIX3'])
-    del (TwoD_hdr['CRVAL3'])
-    del (TwoD_hdr['CDELT3'])
-    del (TwoD_hdr['CTYPE3'])
-    del (TwoD_hdr['NAXIS3'])
-    TwoD_hdr['NAXIS'] = 2
-    TwoD_hdr['CRVAL1'] = 0.
-    #Because we used nx in the linspace for liney we also use it here
-    TwoD_hdr['CDELT1'] = np.sqrt(((x2-x1)*abs(hdr['CDELT1'])/nx)**2+((y2-y1)*abs(hdr['CDELT2'])/nx)**2)*3600.
-
-    TwoD_hdr['CTYPE1'] = 'OFFSET'
-    TwoD_hdr['CUNIT1'] = 'ARCSEC'
-    TwoD_hdr['HISTORY'] = f'EXTRACT_PV: PV diagram extracted with angle {angle} and center {center}'
-    # Then we change the cube and rteturn the PV construct
-    cube[0].header = TwoD_hdr
-    cube[0].data = PV
-
-    return cube
-extract_pv.__doc__ = '''
- NAME:
-    extract_pv
-
- PURPOSE:
-    extract a PV diagram from a cube object. Angle is the PA and center the central location. The profile is extracted over the full length of the cube and afterwards cut back to the finalsize.
-
- CATEGORY:
-     fits_functions
-
- INPUTS:
-    Configuration = Standard FAT Configuration
-    cube_in = is a fits cube object
-    angle = Pa of the slice
-
- OPTIONAL INPUTS:
-    center = [-1,-1,-1]
-    the central location of the slice in WCS map_coordinates [RA,DEC,VSYS], default is the CRVAL values in the header
-
-    finalsize = [-1,-1,-1]
-    final size of the PV-diagram in pixels, default is no cutting
-
-    convert=-1
-    conversion factor for velocity axis, default no conversion
-
- KEYWORD PARAMETERS:
-
- OUTPUTS:
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
-
 
 def prep_cube(Configuration,hdr,data):
-    sf.print_log( f'''PREPROCESSING: starting the preprocessing of the cube
+    print_log( f'''PREPROCESSING: starting the preprocessing of the cube
 ''',Configuration, case = ['debug_start'])
 
     if hdr['CDELT3'] < -1:
-        sf.print_log( f'''PREPROCESSING: Your velocity axis is declining with increasing channels
+        print_log( f'''PREPROCESSING: Your velocity axis is declining with increasing channels
 {"":8s}PREPROCESSING: We reversed the velocity axis.
 ''', Configuration)
         hdr['CDELT3'] = abs(hdr['CDELT3'])
         hdr['CRPIX3'] = hdr['NAXIS3']-hdr['CRPIX3']+1
         data = data[::-1,:,:]
     #Check for zeros
     if np.where(data == 0.):
-        sf.print_log(f'''PREPROCESSING: Your cube contains values exactly 0. If this is padding these should be blanks.
+        print_log(f'''PREPROCESSING: Your cube contains values exactly 0. If this is padding these should be blanks.
 {"":8s}PREPROCESSING: We have changed them to blanks.
 ''', Configuration)
         data[np.where(data == 0.)] = float('NaN')
 
     # check for blank channels and noise statistics
     cube_ok = False
     prev_first_comparison = 0.
@@ -493,29 +393,29 @@
         corner_box_size=int(np.floor(np.mean([hdr['NAXIS1'],hdr['NAXIS2']])/10.))
     while not cube_ok:
         while np.isnan(data[0,:,:]).all():
             data=data[1:,:,:]
             hdr['NAXIS3'] = hdr['NAXIS3']-1
             hdr['CRPIX3'] = hdr['CRPIX3'] - 1
             if hdr['NAXIS3'] < 5:
-                sf.print_log(f'''PREPROCESSING: This cube has too many blanked channels.
+                print_log(f'''PREPROCESSING: This cube has too many blanked channels.
 ''', Configuration,case = ['main', 'screen'])
                 raise BadCubeError("The cube has too many blanked channels")
             log_statement = f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
 '''
-            sf.print_log(f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
+            print_log(f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
 ''', Configuration)
         while np.isnan(data[-1,:,:]).all():
             data=data[:-1,:,:]
             hdr['NAXIS3'] = hdr['NAXIS3']-1
             if hdr['NAXIS3'] < 5:
-                sf.print_log(f'''PREPROCESSING: This cube has too many blanked channels.
+                print_log(f'''PREPROCESSING: This cube has too many blanked channels.
 ''', Configuration,case = ['main', 'screen'])
                 raise BadCubeError("The cube has too many blanked channels")
-            sf.print_log(f'''PREPROCESSING: We are cutting the cube as the last channel is completely blank.
+            print_log(f'''PREPROCESSING: We are cutting the cube as the last channel is completely blank.
 ''', Configuration)
         #Then check the noise statistics
         noise_first_channel = np.nanstd(data[0,:,:])
         noise_last_channel = np.nanstd(data[-1,:,:])
         noise_bottom_right =  np.nanstd(data[:,:corner_box_size,-corner_box_size:])
         noise_top_right =  np.nanstd(data[:,-corner_box_size:,-corner_box_size:])
         noise_bottom_left =  np.nanstd(data[:,:corner_box_size,:corner_box_size])
@@ -527,15 +427,15 @@
         difference = abs((noise_first_channel-noise_last_channel)/noise_first_channel)
         if noise_corner/channel_noise >1.5 and difference < 0.2:
             noise_corner = copy.deepcopy(channel_noise)
         difference2 = abs(channel_noise-noise_corner)/channel_noise
         if difference < 0.2 and np.isfinite(difference) and difference2 < 0.25:
             cube_ok = True
         else:
-            sf.print_log(f'''PREPROCESSING: We are cutting the cube as clearly the noise statistics are off.
+            print_log(f'''PREPROCESSING: We are cutting the cube as clearly the noise statistics are off.
 {"":8s}PREPROCESSING: Noise in the first channel is {noise_first_channel}
 {"":8s}PREPROCESSING: Noise in the last channel is {noise_last_channel}
 {"":8s}PREPROCESSING: Noise in the corners is {noise_corner}
 ''',Configuration,case= ['verbose'])
             first_comparison = abs(noise_first_channel-noise_corner)/noise_corner
             last_comparison = abs(noise_last_channel-noise_corner)/noise_corner
             if prev_first_comparison == 0:
@@ -559,31 +459,31 @@
                     data=data[:-1,:,:]
                     hdr['NAXIS3'] = hdr['NAXIS3'] - 1
                 else:
                     cube_ok = True
 
             if times_cut_first_channel >= 8 and times_cut_last_channel >= 8:
                 cube_ok = True
-                sf.print_log( f'''PREPROCESSING: This cube has non-uniform noise statistics.'
+                print_log( f'''PREPROCESSING: This cube has non-uniform noise statistics.'
 ''',Configuration)
             if hdr['NAXIS3'] < 5:
-                sf.print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
+                print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
 ''',Configuration,case = ['main','screen'])
                 raise BadCubeError('The Cube has noise statistics that cannot be dealt with')
     if ~np.isfinite(noise_corner):
-        sf.print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
+        print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
 ''',Configuration,case = ['main','screen'])
         raise BadCubeError('The Cube has noise statistics that cannot be dealt with')
     #hdr['FATNOISE'] = noise_corner
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         low_noise_indices = np.where(data < -10*noise_corner)
     if len(low_noise_indices) > 0.0001*hdr['NAXIS1']*hdr['NAXIS2']*hdr['NAXIS3']:
         data[low_noise_indices] = float('NaN')
-        sf.print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
+        print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
 {"":8s}PREPROCESSING: We blanked these values.
 ''',Configuration)
 
     #Let's make sure that a central absorption source is treated the same regardless od the size of the cube
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         buffer=5.*hdr['BMAJ']/np.mean([abs(hdr['CDELT1']),abs(hdr['CDELT2'])])
@@ -592,15 +492,15 @@
 
         central_noise_indices = np.where(central < -10*noise_corner)
     if len(central_noise_indices) > 0.0001*4*buffer*hdr['NAXIS3']:
         central[central_noise_indices] = float('NaN')
         data[:,int(hdr['NAXIS2']/2.-buffer):int(hdr['NAXIS2']/2.+buffer),\
                         int(hdr['NAXIS1']/2.-buffer):int(hdr['NAXIS1']/2.+buffer)] =\
                         central
-        sf.print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
+        print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
 {"":8s}PREPROCESSING: We blanked these values.
 ''',Configuration)
 
 
     # Check whether any channels got fully blanked
     blanked_channels = []
     for z in range(hdr['NAXIS3']):
@@ -612,15 +512,15 @@
     #Previously SoFiA was not dealing with blanks properly and the statement went here
     #finally we want to get the noise level from the negative in the final cube
 
     new_noise = np.nanstd(np.hstack([data[data<0],-1.*data[data<0]]))
     #If we have noiseles cubes this will be far to low
     if abs(new_noise/np.mean([channel_noise,noise_corner])) > 4. \
         or abs(new_noise/np.mean([channel_noise,noise_corner])) < 0.25:
-            sf.print_log(f'''PREPROCESSING: There is something odd in the noise statistics of your cube. We are not using the nehgative values
+            print_log(f'''PREPROCESSING: There is something odd in the noise statistics of your cube. We are not using the nehgative values
 ''',Configuration)
             #new_noise = np.mean([channel_noise,noise_corner])
     hdr['FATNOISE'] = new_noise
 
     return data
 prep_cube.__doc__ =f'''
  NAME:
@@ -655,32 +555,32 @@
 def optimized_cube(Configuration,Fits_Files):
     pix_per_beam = Configuration['BEAM_IN_PIXELS'][1]
     if pix_per_beam > Configuration['OPT_PIXEL_BEAM']:
         cube = fits.open(Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE'])
         data = cube[0].data
         hdr = cube[0].header
         if f"{abs(hdr['CDELT1']):.16f}" != f"{abs(hdr['CDELT2']):.16f}":
-            sf.print_log(f'''OPTIMIZED_CUBE: Your input cube does not have square pixels.
+            print_log(f'''OPTIMIZED_CUBE: Your input cube does not have square pixels.
 {"":8s}OPTIMIZED_CUBE: FAT cannot optimize your cube.
 ''', Configuration)
         cube.close()
         required_cdelt = hdr['BMIN']/int(Configuration['OPT_PIXEL_BEAM'])
         ratio = required_cdelt/abs(hdr['CDELT2'])
         opt_data,opt_hdr = regrid_cube(data, hdr, ratio)
 
         fits.writeto(Configuration['FITTING_DIR']+Fits_Files['OPTIMIZED_CUBE'], opt_data,opt_hdr)
 
         Configuration['OPTIMIZED'] = True
-        sf.print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
+        print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
 {"":8s}OPTIMIZED_CUBE: You requested { Configuration['OPT_PIXEL_BEAM']} therefore we regridded the cube into a new cube.
 {"":8s}OPTIMIZED_CUBE: We are using the pixel size of {required_cdelt}.
 ''', Configuration)
 
     else:
-        sf.print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
+        print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
 {"":8s}OPTIMIZED_CUBE: You requested {Configuration['OPT_PIXEL_BEAM']} but we cannot improve the resolution.
 {"":8s}OPTIMIZED_CUBE: We are using the pixel size of the original cube.
 ''', Configuration)
 optimized_cube.__doc__ =f'''
  NAME:
     optimized_cube
 
@@ -705,165 +605,14 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def make_moments(Configuration,Fits_Files,fit_type = 'Undefined',
-                 moments = None,overwrite = False, level=None,
-                  vel_unit= None):
-    if moments is None:
-        moments = [0,1,2]
-    sf.print_log(f'''MAKE_MOMENTS: We are starting to create the moment maps.
-''',Configuration, case = ['debug_start'])
-    if fit_type == 'Generic_Initialize':
-        filename = f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}"
-        basename = f"{Configuration['BASE_NAME']}"
-        directory = f"{Configuration['FITTING_DIR']}/Sofia_Output/"
-        mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
-    elif fit_type == 'Generic_Final':
-        filename = f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits"
-        basename = 'Finalmodel'
-        directory = f"{Configuration['FITTING_DIR']}/Finalmodel/"
-        mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
-    else:
-        filename = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.fits"
-        basename = fit_type
-        directory = f"{Configuration['FITTING_DIR']}{fit_type}"
-        if not level:
-            mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
-
-    cube = fits.open(filename)
-    if vel_unit:
-        cube[0].header['CUNIT3'] = vel_unit
-    if mask_cube:
-        mask = fits.open(mask_cube)
-        with np.errstate(invalid='ignore', divide='ignore'):
-            cube[0].data[mask[0].data < 0.5] = float('NaN')
-        mask.close()
-    else:
-        if not level:
-            level = 3.*np.mean([np.nanstd(cube[0].data[0:2,:,:]),np.nanstd(cube[0].data[-3:-1,:,:])])
-        with np.errstate(invalid='ignore', divide='ignore'):
-            cube[0].data[cube[0].data < level] = float('NaN')
-    try:
-        if cube[0].header['CUNIT3'].lower().strip() == 'm/s':
-            sf.print_log(f"MAKE_MOMENTS: We convert your m/s to km/s. \n", Configuration, case=['verbose'])
-            cube[0].header['CUNIT3'] = 'km/s'
-            cube[0].header['CDELT3'] = cube[0].header['CDELT3']/1000.
-            cube[0].header['CRVAL3'] = cube[0].header['CRVAL3']/1000.
-        elif cube[0].header['CUNIT3'].lower().strip() == 'km/s':
-            pass
-        else:
-            sf.print_log(f"MAKE_MOMENTS: Your Velocity unit {cube[0].header['CUNIT3']} is weird. Your units could be off", Configuration)
-    except KeyError:
-        sf.print_log(f"MAKE_MOMENTS: Your CUNIT3 is missing, that is bad practice. We'll add a blank one but we're not guessing the value", Configuration)
-        cube[0].header['CUNIT3'] = 'Unknown'
-    #Make a 2D header to use
-    hdr2D = copy.deepcopy(cube[0].header)
-    hdr2D.remove('NAXIS3')
-    hdr2D['NAXIS'] = 2
-    # removing the third axis means we cannot correct for varying platescale, Sofia does so this is and issue so let's not do this
-    hdr2D.remove('CDELT3')
-    hdr2D.remove('CTYPE3')
-    hdr2D.remove('CUNIT3')
-    hdr2D.remove('CRPIX3')
-    hdr2D.remove('CRVAL3')
-
-    # we need a moment 0 for the moment 2 as well
-    if 0 in moments:
-        hdr2D['BUNIT'] = f"{cube[0].header['BUNIT']}*{cube[0].header['CUNIT3']}"
-        moment0 = np.nansum(cube[0].data, axis=0) * cube[0].header['CDELT3']
-        moment0[np.invert(np.isfinite(moment0))] = float('NaN')
-        try:
-            hdr2D['DATAMAX'] = np.nanmax(moment0)
-            hdr2D['DATAMIN'] = np.nanmin(moment0)
-            fits.writeto(f"{directory}/{basename}_mom0.fits",moment0,hdr2D,overwrite = overwrite)
-        except ValueError:
-            sf.print_log(f"MAKE_MOMENTS: Your Moment 0 has bad data and we could not write the moment 0 fits file", Configuration)
-
-
-
-    if 1 in moments or 2 in moments:
-        zaxis = cube[0].header['CRVAL3'] + (np.arange(cube[0].header['NAXIS3'])+1 \
-              - cube[0].header['CRPIX3']) * cube[0].header['CDELT3']
-        c=np.transpose(np.resize(zaxis,[cube[0].header['NAXIS1'],cube[0].header['NAXIS2'],len(zaxis)]),(2,1,0))
-        hdr2D['BUNIT'] = f"{cube[0].header['CUNIT3']}"
-        # Remember Python is stupid so z,y,x
-        with np.errstate(invalid='ignore', divide='ignore'):
-            moment1 = np.nansum(cube[0].data*c, axis=0)/ np.nansum(cube[0].data, axis=0)
-        moment1[np.invert(np.isfinite(moment1))] = float('NaN')
-        try:
-            hdr2D['DATAMAX'] = np.nanmax(moment1)
-            hdr2D['DATAMIN'] = np.nanmin(moment1)
-            if 1 in moments:
-                fits.writeto(f"{directory}/{basename}_mom1.fits",moment1,hdr2D,\
-                    overwrite = overwrite)
-
-        except ValueError:
-            sf.print_log(f"MAKE_MOMENTS: Your Moment 1 has bad data and we could not write the moment 0 fits file", Configuration)
-
-        if 2 in moments:
-            d = c - np.resize(moment1,[len(zaxis),cube[0].header['NAXIS2'],cube[0].header['NAXIS1']])
-            with np.errstate(invalid='ignore', divide='ignore'):
-                moment2 = np.sqrt(np.nansum(cube[0].data*d**2, axis=0)/ np.nansum(cube[0].data, axis=0))
-            moment2[np.invert(np.isfinite(moment1))] = float('NaN')
-            try:
-                hdr2D['DATAMAX'] = np.nanmax(moment2)
-                hdr2D['DATAMIN'] = np.nanmin(moment2)
-                fits.writeto(f"{directory}/{basename}_mom2.fits",\
-                    moment2,hdr2D,overwrite = overwrite)
-
-            except ValueError:
-                sf.print_log(f"MAKE_MOMENTS: Your Moment 1 has bad data and we could not write the moment 0 fits file", Configuration)
-
-    cube.close()
-
-make_moments.__doc__ =f'''
- NAME:
-    make_moments
-
- PURPOSE:
-    Make the moment maps
-
- CATEGORY:
-    fits_functions
-
- INPUTS:
-    Configuration = Standard FAT configuration
-    Fits_Files = Standard FAT dictionary with filenames
-
-
- OPTIONAL INPUTS:
-    fit_type = 'Undefined'
-    type of ftting
-
-    moments = [0,1,2]
-    moment maps to create
-
-    overwrite = False
-    overwrite existing maps
-
-    level=None
-    cutoff level to use, if set the mask will not be used
-
-    vel_unit= none
-    velocity unit of the input cube
-
- OUTPUTS:
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
-
 def regrid_cube(data,hdr,ratio):
     regrid_hdr = copy.deepcopy(hdr)
     # First get the shape of the data
     shape = np.array(data.shape, dtype=float)
     #The new shape has to be integers
     new_shape = [int(x/ratio) for x in shape]
     # Which means our real ratio is
@@ -963,7 +712,47 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     scipy.ndimage.map_coordinates, np.array, np.mgrid
 
  NOTE:
 '''
+
+def smooth_mask(Configuration,mask):
+    print_log(f'''SMOOTH_MASK: Starting smooth mask
+''', Configuration)
+
+    # First we smooth the mask
+    mask_data = np.array(mask[0].data,dtype=float)
+    mask_data = ndimage.gaussian_filter(mask_data,sigma=(0.,\
+        Configuration['BEAM_IN_PIXELS'][1] / np.sqrt(8 * np.log(2)),\
+        Configuration['BEAM_IN_PIXELS'][0] / np.sqrt(8 * np.log(2))),order=0)
+    mask_data[mask_data > 0.05] = 1.
+    mask_data[mask_data < 0.05] = 0.
+    mask[0].data=mask_data
+    return mask
+    #reaplly it to get the moments
+
+
+    # If we have a lot of pixels and stuff we need smooth more
+    #So we take the inverse of the initial factor with a standard of 0.75 minimum of 0.5 and a maximum of 1.25
+
+smooth_mask.__doc__ =f'''
+ NAME:
+    smooth_mask
+ PURPOSE:
+    smooth the mask with a beam
+ CATEGORY:
+    fits_functions
+
+ INPUTS:
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+
+ NOTE:
+'''
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/modify_template.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/modify_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,46 +3,55 @@
 
 
 
 import copy
 
 from pyFAT_astro.Support.fat_errors import InitializeError,CfluxError,\
     FunctionCallError,BadConfigurationError,FittingError,FaintSourceError
+from pyFAT_astro.Support.log_functions import print_log
+
 import pyFAT_astro.Support.support_functions as sf
-import pyFAT_astro
 
 import numpy as np
-import os
 import warnings
+from math import isclose
 from scipy.optimize import curve_fit, OptimizeWarning
 from scipy.signal import savgol_filter
-from scipy.interpolate import CubicSpline,Akima1DInterpolator
-
+from scipy.interpolate import CubicSpline
 
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import matplotlib
+    matplotlib.use('pdf')
+    import matplotlib.pyplot as plt
+    import matplotlib.gridspec as gridspec
+    from matplotlib.patches import Ellipse
 
 def apply_new_size(Configuration, new_size ):
     ''' Check whether we want to apply our new size '''
     # we want to have at least a quarter beam difference to apply the size.
-
-    difference = [abs(Configuration['SIZE_IN_BEAMS'][x]-new_size[x]) for x in [0,1]]
-
-
-    if all([(x < Configuration['RING_SIZE']/2.) for x in difference]):
-        sf.print_log(f'''APPLY_NEW_SIZE: The new sizes equal those of the previous fit. Not changing
-''', Configuration,case=['verbose'])
-        return False
-    sf.print_log(f'''APPLY_NEW_SIZE: The new sizes differ from those of the previous fit.
-''', Configuration,case=['verbose'])
+    apply_size = [True,True]
+   
     for i in [0,1]:
-        for sizes in Configuration['OLD_SIZE'][:-1]:
-            if abs(sizes[i] - new_size[i]) < Configuration['RING_SIZE']/2.:
-                sf.print_log(f'''APPLY_NEW_SIZE: The side {i} has been fitted before fixing it.
+        if Configuration['FIX_SIZE'][i]:
+            apply_size[i] = False
+            print_log(f'''APPLY_NEW_SIZE: The size on side {i} is Fixed. Not changing
+''', Configuration,case=['verbose']) 
+        elif abs(Configuration['SIZE_IN_BEAMS'][i]-new_size[i]) < \
+            Configuration['RING_SIZE']/2.:
+            apply_size[i] = False
+            print_log(f'''APPLY_NEW_SIZE: The size on side {i} is equal to that of the previous fit. Not changing
+''', Configuration,case=['verbose'])    
+        else: 
+            for sizes in Configuration['OLD_SIZE'][:-1]:
+                if abs(sizes[i] - new_size[i]) < Configuration['RING_SIZE']/2.:
+                    print_log(f'''APPLY_NEW_SIZE: The side {i} has been fitted before, fixing it to the new size.
 ''', Configuration,case=['verbose'])
-                Configuration['FIX_SIZE'][i] = True
-    return True
+                    Configuration['FIX_SIZE'][i] = True        
+    return apply_size
 apply_new_size.__doc__ =f'''
  NAME:
     apply new size
 
  PURPOSE:
     determine whether the newly calculated size should be written to the configuration
     by comparing to previous sizes
@@ -137,45 +146,59 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def calc_new_size(Configuration,Tirific_Template,radii,sbr_in,sbr_ring_limits ):
+    print_log(f'''CALC_NEW_SIZE: Starting to calculate the new size
+''',Configuration,case=['debug_start'])
 
     sbr=copy.deepcopy(sbr_in)
 
     for i in [0,1]:
         if sbr[i,-1] > 5*  sbr[i,-2]:
               sbr[i,-1]= 0.8*sbr[i,-2]
 
     sm_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',
                             min_error= sbr_ring_limits,no_apply = True,
                             fix_sbr_call = True, profile_in = sbr )
     old_size = copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
+    print_log(f'''CALC_NEW_SIZE: The old size = {old_size}
+''',Configuration,case=['debug_add'])
     new_size = copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
     difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
-    smooth_diff = smooth_profile(Configuration,{'EMPTY':None}, 'ARBITRARY' ,\
+    print_log(f'''CALC_NEW_SIZE: We find the following limiting SBR 
+{'':8s} sbr = {sbr}
+{'':8s} sbr_limits = {sbr_ring_limits}
+{'':8s} difference_with_limit = {difference_with_limit}
+''',Configuration,case=['debug_add'])
+    smooth_diff = smooth_profile(Configuration,{'EMPTY':None}, 'SMOOTH_DIFFERENCE' ,\
         profile_in=difference_with_limit, min_error=[0.,0.],no_fix=True,no_apply=True)
-    sf.print_log(f'''CALC_NEW_SIZE: We find the following smoothed difference profile:
+    print_log(f'''CALC_NEW_SIZE: We find the following smoothed difference profile:
 {'':8s} smooth_diff = {smooth_diff}
-''',Configuration,case=['debug_start'])
+''',Configuration,case=['debug_add'])
     for i in [0,1]:
         #If all last three values are above the limit we need to extend
         if np.all(smooth_diff[i,-3:] > 0.):
             #We fit a Gaussian to the SBR and see where it drops below the last SBR Limit
             try:
                 vals = sf.fit_gaussian(Configuration,radii,sm_sbr[i,:],errors=sbr_ring_limits[i,:])
                 extend_radii = np.linspace(0.,Configuration['MAX_SIZE_IN_BEAMS']*Configuration['BEAM'][0],1000)
-                Gauss_diff = sf.gaussian_function(extend_radii,*vals)-sbr_ring_limits[i,-1]
+                Gauss_profile = sf.gaussian_function(extend_radii,*vals)
+                Gauss_diff = Gauss_profile-sbr_ring_limits[i,-1]
                 this_size=sf.set_limits(extend_radii[np.where(Gauss_diff < 0.)[0][0]]/Configuration['BEAM'][0]+0.5, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
             except FittingError:
+                print_log(f'''CALC_NEW_SIZE: We failed to fit a Gaussian
+''',Configuration,case=['debug_add'])
                 #If we cannot fit a gaussian we extend by a beam
                 this_size=sf.set_limits(radii[-1]/Configuration['BEAM'][0]+1.0, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
             except IndexError:
+                print_log(f'''CALC_NEW_SIZE: We failed to find where the GAussian drop below 0.
+''',Configuration,case=['debug_add'])
                 #If we do not find any values in the gaussian below the limits we extend 2 beams
                 this_size=sf.set_limits(radii[-1]/Configuration['BEAM'][0]+2.0, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
 
             if this_size > new_size[i]+0.5:
                 new_size[i]= copy.deepcopy(this_size)
         else:
             #we need to find where we cross the zero line
@@ -193,28 +216,28 @@
             x1 = float(radii[loc-1])
             x2 = float(radii[loc])
             y1 = float(smooth_diff[i,loc-1])
             y2 = float(smooth_diff[i,loc])
             this_size = sf.set_limits((x1+y1*(x2-x1)/(y1-y2))/Configuration['BEAM'][0],Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
 
 
-            sf.print_log(f'''CALC_NEW_SIZE: The profile for {i} drop below 0. between {x1} and {x2}.
+            print_log(f'''CALC_NEW_SIZE: The profile for {i} drops below zero between {x1} and {x2}.
 {'':8s} with y1 = {y1} and y2 = {y2}
 {'':8s} the new size is {this_size}
 ''',Configuration,case= ['debug_add'])
             if this_size < new_size[i]-0.5:
                 new_size[i]= copy.deepcopy(this_size)
         if Configuration['FIX_RING_SIZE']:
             real_size = new_size[i]-1./5.
             rings = int(real_size/Configuration['RING_SIZE'])
             new_size[i] = rings * Configuration['RING_SIZE']+1./5.
         if new_size[i] < Configuration['TOO_SMALL_GALAXY']:
              new_size[i] = Configuration['TOO_SMALL_GALAXY']
 
-    sf.print_log(f'''CALC_NEW_SIZE: We have the new_size {new_size} compared to what we had before {old_size}
+    print_log(f'''CALC_NEW_SIZE: We have the new_size {new_size} compared to what we had before {old_size}
 ''',Configuration,case = ['debug_add'])
 
     return new_size
 calc_new_size.__doc__ =f'''
  NAME:
     calc_new_size
 
@@ -240,52 +263,51 @@
 
  PROCEDURES CALLED:
     Unspecified
 NOTE:
     The new size is neveer applied to Configuration
 '''
 
-def calculate_change_boundary(Configuration,multiple_used,theta_zero,phi_zero ):
+def calculate_change_boundary(Configuration,multiple,theta_zero,phi_zero,
+                              pa_boun = None, incl_boun = None ):
     change_boundary = []
-    for i in range(3):
-        if i == 0:
-            multiple=multiple_used[0]
-        else:
-            multiple=multiple_used[i-1]
-        poss_theta_bound= []
-        poss_phi_bound = []
-        #we need theta and phi for all options of PA and INCL
-        pa_lim= [Configuration['PA_CURRENT_BOUNDARY'][i][0],\
-                Configuration['PA_CURRENT_BOUNDARY'][i][0],\
-                Configuration['PA_CURRENT_BOUNDARY'][i][1],\
-                Configuration['PA_CURRENT_BOUNDARY'][i][1]]
-        incl_lim = [Configuration['INCL_CURRENT_BOUNDARY'][i][0],\
-                Configuration['INCL_CURRENT_BOUNDARY'][i][1],\
-                Configuration['INCL_CURRENT_BOUNDARY'][i][0],\
-                Configuration['INCL_CURRENT_BOUNDARY'][i][1]]
-        for x,y in zip(pa_lim,incl_lim):
-            theta_tmp,phi_tmp,multiple_tmp = sf.calculate_am_vector(Configuration,[x],[y])
-            # if the multiples do not correspond in the vector can be infinite
-
-            if multiple_tmp[0] != multiple:
-                poss_theta_bound.append(float('NaN'))
-                poss_phi_bound.append(float('NaN'))
-            else:
-                poss_theta_bound.append(float(theta_tmp))
-                poss_phi_bound.append(float(phi_tmp))
-        minimum = -1*np.sqrt(np.min(np.array([x-theta_zero[0] for x in poss_theta_bound],dtype=float))**2\
-                            +np.min(np.array([x-phi_zero[0] for x in poss_phi_bound],dtype=float))**2)
-        maximum = np.sqrt(np.max(np.array([x-theta_zero[0] for x in poss_theta_bound],dtype=float))**2\
-                            +np.max(np.array([x-phi_zero[0] for x in poss_phi_bound],dtype=float))**2)
-        if np.isnan(minimum):
-            minumum = 0.
-        if np.isnan(maximum):
-            maximum = 0.
-        change_boundary.append([minimum,maximum])
-    return change_boundary
+    if pa_boun is None:
+       pa_boun = [Configuration['PA_CURRENT_BOUNDARY'][1][0],
+                 Configuration['PA_CURRENT_BOUNDARY'][1][1]] 
+    if incl_boun is None:
+       incl_boun = [Configuration['INCL_CURRENT_BOUNDARY'][1][0],
+                 Configuration['INCL_CURRENT_BOUNDARY'][1][1]] 
+    
+    poss_theta_bound= []
+    poss_phi_bound = []
+    #we need theta and phi for all options of PA and INCL
+    limit_combined = []
+    for i in [0,1]:
+        for j in [0,1]:
+            limit_combined.append([pa_boun[i],incl_boun[j]])
+
+    for lim in limit_combined:
+        theta_tmp,phi_tmp,multiple_tmp = sf.calculate_am_vector(Configuration,[lim[0]],[lim[1]])
+        # if the multiples do not correspond in the vector can be infinite
+        if multiple_tmp[0] != multiple:
+            poss_theta_bound.append(float('NaN'))
+            poss_phi_bound.append(float('NaN'))
+        else:
+            poss_theta_bound.append(float(theta_tmp))
+            poss_phi_bound.append(float(phi_tmp))
+    minimum = -1*np.sqrt(np.min(np.array([x-theta_zero for x in poss_theta_bound],dtype=float))**2\
+                +np.min(np.array([x-phi_zero for x in poss_phi_bound],dtype=float))**2)
+    maximum = np.sqrt(np.max(np.array([x-theta_zero for x in poss_theta_bound],dtype=float))**2\
+                +np.max(np.array([x-phi_zero for x in poss_phi_bound],dtype=float))**2)
+    if np.isnan(minimum):
+        minumum = 0.
+    if np.isnan(maximum):
+        maximum = 0.
+    
+    return [minimum,maximum]
 
 calculate_change_boundary.__doc__ =f'''
  NAME:
     calculate_change_boundary
 
  PURPOSE:
     when regularising the PA and incl we do this through the change in the am vector
@@ -321,81 +343,86 @@
     changed_angles=False
     incl_in = sf.load_tirific(Configuration,Tirific_Template,Variables= ['INCL','INCL_2'])
     pa_in = sf.load_tirific(Configuration,Tirific_Template,Variables= ['PA','PA_2'])
     incl = copy.deepcopy(incl_in)
     pa = copy.deepcopy(pa_in)
     rad =[float(x) for x in Tirific_Template['RADI'].split()]
 
-    sf.print_log(f'''CHECK_ANGLES: We start with
+    print_log(f'''CHECK_ANGLES: We start with
 {'':8s} radius = {rad}
 {'':8s} PA appr = {pa[0]}
 {'':8s} PA rec = {pa[1]}
 {'':8s} INCL appr = {incl[0]}
 {'':8s} INCL rec = {incl[1]}
 {'':8s} Changed_Angle = {changed_angles}
 ''', Configuration,case=['debug_start'])
 
     for side in [0,1]:
         incl_too_large = (np.array(incl[side],dtype=float) > 90.)
         if incl_too_large.any():
 
-            sf.print_log(f'''CHECK_ANGLES: Several INCL values were too large
+            print_log(f'''CHECK_ANGLES: Several INCL values were too large
 ''', Configuration,case = ['verbose'])
             incl[side] = [180.-x if y else x for x,y in zip(incl[side],incl_too_large)]
             #changed_angles = True
 
         pa_too_large = (np.array(pa[side],dtype=float) > 360.)
         if pa_too_large.any():
             if np.mean(np.array(pa[side],dtype=float)[~pa_too_large]) < 180.:
                 pa[side] = [x-360. if y else x for x,y in zip(pa[side],pa_too_large)]
                 #changed_angles = True
-                sf.print_log(f'''CHECK_ANGLES: Several PA values were too large
+                print_log(f'''CHECK_ANGLES: Several PA values were too large
 ''', Configuration,case=['verbose'])
 
         pa_too_small = (np.array(pa[side],dtype=float) < 0.)
         if pa_too_small.any():
             if np.mean(np.array(pa[side],dtype=float)[~pa_too_small]) > 180.:
                 pa[side] = [x+360. if y else x for x,y in zip(pa[side],pa_too_small)]
                 #changed_angles = True
 
-                sf.print_log(f'''CHECK_ANGLES: Several PA values were too small
+                print_log(f'''CHECK_ANGLES: Several PA values were too small
 ''', Configuration,case=['verbose'])
         pa_tmp,incl_tmp,changed_angles = sf.check_angular_momentum_vector(Configuration,\
                                             rad,pa[side],incl[side],modified= changed_angles,\
                                             side=side)
         #pa_tmp = sf.max_profile_change(Configuration,rad,pa[side],'PA',slope = Configuration['WARP_SLOPE'][side])
         pa[side] = pa_tmp
         #incl_tmp = sf.max_profile_change(Configuration,rad,incl[side],'INCL',slope = Configuration['WARP_SLOPE'][side])
         incl[side] = incl_tmp
 
         #exit()
 
     #Ensure that we have not made PA differences
     if pa[0][0] != pa[1][0]:
         if abs( pa[0][0]-pa[1][0]) > Configuration['MIN_ERROR']['PA'][0]:
-            sf.print_log(f'''CHECK_ANGLES: The central PA differs by too much:
+            print_log(f'''CHECK_ANGLES: The central PA differs by too much:
 {'':8s} differece = { abs( pa[0][0]-pa[1][0])}, max allowed = {Configuration['MIN_ERROR']['PA'][0]}
     ''', Configuration,case=['verbose'])
+            # We need to fix them if we have.
+            mean_pa = np.mean([pa[0][:Configuration['INNER_FIX'][0]],pa[1][:Configuration['INNER_FIX'][1]]])
+            pa[0][:Configuration['INNER_FIX'][0]+1] = mean_pa
+            pa[1][:Configuration['INNER_FIX'][1]+1] = mean_pa
+                 
             changed_angles = True
         else:
-            sf.print_log(f'''CHECK_ANGLES: We correct some computational changes in the PA
+            print_log(f'''CHECK_ANGLES: We correct some computational changes in the PA
     ''', Configuration,case=['verbose'])
         if (pa[0][0] > 360. and pa[1][0] < 360.) or \
             (pa[0][0] < 0. and pa[1][0] > 0.):
                 pa[0][0:3] = pa[1][0:3]
         elif(pa[0][0] < 360. and pa[1][0] > 360.) or \
             (pa[0][0] > 0. and pa[1][0] < 0.):
                 pa[1][0:3] = pa[0][0:3]
 
 
     Tirific_Template['INCL'] = f"{' '.join(f'{x:.2e}' for x in incl[0])}"
     Tirific_Template['INCL_2'] = f"{' '.join(f'{x:.2e}' for x in incl[1])}"
     Tirific_Template['PA'] = f"{' '.join(f'{x:.2e}' for x in pa[0])}"
     Tirific_Template['PA_2'] = f"{' '.join(f'{x:.2e}' for x in pa[1])}"
-    sf.print_log(f'''CHECK_ANGLES: We wrote to the template
+    print_log(f'''CHECK_ANGLES: We wrote to the template
 {'':8s} PA appr = {Tirific_Template['PA']}
 {'':8s} PA rec = {Tirific_Template['PA_2']}
 {'':8s} INCL appr = {Tirific_Template['INCL']}
 {'':8s} INCL rec = {Tirific_Template['INCL_2']}
 ''', Configuration,case=['verbose'])
 
     return changed_angles
@@ -429,55 +456,58 @@
 
  NOTE:
 '''
 
 
 def check_flat(Configuration,profile,error,key, last_reliable_ring = -1,\
                 inner_fix = 4):
+    last_reliable_ring +=2
     if last_reliable_ring == -1 or last_reliable_ring > len(profile)-1:
-        last_reliable_ring = len(profile)-1
+        last_reliable_ring = len(profile)
 
-    sf.print_log(f'''CHECK_FLAT: checking flatness
+    print_log(f'''CHECK_FLAT: checking flatness
 {'':8s}profile = {profile}
 {'':8s}error = {error}
 {'':8s}last_reliable_ring = {last_reliable_ring}
 ''',Configuration, case= ['debug_start'])
 
     inner = np.mean(profile[:inner_fix])
-    mean_error = np.mean(error[:last_reliable_ring])
+   
     if inner_fix+1 < last_reliable_ring:
+        mean_error = np.mean(error[inner_fix+1:last_reliable_ring])
         outer = np.mean(profile[inner_fix+1:last_reliable_ring])
         outer_std = np.std(profile[inner_fix+1:last_reliable_ring])
     else:
         outer = inner
         outer_std = np.mean(error)
+        mean_error = np.mean(error)
 
     if key in ['SDIS']:
         mean_error = mean_error*0.5
         outer_std = 2.*mean_error
     if abs(outer-inner) < mean_error or outer_std  < mean_error:
-        sf.print_log(f'''CHECK_FLAT: If  {abs(outer-inner)} less than {mean_error} or
-{'':8s} The outer variation {outer_std} less than the median error {mean_error} we break and set flat.
+        print_log(f'''CHECK_FLAT: If  {abs(outer-inner)} less than {mean_error} or
+{'':8s} the outer variation {outer_std} less than the median error {mean_error} we break and set flat.
 ''',Configuration, case=['debug_add'])
         return True
     if key in ['INCL','INCL_2']:
         if outer < 40. or inner < 40.:
-            sf.print_log(f'''CHECK_FLAT: If  the outer profile is {outer} hence we set this to flat.
+            print_log(f'''CHECK_FLAT: the outer profile is low inclination {outer} hence we set this to flat.
 ''',Configuration, case=['debug_add'])
             return True
 
     for e,x,y in zip(error[1:last_reliable_ring],profile[1:last_reliable_ring],profile[0:last_reliable_ring]):
-        sf.print_log(f'''CHECK_FLAT: x = {x}, y = {y}, e = {e}
+        print_log(f'''CHECK_FLAT: x = {x}, y = {y}, e = {e}
 ''',Configuration, case=['debug_add'])
         if not x-e/2. < y < x+e/2.:
-            sf.print_log(f'''CHECK_FLAT: This taco is bend
+            print_log(f'''CHECK_FLAT: This taco is bend
 ''',Configuration, case=['debug_add'])
             return False
 
-    sf.print_log(f'''CHECK_FLAT: All values were within the error of eachother
+    print_log(f'''CHECK_FLAT: All values were within the error of eachother
 ''',Configuration, case=['debug_add'])
     return True
 check_flat.__doc__ = '''
  NAME:
     check_flat
 
  PURPOSE:
@@ -507,84 +537,88 @@
 
  NOTE:
 '''
 
 def check_size(Configuration,Tirific_Template, fit_type = 'Undefined', \
         stage = 'initial', Fits_Files= 'No Files' ,current_run='Not Initialized',
         no_apply=False):
-
-    sf.print_log(f'''CHECK_SIZE: Starting check_size with the following parameters:
+    print_log(f'''CHECK_SIZE: Starting check_size with the following parameters:
 {'':8s}Rings = {Configuration['NO_RINGS']}, Size in Beams = {Configuration['SIZE_IN_BEAMS']}
-''',Configuration,case=['debug_start'])
+{'':8s}The Rings isze we use = {Configuration['RING_SIZE']}
+''',Configuration,case=['debug_start','verbose'])
 
 
-    radii, sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
+    sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
     #get the sbr profiles
 
     sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
         array=True)
+    radii = sf.load_tirific(Configuration,Tirific_Template,Variables=['RADI'],\
+        array=True)
     if len(sbr[0]) != len(sbr_ring_limits):
         #Check what the appropriate size should be
 
-        sf.print_log(f'''CHECK_SIZE: Equalizing the sizes
+        print_log(f'''CHECK_SIZE: Equalizing the sizes
 ''',Configuration,case= ['debug_add'])
         if len(sbr[0]) != Configuration['NO_RINGS']:
 
-            sf.print_log(f'''CHECK_SIZE: Interpolating SBR
+            print_log(f'''CHECK_SIZE: Interpolating SBR
 ''',Configuration,case= ['debug_add'])
             old_radii = np.array(sf.load_tirific(Configuration,Tirific_Template, ['RADI']),dtype = float)
             for i in [0,1]:
                 sbr[i] = np.interp(np.array(radii,dtype=float),np.array(old_radii[0],dtype=float),np.array(sbr[i],dtype=float))
-    sf.print_log(f'''CHECK_SIZE: These are the ring SBRs and limits we will use:
+    print_log(f'''CHECK_SIZE: These are the ring SBRs and limits we will use:
 {'':8s}SBR = {sbr}
 {'':8s}limits = {sbr_ring_limits}
 {'':8s}No. Rings  = {Configuration['NO_RINGS']}
 ''',Configuration,case= ['debug_add'])
-    #sbr_ring_limits = 1.25*np.array([sbr_ring_limits,sbr_ring_limits])
     sbr_ring_limits = np.array([sbr_ring_limits,sbr_ring_limits],dtype=float)
-
-    #This part has to change in something new
     size_in_beams = calc_new_size(Configuration,Tirific_Template,radii,sbr,sbr_ring_limits)
     if not no_apply:
         apply_size = apply_new_size(Configuration,size_in_beams)
     else:
-        apply_size = False
-    sf.print_log(f'''CHECK_SIZE: These have been fitted before {Configuration['OLD_SIZE']}
+        apply_size = [False,False]
+    print_log(f'''CHECK_SIZE: These have been fitted before {Configuration['OLD_SIZE']}
 {'':8s} This is new_size {size_in_beams}, This is what currently is in {Configuration['SIZE_IN_BEAMS']}
-''',Configuration,case= ['debug_add'])
-    if apply_size:
-        Configuration['OLD_SIZE'].append(list(copy.deepcopy(Configuration['SIZE_IN_BEAMS'])))
-        for i in [0,1]:
-            if not Configuration['FIX_SIZE'][i]:
-                Configuration['SIZE_IN_BEAMS'][i] = copy.deepcopy(size_in_beams[i])
+''',Configuration,case= ['debug_add']) 
+    trig = False
+    tmp_old_size=list(copy.deepcopy(Configuration['SIZE_IN_BEAMS']))
+    for i in [0,1]:
+        if apply_size[i]:
+            trig = True
+            Configuration['SIZE_IN_BEAMS'][i] = copy.deepcopy(size_in_beams[i])         
+    if trig:
+        Configuration['OLD_SIZE'].append(tmp_old_size)
         ring_size, number_of_rings = sf.set_ring_size(Configuration)
-        sf.print_log(f'''CHECK_SIZE: Applied the size of {Configuration['SIZE_IN_BEAMS']}, ring size {ring_size} resulting in {number_of_rings} rings
+        print_log(f'''CHECK_SIZE: Applied the size of {Configuration['SIZE_IN_BEAMS']}, ring size {ring_size} resulting in {number_of_rings} rings
 ''',Configuration,case=['verbose'])
 
 
     # Set the unreliable parameters
     #the lower the inclination the sooner the RC becomes unreliable
     limit_factor = sf.set_limits(2.5*np.mean(Configuration['LIMIT_MODIFIER']) ,2.,4.)
-    sf.print_log(f'''CHECK_SIZE: Using a limit factor to calculate where the RC is reliable of  {limit_factor}
+    print_log(f'''CHECK_SIZE: Using a limit factor to calculate where the RC is reliable of  {limit_factor}
 ''',Configuration,case= ['debug_add'])
     Configuration['RC_UNRELIABLE'] = get_number_of_rings(Configuration,sbr,limit_factor*sbr_ring_limits)-1
     if Configuration['RC_UNRELIABLE'] == Configuration['NO_RINGS']:
         Configuration['RC_UNRELIABLE'] -= 1
+    
+
     for i in [0,1]:
         corr_val = np.where(sbr[i,2:] > sbr_ring_limits[i,2:]*3.)[0]+2
         if corr_val.size > 0:
             Configuration['LAST_RELIABLE_RINGS'][i] = corr_val[-1]+1
         else:
             Configuration['LAST_RELIABLE_RINGS'][i] = Configuration['NO_RINGS']
-
-    sf.print_log(f'''CHECK_SIZE: We set these as the last reliable rings {Configuration['LAST_RELIABLE_RINGS']}
-{'':8s}The RC is deemed unrliable from ring {Configuration['RC_UNRELIABLE']} on.
+    print_log(f'''CHECK_SIZE: We set these as the last reliable rings {Configuration['LAST_RELIABLE_RINGS']}
+{'':8s}The RC is deemed unreliable from ring {Configuration['RC_UNRELIABLE']} on.
 ''',Configuration,case= ['debug_add'])
 
-    if apply_size:
+
+    if any(apply_size):
         # Do not move this from here else other routines such as sbr_limits are messed up
         set_new_size(Configuration,Tirific_Template,fit_type= fit_type\
             ,current_run = current_run)
         set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type)
         return False
     elif no_apply:
         return False
@@ -625,142 +659,128 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Configuration['RC_UNRELIABLE'] = modified and updated here.
 '''
-def check_for_ring_addition(Configuration,Tirific_Template,sbr,sbr_ring_limits ):
-    new_rings = Configuration['NO_RINGS']
-    if Configuration['OUTER_RINGS_DOUBLED']:
-        factors = [[10.,3.],[7.5,4.],[6.]]
-    else:
-        if Configuration['NO_RINGS'] <= 8:
-            factors = [[5.,1.],[4.,2.],[3.]]
-        elif Configuration['NO_RINGS'] <= 12:
-            factors = [[5.5,1.5],[4.5,2.5],[3.5]]
-        else:
-            factors = [[6.,2.],[5.,3.],[4]]
-    add = False
-    for side in [0,1]:
-        if (sbr[side,-2] > sbr_ring_limits[side,-2]*factors[0][0] and sbr[side,-1] > sbr_ring_limits[side,-1]*factors[0][1]) or \
-            (sbr[side,-2] > sbr_ring_limits[side,-2]*factors[1][0] and sbr[side,-1] > sbr_ring_limits[side,-1]*factors[1][1]) or \
-            sbr[side,-1] > sbr_ring_limits[side,-1]*factors[2][0]:
-            sf.print_log(f'''CHECK_FOR_RING_ADDITION: Checking side {side}:
-{'':8s}{sbr[side,-2:]}
-{'':8s}and the limits:
-{'':8s}{sbr_ring_limits[side,-2:]}
-{'':8s}Thus we check for gaps.
-''', Configuration,case= ['debug_start'])
+def cut_low_rings(Configuration, Tirific_Template,Fits_Files, fit_type = 'Unknown', current_run=None):
+    print_log(f'''CUT_LOW_RINGS: Checking for too low rings in the smoothed profile
+''',Configuration,case= ['debug_start'])
+    sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
+    #get the sbr profiles
+    sbr_profiles = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
+        array=True)
+    radii = sf.load_tirific(Configuration,Tirific_Template,Variables=['RADI'],\
+        array=True)
+    new_size=copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
+    for i in [0,1]:
+        for x in range(len(sbr_profiles[i,:])-1,3,-1):
+            if sbr_profiles[i,x] > sbr_ring_limits[x]:
+                if radii[x]/Configuration['BEAM'][0] < Configuration['SIZE_IN_BEAMS'][i]:
+                    new_size[i] = radii[x]/Configuration['BEAM'][0]
+                break 
+    print_log(f'''CUT_LOW_RINGS: This is or new model size {new_size}
+{'':8s} This was before {Configuration['SIZE_IN_BEAMS']}
+''',Configuration,case= ['debug_add'])        
+    apply_size = apply_new_size(Configuration,new_size)
+    if any(apply_size):
+        for i in [0,1]:
+            if apply_size[i]:
+                Configuration['SIZE_IN_BEAMS'][i] = copy.deepcopy(new_size[i])  
+               
+        #Need to run this to make sure Configuration['NO_RINGS'] gets updated correctly
+        ring_size, number_of_rings = sf.set_ring_size(Configuration)
+        set_new_size(Configuration,Tirific_Template,fit_type= fit_type\
+            ,current_run = current_run)
+        set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type)
+    print_log(f'''CUT_LOW_RINGS: At the end we get
+{'':8s} {Tirific_Template}
+''',Configuration,case= ['debug_add']) 
+    
+    
 
 
-            rad= np.array(sf.load_tirific(Configuration,Tirific_Template, [f'RADI']),dtype = float)
 
-            gap= np.where(sbr[side] < sbr_ring_limits[side])[0]
-            if gap.size > 0:
-                if gap[-1] == len(sbr[side])-1:
-                    sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap (ring = {', '.join([str(x+1) for x in gap])}) that runs to the last ring.
-{'':8s} Not adding based on this side.
-''', Configuration,case= ['debug_add'])
-                    continue
-                while gap[0] < int(len(sbr[side])/2.):
-                    gap = gap[1:]
-                    if len(gap) == 0:
-                        break
-
-            if gap.size > 0:
-                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap in the rings {',  '.join([str(x+1) for x in gap])}.
-{'':8s}{sbr[side]}
-{'':8s}We will check the change in PA and INCLINATION.
-''', Configuration,case= ['debug_add'])
-                ext = ''
-                if side == 1:
-                    ext='_2'
-                angles = sf.load_tirific(Configuration,Tirific_Template,\
-                    Variables=[f'PA{ext}',f'INCL{ext}'],array=True)
-                PA_change =  np.sum(np.array([np.abs(x-y) for x,y in zip(angles[0,gap[0]-1:],angles[0,gap[0]:])]))
-                INCL_change = np.sum(np.array([np.abs(x-y) for x,y in zip(angles[1,gap[0]-1:],angles[1,gap[0]:])]))
-
-                gap_size = sf.convertskyangle(Configuration,[rad[gap[0]],rad[-1]])
-
-                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap {[rad[gap[0]],rad[-1]]} arcsec = {gap_size} kpc
-{'':8s}PA variation = {[np.abs(x-y) for x,y in zip(angles[0,gap[0]-1:],angles[0,gap[0]:])]}
-{'':8s}INCL variation = {[np.abs(x-y) for x,y in zip(angles[1,gap[0]-1:],angles[1,gap[0]:])]}
-''', Configuration,case= ['debug_add'])
-                gap_size = float(gap_size[1]-gap_size[0])
-                if PA_change/gap_size  < Configuration['MAX_CHANGE']['PA'] and INCL_change/gap_size < Configuration['MAX_CHANGE']['INCL']:
-                    add = True
-                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a change  of {PA_change/gap_size} in PA and {INCL_change/gap_size} in INCL.
-{'':8s} The gap is {gap_size} kpc
-''', Configuration,case= ['debug_add'])
-            else:
-                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We did not find a gap so we were are adding.
-''', Configuration,case= ['debug_add'])
-                add=True
 
+cut_low_rings.__doc__  =f'''
+ NAME:
+    cut_low_rings
 
-    if add:
-        sf.print_log(f'''CHECK_FOR_RING_ADDITION:  We are adding a ring (new no ring = {new_rings+1.})
-''', Configuration,case= ['verbose'])
-        new_rings += 1
-    else:
-        sf.print_log(f'''CHECK_FOR_RING_ADDITION: The last rings were found to be:
-{'':8s}{sbr[:,-2:]}
-{'':8s}and the limits:
-{'':8s}{sbr_ring_limits[:,-2:]}
-{'':8s}Thus we keep the ring size.
-''', Configuration,case=['debug_add'])
-    return new_rings
+ PURPOSE:
+    if after the first smooth the outer rings are below the sbr limits they are removed.
+    but only if the smoothing is reran (No_rings < 5)
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Tirific_Template = Standard FAT Tirific Template
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    No output the modified sbrs are writte nto the TiriFiC Template
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE: Very simple function only to be used after smoothing
+'''
 
 def fit_arc(Configuration,radii,sm_profile,error, function_to_fit,key ):
     c2 = sf.set_limits(radii[-1]*0.2,radii[2],radii[int(len(radii)/1.5)])
     est_center = radii[-1]/2.-c2
     est_length = radii[-1]*0.1
     if key in ['SDIS']:
         est_amp = abs(np.max(sm_profile)-np.min(sm_profile))
     else:
         est_amp = np.mean(sm_profile[3:])-np.mean(sm_profile[:4])
     est_mean = np.mean(sm_profile)
 
     if not error.any():
-        error = np.full(len(y),1.)
+        error = np.full(len(sm_profile),1.)
         absolute_sigma = False
     else:
         absolute_sigma = True
     with warnings.catch_warnings():
         warnings.simplefilter("error")
         succes = False
         maxfev= int(100*(len(radii)))
 
         while not succes:
 
-            sf.print_log(f'''FIT_ARC: Starting the curve fit with {maxfev}
+            print_log(f'''FIT_ARC: Starting the curve fit with {maxfev}
 ''',Configuration,case= ['debug_start'])
             try:
                 arc_par,arc_cov  =  curve_fit(function_to_fit, radii, sm_profile,p0=[est_center,est_length,est_amp,est_mean]\
                                             ,sigma=error,absolute_sigma=absolute_sigma,maxfev=maxfev)
                 new_profile = function_to_fit(radii,*arc_par)
                 new_profile[:3] = np.mean(new_profile[:3])
                 succes = True
             except OptimizeWarning:
                 maxfev =  2000*(len(radii))
             except RuntimeError as e:
                 split_error = str(e)
                 if 'Optimal parameters not found: Number of calls to function has reached maxfev' in \
                     split_error:
                     maxfev += 100*int(len(radii))
-                    sf.print_log(f'''FIT_ARC: We failed to find an optimal fit due to the maximum number of evaluations. increasing maxfev to {maxfev}
+                    print_log(f'''FIT_ARC: We failed to find an optimal fit due to the maximum number of evaluations. increasing maxfev to {maxfev}
 ''',Configuration,case= ['debug_add'])
                 else:
-                    sf.print_log(f'''FIT_ARC: Fit arc crashed with an unknow error:
+                    print_log(f'''FIT_ARC: Fit arc crashed with an unknow error:
 {'':8s}{split_error}
 ''',Configuration)
                     raise RuntimeError(split_error)
             if maxfev >  1000*(len(radii)):
-                sf.print_log(f'''FIT_ARC: We failed to find an optimal fit to dispersion, returning the smoothed profile.
+                print_log(f'''FIT_ARC: We failed to find an optimal fit to dispersion, returning the smoothed profile.
 ''',Configuration,case = ['verbose'])
                 succes = True
                 new_profile = copy.deepcopy(sm_profile)
 
     return new_profile#,new_error
 fit_arc.__doc__ =f'''
  NAME:
@@ -786,55 +806,59 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fit_polynomial(Configuration,radii,profile,sm_profile,error, key, \
-                   Tirific_Template,inner_fix = 4,min_error =0., \
+def fit_polynomial(Configuration,radii,profile,error, key, \
+                   Tirific_Template,inner_fix = 4,zero_point=None, \
                    boundary_limits = None, allowed_order= None,
                    return_order= False ):
     if boundary_limits is None:
         boundary_limits = [0,0.]
     if allowed_order is None:
         allowed_order=[None,None]
 
-    sf.print_log(f'''FIT_POLYNOMIAL: starting to fit the polynomial with the following input:
+    print_log(f'''FIT_POLYNOMIAL: starting to fit the polynomial with the following input:
 {'':8s} key = {key}
 {'':8s} radii = {radii}
 {'':8s} profile = {profile}
-{'':8s} sm_profile = {sm_profile}
 {'':8s} error = {error}
 ''',Configuration, case = ['debug_start'])
     only_inner = False
-    if key in ['PA','INCL','Z0','ARBITRARY']:
+    if key in ['PA','INCL']:
+        fixed = inner_fix
+        only_inner = True
+    elif key in ['Z0','THETA_FACTOR','PHI_FACTOR','CHANGE_ANGLE']:
         fixed = inner_fix
         only_inner = True
         error[:fixed] = error[:fixed]/10.
     elif key in ['VROT']:
         #fixed =len(radii)-Configuration['OUTER_SLOPE_START']
         fixed =sf.set_limits(len(radii)-np.min(Configuration['LAST_RELIABLE_RINGS']),1,len(radii))
         error[np.min(Configuration['LAST_RELIABLE_RINGS']):] = Configuration['CHANNEL_WIDTH']
         error[0] = Configuration['CHANNEL_WIDTH']
-        error[1] = error[1]*3.
+        #error[1] = error[1]*3.
     else:
         fixed = 1
 
     if len(radii) > 10.:
         start_order = int(len(radii)/5.)
     else:
         start_order = 0
 
 
 
     st_fit = int(0)
     if key in ['VROT']:
-
+        bound_fit = int(1)
         if np.mean(profile[1:3]) > 120.:
+            if zero_point == None:
+                zero_point = np.mean(profile[1:3])
             st_fit = int(1)
 
         #This needs another -1 because the 0 and 1/5. ring are more or less 1 ring
         max_order = sf.set_limits(len(radii)-fixed-2,3,8)
         #The rotation curve varies a lot so the lower limit should be as high as possible
         #But at least 3 less than max order and maximally 4
         if len(radii)-fixed-2 <= 6:
@@ -842,15 +866,22 @@
         elif len(radii)-fixed-2 <= 10:
             lower_limit=sf.set_limits(4,3,max_order-2)
         else:
             lower_limit=sf.set_limits(5,3,max_order-2)
         start_order = sf.set_limits(start_order,lower_limit,max_order)
 
     else:
-        if key in ['PA','INCL','Z0']:
+        bound_fit = int(0)
+        if key in ['PA']:
+            max_order = sf.set_limits(len(radii)-2,4,8)
+            start_order = 3  
+        elif key in ['INCL']:
+            max_order = sf.set_limits(len(radii)-2,3,5)
+            start_order = 1               
+        elif key in ['Z0']:
             max_order = sf.set_limits(len(radii)-fixed,3,5)
         elif key in ['SBR']:
             max_order = sf.set_limits(len(radii)-2,4,8)
             start_order = 3
         else:
             max_order = sf.set_limits(len(radii)-1,3,7)
 
@@ -859,82 +890,137 @@
             start_order=  allowed_order[0]
     if start_order >= max_order:
         max_order = start_order+1
     if allowed_order[1]:
         if max_order > allowed_order[1]:
             max_order=  allowed_order[1]
 
-    sf.print_log(f'''FIT_POLYNOMIAL: For {key} we start at {start_order} because we have {len(radii)} rings of which {fixed} are fixed
-{'':8s} this gves us a maximum order of {max_order}
+    print_log(f'''FIT_POLYNOMIAL: For {key} we start at {start_order} because we have {len(radii)} rings of which {fixed} are fixed
+{'':8s} this gives us a maximum order of {max_order}
 ''',Configuration,case = ['debug_add'])
+    found = False
+    count = 0
+    failed=False
+    while not found:
+        reduced_chi = []
+        order = range(start_order,max_order+1)
+
+        print_log(f'''FIT_POLYNOMIAL: We will fit the following radii.
+    {'':8s}{radii[st_fit:]}
+    {'':8s} and the following profile:
+    {'':8s}{profile[st_fit:]}
+    {'':8s} weights = {1./error[st_fit:]}
+    {'':8s} we are doing this for the {count} times.
+    ''',Configuration,case = ['debug_add'])
+
+        #make sure there are no 0. in the errors
+        zero_locations = np.where(error[st_fit:] == 0.)[0]
+        if zero_locations.size > 0.:
+            error[zero_locations+st_fit] = 1./np.nanmax(1./error)
 
-    reduced_chi = []
-    order = range(start_order,max_order+1)
-
-    sf.print_log(f'''FIT_POLYNOMIAL: We will fit the following radii.
-{'':8s}{radii[st_fit:]}
-{'':8s} and the following profile:
-{'':8s}{profile[st_fit:]}
-{'':8s} weights = {1./error[st_fit:]}
-''',Configuration,case = ['debug_add'])
+        for ord in order:
+            fit_prof = np.poly1d(np.polyfit(radii[st_fit:],profile[st_fit:],ord,w=1./error[st_fit:]))
 
-    #make sure there are no 0. in the errors
-    zero_locations = np.where(error[st_fit:] == 0.)[0]
-    if zero_locations.size > 0.:
-        error[zero_locations+st_fit] = 1./np.nanmax(1./error)
-
-    for ord in order:
-        fit_prof = np.poly1d(np.polyfit(radii[st_fit:],profile[st_fit:],ord,w=1./error[st_fit:]))
-
-        if st_fit > 0.:
-            fit_profile = np.concatenate(([sm_profile[0]],[e for e in fit_prof(radii[st_fit:])]))
-        else:
-            fit_profile = fit_prof(radii)
-        #fit_profile = fit_prof(radii)
-
-        if key != 'SBR':
-            fit_profile = fix_profile(Configuration, key, fit_profile, Tirific_Template,inner_fix=inner_fix, singular = True,only_inner =only_inner)
-        else:
-            for i in range(len(fit_profile)-5,len(fit_profile)):
-                if fit_profile[i-1] < fit_profile[i]:
-                    fit_profile[i]=fit_profile[i-1]*0.9
-        red_chi = np.sum((profile[st_fit:]-fit_profile[st_fit:])**2/error[st_fit:])/(len(radii[st_fit:])-ord)
-        #We penailze profiles that go outside the boundaries
+            if st_fit > 0.:
+                fit_profile = np.concatenate(([zero_point],[e for e in fit_prof(radii[st_fit:])]))
+            else:
+                fit_profile = fit_prof(radii)
+            #fit_profile = fit_prof(radii)
 
-        if np.sum(np.absolute(np.array(boundary_limits,dtype=float))) != 0.:
-                diff = np.sum(np.array([abs(x-sf.set_limits(x,\
-                                                  boundary_limits[0],\
-                                                  boundary_limits[1])) \
-                                        for x in  fit_profile[st_fit:]],dtype = float))
-                if diff > 1.:
-                    red_chi = red_chi*(diff)
+            if key not in ['SBR','THETA_FACTOR','PHI_FACTOR']:
+                fit_profile = fix_profile(Configuration, key, fit_profile, \
+                    Tirific_Template=Tirific_Template,inner_fix=inner_fix,\
+                    singular = True,only_inner =only_inner)
+            else:
+                for i in range(len(fit_profile)-5,len(fit_profile)):
+                    if fit_profile[i-1] < fit_profile[i]:
+                        fit_profile[i]=fit_profile[i-1]*0.9
+            
+            red_chi = np.sum((profile[st_fit:]-fit_profile[st_fit:])**2/error[st_fit:]**2)/(len(radii[st_fit:])-ord)
+            #We penailze profiles that go outside the boundaries
+            print_log(f'''FIT_POLYNOMIAL: From the final profile we get chi**2 = {red_chi}
+{'':8s} {key} = {', '.join([str(x) for x in fit_profile[st_fit:]])}
+''',Configuration,case = ['debug_add'])
+            if np.sum(np.absolute(np.array(boundary_limits,dtype=float))) != 0.:
+                    with warnings.catch_warnings():
+                        warnings.filterwarnings("error",category=RuntimeWarning)
+                        
+                        try:                       
+                            diff = np.sum(np.array([abs(x-sf.set_limits(x,\
+                                                    boundary_limits[0],\
+                                                    boundary_limits[1]))/abs(x) \
+                                            for x in  fit_profile[bound_fit:]],dtype = float))
+                        except RuntimeWarning:
+                            if key in ['THETA_FACTOR','PHI_FACTOR']:
+                                diff = np.where(abs(fit_profile[bound_fit:]) > 1.)[0]
+                                if len(diff) > 0:
+                                    diff = 1.5
+                                else:
+                                    diff = 0.
+                            elif key in ['CHANGE_ANGLE']:
+                                diff=0.
+                            else:    
+                                print_log(f'''FIT_POLYNOMIAL: We are throwing an error as there should not be 0's in the diff,
+{'':8s} boundary_limits =  {boundary_limits}
+{'':8s} fit_profile  = {fit_profile[bound_fit:]}
+{'':8s} For the parameter {key}
+''',Configuration,case = ['debug_add'])
+                                raise RuntimeError(f"The profile in fit_polynomial should not have zeros.") 
 
-        reduced_chi.append(red_chi)
+                       
+                    if diff > 1. and not np.isnan(diff):
+                        print_log(f'''FIT_POLYNOMIAL: because of crossing {boundary_limits}
+{'':8s} we penalize the orginal chi**2 {red_chi} of order {ord} with {diff}
+{'':8s} the fitted profile is {fit_profile}
+''',Configuration,case = ['debug_add'])
+                        red_chi = red_chi*(diff)
+            if red_chi < 1.:
+                red_chi = float('NaN')
+            reduced_chi.append(red_chi)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore",message="All-NaN axis encountered"\
+                            ,category=RuntimeWarning)
+            if not np.isnan(np.nanmin(reduced_chi)):
+                found = True
+            else:
+                error = error/2.
+                count += 1
+        if count > 100 or np.sum(error) == 0.:
+            print_log(f'''FIT_POLYNOMIAL: we failed to fit a polynomial
+''',Configuration,case = ['debug_add'])
+            found = True
+            failed =True     
         #if key in ['VROT'] and Configuration['NO_RINGS'] < 2.5*max_order:
         #    reduced_chi[-1] = reduced_chi[-1]*(ord/Configuration['NO_RINGS'])**2.5
-    sf.print_log(f'''FIT_POLYNOMIAL: We have fitted these:
+    if not failed:
+        print_log(f'''FIT_POLYNOMIAL: We have fitted these:
 {'':8s} order = {[x for x in order]}
-{'':8s} reducuced chi = {reduced_chi}
+{'':8s} reduced chi = {reduced_chi}
+''',Configuration,case = ['debug_add'])
+        reduced_chi = np.array(reduced_chi,dtype = float)
+        final_order = order[np.where(np.nanmin(reduced_chi ) == reduced_chi )[0][0]]
+    else:
+        print_log(f'''FIT_POLYNOMIAL: we failed to fit a polynomial
+{'':8s} order = 0
 ''',Configuration,case = ['debug_add'])
-    reduced_chi = np.array(reduced_chi,dtype = float)
-    final_order = order[np.where(np.min(reduced_chi ) == reduced_chi )[0][0]]
+        final_order=0.
 
-    sf.print_log(f'''FIT_POLYNOMIAL: We have regularised {key} with a polynomial of order {final_order}.
+    print_log(f'''FIT_POLYNOMIAL: We have regularised {key} with a polynomial of order {final_order}.
 ''',Configuration,case=['verbose'])
     fit_profile = np.poly1d(np.polyfit(radii[st_fit:],profile[st_fit:],final_order,w=1./error[st_fit:]))
     if st_fit > 0.:
-        new_profile = np.concatenate(([sm_profile[0]],[e for e in fit_profile(radii[st_fit:])]))
+        new_profile = np.concatenate(([zero_point],[e for e in fit_profile(radii[st_fit:])]))
     else:
         new_profile = fit_profile(radii)
     #if key in ['VROT'] and profile[1] < profile[2]:
     #    new_profile[1] = profile[1]
-    if key != 'SBR':
+    if key not in ['SBR','THETA_FACTOR','PHI_FACTOR']:
         new_profile = fix_profile(Configuration, key, new_profile, \
-            Tirific_Template,inner_fix=inner_fix,singular = True,\
-            only_inner =only_inner)
+            Tirific_Template=Tirific_Template,inner_fix=inner_fix,\
+            singular = True,only_inner=only_inner)
     else:
         for i in range(len(fit_profile)-5,len(fit_profile)):
             if fit_profile[i-1] < fit_profile[i]:
                 fit_profile[i]=fit_profile[i-1]*0.9
     if return_order:
         return new_profile,final_order
     else:
@@ -949,63 +1035,64 @@
  CATEGORY:
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     radii = rings in arcsec of profiles to regularise
     profile = profile to be regularised
-    sm_profile = smoothed profile
     error = errors on the profile
     key = parameter that is being regularised
     Tirific_Template = standard tirific template
 
  OPTIONAL INPUTS:
-
-
-    min_error =0.
-    the error should always be large than this value
+    zero_point = The inner point for the RC 
 
  OUTPUTS:
     polynomial fitted profile
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def fix_outer_rotation(Configuration,profile):
 
-    sf.print_log(f'''FIX_OUTER_ROTATION: adjust last rings of VROT profile:
+    print_log(f'''FIX_OUTER_ROTATION: adjust last rings of VROT profile:
 {'':8s}{profile}
 {'':8s} from ring {Configuration['RC_UNRELIABLE']} we do not trust the rings.
 ''',Configuration,case = ['debug_start'])
     profile = np.array(profile,dtype=float)
     # if the outer parts are less then 5 channels there is something wrong And we just take a flat curve from max
-    if np.mean(profile[Configuration['RC_UNRELIABLE']:]) < 5.*Configuration['CHANNEL_WIDTH']:
-        Configuration['RC_UNRELIABLE'] = int(np.where(np.max(profile) == profile)[0][0])+1
-        if Configuration['RC_UNRELIABLE'] < Configuration['NO_RINGS']-1:
-            profile[Configuration['RC_UNRELIABLE']:] = profile[Configuration['RC_UNRELIABLE']-1]
-
-            sf.print_log(f'''FIX_OUTER_ROTATION: we adjusted the unreliable part.
-{'':8s}{profile}
-{'':8s} from ring {Configuration['RC_UNRELIABLE']} we do not trust the rings.
-    ''',Configuration, case= ['debug_add'])
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore",message="Mean of empty slice."\
+                            ,category=RuntimeWarning) 
+        warnings.filterwarnings("ignore",message="invalid value encountered in scalar divide"\
+                            ,category=RuntimeWarning)
+        if np.mean(profile[Configuration['RC_UNRELIABLE']:]) < 5.*Configuration['CHANNEL_WIDTH']:
+            Configuration['RC_UNRELIABLE'] = int(np.where(np.max(profile) == profile)[0][0])+1
+            if Configuration['RC_UNRELIABLE'] < Configuration['NO_RINGS']-1:
+                profile[Configuration['RC_UNRELIABLE']:] = profile[Configuration['RC_UNRELIABLE']-1]
+
+                print_log(f'''FIX_OUTER_ROTATION: we adjusted the unreliable part.
+    {'':8s}{profile}
+    {'':8s} from ring {Configuration['RC_UNRELIABLE']} we do not trust the rings.
+        ''',Configuration, case= ['debug_add'])
 
     #inner_slope = int(round(sf.set_limits(NUR*(4.-Configuration['LIMIT_MODIFIER'][0])/4.,round(NUR/2.),NUR-2)))
     if Configuration['RC_UNRELIABLE'] < Configuration['NO_RINGS']-1 and np.mean(profile[1:3]) > 180.:
         profile[Configuration['RC_UNRELIABLE']:] = profile[Configuration['RC_UNRELIABLE']-1]
 
     for i in range(int(Configuration['NO_RINGS']*3./4),Configuration['NO_RINGS']-1):
         if profile[i+1] > profile[i]*1.3:
             profile[i+1] = profile[i]*1.3
 
-    sf.print_log(f'''FIX_OUTER_ROTATION: this is corrected profile:
+    print_log(f'''FIX_OUTER_ROTATION: this is corrected profile:
 {profile}
 ''',Configuration, case= ['debug_add'])
 
     return profile
 fix_outer_rotation.__doc__ =f'''
  NAME:
     fix_outer_rotation
@@ -1030,75 +1117,83 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Declining rotation curves are dealt with in no_declining_vrot
 '''
 
-def fix_profile(Configuration, key, profile, Tirific_Template, inner_fix = None,\
-                    singular = False,only_inner = False ):
-    if inner_fix is None:
-        inner_fix = [4,4]
+def fix_profile(Configuration, key, profile, Tirific_Template = None,\
+                 inner_fix = 4,singular = False,only_inner = False ):
+  
     if isinstance(inner_fix,int):
-        inner_fix = [inner_fix]
-    sf.print_log(f'''FIX_PROFILE: Starting to fix {key} with the input values:
+        if singular:
+            inner_fix = [inner_fix]
+        else:
+            inner_fix = [inner_fix,inner_fix]
+       
+    print_log(f'''FIX_PROFILE: Starting to fix {key} with the input values:
 {'':8s}{profile}
 ''', Configuration, case= ['debug_add'])
+    if key  == 'VROT' and Tirific_Template is None:
+        print_log(f'''FIX_PROFILE: To fix VROT  we require a Tirific Template 
+''', Configuration,case = ['main','screen'])
+        raise FunctionCallError("FIX_PROFILE:  To fix VROT  we require a Tirific Template.")
 
     if key == 'SBR':
-        sf.print_log(f'''FIX_PROFILE: To fix sbr profiles use FIX_SBR.
+        print_log(f'''FIX_PROFILE: To fix sbr profiles use FIX_SBR.
 ''', Configuration,case = ['main','screen'])
         raise FunctionCallError("FIX_PROFILE: To fix sbr profiles use check SBR.")
     if singular:
         indexes = [0]
         profile = np.array([profile,profile])
-        inner_mean = np.nanmean([profile[0,:inner_fix[0]]])
+        if key not in ['THETA_FACTOR','PHI_FACTOR','CHANGE_ANGLE']:
+            inner_mean = np.nanmean([profile[0,:inner_fix[0]]])
+        else:
+            inner_mean = 0.
     else:
         indexes = [0,1]
-        if np.sum(inner_fix) != 0.:
+        if np.sum(inner_fix) != 0. and key not in ['THETA_FACTOR','PHI_FACTOR','CHANGE_ANGLE'] :
             inner_mean = np.nanmean(np.concatenate((profile[0,:inner_fix[0]],profile[1,:inner_fix[1]])))
         else:
             inner_mean= 0.
 
     profile = np.array(profile,dtype=float)
-    rad = [float(x) for x in Tirific_Template['RADI'].split()]
-
     if key in ['VROT']:
         indexes = [0]
         inner_mean = 0.
         profile[0,0] = 0.
     else:
         for i in indexes:
             profile[i,:inner_fix[i]] = inner_mean
-        sf.print_log(f'''FIX_PROFILE: the  {inner_fix} inner rings are fixed for the profile:
+        print_log(f'''FIX_PROFILE: the  {inner_fix} inner rings are fixed for the profile:
 {'':8s} profile = {profile[i,:]}
 ''', Configuration,case=['debug_add'])
-    sf.print_log(f'''FIX_PROFILE: the  inner mean is {inner_mean}.
+    print_log(f'''FIX_PROFILE: the  inner mean is {inner_mean}.
 ''', Configuration,case=['debug_add'])
 
     for i in indexes:
-        sf.print_log(f'''FIX_PROFILE: From ring {Configuration['LAST_RELIABLE_RINGS'][i]} on we do not trust these rings.
+        print_log(f'''FIX_PROFILE: From ring {Configuration['LAST_RELIABLE_RINGS'][i]} on we do not trust these rings.
 ''', Configuration,case=['debug_add'])
         if Configuration['LAST_RELIABLE_RINGS'][i] < len(profile[i,:]) and not only_inner:
             #profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:] = profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:]*0.25+profile[i,Configuration['LAST_RELIABLE_RINGS'][i]-1]*0.75
             profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:] = profile[i,Configuration['LAST_RELIABLE_RINGS'][i]-1]
-        sf.print_log(f'''FIX_PROFILE:After fixing the last reliable rings
+        print_log(f'''FIX_PROFILE:After fixing the last reliable rings
 {'':8s} profile = {profile[i,:]}
 ''', Configuration,case=['debug_add'])
         if key == 'VROT':
             profile[i] =fix_outer_rotation(Configuration,profile[i])
         elif inner_fix[i] != 0:
             xrange = sf.set_limits((int(round(len(profile[0])-5.)/4.)),1,4)
         # need to make sure this connects smoothly
             for x in range(0,xrange):
                 if inner_fix[i]+x < len(profile[i,:]):
                     profile[i,inner_fix[i]+x] = 1/(x+4./xrange)*inner_mean+ (1-1/(x+4./xrange))*profile[i,inner_fix[i]+x]
             #if key in ['PA','INCL']:
             #    profile[i,:] = sf.max_profile_change(Configuration,rad,profile[i,:],key)
-        sf.print_log(f'''FIX_PROFILE:After smoothed transition
+        print_log(f'''FIX_PROFILE:After smoothed transition
 {'':8s} profile = {profile[i,:]}
 ''', Configuration,case=['debug_add'])
         #profile[:,:Configuration['INNER_FIX']] = np.nanmean(profile[:,:Configuration['INNER_FIX']])
         if key in ['SDIS']:
             inner_max = np.nanmax(profile[i,:int(len(profile[i,:])/2.)])
             mean = np.nanmean(profile[i,:])
             if inner_mean < mean or inner_mean < np.nanmean(profile[i,-3:]):
@@ -1113,15 +1208,15 @@
         tmp  = no_declining_vrot(Configuration,Tirific_Template,profile = profile[0])
         profile[0] = tmp
         profile[1] = tmp
     if singular:
         profile = profile[0]
 
 
-    sf.print_log(f'''FIX_PROFILE: The final profile for {key} is:
+    print_log(f'''FIX_PROFILE: The final profile for {key} is:
 {'':8s}{profile}
 ''', Configuration,case=['debug_add'])
     return profile
 fix_profile.__doc__ =f'''
  NAME:
     fix_profile
 
@@ -1155,78 +1250,83 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def fix_sbr(Configuration,Tirific_Template, smooth = False, initial = False ):
-    sf.print_log(f'''FIX_SBR: Starting a SBR check.
+    print_log(f'''FIX_SBR: Starting a SBR check.
 ''',Configuration,case=['debug_start'])
 
     # get the cutoff limits
-    radii,cutoff_limits = sf.sbr_limits(Configuration,Tirific_Template)
+    cutoff_limits = sf.sbr_limits(Configuration,Tirific_Template)
     cutoff_limits = np.array([cutoff_limits,cutoff_limits],dtype=float)
+    print_log(f'''FIX_SBR: Using these cutoff limits.
+{'':8s}cutoff_limits = {cutoff_limits}
+''',Configuration,case=['debug_add'])
     # Then get the profile from the template
-    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
-        array=True)
-    sf.print_log(f'''FIX_SBR: Before modify.
+    radii = sf.load_tirific(Configuration,Tirific_Template,Variables=['RADI'],array=True)
+    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'], array=True)
+    original_sbr=copy.deepcopy(sbr)
+    print_log(f'''FIX_SBR: Before modify.
 {'':8s}sbr from template = {sbr}
 ''',Configuration,case=['debug_add'])
     # First make a correction on the inner 2 values
     sbr = inner_sbr_fix(Configuration,sbr,cutoff_limits)
     # Let's use a smoothed profile for the fittings
     sm_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',
                             min_error= cutoff_limits,no_apply = True,
                             fix_sbr_call = True,profile_in = sbr )
 
-    sf.print_log(f'''FIX_SBR: Before modify.
+    print_log(f'''FIX_SBR: Before modify.
 {'':8s}sbr  = {sbr}
 {'':8s}sm_sbr  = {sm_sbr}
 ''',Configuration,case=['debug_add'])
 
     # We interpolate negative values as well as values below the limits inner part with a cubi
     errors = get_error(Configuration,sbr,sm_sbr,'SBR',min_error=cutoff_limits)
-    sf.print_log(f'''FIX_SBR: retrieved errors.
+    print_log(f'''FIX_SBR: retrieved errors.
 {'':8s}errors  = {errors}
 ''',Configuration,case=['debug_add'])
     no_zero_sbr = copy.deepcopy(sm_sbr)
     zeros = np.where(no_zero_sbr < 1e-9)
     no_zero_sbr[zeros] = 0.1*cutoff_limits[zeros]
     error_weights = cutoff_limits/no_zero_sbr*1./np.nanmin(cutoff_limits[:,2:]/no_zero_sbr[:,2:])
     error_weights[:,0] = 3.
     for i in [0,1]:
         error_weights[i] = [x if x <100. else 100. for x in error_weights[i]]
     errors =errors*error_weights
-    sf.print_log(f'''FIX_SBR: weighed errors errors.
+    print_log(f'''FIX_SBR: weighed errors errors.
 {'':8s}sm_sbr = {sm_sbr}
 {'':8s}cutoff_limits  = {cutoff_limits}
 {'':8s}errors  = {errors}
 {'':8s}weights  = {error_weights}
 ''',Configuration,case=['debug_add'])
 
 
     store_gaussian = []
     for i in [0,1]:
         corr_val = np.where(sbr[i,2:] > cutoff_limits[i,2:])[0]+2
         # If we have enough safe values in the profile we attempt to fit it
         if corr_val.size > 3.:
             fit_sbr = sm_sbr[i,corr_val]
-            sf.print_log(f'''FIX_SBR: The values used for fitting are {fit_sbr}.
+            print_log(f'''FIX_SBR: The values used for fitting are {fit_sbr}.
 ''',Configuration,case=['debug_add'])
             try:
                 if 'SBR' in Configuration['FIXED_PARAMETERS'][0] \
                     or initial:
-                    vals = sf.fit_gaussian(Configuration,radii[corr_val],fit_sbr,errors=errors[i,corr_val])
+                    vals = sf.fit_gaussian(Configuration,radii[corr_val],\
+                                fit_sbr,errors=errors[i,corr_val])
                     gaussian = sf.gaussian_function(radii,*vals)
                 else:
-                    gaussian = fit_polynomial(Configuration,radii,sbr[i,:],sm_sbr[i,:],errors[i,:],'SBR', Tirific_Template,\
-                                             min_error=cutoff_limits[i,:])
+                    gaussian = fit_polynomial(Configuration,radii,sbr[i,:],\
+                        errors[i,:],'SBR', Tirific_Template)
                 # if the peak of this gaussian is in the inner two points replace it with the smoothed profile
                 if np.any(np.where(np.max(gaussian) == gaussian)[0] < 2):
-                    sf.print_log(f'''FIX_SBR: We are trying to replace the inner gaussian.
+                    print_log(f'''FIX_SBR: We are trying to replace the inner gaussian.
 {'':8s} gaussian = {gaussian[[0,1]]}
 {'':8s} sm_sbr = {sm_sbr[i,[0,1]]}
 ''',Configuration,case=['debug_add'])
                     gaussian[[0,1]] = sm_sbr[i,[0,1]]
             except FittingError:
                 # If we fail we try a CubicSpline interpolation
                 try:
@@ -1253,83 +1353,77 @@
     # and where we are lower than the cutoff we replace with the 1.2 *cutoff unless we smoothed
     if not smooth:
         sbr[np.where(sbr<cutoff_limits)] = 2.*cutoff_limits[np.where(sbr<cutoff_limits)]
         #if our warp_slope is very small we want to increase the SBR significantly
         for i in [0,1]:
             if Configuration['WARP_SLOPE'][i] <  0.75*(Configuration['NO_RINGS']) and Configuration['WARP_SLOPE'][i] != None:
                 sbr[i,Configuration['WARP_SLOPE'][i]:] = 0.5*sbr[i,Configuration['WARP_SLOPE'][i]-1]+2.5*sbr[i,Configuration['WARP_SLOPE'][i]:]
-    else:
+  
 
-        #sbr[np.where(sbr<cutoff_limits/2.)] = 1e-16
-        #no rising outer end profiles
-        for i in [0,1]:
-            counter = len(sbr[i,:])-1
-            found_good  = False
-            sf.print_log(f'''FIX_SBR: check sbr vs limits
-{'':8s}sbr = {sbr[i, :]}
-{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
-{'':8s}counter = {counter}
-''',Configuration,case=['debug_add'])
-            while not found_good and counter > 0:
-                if sbr[i, counter] < cutoff_limits[i,counter]/2.:
-                    if counter > 3:
-                        sbr[i, counter] = 1e-16
-                    else:
-                        sbr[i, counter] = cutoff_limits[i,counter]*1.5
-                    counter -= 1
-                else:
-                    found_good =True
-            if counter == 0:
-                sf.print_log(f'''FIX_SBR: We set all off the SBR to 1e-16
-{'':8s}sbr = {sbr[i, :]}
-{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
-{'':8s}counter = {counter}
-''',Configuration,case=['debug_add'])
-                raise FaintSourceError(f"After correcting the SBRs all values we're below the cutoff limit, your source is too faint.")
-            if sbr[i,-2] < sbr[i,-1]:
-                last = sbr[i,-1]
-                second = sbr[i,-2]
-                sbr[i,-2] = last
-                sbr[i,-1] = second
-            sf.print_log(f'''FIX_SBR: check sbr vs limits after
-{'':8s}sbr = {sbr[i, :]}
-{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
-{'':8s}counter = {counter}
-''',Configuration,case=['debug_add'])
+      
 
     # and ensure that both sides the inner two rings are the same
     sbr[:,[0,1]] = np.mean(sbr[:,[0,1]])
-    sf.print_log(f'''FIX_SBR: after ensuring both ring are the same
+    print_log(f'''FIX_SBR: after ensuring both ring are the same
 {'':8s}sbr = {sbr[i, :]}
 ''',Configuration,case=['debug_add'])
     #And that they are less then 3/4 of ring 3 unless ring 3 is blanked
     ring_three = np.min(sbr[[0,1],2])
     if ring_three < 1e-15:
         ring_three = sbr[0,1]*4
 
     if sbr[0,1] > 3/4.* ring_three:
         sbr[:,[0,1]] = 3/4.* ring_three
 
-    sf.print_log(f'''FIX_SBR: after ring three
+    print_log(f'''FIX_SBR: after ring three
 {'':8s}sbr = {sbr[i, :]}
 ''',Configuration,case=['debug_add'])
     if smooth and len(sbr[0]) > 6:
         for j in [0,1]:
             fit_profile = sbr[j]
             for i in range(len(fit_profile)-5,len(fit_profile)):
                 if fit_profile[i-1] < fit_profile[i]:
                     fit_profile[i]=fit_profile[i-1]*0.9
             sbr[j] = fit_profile
 
-    sf.print_log(f'''FIX_SBR: After modify.
+    # And finally we need to make sure all values are positive and reasonable
+    # And that values that are not fitted are set to 0.   
+    not_too_faint = False             
+    for i in [0,1]:
+        #In setting rings to fit the Tirific rings start at one but python is 0 based
+        last_ring_to_fit = np.where(radii <= \
+            Configuration['SIZE_IN_BEAMS'][i]*Configuration['BEAM'][0])\
+                [0][-1]   #+1            
+        for n in range(len(sbr[i,:])):
+            if n > last_ring_to_fit: 
+                sbr[i,n] = 0. 
+            elif sbr[i,n] < cutoff_limits[i,n]:
+                sbr[i,n] = cutoff_limits[i,n]*1.5
+            else:
+                not_too_faint = True
+        if sbr[i,last_ring_to_fit-1] < sbr[i,last_ring_to_fit]:
+                last = sbr[i,last_ring_to_fit]
+                second = sbr[i,last_ring_to_fit-1]
+                sbr[i,last_ring_to_fit-1] = last
+                sbr[i,last_ring_to_fit] = second         
+    if smooth and not not_too_faint:
+        print_log(f'''FIX_SBR: All SBR rings are below the cutoff limits
+{'':8s}original sbr = {original_sbr}
+{'':8s}cutoff_limits  = {cutoff_limits}
+''',Configuration,case=['debug_add'])
+        raise FaintSourceError(f"After correcting the SBRs all values we're below the cutoff limit, your source is too faint.")
+           
+
+
+    print_log(f'''FIX_SBR: After modify.
 {'':8s}{sbr}
 ''',Configuration,case=['debug_add'])
     Tirific_Template['SBR'] = f"{' '.join([f'{x:.2e}' for x in sbr[0]])}"
     Tirific_Template['SBR_2'] = f"{' '.join([f'{x:.2e}' for x in sbr[1]])}"
-    sf.print_log(f'''FIX_SBR: We checked the surface brightness profiles.
+    print_log(f'''FIX_SBR: We checked the surface brightness profiles.
 ''',Configuration,case=['verbose'])
 fix_sbr.__doc__ =f'''
  NAME:
     fix_sbr
 
  PURPOSE:
     Correct the surface brightness profile against outliers.
@@ -1437,78 +1531,71 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_error(Configuration,profile,sm_profile,key,min_error = None,\
+def get_error(Configuration,profile,sm_profile,key,min_error = 0.,\
     singular = False,weights= None,apply_max_error = False ):
-
-    if min_error is None:
-        min_error = [0.]
     if weights is None:
         weights= [1.]
-    try:
-        size= len(min_error)
-        min_error = np.array(min_error,dtype=float)
-    except TypeError:
-        min_error = np.array([min_error],dtype=float)
-
-    sf.print_log(f'''GET_ERROR: starting;
-{'':8s}original profile = {profile}
-{'':8s}new profile = {sm_profile}
-{'':8s}weights = {weights}
-{'':8s}singular = {singular}
-{'':8s}min_error = {min_error}
-{'':8s}max_error = {apply_max_error}
+    print_log(f'''GET_ERROR: starting;
 ''',Configuration, case=['debug_start'])
-
     if singular:
         if len(weights) == 1:
             weights = np.full((len(profile)),weights[0])
-        profile = [profile]
-        sm_profile = [sm_profile]
+        profile = np.array([profile],dtype=float)
+        sm_profile = np.array([sm_profile],dtype=float)
         error =[[]]
         sides = [0]
-
+     
     else:
-        error = [[],[]]
+        error = [[],[]] 
+        profile = np.array(profile,dtype=float)
         if len(weights) == 1:
             weights = np.full((len(profile[0]),len(profile[1])),1.)
         sides =[0,1]
-    sf.print_log(f'''GET_ERROR: using these weights =
-{'':8s}{weights}
-''',Configuration,case=['debug_add'])
+    min_error = get_min_error(Configuration,min_error_in=min_error,profile=profile,parameter=key)
+    if singular:
+        if min_error.shape[0] != 1:
+            min_error = np.array([min_error],dtype=float)
+    print_log(f'''GET_ERROR: Using these values;
+{'':8s}original profile = {profile}
+{'':8s}new profile = {sm_profile}
+{'':8s}weights = {weights}
+{'':8s}singular = {singular}
+{'':8s}min_error = {min_error}
+{'':8s}max_error = {apply_max_error}
+''',Configuration, case=['debug_add'])
+    
     for i in sides:
         error[i] = abs(profile[i]-sm_profile[i])/2.
         error[i]= error[i]/weights[i]
-        if len(min_error.shape) == 2:
-            error[i] = [np.max([y,x]) for x,y in zip(error[i],min_error[i])]
-        elif len(min_error) == len(error[i]):
-            error[i] = [np.max([y,x]) for x,y in zip(error[i],min_error)]
-        else:
-            error[i] = [np.max([x,min_error[0]]) for x in error[i]]
+       
+        error[i] = [np.max([y,x]) for x,y in zip(error[i],min_error[i])]
+        
         if apply_max_error:
             if len(Configuration['MAX_ERROR'][key]) == len(error[i]):
                 error[i] = [np.nanmin([x,y]) for x,y in zip(error[i],Configuration['MAX_ERROR'][key])]
             else:
                 error[i] = [np.nanmin([x,float(Configuration['MAX_ERROR'][key][0])]) for x in error[i]]
         if key in ['PA','INCL','Z0','ARBITRARY']:
             error[i][:Configuration['INNER_FIX'][i]+1] = [np.min(min_error) for x in error[i][:Configuration['INNER_FIX'][i]+1]]
     if singular:
         error = np.array(error[0],dtype=float)
     else:
         error = np.array(error,dtype=float)
-    if np.sum(error) == 0.:
-        error[:] = min_error
-    if 0. in error:
-        error[error == 0.] = np.min(error[error > 0.])
+    
+    low = np.where(error < min_error)
+    if np.sum(low) > 0.:
+        error[low] =min_error[low]
 
-    sf.print_log(f'''GET_ERROR: error =
+  
+    print_log(f'''GET_ERROR: error =
 {'':8s}{error}
 ''',Configuration,case=['debug_add'])
     return error
 get_error.__doc__ =f'''
  NAME:
     get_error
 
@@ -1544,59 +1631,113 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: the maximum errors are defined in main.py
 '''
-
+def get_min_error(Configuration,profile = None,min_error_in = None, parameter = None):
+    if profile is None:
+        raise FunctionCallError(f'You have to provide a profile to match')
+    if min_error_in is None:
+        if parameter is None:
+            raise FunctionCallError(f'You have to provide a parameter (parameter=) or input min_error (min_error_in=)')
+        else:
+            if parameter in Configuration['MIN_ERR']:
+                min_error = np.full(profile.shape,Configuration['MIN_ERR'][parameter][0])
+            else:
+                min_error = 0.
+    else:
+        min_error = copy.deepcopy(min_error_in)
+    
+    #If they have the same shape we stop here
+   
+    
+    # else we first check it is equivalant
+    if sf.isiterable(min_error):
+        min_error= np.array(min_error,dtype=float)
+        if min_error.shape == profile.shape:
+            return min_error
+        print_log(f'''GET_MIN_ERROR:  These are the input shapes:
+{'':8s} min_errror =  {min_error.shape} 
+{'':8s} profile =  {profile.shape}
+''',Configuration,case=['debug_add'])
+        try:
+            if min_error.shape[0] == profile.shape[1]:
+                min_error = np.array([min_error,min_error],dtype=float)
+            elif min_error.shape[0] == 1:
+                min_error = np.full(profile.shape,min_error[0])
+            else:
+                tmp_err1,profile1 = sf.make_equal_length(min_error[0],profile[0]) 
+                tmp_err2,profile2 = sf.make_equal_length(min_error[1],profile[1])
+                min_error = np.array([tmp_err1,tmp_err2],dtype=float)
+        
+        except IndexError:
+            print_log(f'''GET_MIN_ERROR: Assuming singular
+''',Configuration,case=['debug_add'])
+            if min_error.shape[0] == 1:
+                min_error = np.full(profile.shape,min_error[0])
+            else:
+                tmp_err1,profile1 = sf.make_equal_length(min_error[0],profile[0]) 
+                min_error = np.array([tmp_err1],dtype=float)
+    else:
+        print_log(f'''GET_MIN_ERROR:  min_error is not iterable
+''',Configuration,case=['debug_add'])
+        min_error = np.full(profile.shape,min_error)
+    if min_error.shape != profile.shape:
+        print_log(f'''GET_MIN_ERROR:  These are the input shapes:
+{'':8s} min_errror =  {min_error.shape} 
+{'':8s} profile =  {profile.shape}
+''',Configuration,case=['debug_add'])
+        raise FunctionCallError('GET_MIN_ERROR: the min error and profile shape are not matching')
+    return min_error          
 
 def get_number_of_rings(Configuration,sbr,sbr_ring_limits ):
     '''Determine whether the amount of rings is good for the limits or not'''
     new_rings = Configuration['NO_RINGS']
     difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
     if np.all(difference_with_limit[:,-1] < 0.):
-        sf.print_log(f'''GET_NUMBER_OF_RINGS: both last rings are below the limit
+        print_log(f'''GET_NUMBER_OF_RINGS: both last rings are below the limit
 ''',Configuration,case=['debug_start'])
         for i in range(len(difference_with_limit[0,:])-1,int(new_rings/2.),-1):
-            sf.print_log(f'''GET_NUMBER_OF_RINGS: Checking ring {i}
+            print_log(f'''GET_NUMBER_OF_RINGS: Checking ring {i}
 ''',Configuration,case=['debug_add'])
             if np.all(difference_with_limit[:,i] < 0.):
                 #check that 1 any of the lesser rings are bright enough
                 if np.any(sbr[:,i-1] > 1.5 *sbr_ring_limits[:,i-1]):
                     new_rings = i+1
-                    sf.print_log(f'''GET_NUMBER_OF_RINGS: we find that the previous rings are bright enough, rings = {new_rings}
+                    print_log(f'''GET_NUMBER_OF_RINGS: we find that the previous rings are bright enough, rings = {new_rings}
 ''',Configuration,case=['debug_add'])
                     break
                 else:
-                    sf.print_log(f'''GET_NUMBER_OF_RINGS: the previous rings are not bright enough so we reduce 1, old_rings = {new_rings}, new_rings = {i}
+                    print_log(f'''GET_NUMBER_OF_RINGS: the previous rings are not bright enough so we reduce 1, old_rings = {new_rings}, new_rings = {i}
 ''',Configuration,case=['debug_add'])
                     new_rings = i
             else:
                 #if not both values are below than this is the extend we want
                 new_rings = i+1
-                sf.print_log(f'''GET_NUMBER_OF_RINGS: Not both rings warrant cutting, rings = {new_rings}
+                print_log(f'''GET_NUMBER_OF_RINGS: Not both rings warrant cutting, rings = {new_rings}
 ''',Configuration,case=['debug_add'])
                 break
     else:
-        sf.print_log(f'''GET_NUMBER_OF_RINGS: Not both last rings are below the limit
+        print_log(f'''GET_NUMBER_OF_RINGS: Not both last rings are below the limit
 ''',Configuration,case=['debug_add'])
         # if they are not we first check wether both second to last rings are
         if ((difference_with_limit[0,-2] < 0.) and (sbr[0,-1] < 2*sbr_ring_limits[0,-1]) and (difference_with_limit[1,-1] < 0.)) or \
             ((difference_with_limit[1,-2] < 0.) and (sbr[1,-1] < 2*sbr_ring_limits[1,-1]) and (difference_with_limit[0,-1] < 0.)) or\
             ((difference_with_limit[0,-2] < 0.) and (difference_with_limit[1,-2] < 0.) and (sbr[0,-1] < 3*sbr_ring_limits[0,-1]) and (sbr[1,-1] < 3*sbr_ring_limits[1,-1])):
             new_rings -= 1
-            sf.print_log(f'''GET_NUMBER_OF_RINGS: A second ring is too faint, rings = {new_rings}
+            print_log(f'''GET_NUMBER_OF_RINGS: A second ring is too faint, rings = {new_rings}
 ''',Configuration,case=['debug_add'])
         elif np.all(difference_with_limit[:,-2] < 0.) and np.all(sbr[:,-1] < 5*sbr_ring_limits[:,-1]):
             new_rings -= 1
-            sf.print_log(f'''GET_NUMBER_OF_RINGS: Both second rings are too faint, rings = {new_rings}
+            print_log(f'''GET_NUMBER_OF_RINGS: Both second rings are too faint, rings = {new_rings}
 ''',Configuration,case=['debug_add'])
         else:
-            sf.print_log(f'''GET_NUMBER_OF_RINGS: The second rings are too bright and do not allow for cutting.
+            print_log(f'''GET_NUMBER_OF_RINGS: The second rings are too bright and do not allow for cutting.
 ''',Configuration,case=['debug_add'])
     return new_rings
 get_number_of_rings.__doc__ =f'''
  NAME:
     get_number_of_rings
 
  PURPOSE:
@@ -1620,22 +1761,83 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def get_ring_weights(Configuration,Tirific_Template):
+    print_log(f'''GET_RING_WEIGTHS: Getting the importance of the rings in terms of SBR.
+''',Configuration,case=['debug_start'])
+    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=["SBR",f"SBR_2"],\
+                array=True )
+    
+    print_log(f'''GET_RING_WEIGTHS: retrieve this sbr.
+{'':8s} sbr = {sbr}
+''',Configuration,case=['debug_add'])
+    cut_off_limits = sf.sbr_limits(Configuration,Tirific_Template )
+    print_log(f'''GET_RING_WEIGTHS: retrieved these cut_off_limits.
+{'':8s} col = {cut_off_limits}
+''',Configuration,case=['debug_add'])
+    sm_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',
+                            min_error= [cut_off_limits,cut_off_limits],no_apply = True,
+                            fix_sbr_call = True, profile_in = sbr )
+    print_log(f'''GET_RING_WEIGTHS: retrieve this sbr.
+{'':8s} sbr = {sbr}
+{'':8s} using sm_sbr {sm_sbr}
+''',Configuration,case=['debug_add'])
+
+    weights= [[],[]]
+    for i in [0,1]:
+        weights[i] = [sf.set_limits(x/y,0.1,10.) for x,y in zip(sm_sbr[i],cut_off_limits)]
+        weights[i] = weights[i]/np.nanmax(weights[i])
+        weights[i][0:2] = np.nanmin(weights[i])
+        weights[i] = [sf.set_limits(x,0.1,1.) for x in weights[i]]
+    print_log(f'''GET_RING_WEIGTHS: Obtained the following weights.
+{'':8s}{weights}
+''',Configuration,case=['debug_add'])
+    return np.array(weights,dtype = float)
+
+get_ring_weights.__doc__=f'''
+ NAME:
+    get_ring_weights
+
+ PURPOSE:
+    Get the importance of the rings based on how much the SBR lies above the noise limit for each ring
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Tirific_Template = Standard Tirific template containg the SBR profiles
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    numpy array with the weight normalized to the the maximum.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+    Weight 1 is most important, weight 0. least important.
+    Errors should be divided by these weights to reflect the importance
+'''
 def get_warp_slope(Configuration,Tirific_Template):
-    sf.print_log(f'''GET_WARP_SLOPE: We have {Tirific_Template['NUR']} rings in the template. and this should be {Configuration['NO_RINGS']}
+    print_log(f'''GET_WARP_SLOPE: We have {Tirific_Template['NUR']} rings in the template. and this should be {Configuration['NO_RINGS']}
 ''', Configuration,case=['debug_start'])
-    radii, sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
+    sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
     #get the sbr profiles
     sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
                 array=True)
-    sf.print_log(f'''GET_WARP_SLOPE: We have {len(sbr_ring_limits)} rings in our limits.
+    print_log(f'''GET_WARP_SLOPE: We have {len(sbr_ring_limits)} rings in our limits.
 {'':8s}GET_WARP_SLOPE: And we have {len(sbr[0])} rings in our profiles.
 ''', Configuration,case=['debug_add'])
     warp_slope = [int(Tirific_Template['NUR']),int(Tirific_Template['NUR'])]
     sbr_ring_limits = 1.5*np.array([sbr_ring_limits,sbr_ring_limits],dtype=float)
     difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
     for i in [0,1]:
         slope = difference_with_limit[i]
@@ -1660,15 +1862,15 @@
         if final > Configuration['LAST_RELIABLE_RINGS'][i]-1:
             final = Configuration['LAST_RELIABLE_RINGS'][i]-1
         # we have to vary some rings else tirific will break with a segmentation fault
         if final < 2:
             final = 2
 
         warp_slope[i] = int(final)
-    sf.print_log(f'''GET_WARP_SLOPE: We find a slope of {warp_slope}.
+    print_log(f'''GET_WARP_SLOPE: We find a slope of {warp_slope}.
 ''', Configuration,case=['debug_add'])
     Configuration['WARP_SLOPE'] = warp_slope
     incl = sf.load_tirific(Configuration,Tirific_Template,Variables=['INCL','INCL_2'],\
             array=True)
     if np.mean(incl[:,:int(Configuration['NO_RINGS']/2.)]) < 35. :
         if 'INCL' not in Configuration['FIXED_PARAMETERS'][0]:
             Configuration['FIXED_PARAMETERS'][0].append('INCL')
@@ -1699,45 +1901,45 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def inner_sbr_fix(Configuration,sbr,cutoff_limits ):
-    sf.print_log(f'''INNER_SBR_FIX: Checking the SBR inner points for runaway values
+    print_log(f'''INNER_SBR_FIX: Checking the SBR inner points for runaway values
 {'':8s} sbr in  = {sbr}
 ''',Configuration,case=['debug_start'])
 
     if np.all(sbr[:,0] > 2*sbr[:,2]) or np.all(sbr[:,1] > 2*sbr[:,2]):
-        sf.print_log(f'''INNER_SBR_FIX: We need to correct
+        print_log(f'''INNER_SBR_FIX: We need to correct
 {'':8s} sbr 0  = {sbr[:,0]} sbr 1  = {sbr[:,1]} sbr 2  = {sbr[:,2]}
 ''',Configuration,case=['debug_add'])
         if np.mean(sbr[:,2]) > cutoff_limits[0,2]:
             sbr[:,[0,1]] = np.mean(sbr[:,2])
-            sf.print_log(f'''INNER_SBR_FIX: We need to correct with mean
+            print_log(f'''INNER_SBR_FIX: We need to correct with mean
 {'':8s} mean = {np.mean(sbr[:,2])}
 ''',Configuration,case=['debug_add'])
         else:
-            sf.print_log(f'''INNER_SBR_FIX: We need to correct with cut_off_limits
+            print_log(f'''INNER_SBR_FIX: We need to correct with cut_off_limits
 {'':8s} limit = {1.5*cutoff_limits[0,2]}
 ''',Configuration,case=['debug_add'])
             sbr[:,[0,1,2]] = 1.5*cutoff_limits[0,2]
     if np.any(sbr[:,0] > sbr[:,1]):
-        sf.print_log(f'''INNER_SBR_FIX: We correct 0 point
+        print_log(f'''INNER_SBR_FIX: We correct 0 point
 {'':8s} mean 1 = {np.mean(sbr[:,1])}
 ''',Configuration,case=['debug_add'])
         sbr[:,0] = np.mean(sbr[:,1])
 
     for i in [0,1]:
         if np.any(sbr[:,i] < cutoff_limits[:,2]):
-            sf.print_log(f'''INNER_SBR_FIX: correcting ring {i}
+            print_log(f'''INNER_SBR_FIX: correcting ring {i}
 ''',Configuration,case=['debug_add'])
             sbr[:,i] = 1.5*cutoff_limits[0,2]
 
-    sf.print_log(f'''INNER_SBR_FIX: the fixed sbr {sbr}
+    print_log(f'''INNER_SBR_FIX: the fixed sbr {sbr}
 ''',Configuration,case=['debug_add'])
 
     return sbr
 inner_sbr_fix.__doc__ =f'''
  NAME:
     inner_sbr_fix
 
@@ -1765,27 +1967,27 @@
 
  NOTE:
 '''
 
 def modify_flat(Configuration,profile,original_profile,errors,key,inner_fix = None):
     if inner_fix is None:
         inner_fix = [4,4]
-    sf.print_log(f'''MODIFY_FLAT: These {key} profiles are checked to be flat.
+    print_log(f'''MODIFY_FLAT: These {key} profiles are checked to be flat.
 {'':8s} profile = {profile}
 {'':8s} original_profile = {original_profile}
 {'':8s} errors = {errors}
 ''',Configuration,case=['debug_start'])
 
     flatness = []
 
 
     for side in [0,1]:
          flatness.append(check_flat(Configuration,profile[side],errors[side],key,inner_fix=inner_fix[side]\
                                     ,last_reliable_ring= Configuration['LAST_RELIABLE_RINGS'][side]))
-    sf.print_log(f'''MODIFY_FLAT: Side 0 is flat = {flatness[0]}
+    print_log(f'''MODIFY_FLAT: Side 0 is flat = {flatness[0]}
 {'':8s} Side 1 is flat = {flatness[1]}
 ''',Configuration,case=['debug_add'])
 
     if all(flatness):
         if key in ['PA','INCL']:
             profile[:] = profile[0,0]
         else:
@@ -1813,15 +2015,15 @@
                 profile[:,0:3] = flat_val
                 profile[:,4] = (flat_val+profile[:,4])/2.
             else:
                 profile[:] = np.nanmedian(original_profile[:,:round(len(original_profile)/2.)])
                 errors = get_error(Configuration,original_profile,profile,key,\
                         apply_max_error = True,min_error =np.nanmin(errors))
 
-    sf.print_log(f'''MODIFY_FLAT: Returning:
+    print_log(f'''MODIFY_FLAT: Returning:
 {'':8s} profile = {profile}
 {'':8s} errors = {errors}
 ''',Configuration,case=['debug_add'])
     return profile,errors
 modify_flat.__doc__ =f'''
  NAME:
     modify_flat
@@ -1851,38 +2053,38 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def no_declining_vrot(Configuration, Tirific_Template, profile = None):
-    sf.print_log(f'''NO_DECLINING_VROT: make RC flat from highest point on.
+    print_log(f'''NO_DECLINING_VROT: make RC flat from highest point on.
 {'':8s}NO_DECLINING_VROT: But only for low value RCs
 ''',Configuration, case=['debug_start'])
     no_input = False
     if profile is None:
         no_input = True
         profile = sf.load_tirific(Configuration,Tirific_Template,Variables=['VROT'],\
                     array=True)
     RCval = np.mean(profile[2:])
     RCmax = np.where(profile == np.max(profile))[0]
     if len(RCmax) > 1:
         RCmax = RCmax[0]
-    sf.print_log(f'''NO_DECLINING_VROT: We find the maximum at ring {RCmax}
+    print_log(f'''NO_DECLINING_VROT: We find the maximum at ring {RCmax}
 {'':8s}NO_DECLINING_VROT: And a mean value of {RCval}.
 ''',Configuration,case=['debug_add'])
     Configuration['OUTER_SLOPE_START'] = Configuration['NO_RINGS']-1
     if RCmax < len(profile)/2. or RCval > 180.:
-        sf.print_log(f'''NO_DECLINING_VROT: We shan't adapt the RC
+        print_log(f'''NO_DECLINING_VROT: We shan't adapt the RC
 ''',Configuration,case=['debug_add'])
     else:
         for i in range(int(len(profile)/2.),len(profile)-1):
             if profile[i+1] < profile[i]:
                 profile[i:] =profile[i]
-                sf.print_log(f'''NO_DECLINING_VROT: Flattening from ring {i} on.)
+                print_log(f'''NO_DECLINING_VROT: Flattening from ring {i} on.)
     ''',Configuration,case=['debug_add'])
                 Configuration['OUTER_SLOPE_START'] = i+2
                 break
 
     #and we check that the last parts are not declining too much in anycase
     # For galaxies with more than 10 rings let's make sure the last quarter is not declinining steeply
     if Configuration['NO_RINGS'] > 10:
@@ -1932,96 +2134,110 @@
     Unspecified
 
  NOTE:
 '''
 
 
 def regularise_profile(Configuration,Tirific_Template, key,min_error= None, \
-                            no_apply =False):
+                            no_apply =False,warp=False):
     if min_error is None:
-        min_error= [0.]
-    if key in ['PA','INCL']:
-        raise FunctionCallError('The warp is regularised in regularise_warp. regularise profile is for singular profiles only.')
-
-        # We start by getting an estimate for the errors
+        if key in Configuration['MIN_ERROR']:
+            min_error= Configuration['MIN_ERROR'][key]
+        else: 
+            min_error = [0.]
+    if key in ['PA','INCL'] and not warp:
+        raise FunctionCallError('The warp is regularised in regularise_warp. ')
+    # We start by getting an estimate for the errors
     min_error=np.array(min_error,dtype=float)
-    weights = sf.get_ring_weights(Configuration,Tirific_Template)
+    weights = get_ring_weights(Configuration,Tirific_Template)
     #For a lot of things it is important to use a unmodified input profile but we have to avoid the declining vrot
     if key == 'VROT':
         no_declining_vrot(Configuration, Tirific_Template)
-    profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
-    diff = np.sum(profile[0]-profile[1])#Check that we have two profiles
+    profile = sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"],array=True)
+    diff = abs(np.sum(profile[0]-profile[1]))#Check that we have two profiles
 
-    if diff <1e-8:
-        diff =0.
+    
 
     #First if we have an RC we flatten the curve
-    sf.print_log(f'''REGULARISE_PROFILE: profile of {key} before regularistion
+    print_log(f'''REGULARISE_PROFILE: profile of {key} before regularistion
 {'':8s}{profile[0]}
 {'':8s}{profile[1]}
 {'':8s}The minimal error is
 {'':8s}{min_error}
 ''',Configuration,case=['debug_start'])
-    # get a smoothed profiles
-    sm_profile = smooth_profile(Configuration,Tirific_Template, key ,min_error=min_error,no_apply=True)
+    #if the profiles is fixed we do not have to regularise and we return a flatted profile
+    if key in Configuration['FIXED_PARAMETERS'][0]:
+        for i in [0,1]:
+            profile[i][:]=np.mean(profile[i])  
+        set_errors(Configuration,Tirific_Template,key,min_error=min_error)
+        return profile
 
-    error = get_error(Configuration,profile,sm_profile,key,min_error=min_error,weights = weights)
+    # get a smoothed profiles
+    sm_profile = smooth_profile(Configuration,Tirific_Template, key \
+                                ,min_error=min_error,no_apply=True)
 
+   
+    error = get_error(Configuration,profile,sm_profile,key,\
+                        min_error=min_error,weights = weights)
+    if key in ['PA']:
+        for i in [0,1]:
+            error[i,:] = [np.mean([np.sqrt(x),min_error[0]]) if \
+                          np.sqrt(x) > min_error[0] else x for x in error[i,:]]
 
+  
     if key in ['SDIS','VROT']:
-        diff = False
-    if diff:
-        sf.print_log(f'''REGULARISE_PROFILE: Treating both sides independently.
+        diff = 0.
+    if diff > 1e-8:
+        print_log(f'''REGULARISE_PROFILE: Treating both sides independently.
 ''',Configuration,case=['debug_add'])
         sides = [0,1]
     else:
-        sf.print_log(f'''REGULARISE_PROFILE: Found symmetric profiles.
+        print_log(f'''REGULARISE_PROFILE: Found symmetric profiles.
 ''',Configuration,case=['debug_add'])
         sides = [0]
-        error[0] = np.array([np.mean([x,y]) for x,y in zip(error[0],error[1])],dtype=float)
+        error[0] = np.array([np.mean([x,y]) for x,y in \
+                                zip(error[0],error[1])],dtype=float)
 
     radii =sf.set_rings(Configuration)
     for i in sides:
-
         if key in ['SDIS']:
             function_to_fit =arc_tan_sdis_function
-            fit_profile = fit_arc(Configuration,radii,sm_profile[i],error[i],function_to_fit,key)
+            fit_profile = fit_arc(Configuration,radii,sm_profile[i],\
+                                    error[i],function_to_fit,key)
         else:
 
-            fit_profile = fit_polynomial(Configuration,radii,profile[i],sm_profile[i],error[i],key, Tirific_Template,\
-                                         inner_fix = Configuration['INNER_FIX'][i],min_error=min_error,\
-                                         boundary_limits= Configuration[f"{key}_CURRENT_BOUNDARY"][i+1])
+            fit_profile = fit_polynomial(Configuration,radii,\
+                profile[i],error[i],key, Tirific_Template,\
+                inner_fix = Configuration['INNER_FIX'][i],\
+                boundary_limits= Configuration[f"{key}_CURRENT_BOUNDARY"][i+1])
         profile[i] = fit_profile
 
-    if not diff:
+    if diff < 1e-8:
         profile[1] = profile[0]
 
     original = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
     error = get_error(Configuration,original,profile,key,weights=weights,apply_max_error = True,min_error=min_error)
-    sf.print_log(f'''REGULARISE_PROFILE: This the fitted profile without corrections:
+    print_log(f'''REGULARISE_PROFILE: This the fitted profile without corrections:
 {'':8s}{profile}
 ''',Configuration,case=['debug_add'])
 #then we want to fit the profiles with a polynomial
-    if key not in ['SBR','VROT','SDIS']:
+    if key not in ['SBR','VROT','SDIS','PA','INCL']:
         #We should not fix the profile again as the fitted profile is fixed should be good
-
         profile,error = modify_flat(Configuration, profile, original, error,key,inner_fix= Configuration['INNER_FIX'])
-
-
     format = sf.set_format(key)
 
     if not no_apply:
         Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[0,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[1,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[0,:int(Configuration['NO_RINGS'])]])}")
         Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[1,:int(Configuration['NO_RINGS'])]])}")
         #if key in ['INCL'] and np.mean( profile[:,int(Configuration['NO_RINGS']/2.):int(Configuration['NO_RINGS'])]) < 40.:
         #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original,profile)
 
-        sf.print_log(f'''REGULARISE_PROFILE: And this has gone to the template.
+        print_log(f'''REGULARISE_PROFILE: And this has gone to the template.
 {'':8s}{key} = {Tirific_Template[key]}
 {'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
 ''',Configuration,case=['debug_add'])
     return profile
 regularise_profile.__doc__ =f'''
@@ -2059,174 +2275,252 @@
 
  NOTE: Errors are not returned but they are written to the template
 '''
 
 
 def regularise_warp(Configuration,Tirific_Template, min_error = None, \
                         no_apply =False,smooth_only=False):
+    ''' 
+    Initially we did this by fitting a polynomial to the change_angle and
+    The factors but that sometimes led to very bad results. The we tried
+    to merely use smoothing on the factors but that leaves saw tooth
+    if we smooth and fit Theta and Phi individually this can lead to weird results
+    We cannot smooth the factors either they have to fitted with a polynomial
+    The fixed part  should be equal to fix+1 
+    Well it seems that the best option is to regularise the the profiles and 
+    only use an angular momentum check during the fitting.
+    but as we are running it every iteration we are not exactly sure what happens 
+    in the fitting
+    '''
+     # We start by getting an estimate for the errors
     if min_error is None:
-        min_error = [0.,0.]
-        # We start by getting an estimate for the errors
-    min_error=np.array(min_error,dtype=float)
-    weights = sf.get_ring_weights(Configuration,Tirific_Template)
-    profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [f"PA",f"PA_2",f"INCL",f"INCL_2"]),dtype=float)
-    diff = np.sum(profile[0]-profile[1])+np.sum(profile[2]-profile[3])  #Check that we have two profiles
-    if diff <1e-8:
-        diff = False
-    else:
-        diff = True
-
-    sf.print_log(f'''REGULARISE_WARP: profile of the warp before regularistion
-{'':8s}PA = {profile[0]}
-{'':8s}PA_2 = {profile[1]}
-{'':8s}INCL = {profile[2]}
-{'':8s}INCL_2 = {profile[3]}
-{'':8s}The minimal error is
-{'':8s}PA min Error = {min_error[0]}, INCL min Error = {min_error[1]}
-''',Configuration,case=['debug_start'])
-    # get a smoothed profiles
-    Theta,Phi,multiple= sf.calculate_am_vector(Configuration,profile[0],profile[2])
-    plus_Theta,plus_Phi,plus_multiple= sf.calculate_am_vector(Configuration,profile[1],profile[3])
-    Theta = np.array([Theta,plus_Theta],dtype=float)
-    Phi = np.array([Phi,plus_Phi],dtype=float)
-    multiple = np.array([multiple,plus_multiple],dtype=float)
-
-    high_theta,high_phi,high_multiple = sf.calculate_am_vector(Configuration,profile[0]+min_error[0],profile[2]+min_error[1])
-    if not np.array_equiv(high_multiple,multiple):
-        high_theta,high_phi,high_multiple = sf.calculate_am_vector(Configuration,profile[0]-min_error[0],profile[2]-min_error[1])
-    low_theta,low_phi,low_multiple = sf.calculate_am_vector(Configuration,profile[1]+min_error[0],profile[3]+min_error[1])
-    if not np.array_equiv(low_multiple,multiple):
-        low_theta,low_phi,low_multiple = sf.calculate_am_vector(Configuration,profile[1]-min_error[0],profile[3]-min_error[1])
-
-    min_change_error = np.sqrt(np.min(np.array([np.min([abs(x-y),abs(w-z)]) for x,y,w,z in zip(Theta[0],high_theta,Theta[1],low_theta)],dtype=float))**2+\
-            np.min(np.array([np.min([abs(x-y),abs(w-z)]) for x,y,w,z in zip(Phi[0],high_phi,Phi[1],low_phi)],dtype=float))**2)
-
-    sf.print_log(f'''REGULARISE_WARP: These converted arrays
-{'':8s}Theta = {Theta[0,:]}
-{'':8s}Theta_2 = {Theta[1,:]}
-{'':8s}Phi = {Phi[0,:]}
-{'':8s}Phi_2 = {Phi[1,:]}
-{'':8s}The minimal error is
-{'':8s}min change Error = {min_change_error}
-''',Configuration,case=['debug_add'])
+        if 'PA' in Configuration['MIN_ERROR'] and 'INCL' in \
+            Configuration['MIN_ERROR']:
+            min_error = [Configuration['MIN_ERROR']['PA'],\
+                         Configuration['MIN_ERROR']['INCL']]
+        else:
+            min_error = [0.,0.]
 
-    theta_zero = Theta[:,0]
-    phi_zero = Theta[:,0]
-    multiple_zero = multiple[:,0]
-     #Let's combine the variation as fraction of the existing angle
-    theta_change= np.array([[float(x-theta_zero[0]) for x in Theta[0]],\
-                            [float(x-theta_zero[1]) for x in Theta[1]]],dtype=float)
-    phi_change= np.array([[float(x-phi_zero[0]) for x in Phi[0]],\
-                            [float(x-phi_zero[1]) for x in Phi[1]]],dtype=float)
+    min_error=np.array(min_error,dtype=float)
+    weights = get_ring_weights(Configuration,Tirific_Template)
+   
+    #if the PA and INCL are fixed we stop here
+    if 'PA' in Configuration['FIXED_PARAMETERS'][0] and 'INCL' in \
+          Configuration['FIXED_PARAMETERS'][0]:
+        profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [f"PA",f"PA_2",f"INCL",f"INCL_2"]),dtype=float)
+        for i in [0,1,2,3]:
+            profile[i][:]=np.mean(profile[i])
+        for i,key in enumerate(['PA','INCL']):  
+            set_errors(Configuration,Tirific_Template,key,min_error=min_error[i])
+        return profile
 
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore",message="invalid value encountered in true_divide"\
-                            ,category=RuntimeWarning)
-        theta_factor = np.sqrt(theta_change**2/(theta_change**2+phi_change**2))\
-                    *(theta_change)/abs(theta_change)
-        theta_factor[np.where(np.array(theta_change) == 0.)] = 0.
-        phi_factor = np.sqrt(phi_change**2/(theta_change**2+phi_change**2))*(phi_change)/abs(phi_change)
-        phi_factor[np.where(np.array(phi_change) == 0.)] = 0.
-    sf.print_log(f'''REGULARISE_WARP: These converted arrays
-{'':8s}Theta_factor = {theta_factor[0,:]}
-{'':8s}Theta_factor_2 = {theta_factor[1,:]}
-{'':8s}Phi_factor = {phi_factor[0,:]}
-{'':8s}Phi_factor_2 = {phi_factor[1,:]}
-''',Configuration,case=['debug_add'])
-    in_zero = np.where(np.array(theta_change+phi_change) == 0.)
-    phi_factor[in_zero]=0.
-    theta_factor[in_zero]=0.
-    change_angle = np.sqrt(theta_change**2+phi_change**2)
-    change_angle[in_zero] =0.
-    change_boundary = calculate_change_boundary(Configuration,multiple_zero,theta_zero,phi_zero)
-    sm_change_angle = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=change_angle, min_error=min_change_error,no_apply=True)
-    sm_theta_factor = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=theta_factor, min_error=0.005,no_apply=True)
-    sm_phi_factor = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=phi_factor, min_error=0.005,no_apply=True)
-
-    error_change_angle = get_error(Configuration,change_angle,sm_change_angle,'ARBITRARY',min_error=min_change_error,weights = weights)
-    error_theta_factor = get_error(Configuration,theta_factor,sm_theta_factor,'ARBITRARY',min_error=0.005,weights = weights)
-    error_phi_factor = get_error(Configuration,phi_factor,sm_phi_factor,'ARBITRARY',min_error=0.005,weights = weights)
 
-    if diff:
-        sf.print_log(f'''REGULARISE_WARP: Treating both sides independently.
+   
+    if smooth_only:
+        pa_both_sides = smooth_profile(Configuration,Tirific_Template, 'PA' ,\
+                    min_error=min_error[0]/3.,no_fix=False,no_apply=True)
+    
+        incl_both_sides = smooth_profile(Configuration,Tirific_Template, 'INCL' ,\
+                    min_error=min_error[1]/3.,no_fix=True,no_apply=True)
+
+    else:
+        pa_both_sides = regularise_profile(Configuration,Tirific_Template,\
+                        'PA',warp=True,no_apply=True) 
+    
+        incl_both_sides = regularise_profile(Configuration,Tirific_Template,\
+                        'INCL',warp=True,no_apply=True) 
+    
+    profile= np.concatenate((pa_both_sides,incl_both_sides))  
+    diff = abs(np.sum(profile[0]-profile[1]))+abs(np.sum(profile[2]-profile[3]))  #Check that we have two profiles
+    if diff < 1e-8:
+        print_log(f'''REGULARISE_WARP: Found symmetric profiles.
 ''',Configuration,case=['debug_add'])
-        sides = [0,1]
+        sides = [0]  
     else:
-        sf.print_log(f'''REGULARISE_WARP: Found symmetric profiles.
-''',Configuration,case=['debug_add'])
-        sides = [0]
-
-    radii =sf.set_rings(Configuration)
+        print_log(f'''REGULARISE_WARP: Treating both sides independently.
+''',Configuration,case=['debug_add'])      
+        sides = [0,1]
+    radii =sf.set_rings(Configuration)    
     for i in sides:
-        sf.print_log(f'''REGULARISE_WARP: For side {i} we  regularise the following profile.
-{'':8s} change_angle = {change_angle[i]}
-{'':8s} sm_change_angle = {sm_change_angle[i]}
-''',Configuration,case=['debug_add'])
+        #put the pa and inc in a single profile
+        one_side_profile = [profile[i],profile[i+2]] 
+        print_log(f'''REGULARISE_WARP: profile of the warp for side {i} before regularistion
+{'':8s}PA = {one_side_profile[0]}
+{'':8s}INCL = {one_side_profile[1]}
+{'':8s}The minimal error is
+{'':8s}PA min Error = {min_error[0]}, INCL min Error = {min_error[1]}
+''',Configuration,case=['debug_start'])
+        #we need to fix them in the inner part before transforming
+        pa = fix_profile(Configuration, 'PA', \
+            one_side_profile[0], inner_fix = Configuration['INNER_FIX'][i],\
+            singular = True,only_inner = True )
+        inclination = fix_profile(Configuration, 'INCL', \
+            one_side_profile[1], inner_fix = Configuration['INNER_FIX'][i],\
+            singular = True,only_inner = True )
+        #first fit PA and INCL indpendently
+        #pa,inclination,changed_angles = sf.check_angular_momentum_vector(Configuration,\
+        #    radii,one_side_profile[0],one_side_profile[1],side=i,regularise=True)
+
+        
         if smooth_only:
-            new_change_angle = sm_change_angle[i]
-            new_theta_factor = theta_factor[i]
-            new_phi_factor = phi_factor[i]
-        else:
-            new_change_angle,fit_order = fit_polynomial(Configuration,radii,change_angle[i],sm_change_angle[i],error_change_angle[i],'ARBITRARY', Tirific_Template,\
-                                         inner_fix = Configuration['INNER_FIX'][i],min_error=min_change_error,\
-                                         allowed_order= [2,5],boundary_limits= change_boundary[i+1], return_order=True)
-            new_theta_factor = fit_polynomial(Configuration,radii,theta_factor[i],sm_theta_factor[i],error_theta_factor[i],'ARBITRARY', Tirific_Template,\
-                                         inner_fix = Configuration['INNER_FIX'][i],min_error=0.005,\
-                                         allowed_order= [fit_order,fit_order],boundary_limits= [0.,1.])
-            new_phi_factor = fit_polynomial(Configuration,radii,phi_factor[i],sm_phi_factor[i],error_phi_factor[i],'ARBITRARY', Tirific_Template,\
-                                         inner_fix = Configuration['INNER_FIX'][i],min_error=0.005,\
-                                         allowed_order= [fit_order,fit_order],boundary_limits= [0.,1.])
-        sf.print_log(f'''REGULARISE_WARP:
-{'':8s} new_change_angle = {new_change_angle}
-{'':8s} new_theta_factor = {new_theta_factor}
-{'':8s} new_phi_factor  = {new_phi_factor}
-''',Configuration,case=['debug_add'])
-        new_theta_change = new_change_angle*new_theta_factor
-        new_phi_change = new_change_angle*new_phi_factor
-
-        Theta[i] = theta_zero[i]+new_theta_change
-        Phi[i] = phi_zero[i]+new_phi_change
-        sf.print_log(f'''REGULARISE_WARP:
-{'':8s} Theta = {Theta[i]}
-{'':8s} Phi = {Phi[i]}
+        # get Phi and Theta for both sides
+            Theta,Phi,multiple= sf.calculate_am_vector(Configuration,
+                                    one_side_profile[0],one_side_profile[1])
+            
+            
+            high_theta,high_phi,high_multiple = sf.calculate_am_vector(\
+                Configuration,one_side_profile[0]+min_error[0],\
+                one_side_profile[1]+min_error[1])
+            if not np.array_equiv(high_multiple,multiple):
+                high_theta,high_phi,high_multiple = sf.calculate_am_vector(\
+                Configuration,one_side_profile[0]-min_error[0],\
+                one_side_profile[1]-min_error[1])
+
+            min_change_error = np.sqrt(np.min(np.array([abs(x-y)\
+                for x,y in zip(Theta,high_theta)],dtype=float))**2+\
+                np.min(np.array([abs(x-y) for x,y in zip(Phi,high_phi)],dtype=float))**2)
+
+            print_log(f'''REGULARISE_WARP: These converted arrays for side {i}
+{'':8s}Theta = {Theta}
+{'':8s}Phi = {Phi}
+{'':8s}The minimal error is
+{'':8s}min change Error = {min_change_error}
 ''',Configuration,case=['debug_add'])
-        pa,inclination=sf.calculate_am_vector(Configuration,Theta[i],Phi[i],multiple = multiple[i], invert=True)
+            multiple_zero = multiple[0]
+            
+            #Calculate the change angle
+            change_angle = sf.calculate_change_angle(Configuration,Theta,Phi)
+                #if this side is not warping we have to skip
+            if np.sum(change_angle['CHANGE_ANGLE']) == 0.:
+                continue
+            change_boundary = calculate_change_boundary(Configuration,multiple_zero,\
+                        change_angle['THETA']['ZERO'],change_angle['PHI']['ZERO'],\
+                        pa_boun =Configuration['PA_CURRENT_BOUNDARY'][i+1],\
+                        incl_boun =Configuration['INCL_CURRENT_BOUNDARY'][i+1])
+            sm_change_angle = smooth_profile(Configuration,Tirific_Template, 'CHANGE_ANGLE' \
+                ,profile_in=change_angle['CHANGE_ANGLE'],\
+                min_error=min_change_error,no_apply=True,no_fix =True,singular=True)
+            
+
+            sm_theta_factor,sm_phi_factor = smooth_factor_profile(Configuration, \
+                change_angle,radii,inner_fix=Configuration['INNER_FIX'][i],\
+                Tirific_Template=Tirific_Template)
+          
+           
+            error_change_angle = get_error(Configuration,change_angle['CHANGE_ANGLE'],\
+                sm_change_angle,'CHANGE_ANGLE',min_error=min_change_error,\
+                weights = weights,singular=True)
+            
+            print_log(f'''REGULARISE_WARP: For side {i} we  regularise the following profile.
+        {'':8s} change_angle = {change_angle['CHANGE_ANGLE'][i]}
+        {'':8s} sm_change_angle = {sm_change_angle[i]}
+        ''',Configuration,case=['debug_add'])
+            #if smooth_only:
+            new_change_angle = sm_change_angle
+            #    new_theta_factor = sm_theta_factor
+            #    new_phi_factor = sm_phi_factor
+            #else:
+                
+            #    new_change_angle,fit_order = fit_polynomial(Configuration,radii,\
+            #        change_angle['CHANGE_ANGLE'],error_change_angle,'CHANGE_ANGLE', Tirific_Template,\
+            #        inner_fix = Configuration['INNER_FIX'][i],\
+            #        allowed_order= [3,6],boundary_limits= change_boundary, return_order=True)
+                
+            print_log(f'''REGULARISE_WARP:
+        {'':8s} new_change_angle = {new_change_angle}
+        {'':8s} new_theta_factor = {sm_theta_factor}
+        {'':8s} new_phi_factor  = {sm_phi_factor}
+        ''',Configuration,case=['debug_add'])
+            new_change_dict = copy.deepcopy(change_angle)
+            new_change_dict['CHANGE_ANGLE'] = new_change_angle
+            new_change_dict['THETA']['FACTOR'] = sm_theta_factor
+            new_change_dict['PHI']['FACTOR'] = sm_phi_factor
+            #tyr= True
+            #if tyr:
+            #    plot_output(radii,change_angle,new_change_dict,i)
+                
+
+                                
+            print_log(f'''REGULARISE_WARP: For side {i} we get
+        {'':8s} Original Theta = {Theta}
+        {'':8s} Original Phi = {Phi}
+        ''',Configuration,case=['debug_add']) 
+                    
+            Theta,Phi = sf.revert_change_angle(Configuration,new_change_dict)
+            
+            print_log(f'''REGULARISE_WARP: For side {i} we get
+        {'':8s} Theta = {Theta}
+        {'':8s} Phi = {Phi}
+        ''',Configuration,case=['debug_add'])
+            
+            pa,inclination=sf.calculate_am_vector(Configuration,Theta,\
+                                Phi,multiple = multiple, invert=True)
+    
+        pa[:Configuration['INNER_FIX'][i]] = np.mean(pa[:Configuration['INNER_FIX'][i]])
+        inclination[:Configuration['INNER_FIX'][i]] = np.mean(inclination[:Configuration['INNER_FIX'][i]])
         profile[i]=pa
         profile[i+2]=inclination
-
-
-    if not diff:
+        #if i == 0:
+        #    print('Decidedly odd')
+        #    print(pa,inclination)
+            
+           
+    
+    if np.sum(sides) == 0.:
         profile[1] = profile[0]
         profile[3] = profile[2]
-    #exit()
+    else:
+        #print(profile,Configuration['INNER_FIX'])
+        fixed = np.mean(np.concatenate((profile[0,:Configuration['INNER_FIX'][0]],
+                          profile[1,:Configuration['INNER_FIX'][1]])))
+        profile[0,:Configuration['INNER_FIX'][0]]= fixed
+        profile[1,:Configuration['INNER_FIX'][1]]= fixed
+        fixed = np.mean(np.concatenate((profile[2,:Configuration['INNER_FIX'][0]],
+                          profile[3,:Configuration['INNER_FIX'][1]])))
+        profile[2,:Configuration['INNER_FIX'][0]]= fixed
+        profile[3,:Configuration['INNER_FIX'][1]]= fixed
+       
     error= copy.deepcopy(profile)
     error[:] = 0
+   
     for i,key in enumerate(['PA','INCL']):
-        original = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
-        sm_profile = smooth_profile(Configuration,Tirific_Template, key ,profile_in=profile[2*i:2*i+2], min_error=min_error[i]/3.,no_fix=True,no_apply=True)
-        sm_error =  get_error(Configuration,original,sm_profile,key,weights=weights,apply_max_error = True,min_error=min_error[i]/3.)
+        original = np.array(sf.load_tirific(Configuration,Tirific_Template,\
+                                             [key,f"{key}_2"]),dtype=float)
+        sm_profile = smooth_profile(Configuration,Tirific_Template, key ,\
+                    profile_in=profile[2*i:2*i+2], min_error=min_error[i]/3.,\
+                    no_fix=True,no_apply=True)
+        sm_error =  get_error(Configuration,original,sm_profile,key,\
+                weights=weights,apply_max_error = True,\
+                min_error=min_error[i]/3.)
+        
         # As there is too much in flux we do not want to flatten the warp in the first iteration
-        if Configuration['ITERATIONS'] > 1:
-            sm_profile,sm_error = modify_flat(Configuration, sm_profile, original, sm_error,key,inner_fix= Configuration['INNER_FIX'])
+        #if Configuration['ITERATIONS'] > 1:       
+        #    sm_profile,sm_error = modify_flat(Configuration, profile[2*i:2*i+2],\
+        #             original, sm_error,key,inner_fix= Configuration['INNER_FIX'])
+    
         profile[2*i:2*i+2]=sm_profile
-        error[2*i:2*i+2] = get_error(Configuration,original,profile[2*i:2*i+2],key,weights=weights,apply_max_error = True,min_error=min_error[i])
+        error[2*i:2*i+2] = get_error(Configuration,original,profile[2*i:2*i+2],\
+                    key,weights=weights,apply_max_error = True,\
+                    min_error=min_error[i])
         format = sf.set_format(key)
         if not no_apply:
             Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[2*i,:int(Configuration['NO_RINGS'])]])}"
             Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[2*i+1,:int(Configuration['NO_RINGS'])]])}"
             Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[2*i,:int(Configuration['NO_RINGS'])]])}")
             Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[2*i+1,:int(Configuration['NO_RINGS'])]])}")
 
-            sf.print_log(f'''REGULARISE_PROFILE: This has gone to the template.
+            print_log(f'''REGULARISE_WARP: This has gone to the template.
 {'':8s}{key} = {Tirific_Template[key]}
 {'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
 ''',Configuration,case=['debug_add'])
+    
     return profile
+
 regularise_warp.__doc__ =f'''
  NAME:
     regularise_warp
 
  PURPOSE:
     Regularise a the PA and INCL by smoothing the AM vector
 
@@ -2253,72 +2547,96 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Errors are not returned but they are written to the template
 '''
-
+def plot_output(radius, input_parameters, output_parameters,i):
+        colors = ['r','b','g','k']
+        plt.figure(89,figsize=(16,16),dpi=300,facecolor = 'w', edgecolor = 'k')
+        plt.subplot(2,1,1)
+        count=0
+                    
+
+            
+        plt.plot(radius,input_parameters['CHANGE_ANGLE'],c=colors[count],label='Change Angle' )
+        plt.plot(radius,output_parameters['CHANGE_ANGLE'],c=colors[count],linestyle='--',lw=3 )
+
+        plt.subplot(2,1,2)
+        plt.plot(radius,input_parameters['THETA']['FACTOR'],c=colors[count],label='THETA_FACTOR' )
+        plt.plot(radius,output_parameters['THETA']['FACTOR'],c=colors[count],linestyle='--',lw=3 )
+        count =1
+        plt.plot(radius,input_parameters['PHI']['FACTOR'],c=colors[count],label='PHI_FACTOR' )
+        plt.plot(radius,output_parameters['PHI']['FACTOR'],c=colors[count],linestyle='--',lw=3 )
+
+
+        plt.subplot(2,1,1)    
+        plt.legend()
+        plt.subplot(2,1,2)    
+        plt.legend()
+        plt.savefig(f"/home/peter/FAT_Main/Component_Test/Angular_Momentum/Comparison_Angle_{i}.png", bbox_inches='tight')
+        plt.close()
 
 def set_boundary_limits(Configuration,Tirific_Template,key,values = None, \
                         tolerance = 0.01, fixed = False):
     if values is None:
         values = [0.,0.]
-    sf.print_log(f'''SET_BOUNDARY_LIMITS: checking limits for {key},
+    print_log(f'''SET_BOUNDARY_LIMITS: checking limits for {key},
 {'':8s} current Boundaries = {Configuration[f"{key}_CURRENT_BOUNDARY"]}
 {'':8s} values = {values}
 ''',Configuration,case=['debug_start'])
     profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype = float)
     current_boundaries = Configuration[f"{key}_CURRENT_BOUNDARY"]
 
     if key == 'VROT' and np.sum(values) != 0.:
         current_boundaries =[[values[0]-values[1]*5.,values[0]+values[1]*5.] for x in range(3)]
     if np.sum(current_boundaries) == 0. and np.sum(values) != 0.:
         current_boundaries =[[values[0]-values[1],values[0]+values[1]] for x in range(3)]
-        sf.print_log(f'''SET_BOUNDARY_LIMITS: set boundaries from values
+        print_log(f'''SET_BOUNDARY_LIMITS: set boundaries from values
 {'':8s} current Boundaries = {current_boundaries}
 ''',Configuration,case=['debug_add'])
     elif np.sum(current_boundaries) == 0. and np.sum(values) == 0.:
         raise FunctionCallError(f'SET_BOUNDARY_LIMITS: if boundaries are not set in the Configuration call set_boundary_limits with values')
     else:
-        sf.print_log(f'''SET_BOUNDARY_LIMITS: Checking
+        print_log(f'''SET_BOUNDARY_LIMITS: Checking
 {'':8s} current Boundaries = {current_boundaries}
 {'':8s} Applying to the profiles {profile}
 ''',Configuration,case=['debug_add'])
 
         if fixed:
             range_to_check = [0]
         else:
             range_to_check = [0,1,2]
         for i in range_to_check:
 
             buffer = np.array(float(current_boundaries[i][1]-current_boundaries[i][0])*2,dtype=float)\
                     *np.array([tolerance,0.25],dtype=float)
-            sf.print_log(f'''SET_BOUNDARY_LIMITS: Using a buffer of {buffer[0]} and a change of {buffer[1]}.
+            print_log(f'''SET_BOUNDARY_LIMITS: Using a buffer of {buffer[0]} and a change of {buffer[1]}.
 ''',Configuration,case=['debug_add'])
             if i == 0:
                 profile_part = profile[0,:int(np.min(Configuration['INNER_FIX']))+1]
                 infix = np.min(Configuration['INNER_FIX'])
             else:
                 profile_part = profile[i-1,Configuration['INNER_FIX'][i-1]:]
                 infix = Configuration['INNER_FIX'][i-1]
                 #Configuration['LAST_RELIABLE_RINGS'][i-1]]
-            sf.print_log(f'''SET_BOUNDARY_LIMITS: Checking {profile_part}.
+            print_log(f'''SET_BOUNDARY_LIMITS: Checking {profile_part}.
 {'':8s} because for this part the inner fix = {infix}
     ''',Configuration,case=['debug_add'])
             #check the upper bounderies
             on_boundary = np.where(profile_part > float(current_boundaries[i][1])-buffer[0])[0]
-            sf.print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the upper {on_boundary}.
+            print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the upper {on_boundary}.
     ''',Configuration,case=['debug_add'])
             if len(on_boundary) > 0:
                 if on_boundary[0] != len(profile[0])-1:
                     current_boundaries[i][1] = current_boundaries[i][1] + buffer[1]
             #check the lower boundaries.
             on_boundary = np.where(profile_part < float(current_boundaries[i][0])+buffer[0])[0]
-            sf.print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the lower {on_boundary}.
+            print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the lower {on_boundary}.
     ''',Configuration,case=['debug_add'])
             if len(on_boundary) > 0:
                 if on_boundary[0] != len(profile[0])-1:
                     current_boundaries[i][0] = current_boundaries[i][0] - buffer[1]
     low = [x[0] for x in current_boundaries]
     high= [x[1] for x in current_boundaries]
     if key == 'Z0':
@@ -2337,18 +2655,18 @@
         high = [x if x > 170. else 170. for x in high]
         low = [x if x < 190. else 190. for x in low]
         if abs(high[1]-high[2]) > 30:
             high[1:] = [np.max(high[1:]) for x in high[1:]]
         if abs(low[1]-low[2]) > 30:
             low[1:] = [np.min(low[1:]) for x in low[1:]]
 
-    sf.print_log(f'''SET_BOUNDARY_LIMITS:We use these low = {low} and these high {high} to set {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
+    print_log(f'''SET_BOUNDARY_LIMITS:We use these low = {low} and these high {high} to set {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
 ''',Configuration,case=['debug_add'])
     sf.set_boundaries(Configuration,key,low,high)
-    sf.print_log(f'''SET_BOUNDARY_LIMITS: We have adjusted the boundaries to  {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
+    print_log(f'''SET_BOUNDARY_LIMITS: We have adjusted the boundaries to  {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
 ''',Configuration,case=['debug_add'])
 
 set_boundary_limits.__doc__ =f'''
  NAME:
     set_boundary_limits
 
  PURPOSE:
@@ -2382,37 +2700,37 @@
 
  NOTE:
 '''
 
 def set_cflux(Configuration,Tirific_Template):
 
     if any(np.isnan(Configuration['NO_POINTSOURCES'])):
-        sf.print_log(f'''SET_CFLUX: We detected an infinite number of model point sources.
+        print_log(f'''SET_CFLUX: We detected an infinite number of model point sources.
 {"":8s}SET_CFLUX: This must be an error. Exiting the fitting.
 ''',Configuration,case=['main','screen'])
         raise CfluxError('The model had infinite point sources')
     if np.max(Configuration['SIZE_IN_BEAMS']) < 15:
         factor = 1.
     else:
         factor=(np.max(Configuration['SIZE_IN_BEAMS'])/15.)**1.5
     triggered = 0
     if not 0.5e6 < Configuration['NO_POINTSOURCES'][0] < 2.2e6:
         new_cflux = sf.set_limits(float(Tirific_Template['CFLUX'])*Configuration['NO_POINTSOURCES'][0]/(factor*1e6),1e-7,5e-3)
-        sf.print_log(f'''SET_CFLUX: CFLUX is adapted from {Tirific_Template['CFLUX']} to {new_cflux:.2e}
+        print_log(f'''SET_CFLUX: CFLUX is adapted from {Tirific_Template['CFLUX']} to {new_cflux:.2e}
 ''',Configuration,case=['verbose'])
         Tirific_Template['CFLUX'] = f"{new_cflux:.2e}"
         triggered = 1
     if not 0.5e6 < Configuration['NO_POINTSOURCES'][1] < 2.2e6:
         new_cflux = sf.set_limits(float(Tirific_Template['CFLUX_2'])*Configuration['NO_POINTSOURCES'][1]/(factor*1e6),1e-7,5e-3)
-        sf.print_log(f'''SET_CFLUX: CFLUX_2 is adapted from {Tirific_Template['CFLUX_2']} to {new_cflux:.2e}
+        print_log(f'''SET_CFLUX: CFLUX_2 is adapted from {Tirific_Template['CFLUX_2']} to {new_cflux:.2e}
 ''',Configuration,case=['verbose'])
         Tirific_Template['CFLUX_2'] = f"{new_cflux:.2e}"
         triggered = 1
     if not triggered:
-        sf.print_log(f'''SET_CFLUX: CFLUXES are within the required limits.
+        print_log(f'''SET_CFLUX: CFLUXES are within the required limits.
 ''',Configuration,case=['verbose'])
 set_cflux.__doc__ =f'''
  NAME:
     set_cflux
 
  PURPOSE:
     Check CFLUX values and make sure they are in the right order for the amount of point sources
@@ -2440,15 +2758,15 @@
 
 def set_errors(Configuration,Tirific_Template,key,min_error = 0.):
     error = np.full((2,int(Configuration['NO_RINGS'])),min_error)
     format=sf.set_format(key)
     Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[0,:int(Configuration['NO_RINGS'])]])}")
     Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[1,:int(Configuration['NO_RINGS'])]])}")
 
-    sf.print_log(f'''SET_ERRORS: This has gone to the template.
+    print_log(f'''SET_ERRORS: This has gone to the template.
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
 ''',Configuration,case=['debug_start'])
 set_errors.__doc__ =f'''
  NAME:
     set_errors
 
@@ -2485,15 +2803,15 @@
          initial_estimates = None):
     if parameters_to_adjust is None:
         parameters_to_adjust = ['NO_ADJUSTMENT']
     if modifiers is None:
         modifiers = ['EMPTY']
     if initial_estimates is None:
         initial_estimates = ['EMPTY']
-    sf.print_log(f'''SET_FITTING_PARAMETERS: We are starting with these modifiers.
+    print_log(f'''SET_FITTING_PARAMETERS: We are starting with these modifiers.
 {'':8s} {modifiers}
 ''',Configuration,case=['debug_start'])
     try:
         if modifiers[0] == 'EMPTY':
             modifiers = {}
     except KeyError:
         pass
@@ -2508,18 +2826,22 @@
         Tirific_Template['LOOPS'] = "10"
     else:
         Tirific_Template['LOOPS'] = f"{Configuration['LOOPS']}"
     fitting_settings = {}
     fitting_keys = ['VARY','VARINDX','MODERATE','DELEND','DELSTART','MINDELTA','PARMAX','PARMIN']
 
     if 'INCL' not in initial_estimates:
-        profile = np.array([np.mean([x,y]) for x,y in \
-                    zip(sf.load_tirific(Configuration,Tirific_Template, ['INCL']),\
-                    sf.load_tirific(Configuration,Tirific_Template, [f"INCL_2"]) )],dtype=float)
-        diff = abs(np.max(profile)-np.min(profile))/10.
+        try:
+            profile = np.array([np.mean([x,y]) for x,y in \
+                zip(sf.load_tirific(Configuration,Tirific_Template, ['INCL']),\
+                sf.load_tirific(Configuration,Tirific_Template, [f"INCL_2"]) )],dtype=float)  
+            diff = abs(np.max(profile)-np.min(profile))/10.
+        except ValueError:
+            profile = sf.load_tirific(Configuration,Tirific_Template, ['INCL'],array=True)
+            diff = abs(np.max(profile)-np.min(profile))/10.
         initial_estimates['INCL'] = [profile[0],sf.set_limits(diff,1.,5.)/np.sin(np.radians(profile[0]))]
 
     if parameters_to_adjust[0] == 'NO_ADJUSTMENT':
         if stage in ['initial','run_cc','after_cc']:
             if initial_estimates['INCL'][0] < 30.:
                 parameters_to_adjust = ['VSYS','SBR','XPOS','YPOS','PA','SDIS','INCL','VROT']
             elif initial_estimates['INCL'][0] < 50.:
@@ -2544,15 +2866,15 @@
                     parameters_to_adjust = ['SBR','VROT','PA','INCL','SDIS','Z0']
 
                 if Configuration['CENTRAL_CONVERGENCE']:
                     parameters_to_adjust = parameters_to_adjust+['VSYS','XPOS','YPOS']
                 else:
                     parameters_to_adjust = ['VSYS','XPOS','YPOS']+parameters_to_adjust
         else:
-            sf.print_log(f'''SET_FITTING_PARAMETERS: No default adjustment for unknown stage.
+            print_log(f'''SET_FITTING_PARAMETERS: No default adjustment for unknown stage.
 ''',Configuration)
             raise InitializeError('No default adjustment for unknown stage. ')
 
     for center in Configuration['CENTRAL_FIX']:
         if center in parameters_to_adjust:
             parameters_to_adjust.remove(center)
 
@@ -2578,15 +2900,15 @@
                 initial_estimates['YPOS'] = [profile[0],0.1*Configuration['BEAM_IN_PIXELS'][1]*Configuration['PIXEL_SIZE']]
             elif key == 'SDIS':
                 initial_estimates['SDIS'] = [np.mean(profile),Configuration['CHANNEL_WIDTH']]
             elif key == 'Z0':
                 initial_estimates['Z0'] = sf.convertskyangle(Configuration,[0.2,0.05], physical = True)
 
         if key not in modifiers:
-            sf.print_log(f'''SET_FITTING_PARAMETERS: Adding {key} to the modifiers
+            print_log(f'''SET_FITTING_PARAMETERS: Adding {key} to the modifiers
 ''',Configuration,case=['debug_add'])
             if key == 'Z0': modifiers['Z0'] = [0.5,0.5,2.]
             elif key in ['XPOS','YPOS']:
                 if Configuration['CENTRAL_CONVERGENCE']:
                     modifiers[key] = [0.5,0.5,1.]
                 else:
                     modifiers[key] = [1.,1.,2.]
@@ -2601,15 +2923,15 @@
                 elif key == 'SDIS': modifiers['SDIS'] =  [1.,1.,2.]
             else:
                 if key == 'INCL': modifiers['INCL'] = [2.0,0.5,0.5]
                 elif key == 'PA': modifiers['PA'] =[1.0,1.0,2.0]
                 elif key == 'SDIS': modifiers['SDIS'] =  [1.,1.,0.5]
 
     for key in modifiers:
-        sf.print_log(f'''SET_FITTING_PARAMETERS: This {key} is in modifiers
+        print_log(f'''SET_FITTING_PARAMETERS: This {key} is in modifiers
 {'':8s} With these values {modifiers[key]}
 ''',Configuration,case=['debug_add'])
     ###############-- Modfier adaptations for large galaxies ####################
     if Configuration['OUTER_RINGS_DOUBLED']:
         for par_to_change in ['XPOS','YPOS']:
             if par_to_change in modifiers:
                 modifiers[par_to_change]  = np.array(modifiers[par_to_change],dtype=float)*\
@@ -2628,38 +2950,38 @@
                 modifiers['INCL'][0:1] =np.array(modifiers['INCL'][0:1],dtype=float)*(0.1/1.0)
                 modifiers['INCL'][2] = float(modifiers['INCL'][2])*5.
             if 'SDIS' in modifiers:
                 modifiers['SDIS'][0:1] = np.array(modifiers['SDIS'][0:1],dtype=float)*1.5
                 modifiers['SDIS'][2] = float(modifiers['SDIS'][2])*0.5
             if 'VSYS' in modifiers:
                 modifiers['VSYS'][0] = modifiers['VSYS'][0]*1.5
-            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 30.
+            print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 30.
 {'':8s} {modifiers}
 ''',Configuration,case=['debug_add'])
         elif initial_estimates['INCL'][0] < 50.:
             if 'Z0' in modifiers:
                 modifiers['Z0'][0:1] = np.array(modifiers['Z0'][0:1],dtype=float)*(0.4/0.5)
                 modifiers['Z0'][2] = float(modifiers['Z0'][2])*1.2
             if 'INCL' in modifiers:
                 modifiers['INCL'][0:1] =np.array( modifiers['INCL'][0:1],dtype=float)*(0.5/1.0)
                 modifiers['INCL'][2] = float(modifiers['INCL'][2])*1.5
-            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 50.
+            print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 50.
 {'':8s} {modifiers}
 ''',Configuration,case=['debug_add'])
         elif initial_estimates['INCL'][0] > 75.:
             if 'Z0' in modifiers:
                 modifiers['Z0'][0:1] = np.array(modifiers['Z0'][0:1],dtype=float)*(1.25)
                 modifiers['Z0'][2] = float(modifiers['Z0'][2])*0.5
             if 'INCL' in modifiers:
                 modifiers['INCL'][0:1] = np.array(modifiers['INCL'][0:1],dtype=float)*(1.5/1.0)
                 modifiers['INCL'][2] = float(modifiers['INCL'][2])*0.25
             if 'SDIS' in modifiers:
                 modifiers['SDIS'][0:1] = np.array(modifiers['SDIS'][0:1],dtype=float)*0.5
                 modifiers['SDIS'][2] = float(modifiers['SDIS'][2])*1.5
-            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the modifiers after correcting > 75.
+            print_log(f'''SET_FITTING_PARAMETERS: These are the modifiers after correcting > 75.
 {'':8s} {modifiers}
 ''',Configuration,case=['debug_add'])
         else:
             pass
     else:
         if initial_estimates['INCL'][0] < 40.:
             if 'INCL' in modifiers:
@@ -2731,15 +3053,17 @@
                 try:
                     inner[0] = int(sf.set_limits(inner[0]*fact,4,Configuration['NO_RINGS']/2.))
                     inner[1] = int(sf.set_limits(inner[1]*fact,4,Configuration['NO_RINGS']/2.))
                 except TypeError:
                     inner = int(sf.set_limits(inner*fact,4,Configuration['NO_RINGS']/2.))
             # set the moderate value
             moderate = set_generic_moderate(Configuration,key)
-
+            #If we do a single disk then symmetric is always true
+            if Configuration['NUMBER_OF_DISKS'] == 1:
+                symmetric = True
 
             fitting_settings[key] =  set_generic_fitting(Configuration,key,\
                 stage = stage, basic_variation = initial_estimates[key][1],\
                 slope= slope, flat_slope = flat_slope,fixed =fixed, \
                 flat_inner = inner, step_modifier = modifiers[key], \
                 symmetric = symmetric,moderate = moderate)
 
@@ -2753,15 +3077,15 @@
                 if  fit_key in fitting_settings[key]:
                     format = sf.set_format(key)
 
                     if fit_key in ['DELSTART','DELEND','MINDELTA']:
                     #if fit_key in ['DELEND','MINDELTA']:
                         # These should never be 0.
                         if fit_key == 'MINDELTA':
-                            sf.print_log(f'''SET_FITTING_PARAMETERS: The MINDELTA for {key} should never be below {Configuration['MIN_ERROR'][key][0]*0.1}.
+                            print_log(f'''SET_FITTING_PARAMETERS: The MINDELTA for {key} should never be below {Configuration['MIN_ERROR'][key][0]*0.1}.
 ''',Configuration,case=['debug_add'])
 
                         for i,x in enumerate(fitting_settings[key][fit_key]):
                             while float(f'{fitting_settings[key][fit_key][i]:{format}}') == 0.:
                                 if float(fitting_settings[key][fit_key][i]) == 0.:
                                     fitting_settings[key][fit_key][i] += 0.01
                                 else:
@@ -2837,35 +3161,35 @@
                         fixed = True, moderate = 3, step_modifier = None,\
                         flat_inner = 3):
     if slope is None:
         slope = [None, None]
     if step_modifier is None:
         step_modifier = [1.,1.,1.]
 
-    sf.print_log(f'''SET_GENERIC_FITTING: We are processing {key}.
+    print_log(f'''SET_GENERIC_FITTING: We are processing {key}.
 ''', Configuration, case=['debug_start'])
     if isinstance(flat_inner,int):
         flat_inner = [flat_inner,flat_inner]
     NUR = Configuration['NO_RINGS']
     input= {}
-    sf.print_log(f'''SET_GENERIC_FITTING: flat is {fixed}
+    print_log(f'''SET_GENERIC_FITTING: flat is {fixed}
 ''', Configuration,case=['debug_add'])
     if (stage in ['after_os','final_os','after_cc','after_ec','parameterized']) or fixed:
-        sf.print_log(f'''SET_GENERIC_FITTING: Fitting all as 1.
+        print_log(f'''SET_GENERIC_FITTING: Fitting all as 1.
 ''', Configuration,case=['debug_add'])
         input['VARY'] =  np.array([f"{key} 1:{NUR} {key}_2 1:{NUR}"],dtype=str)
         input['PARMAX'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][0][1]],dtype=float)
         input['PARMIN'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][0][0]],dtype=float)
         input['MODERATE'] = np.array([moderate],dtype=int) #How many steps from del start to del end
         input['DELSTART'] = np.array([basic_variation*step_modifier[0]],dtype=float) # Starting step
         input['DELEND'] = np.array([0.1*basic_variation*step_modifier[1]],dtype=float) #Ending step
         input['MINDELTA'] = np.array([0.05*basic_variation*step_modifier[2]],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
     else:
         if not symmetric:
-            sf.print_log(f'''SET_GENERIC_FITTING: implementing a varying non-symmetric profile.
+            print_log(f'''SET_GENERIC_FITTING: implementing a varying non-symmetric profile.
 {'':8s} step_modifier = {step_modifier}
 {'':8s} variations = {basic_variation}
 {'':8s} limits = {Configuration[f'{key}_CURRENT_BOUNDARY']}
 ''', Configuration,case=['debug_add'])
             input['VARY'] = []
             end = []
             add = ''
@@ -2888,15 +3212,15 @@
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][2][0],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][0][0]],dtype=float)
             input['MODERATE'] =np.array([moderate,moderate,moderate],dtype=float) #How many steps from del start to del end
             input['DELSTART'] =np.array([2.,2.,0.5],dtype=float)*step_modifier[0]*basic_variation# Starting step
             input['DELEND'] = np.array([0.1,0.1,0.05],dtype=float)*step_modifier[1]*basic_variation#Ending step
             input['MINDELTA'] = np.array([0.1,0.1,0.075],dtype=float)*step_modifier[2]*basic_variation #saturation criterum when /SIZE SIZE should be 10 troughout the code
         else:
-            sf.print_log(f'''SET_GENERIC_FITTING: implementing a varying symmetric profile
+            print_log(f'''SET_GENERIC_FITTING: implementing a varying symmetric profile
 {'':8s} step_modifier = {step_modifier}
 {'':8s} basic_variation = {basic_variation}
 {'':8s} limits = {Configuration[f'{key}_CURRENT_BOUNDARY']}
 ''', Configuration,case=['debug_add'])
             flat_inner = int(np.min(flat_inner))
             if flat_inner+1 >= NUR:
                 input['VARY'] =  np.concatenate((np.array([f"!{key} {NUR} {key}_2 {NUR}"],dtype=str),\
@@ -3123,109 +3447,115 @@
     Unspecified
 
  NOTE:
 '''
 #function to check that all parameters in template have the proper length.
 def set_new_size(Configuration,Tirific_Template, fit_type = 'Undefined',
                     current_run='Not Initialized', Variables = None):
+
     if Variables is None:
         Variables =['VROT','Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS',\
             'VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2',\
             'SDIS_2', 'AZ1P', 'AZ1W' ,'AZ1P_2','AZ1W_2', 'RADI']
 
-    sf.print_log(f'''SET_NEW_SIZE: Starting the adaptation of the size in the template
+    print_log(f'''SET_NEW_SIZE: Starting the adaptation of the size in the template
 ''',Configuration,case=['debug_start'])
     for key in Variables:
         if not key in Tirific_Template:
             Variables.remove(key)
     parameters = sf.load_tirific(Configuration,Tirific_Template,Variables)
     # do a check on whether we need to modify all
     radii = sf.set_rings(Configuration)
     if not Configuration['NEW_RING_SIZE']:
-        sf.print_log(f'''SET_NEW_SIZE: The rings size is stable and we are not interpolating
+        print_log(f'''SET_NEW_SIZE: The rings size is stable and we are not interpolating
 ''',Configuration,case=['debug_add'])
         interpolate = False
     else:
-        sf.print_log(f'''SET_NEW_SIZE: The rings size is updated and we are interpolating the old values.
+        print_log(f'''SET_NEW_SIZE: The rings size is updated and we are interpolating the old values.
 ''',Configuration,case= ['verbose'])
         old_radii = parameters[Variables.index('RADI')]
         Configuration['NEW_RING_SIZE'] = False
         interpolate = True
     #if we add a ring we need to make sure that the radius gets extended
     if len(radii) > len(parameters[Variables.index('RADI')]):
         parameters[Variables.index('RADI')] = radii
         #and the last SBR values are far too high, set them to zero such that fix_sbr will correct them
         for i in [-3,-2,-1]:
             parameters[Variables.index('SBR')][i] = 0.
             parameters[Variables.index('SBR_2')][i] = 0.
 
 
     for i,key in enumerate(Variables):
-        sf.print_log(f'''SET_NEW_SIZE: We are processing {key}
+        print_log(f'''SET_NEW_SIZE: We are processing {key}
 {'':8s}SET_NEW_SIZE: We have a parameter of length {len(parameters[i])}.
 {'':8s}SET_NEW_SIZE: Our current number of rings in the model is {Configuration['NO_RINGS']}.
 {'':8s}SET_NEW_SIZE: {parameters[i]}
 ''',Configuration,case=['debug_add'])
         if key == 'RADI':
             Tirific_Template[key] = f" {' '.join([f'{x:.2f}' for x in radii])}"
         else:
             if interpolate:
                 radii_int=np.array(radii,dtype=float)
                 old_radii_int = np.array(old_radii,dtype=float)
                 parameters_int = copy.deepcopy(parameters[i])
-                sf.print_log(f'''SET_NEW_SIZE: We are interpolating par = {parameters_int} old radii={old_radii_int} new radii={radii_int}
+                print_log(f'''SET_NEW_SIZE: We are interpolating par = {parameters_int} old radii={old_radii_int} new radii={radii_int}
     ''',Configuration,case=['debug_add'])
                 if len(parameters_int) > len(old_radii_int):
-                    sf.print_log(f'''SET_NEW_SIZE: The parameters have more values than the radii. Cutting the end.
+                    print_log(f'''SET_NEW_SIZE: The parameters have more values than the radii. Cutting the end.
     ''',Configuration,case=['debug_add'])
                     parameters_int = parameters_int[:len(old_radii)-1]
                 elif len(parameters_int) < len(old_radii_int):
-                    sf.print_log(f'''SET_NEW_SIZE: The parameters have less values than the radii. Adding the last value until match.
+                    print_log(f'''SET_NEW_SIZE: The parameters have less values than the radii. Adding the last value until match.
     ''',Configuration,case=['debug_add'])
                     while len(parameters_int) < len(old_radii_int):
                         parameters_int.append(parameters_int[-1])
 
                 parameters[i] = list(np.interp(radii_int,old_radii_int,np.array(parameters_int,dtype=float)))
                 del radii_int
                 del old_radii_int
                 del parameters_int
             format = sf.set_format(key)
 
+          
             if len(parameters[i]) > Configuration['NO_RINGS']-1:
                 # if we are cutting a ring it is likely the outer ring have done weird stuff so we flatten the curve
-
                 Tirific_Template[key] =f" {' '.join([f'{x:{format}}' for x in parameters[i][:int(Configuration['NO_RINGS'])]])}"
+
             elif len(parameters[i]) <= Configuration['NO_RINGS']-1:
                 # We simply add the last value
                 counter = len(parameters[i])
                 while counter !=  Configuration['NO_RINGS']:
                     Tirific_Template[key] = Tirific_Template[key] + f" {parameters[i][-1]:{format}}"
                     counter += 1
-        sf.print_log(f'''SET_NEW_SIZE: We wrote the following line {Tirific_Template[key]}
+                   
+                       
+        print_log(f'''SET_NEW_SIZE: We wrote the following line {Tirific_Template[key]}
 ''',Configuration,case=['debug_add'])
 
     #Replace the old ring numbers in VARY and VARINDX
-    old_rings = sf.calc_rings(Configuration,size_in_beams = int(round(np.max([float(Configuration['OLD_SIZE'][-1][0]),float(Configuration['OLD_SIZE'][-1][1])]))), ring_size  = 0.)
+    #old_rings = sf.calc_rings(Configuration,size_in_beams = int(round(np.max([float(Configuration['OLD_SIZE'][-1][0]),float(Configuration['OLD_SIZE'][-1][1])]))), ring_size  = 0.)
+    old_rings = int(copy.deepcopy(Tirific_Template['NUR']))
     current_rings = sf.calc_rings(Configuration)
     #This could lead to replacing a value smaller than the other side
     Tirific_Template['VARY'] = Tirific_Template['VARY'].replace(f"{old_rings}",f"{current_rings}")
     Tirific_Template['VARINDX'] = Tirific_Template['VARINDX'].replace(f"{old_rings-1}",f"{current_rings-1}")
+    Tirific_Template['VARINDX'] = Tirific_Template['VARINDX'].replace(f"{old_rings}",f"{current_rings}")
     Tirific_Template['NUR'] = f"{current_rings}"
     # if we cut we want to flatten things
     #if current_rings < old_rings:
     #    flatten_the_curve(Configuration,Tirific_Template)
     # Check whether the galaxy has become to small for variations
     if np.sum(Configuration['SIZE_IN_BEAMS']) > Configuration['MINIMUM_WARP_SIZE']:
         Configuration['FIXED_PARAMETERS'][0] = Configuration['FIXED_PARAMETERS'][1]
     else:
         for parameter in ['INCL','Z0','SDIS','PA']:
             if parameter not in Configuration['FIXED_PARAMETERS'][0]:
                 Configuration['FIXED_PARAMETERS'][0].append(parameter)
         flatten_the_curve(Configuration,Tirific_Template)
-    sf.print_log(f'''The following parameters will be fixed'
+    print_log(f'''The following parameters will be fixed'
 {'':8s} {Configuration['FIXED_PARAMETERS'][0]}
 ''',Configuration,case=['debug_add'])
 
     #update the limit_modifier
     sf.set_limit_modifier(Configuration,Tirific_Template)
     # Maybe increase the amount of loops in smaller galaxies
     #set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type)
@@ -3267,21 +3597,23 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+
 def set_overall_parameters(Configuration, Fits_Files,Tirific_Template,\
                 fit_type='Undefined', flux = None):
-
+    print_log(f'''SET_OVERALL_PARAMETERS: startin to set the overall parameters.
+''',Configuration,case=['debug_add'])
     if Configuration['OPTIMIZED']:
         Tirific_Template['INSET'] = f"{Fits_Files['OPTIMIZED_CUBE']}"
     else:
-        Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+        Tirific_Template['INSET'] = f"{Fits_Files['TIR_RUN_CUBE']}"
 
     if Configuration['NO_RINGS'] < 20:
         Tirific_Template['INIMODE'] = '1'
     elif Configuration['NO_RINGS'] < 30:
         Tirific_Template['INIMODE'] = '2'
     else:
         Tirific_Template['INIMODE'] = '3'
@@ -3360,163 +3692,209 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
  '''
 
 def set_sbr_fitting(Configuration,Tirific_Template, stage = 'no_stage'):
-    sf.print_log(f'''SET_SBR_FITTING: We are setting the SBR limits.
+    print_log(f'''SET_SBR_FITTING: We are setting the SBR limits.
 {'':8s} No_Rings = {Configuration['NO_RINGS']}
 ''',Configuration,case=['debug_start'])
     sbr_input = {}
     inner_ring = 2
-    sbr_profile=np.array(sf.load_tirific(Configuration,Tirific_Template, ['SBR','SBR_2']),dtype=float)
+    sbr_profile= sf.load_tirific(Configuration,Tirific_Template,Variables= ['SBR','SBR_2'],array=True)
+    radii= sf.load_tirific(Configuration,Tirific_Template, Variables=['RADI'],array=True)
+    last_ring_to_fit = []
+    for i in [0,1]:
+        last_ring_to_fit.append(np.where(radii <= \
+            Configuration['SIZE_IN_BEAMS'][i]*Configuration['BEAM'][0])[0][-1])
+        
+  
+
     if stage in ['initial','run_cc','initialize_ec','run_ec','initialize_os','run_os']:
-        radii,sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
+        sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
         if stage in ['run_ec','run_os']:
             sbr_ring_limits[-4:]=[x/5 for x in sbr_ring_limits[-4:]]
-        sf.print_log(f'''SET_SBR_FITTING: Using these SBR limits.
+        print_log(f'''SET_SBR_FITTING: Using these SBR limits.
 {'':8s} limits = {sbr_ring_limits}
 {'':8s} no of limits = {len(sbr_ring_limits)}
 ''',Configuration,case=['debug_add'])
         if stage in ['initial','run_cc']:
             max_size = 4
         elif stage in ['initialize_ec','run_ec','initialize_os','run_os']:
             max_size = 2.
         #Make sure the SBR profile is not dropping below the minimum we are setting
 
         fact= [2.,2.]
         format = sf.set_format('SBR')
-        pmax = copy.deepcopy(sbr_profile)
-        pmin = copy.deepcopy(sbr_profile)
-        pmax[:,:] = 1.
-        pmin[:,:] = 0.
+        pmax = np.full((2,len(sbr_profile[0,:])),1.)
+        pmin = np.full((2,len(sbr_profile[0,:])),0.)
         for i in [0,1]:
             if stage in ['initialize_os']:
                 fact[i] = 0.75
             elif Configuration['SIZE_IN_BEAMS'][i] < max_size:
                 fact[i]=2.5
 
             for x in range(len(radii)-1,inner_ring-1,-1):
-                if radii[x] < Configuration['SIZE_IN_BEAMS'][i]*Configuration['BEAM'][0]:
+                if radii[x] <= Configuration['SIZE_IN_BEAMS'][i]*Configuration['BEAM'][0]:
                     sbr_profile[i,x] = sf.set_limits(sbr_profile[i,x],sbr_ring_limits[x]/fact[i]*2.,1.)
-
                 else:
                     sbr_profile[i,x] = 0.
             sbr_profile[i,:inner_ring] = [sf.set_limits(x,np.min(sbr_ring_limits),1.) for x in sbr_profile[i,:inner_ring]]
             if i == 0:
                 ext=''
             else:
                 ext='_2'
             Tirific_Template[f"SBR{ext}"]= f"{' '.join([f'{x:{format}}' for x in sbr_profile[i]])}"
 
         sbr_smoothed_profile = smooth_profile(Configuration,Tirific_Template,'SBR',
                                 min_error= [sbr_ring_limits,sbr_ring_limits],no_apply = True,
                                 fix_sbr_call = True,profile_in = sbr_profile )
         sbr_av_smoothed = [(x+y)/2. for x,y in zip(sbr_smoothed_profile[0],sbr_smoothed_profile[1])]
-        sf.print_log(f'''SET_SBR_FITTING:
+        print_log(f'''SET_SBR_FITTING:
 {'':8s} This is the mean SNR {Configuration['SNR']}
 beamarea = {Configuration['BEAM_AREA']}, channelwidth = {Configuration['CHANNEL_WIDTH']}, noise = {Configuration['NOISE']}
 ''',Configuration,case=['debug_add'])
 
         #if x < 4:
         limits_for_max = True
         if Configuration['SNR'] > 10:
             limits_for_max = False
-            sf.print_log(f'''SET_SBR_FITTING:
+            print_log(f'''SET_SBR_FITTING:
 {'':8s} The SNR is so high that we will not use the ring limits for parmax
 ''',Configuration,case=['debug_add'])
 
         for i in [0,1]:
             mean_signal = Configuration['SNR']*Configuration['NOISE']/\
                     (Configuration['BEAM_AREA']*Configuration['SIZE_IN_BEAMS'][i]/2.)\
                     *Configuration['CHANNEL_WIDTH'] #in Jy/arcsec *km/s
-            sf.print_log(f'''SET_SBR_FITTING:
+            print_log(f'''SET_SBR_FITTING:
 {'':8s} mean_signal = {mean_signal}
 ''',Configuration,case=['debug_add'])
             for x in range(len(radii)-1,inner_ring-1,-1):
 
                 #    min_max = sf.set_limits(sbr_ring_limits[x]*30.,1e-3,0.9 )
                 #else:
                 #    min_max = sbr_ring_limits[x]*30.
 
                 if  sbr_profile[i,x] > 0.:
                     if limits_for_max:
                         pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*20.,sbr_ring_limits[x]*30.,1.)
                     else:
                         pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*20.,\
                             mean_signal*100./(radii[x])**0.5,1.)
-                    pmin[i,x] = sbr_ring_limits[x]/fact[i]
                 else:
                     if limits_for_max:
                         pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*5.\
                         ,sbr_ring_limits[x]*10.,sbr_ring_limits[x]*30.)
                     else:
                         pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*5.\
                         , mean_signal*50./(radii[x])**0.5, mean_signal*200./(radii[x])**0.5)
-                    pmin[i,x] = 0.
+                pmin[i,x] = sbr_ring_limits[x]/fact[i]
 
 
+     
+       
+        if np.mean(Configuration['SIZE_IN_BEAMS']) < max_size or Configuration['NUMBER_OF_DISKS'] == 1:
+            extend = np.max(last_ring_to_fit)
+               
+            sbr_input['VARY'] =  np.array([f"SBR {x+1} SBR_2 {x+1}" for x \
+                in range(extend,inner_ring-1,-1)],dtype=str)
 
-        if np.mean(Configuration['SIZE_IN_BEAMS']) < max_size:
-            sbr_input['VARY'] =  np.array([f"SBR {x+1} SBR_2 {x+1}" for x in range(len(radii)-1,inner_ring-1,-1)],dtype=str)
 
-
-            sbr_input['PARMAX'] = np.array([sf.set_limits(sbr_av_smoothed[x-1]*10.,np.mean(pmax[:,x]),1.) for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
+            sbr_input['PARMAX'] = np.array([sf.set_limits(sbr_av_smoothed[x-1]\
+                *10.,np.mean(pmax[:,x]),1.) for x in range(len(radii)-1,\
+                    inner_ring-1,-1)],dtype=float)
             #if stage in ['initial','run_cc']:
             #    sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/2. if x <= (3./4.)*len(radii) else 0 for x in range(len(radii)-1,inner_ring-1,-1)])
             #elif stage in ['initialize_ec','run_ec']:
 
-            sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/np.max(fact) for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
-            sbr_input['MODERATE'] = np.array([5 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #How many steps from del start to del end
-            sbr_input['DELSTART'] = np.array([1e-4 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) # Starting step
-            sbr_input['DELEND'] = np.array([2.5e-6 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #Ending step
-            sbr_input['MINDELTA'] = np.array([5e-6 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
+            sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/np.max(fact) for x in range(extend,inner_ring-1,-1)],dtype=float)
+            sbr_input['MODERATE'] = np.array([5 for x in range(extend,inner_ring-1,-1)],dtype=float) #How many steps from del start to del end
+            sbr_input['DELSTART'] = np.array([1e-4 for x in range(extend,inner_ring-1,-1)],dtype=float) # Starting step
+            sbr_input['DELEND'] = np.array([2.5e-6 for x in range(extend,inner_ring-1,-1)],dtype=float) #Ending step
+            sbr_input['MINDELTA'] = np.array([5e-6 for x in range(extend,inner_ring-1,-1)],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
         else:
-            sbr_input['VARY'] =  np.array([[f"SBR {x+1}",f"SBR_2 {x+1}"] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=str).reshape((len(radii)-inner_ring)*2)
-
-
-
+            input_variables = ['VARY','PARMAX','PARMIN','MODERATE','DELSTART','DELEND','MINDELTA']
+            for key in input_variables:
+                sbr_input[key] = []
 
+            ext = ''
+            for x in  range(np.max(last_ring_to_fit),inner_ring-1,-1):
+                for i in [0,1]:
+                    if x <= last_ring_to_fit[i]:
+                        if i == 0:
+                            ext = ''
+                        else:
+                            ext='_2'
+                        sbr_input['VARY'].append(f'SBR{ext} {x+1}') 
+                        sbr_input['PARMAX'].append(pmax[i,x]) 
+                        sbr_input['PARMIN'].append(pmin[i,x]) 
+                        sbr_input['MODERATE'].append(5.)
+                        sbr_input['DELSTART'].append(sbr_smoothed_profile[i,x]/10.) 
+                        sbr_input['DELEND'].append(sbr_ring_limits[x]/20.) 
+                        sbr_input['MINDELTA'].append(sbr_ring_limits[x]/20.)
+            for key in input_variables:
+                sbr_input[key] =np.array(sbr_input[key]) 
+            '''           
+            sbr_input['VARY'] =  np.array([[f"SBR {x+1}",f"SBR_2 {x+1}"] for x in range(extend,inner_ring-1,-1)],dtype=str).reshape((len(radii)-inner_ring)*2)
             #pmax = np.array([np.full(2,sf.set_limits(sbr_av_smoothed[x-1]*20.,sbr_ring_limits[x]*30.,1.)) for x in range(len(radii)-1,inner_ring-1,-1)], dtype=float)
             sbr_input['PARMAX'] = np.array([[pmax[0,x],pmax[1,x]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             #sbr_input['PARMAX'] = np.array([[sf.set_limits(sbr_smoothed_profile[0,x-1]*20.,sbr_ring_limits[x]*30.,1.),sf.set_limits(sbr_smoothed_profile[1,x-1]*20.,sbr_ring_limits[x]*30.,1.)] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
         #if stage in ['initial','run_cc']:
             #    sbr_input['PARMIN'] = np.array([[sbr_ring_limits[x]/2.,sbr_ring_limits[x]/2.] if x <= (3./4.)*len(radii) else [0.,0.] for x in range(len(radii)-1,inner_ring-1,-1)]).reshape((len(radii)-inner_ring)*2)
             #elif stage in ['initialize_ec','run_ec']:
             sbr_input['PARMIN']  = np.array([[pmin[0,x],pmin[1,x]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             #sbr_input['PARMIN'] = np.array([[sbr_ring_limits[x]/fact[0],sbr_ring_limits[x]/fact[1]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             sbr_input['MODERATE'] = np.array([[5,5] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2) #How many steps from del start to del end
             sbr_input['DELSTART'] = np.array([[1e-4,1e-4] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2) # Starting step
             sbr_input['DELEND'] = np.array([[sbr_ring_limits[x]/20.,sbr_ring_limits[x]/20.] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             sbr_input['MINDELTA'] = np.array([[sbr_ring_limits[x]/20.,sbr_ring_limits[x]/20.] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
-
-        sbr_input['VARY'] = np.concatenate((sbr_input['VARY'],[f"SBR {' '.join([str(int(x)) for x in range(1,inner_ring+1)])} SBR_2 {' '.join([str(int(x)) for x in range(1,inner_ring+1)])}"]),axis=0)
+            '''
+        sbr_input['VARY'] = np.concatenate((sbr_input['VARY'],\
+            [f"SBR {' '.join([str(int(x)) for x in range(1,inner_ring+1)])} SBR_2 {' '.join([str(int(x)) for x in range(1,inner_ring+1)])}"]\
+            ),axis=0)
         if limits_for_max:
-            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],[sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],sbr_smoothed_profile[1,2:4]])*4.,sbr_ring_limits[2],np.max(sbr_profile))]))
+            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],\
+                [sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],\
+                sbr_smoothed_profile[1,2:4]])*4.,sbr_ring_limits[2],\
+                np.max(sbr_profile))]))
         else:
-            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],[sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],sbr_smoothed_profile[1,2:4]])*4.,mean_signal*100,1.)]))
+            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],\
+                [sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],\
+                sbr_smoothed_profile[1,2:4]])*4.,mean_signal*100,1.)]))
 
         if Configuration['CENTRAL_CONVERGENCE']:
             sbr_input['PARMIN'] = np.concatenate((sbr_input['PARMIN'],[np.min(sbr_ring_limits)]))
         else:
             sbr_input['PARMIN'] = np.concatenate((sbr_input['PARMIN'],[sbr_ring_limits[inner_ring]*1.5]))
         sbr_input['MODERATE'] = np.concatenate((sbr_input['MODERATE'],[5]))
         sbr_input['DELSTART'] = np.concatenate((sbr_input['DELSTART'],[1e-5]))
         sbr_input['DELEND'] = np.concatenate((sbr_input['DELEND'],[1e-6]))
         sbr_input['MINDELTA'] = np.concatenate((sbr_input['MINDELTA'],[2e-6]))
-    elif stage in ['after_cc','after_ec','after_os']:
+    elif stage in ['after_cc','after_ec','after_os'] :
         #Used in Fit_Smoothed_Check
-        sbr_input['VARY'] = [f"SBR 3:{Configuration['NO_RINGS']}, SBR_2 3:{Configuration['NO_RINGS']}"]
-        sbr_input['PARMAX'] = np.concatenate(([np.max(sbr_profile[0,2:])*3.],[np.max(sbr_profile[1,2:])*3.]))
-        sbr_input['PARMIN'] = np.concatenate(([0],[0]))
-        sbr_input['MODERATE'] = np.concatenate(([5],[5]))
-        sbr_input['DELSTART'] = np.concatenate(([1e-5],[1e-5]))
-        sbr_input['DELEND'] = np.concatenate(([1e-6],[1e-6]))
-        sbr_input['MINDELTA'] = np.concatenate(([2e-6],[2e-6]))
+        # Initialize the parameters
+        par_to_fill = ['PARMAX','PARMIN','MODERATE','DELSTART',\
+                'DELEND','MINDELTA']
+        value =       [np.max(sbr_profile[0,2:])*3., 0., 5. , 1e-5, 1e-6,2e-6]
+        # initialize
+        for var in par_to_fill:
+            sbr_input[var] = []
+
+        if Configuration['NUMBER_OF_DISKS'] == 2:
+            sbr_input['VARY'] = [f"SBR {inner_ring+1}:{last_ring_to_fit[0]+1}, SBR_2 {inner_ring+1}:{last_ring_to_fit[1]+1}"]
+        else:
+            sbr_input['VARY'] = [f"SBR {inner_ring+1}:{last_ring_to_fit[0]+1} SBR_2 {inner_ring+1}:{last_ring_to_fit[1]+1}"]
+
+        for i in range(Configuration['NUMBER_OF_DISKS']):
+            for i,var in enumerate(par_to_fill):
+                sbr_input[var].append(value[i])
+        for var in par_to_fill:
+            sbr_input[var] = np.array(sbr_input[var])
 
     return sbr_input
 set_sbr_fitting.__doc__ =f'''
  NAME:
     set_sbr_fitting
 
  PURPOSE:
@@ -3550,15 +3928,15 @@
 
 def set_vrot_fitting(Configuration, stage = 'initial', rotation = None):
     if rotation is None:
         rotation = [100,5.]
     NUR = Configuration['NO_RINGS']
     vrot_input = {}
 
-    sf.print_log(f'''SET_VROT_FITTING: We are setting the VROT limits.
+    print_log(f'''SET_VROT_FITTING: We are setting the VROT limits.
 {'':8s} No_Rings = {Configuration['NO_RINGS']}
 {'':8s} Limits = {Configuration['VROT_CURRENT_BOUNDARY'][0]}
 ''',Configuration,case=['debug_start'])
     if stage in ['final_os']:
         modifier= [Configuration['LIMIT_MODIFIER'][0]/2.,Configuration['LIMIT_MODIFIER'][0],Configuration['LIMIT_MODIFIER'][0]/4.]
     elif stage in ['after_os']:
         modifier= [Configuration['LIMIT_MODIFIER'][0]/3.,Configuration['LIMIT_MODIFIER'][0]/2.,Configuration['LIMIT_MODIFIER'][0]/5.]
@@ -3577,15 +3955,15 @@
     vrot_input['DELSTART'] = np.array([2.*Configuration['CHANNEL_WIDTH']*modifier[0]],dtype=float) # Starting step
     #These were lower in the original fat
     vrot_input['DELEND'] = np.array([0.1*Configuration['CHANNEL_WIDTH']*modifier[1]],dtype=float) #Ending step
     vrot_input['MINDELTA'] = np.array([0.1*Configuration['CHANNEL_WIDTH']*modifier[2]],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
     #if there is not values in the center we connect the inner ring to the next ring
     forvarindex = ''
     if Configuration['NO_RINGS'] > 5:
-        if Configuration['EXCLUDE_CENTRAL'] or rotation[0] > 150.:
+        if Configuration['EXCLUDE_CENTRAL']: # Let's remove this for now as from ESO 92_G021 and serveral masssive tests it seems a bad idea or rotation[0] > 150.:
             forvarindex = 'VROT 2 VROT_2 2 '
         if Configuration['OUTER_SLOPE_START'] == NUR:
             if Configuration['NO_RINGS'] > 5:
                 inner_slope =  int(round(sf.set_limits(Configuration['RC_UNRELIABLE'],round(NUR/2.),NUR-1)))
             else:
                 inner_slope = NUR
             if Configuration['NO_RINGS'] > 15 and inner_slope > int(Configuration['NO_RINGS']*4./5.) :
@@ -3638,118 +4016,236 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def smooth_factor_profile(Configuration, change_angle,radius,inner_fix= None,\
+                          Tirific_Template= None):
+    print_log(f'''SMOOTH_PROFILE: Starting to smooth the phi and theta factor profile.
+Original Phi = {change_angle['PHI']['FACTOR']}
+Original Theta = {change_angle['THETA']['FACTOR']}             
+''',Configuration,case= ['debug_start'])
+    if inner_fix  is None:
+        inner_fix = Configuration['INNER_FIX'][0]
+    theta_factor  = change_angle['THETA']['FACTOR'][inner_fix:]   
+    phi_factor =  change_angle['PHI']['FACTOR'][inner_fix:]
+    
+    #Smoothing doesn't work
+    theta_factor = np.concatenate((np.full(inner_fix,theta_factor[0]),theta_factor))
+    phi_factor = np.concatenate((np.full(inner_fix,phi_factor[0]),phi_factor))
+    if np.mean( theta_factor) !=  theta_factor[0]:
+        theta_factor = fit_polynomial(Configuration,radius,\
+                    theta_factor,np.full(len(theta_factor),0.1),'THETA_FACTOR', Tirific_Template,\
+                    inner_fix = inner_fix,allowed_order= [1,6],
+                    boundary_limits= [-1,1])
+    if np.mean(phi_factor) !=  phi_factor[0]:  
+        phi_factor = fit_polynomial(Configuration,radius,\
+                phi_factor,np.full(len(phi_factor),0.1),'PHI_FACTOR', Tirific_Template,\
+                inner_fix = inner_fix,allowed_order= [1,6],
+                boundary_limits= [-1,1])
+    
+    #theta_factor = np.concatenate((np.zeros(inner_fix),theta_factor))
+    #reapply the signs
+    #with warnings.catch_warnings():
+    #    warnings.filterwarnings("ignore",message="invalid value encountered in divide"\
+     #                       ,category=RuntimeWarning)
+    #    theta_factor = theta_factor*change_angle['THETA']['FACTOR']\
+    #        /abs(change_angle['THETA']['FACTOR'])
+    #theta_factor[np.isnan(theta_factor)] = 0.
+
+    #if len (phi_factor) > 3:
+    #    phi_factor= savgol_filter(phi_factor, 3, 1)
+    #phi_factor = np.concatenate((np.zeros(inner_fix),phi_factor))
+    #with warnings.catch_warnings():
+    #    warnings.filterwarnings("ignore",message="invalid value encountered in divide"\
+    #                        ,category=RuntimeWarning)
+    #    phi_factor = phi_factor*change_angle['PHI']['FACTOR']\
+    #        /abs(change_angle['PHI']['FACTOR'])
+    #phi_factor[np.isnan(phi_factor)] = 0.
+
+    #Then the factor together need to 1.
+    theta_factor,phi_factor=ensure_total_dist(Configuration,\
+        theta_factor,phi_factor,inner_fix=inner_fix)    
+    return theta_factor,phi_factor
+
+def ensure_total_dist(Configuration,theta_factor,phi_factor,inner_fix=3):
+    print_log(f'''ensure_total_dist: Starting to level the factors to add to 1 in square
+Original Phi = {phi_factor}
+Original Theta = {theta_factor}             
+''',Configuration,case= ['debug_start'])
+
+    for i in range(len(theta_factor)):
+        #if i < inner_fix:
+        #    if phi_factor[i]+theta_factor[i] != 0:
+        #        raise RuntimeError('The fixed part of the factors is not 0')
+        #else:
+                new_comb =  phi_factor[i]**2+theta_factor[i]**2
+                diff = np.sqrt(abs(1.-new_comb)/2.)
+                if phi_factor[i] == 0.:
+                    tmp_phi = abs(1-abs(theta_factor[i]))
+                else:
+                    tmp_phi = phi_factor[i]
+                if theta_factor[i] == 0.:
+                    tmp_theta = abs(1-abs(phi_factor[i]))
+                else:
+                    tmp_theta = theta_factor[i]
+                count = 0
+                while not isclose(new_comb,1.,abs_tol=1e-3):
+                    if new_comb >   1.:
+                        diff = -1.*abs(diff/2.)
+                    else:
+                        diff = abs(diff/2.)
+                    tmp_phi =  tmp_phi+diff*phi_factor[i]/abs(phi_factor[i])
+                    tmp_theta =  tmp_theta+diff*theta_factor[i]/abs(theta_factor[i])
+                    new_comb =  tmp_phi**2+tmp_theta**2
+                    if abs(diff) < 1e-7:
+                        tmp_phi = phi_factor[i]
+                        tmp_theta = theta_factor[i] 
+                        diff = float(np.random.default_rng().random())
+                        new_comb =  tmp_phi**2+tmp_theta**2 
+                    count += 1
+                    if count > 1000:
+                        break   
+                if np.isnan(tmp_phi):
+                    tmp_phi=0.
+                if np.isnan(tmp_theta):
+                    tmp_theta=0.
+                phi_factor[i]=tmp_phi
+                theta_factor[i]=tmp_theta
+    return theta_factor,phi_factor
+
 def smooth_profile(Configuration,Tirific_Template,key,min_error = 0.  \
                     ,profile_in = None, no_apply =False,no_fix = False,\
-                    fix_sbr_call=False):
-    sf.print_log(f'''SMOOTH_PROFILE: Starting to smooth the {key} profile.
+                    fix_sbr_call=False,singular=False,inner_fix=None):
+    print_log(f'''SMOOTH_PROFILE: Starting to smooth the {key} profile.
 ''',Configuration,case= ['debug_start'])
     if key == 'SBR' and not fix_sbr_call:
         error_message = f'''SMOOTH_PROFILE: Do not use smooth_profile for the SBR, SBR is regularised in fix_sbr'''
-        sf.print_log(error_message,Configuration,\
+        print_log(error_message,Configuration,\
             case= ['main','screen'])
         raise FunctionCallError(error_message)
     if fix_sbr_call:
         no_fix=True
     if key in 'ARBITRARY' and (profile_in is None or no_apply is not True):
         error_message = f'''SMOOTH_PROFILE: We cannot read or write an ARBITRARY profile from the template.'''
-        sf.print_log(error_message,Configuration,\
+        print_log(error_message,Configuration,\
             case= ['main','screen'])
         raise FunctionCallError(error_message)
 
 
     if profile_in is None:
         profile = np.array(sf.load_tirific(Configuration,Tirific_Template,[key,f"{key}_2"]),dtype = float)
     else:
         profile= copy.deepcopy(profile_in)
 
     original_profile = copy.deepcopy(profile)
     min_error = np.array(min_error,dtype=float)
     if min_error.size == 1:
         min_error = np.full(profile.size,min_error)
-    if key in ['INCL','Z0', 'PA','ARBITRARY']:
-        inner_fixed = Configuration['INNER_FIX']
-    elif key in ['SDIS']:
-        inner_fixed = [4,4]
+    if inner_fix is None:
+        if key in ['INCL','Z0', 'PA','ARBITRARY','CHANGE_ANGLE','THETA_FACTOR','PHI_FACTOR']:
+            inner_fixed = Configuration['INNER_FIX']
+        elif key in ['SDIS']:
+            inner_fixed = [4,4]
+        else:
+            inner_fixed = [0,0]
     else:
-        inner_fixed = [0,0]
-
+        inner_fixed = inner_fix
     #he sbr profile is already fixed before getting to the smoothing
     if not no_fix:
-        profile =fix_profile(Configuration, key, profile, Tirific_Template,\
-                    inner_fix = inner_fixed)
+        profile =fix_profile(Configuration, key, profile,\
+                    Tirific_Template=Tirific_Template,\
+                    inner_fix = inner_fixed,singular=singular)
+       
 
     if key == 'VROT':
         #if profile[0,1] > profile[0,2] or np.mean(profile[1:3]) > 120.:
         if np.mean([profile[0][1:3],profile[1][1:3]]) > 120.:
             shortened =True
             profile = np.delete(profile, 0, axis = 1)
         else:
             shortened = False
-    sf.print_log(f'''SMOOTH_PROFILE: retrieved profile.
+    print_log(f'''SMOOTH_PROFILE: retrieved profile.
 {'':8s}{profile}
 ''',Configuration,case= ['debug_add'])
     # savgol filters do not work for small array
+    
     for i in [0,1]:
-        if len(profile[i]) <= 8:
+        if singular:
+            if i ==1:
+              continue
+            else:
+                singular_profile= copy.deepcopy(profile)  
+        else:
+            singular_profile= copy.deepcopy(profile[i]) 
+        if key in ['THETA_FACTOR','PHI_FACTOR']:
+            sign = [x/abs(x) if x !=0. else 1. for x in singular_profile]
+            singular_profile = abs(singular_profile)
+        if len(singular_profile) <= 8:
             #In this case we are using a cubic spline so no smoothing required
             pass
-        elif len(profile[i]) < 15:
-            profile[i] = savgol_filter(profile[i], 3, 1)
-        elif len(profile[i]) < 20:
-            profile[i] = savgol_filter(profile[i], 5, 2)
-        elif len(profile[i]) < 25:
-            profile[i] = savgol_filter(profile[i], 7, 3)
+        elif len(singular_profile) < 15:
+            singular_profile= savgol_filter(singular_profile, 3, 1)
+        elif len(singular_profile) < 20:
+            singular_profile= savgol_filter(singular_profile, 5, 2)
+        elif len(singular_profile) < 25:
+            singular_profile = savgol_filter(singular_profile, 7, 3)
         else:
-            profile[i] = savgol_filter(profile[i], 9, 4)
+            singular_profile = savgol_filter(singular_profile, 9, 4)
         if fix_sbr_call:
-            below_zero = np.where(profile[i,:int(len(profile)/2.)] < 0.)[0]
+            below_zero = np.where(singular_profile[:int(len(profile)/2.)] < 0.)[0]
             if below_zero.size > 0.:
-                profile[i,below_zero] = min_error[i,below_zero]
-            below_zero = np.where(profile[i,int(len(profile)/2.):] < 0.)[0]+int(len(profile)/2.)
+                singular_profile[below_zero] = min_error[i,below_zero]
+            below_zero = np.where(singular_profile[int(len(profile)/2.):] < 0.)[0]+1
             if below_zero.size > 0.:
-                profile[i,below_zero] = profile[i,below_zero-1]/2.
+                singular_profile[below_zero] = singular_profile[below_zero-1]/2.
+        if key in ['THETA_FACTOR','PHI_FACTOR']:
+            singular_profile =  singular_profile*sign
+        if singular:
+            profile=singular_profile
+        else:
+            profile[i]=singular_profile
 
     # Fix the settings
     format = sf.set_format(key)
     if key == 'VROT':
         if shortened:
             tmp = [[],[]]
             tmp[0] = np.hstack([[0.], profile[0]])
             tmp[1] = np.hstack([[0.], profile[1]])
             profile =  np.array(tmp,dtype=float)
         else:
             profile[:,0] = 0.
 
     if not no_fix:
-        profile =fix_profile(Configuration, key, profile, Tirific_Template,inner_fix=inner_fixed)
+        profile =fix_profile(Configuration, key, profile,\
+            Tirific_Template=Tirific_Template,\
+            inner_fix=inner_fixed,singular=singular)
 
 
-    sf.print_log(f'''SMOOTH_PROFILE: profile after smoothing.
+    print_log(f'''SMOOTH_PROFILE: profile after smoothing.
 {'':8s}{profile}
 ''',Configuration,case= ['debug_add'])
     if not no_apply:
-        weights = sf.get_ring_weights(Configuration,Tirific_Template)
+        weights = get_ring_weights(Configuration,Tirific_Template)
         errors = get_error(Configuration,original_profile,profile,key,weights = weights, min_error=min_error)
         if key not in ['VROT']:
             # Check whether it should be flat
             profile,errors =modify_flat(Configuration,profile,original_profile,errors,key,inner_fix=inner_fixed)
 
         Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[0,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[1,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in errors[0,:int(Configuration['NO_RINGS'])]])}")
         Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in errors[1,:int(Configuration['NO_RINGS'])]])}")
         #if key in ['INCL'] and np.mean( profile[:,int(Configuration['NO_RINGS']/2.):int(Configuration['NO_RINGS'])]) < 40.:
         #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original_profile,profile)
 
-        sf.print_log(f'''SMOOTH_PROFILE: This has gone to the template
+        print_log(f'''SMOOTH_PROFILE: This has gone to the template
 {'':8s}{key} = {Tirific_Template[key]}
 {'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
 ''',Configuration,case= ['debug_add'])
 
     return profile
@@ -3797,22 +4293,22 @@
 '''
 
 def update_disk_angles(Configuration,Tirific_Template):
     extension = ['','_2']
     for ext in extension:
         PA = np.array(sf.load_tirific(Configuration,Tirific_Template,[f'PA{ext}']),dtype=float)
         inc = np.array(sf.load_tirific(Configuration,Tirific_Template,[f'INCL{ext}']),dtype=float)
-        sf.print_log(f'''UPDATE_DISK_ANGLES: abtained  this from the template
+        print_log(f'''UPDATE_DISK_ANGLES: obtained  this from the template
 {'':8s} inc{ext} = {inc}
 {'':8s} PA{ext} = {PA}
 ''', Configuration,case= ['debug_start'])
         angle_adjust=np.array(np.tan((PA[0]-PA)*np.cos(inc*np.pi/180.)*np.pi/180.)*180./np.pi,dtype = float)
         if ext == '_2':
             angle_adjust[:] +=180.
-        sf.print_log(f'''UPDATE_DISK_ANGLES: adusting AZ1P{ext} with these angles
+        print_log(f'''UPDATE_DISK_ANGLES: adusting AZ1P{ext} with these angles
 {'':8s}{angle_adjust}
 ''', Configuration,case= ['debug_add'])
         Tirific_Template.insert(f'AZ1W{ext}',f'AZ1P{ext}',f"{' '.join([f'{x:.2f}' for x in angle_adjust])}")
 update_disk_angles.__doc__ =f'''
  NAME:
     update_disk_angles
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/read_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/read_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in FAT to read input files
 
 from pyFAT_astro.Support.fits_functions import check_mask,create_fat_cube
-from pyFAT_astro.Support.fat_errors import BadCatalogueError, NoConfigFile, \
+from pyFAT_astro.Support.fat_errors import BadCatalogueError, InputError, \
     BadSourceError
+from pyFAT_astro.Support.log_functions import print_log,update_statistics
 from pyFAT_astro.Support.modify_template import fix_sbr
-import pyFAT_astro.Support.support_functions as sf
-import pyFAT_astro
 
+import pyFAT_astro.Support.support_functions as sf
 
 from astropy.io import fits
 from astropy.wcs import WCS
 from scipy import ndimage
 import warnings
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import matplotlib
     matplotlib.use('pdf')
     import matplotlib.pyplot as plt
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     from matplotlib.patches import Ellipse
     import matplotlib.axes as maxes
 import os
-import time
 import copy
 import numpy as np
 try:
     from importlib.resources import open_text as pack_open_txt
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     from importlib_resources import open_text as pack_open_txt
 
 
-import shutil
-import traceback
-
 
 from pyFAT_astro import Templates as templates
 #Function to read a FAT input Catalogue
 
 
 def catalogue(filename,split_char='|'):
     Catalogue = sf.Proper_Dictionary({})
@@ -114,29 +110,29 @@
  NOTE:
 '''
 
 def check_edge_limits(xmin,xmax,ymin,ymax,zmin,zmax,Configuration ,\
         beam_edge = 0.5, vel_edge = 0.5 ):
     diff = np.array([xmin,abs(xmax - Configuration['NAXES'][0]),
                      ymin,abs(ymax - Configuration['NAXES'][1])],dtype = float)
-    sf.print_log(f'''CHECK_EDGE_LIMIT: We find these differences and this edge size {beam_edge*Configuration['BEAM_IN_PIXELS'][0]}
+    print_log(f'''CHECK_EDGE_LIMIT: We find these differences and this edge size {beam_edge*Configuration['BEAM_IN_PIXELS'][0]}
 {'':8s} diff  = {diff}
 ''',Configuration, case=['debug_start'])
     if np.where(diff < beam_edge*Configuration['BEAM_IN_PIXELS'][0])[0].size:
         return True
     diff = np.array([zmin,abs(zmax-Configuration['NAXES'][2])],dtype=float)
-    sf.print_log(f'''CHECK_EDGE_LIMIT: And for velocity edge =  {vel_edge}
+    print_log(f'''CHECK_EDGE_LIMIT: And for velocity edge =  {vel_edge}
 {'':8s} diff  = {diff}
 ''',Configuration, case=['debug_add'])
     if np.where(diff < vel_edge)[0].size:
-        sf.print_log(f"CHECK_EDGE_LIMIT: On the edge",Configuration,\
+        print_log(f"CHECK_EDGE_LIMIT: On the edge. \n",Configuration,\
             case=['verbose'])
         return True
     else:
-        sf.print_log(f"CHECK_EDGE_LIMIT: Off the edge",Configuration,\
+        print_log(f"CHECK_EDGE_LIMIT: Off the edge. \n",Configuration,\
             case=['verbose'])
         return False
 check_edge_limits.__doc__ =f'''
  NAME:
     check_edge_limits
 
  PURPOSE:
@@ -163,26 +159,116 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     abs, np.where, np.array, print_log,
 
  NOTE:
 '''
+def check_source_brightness(Configuration,Fits_Files,moment= False):
+
+    if not moment:
+        Cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}"\
+            ,uint = False, do_not_scale_image_data=True,ignore_blank = True,\
+             output_verify= 'ignore')
+        Mask = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",\
+            uint = False, do_not_scale_image_data=True,ignore_blank = True, \
+            output_verify= 'ignore')
+        data = Cube[0].data[Mask[0].data > 0.5]
+        snr = np.sort(data/Configuration['NOISE'])[::-1]
+        checking= 'Cube'
+        Cube.close()
+        Mask.close()
+        case = ['debug_add']
+        fact = 1.
+        fact_mean = 1.
+    else:
+        Moment = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}")
+    #model_mom0 = sf.remove_inhomogeneities(Configuration,model_mom0,inclination=float(current[1][0]), pa = float(current[2][0]), center = [current[3][0],current[4][0]])
+        Channels = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}")
+        noisemap = np.sqrt(Channels[0].data)*Configuration['NOISE']*\
+            Configuration['CHANNEL_WIDTH']
+        data = Moment[0].data
+        snr= np.sort(Moment[0].data[Moment[0].data > 0]/\
+            noisemap[Moment[0].data > 0])[::-1]
+        checking= 'Moment 0 Map'
+        case = ['main','screen']
+        fact=2.
+        fact_mean =  3./Configuration['SOURCE_MEAN_SNR']
+    #The following should only be run if we ran sofia
+    Too_Faint = False
+    #Check that the source is bright enough
+    Max_SNR = snr[int(len(snr)*Configuration['SOURCE_MAX_FRACTION']*fact)]
+
+    if Max_SNR < Configuration['SOURCE_MAX_SNR']:
+        print_log(f'''CHECK_SOURCE_BRIGHTNESS: The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100.*fact}% of selected pixels does not always exceed {Configuration['SOURCE_MAX_SNR']} in the {checking}.
+At the cutoff the SNR = {Max_SNR}.
+''', Configuration,case = case)
+        Too_Faint = True
+            #raise BadSourceError(f"The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100.}% of selected pixels does not always exceed {Configuration['SOURCE_MAX_SNR']}. Aborting.")
+    else:
+        print_log(f'''CHECK_SOURCE_BRIGHTNESS: The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100.*fact}% of selected pixels always exceeds {Configuration['SOURCE_MAX_SNR']} in the {checking}.
+At the cutoff the SNR = {Max_SNR}.
+''', Configuration)
+    Mean_SNR = np.nanmean(snr)
+    if Mean_SNR < Configuration['SOURCE_MEAN_SNR']*fact_mean:
+        print_log(f'''CHECK_SOURCE_BRIGHTNESS: The mean SNR of the pixels in the mask is {Mean_SNR} in the {checking}.
+This is less than {Configuration['SOURCE_MEAN_SNR']*fact_mean} and therefore deemed too faint.
+''', Configuration,case= case)
+        Too_Faint = True
+            #raise BadSourceError(f"The mean SNR of the pixels in the mask is {Mean_SNR}. This is too faint.")
+    else:
+        print_log(f'''CHECK_SOURCE_BRIGHTNESS: The mean SNR of the pixels in the mask is {Mean_SNR} in the {checking}.
+''', Configuration)
+
+    return Too_Faint,Max_SNR
+
+check_source_brightness.__doc__ =f'''
+ NAME:
+    check_source_brightness
+
+ PURPOSE:
+    Check the cube or the moment 0 map whether the source is bright enogh the process
+
+ CATEGORY:
+    read_functions
+
+ INPUTS:
+    Configuration = Fat Configuration
+    Fits_Files = The fits files used
+
+
+ OPTIONAL INPUTS:
+    moments  = False
+        flag to check the moment 0 map instead of the cube
+ OUTPUTS:
+    Boolean which is true if the source is too faint
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    abs, np.where, np.array, print_log,
+
+ NOTE:
+'''
+
+
 
 def extract_vrot(Configuration,map ,angle,center):
-    sf.print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
+    print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
 {'':8s} PA= {angle}
 {'':8s} center= {center}
 ''',Configuration, case=['debug_start'])
+   
     maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map,angle,center=center)
+   
     # We should base extracting the RC on where the profile is negative and positive to avoid mistakes in the ceneter coming through
     neg_index = np.where(maj_profile < 0.)[0]
     pos_index = np.where(maj_profile > 0.)[0]
 
-    sf.print_log(f'''EXTRACT_VROT: The resolution on the extracted axis
+    print_log(f'''EXTRACT_VROT: The resolution on the extracted axis
 {'':8s} resolution = {maj_resolution}
 ''',Configuration,case= ['debug_add'])
     avg_profile = []
     neg_profile = []
     #pos_profile = []
     diff = 0.
     counter = 1.
@@ -205,18 +291,18 @@
         if Configuration['BEAM_IN_PIXELS'][0]/maj_resolution < i < -2.*beam_back:
             avg_profile[beam_back] = avg_profile[beam_back]+0.25*avg_profile[int(beam_back/2.)]+0.1*avg_profile[-1]
         elif -2.*beam_back <= i < -3.*beam_back:
             avg_profile[beam_back] = avg_profile[beam_back]+0.25/counter*avg_profile[int(beam_back/2.)]+0.1/counter*avg_profile[-1]
             counter += 1
             #neg_profile[beam_back] = neg_profile[beam_back]+0.5*neg_profile[int(beam_back/2.)]+0.1*neg_profile[-1]
             #pos_profile[beam_back] = pos_profile[beam_back]+0.5*pos_profile[int(beam_back/2.)]+0.1*pos_profile[-1]
-    sf.print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
+    print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
 ''',Configuration,case= ['debug_add'])
     ring_size_req = Configuration['BEAM_IN_PIXELS'][0]/maj_resolution
-    sf.print_log(f'''EXTRACT_VROT: We need a rings size of
+    print_log(f'''EXTRACT_VROT: We need a rings size of
 {'':8s} ringsize= {ring_size_req}
 {'':8s} because bmaj in pixels  ={Configuration['BEAM_IN_PIXELS'][0]}  and the resolution of the profile = {maj_resolution} pixels
 ''',Configuration,case= ['debug_add'])
     profile = np.array(avg_profile[0::int(ring_size_req)],dtype=float)
 
     try:
         profile[np.isnan(profile)] = profile[~np.isnan(profile)][-1]
@@ -224,23 +310,23 @@
         profile = []
 
     if len(profile) < 1:
         if len(avg_profile) > 0.:
             profile = np.array([np.max(avg_profile)],dtype=float)
         else:
             profile = np.array([Configuration['CHANNEL_WIDTH']*2.],dtype=float)
-    sf.print_log(f'''EXTRACT_VROT: Unlimited profile
+    print_log(f'''EXTRACT_VROT: Unlimited profile
 {'':8s} unlimited  RC= {profile}
 ''',Configuration,case= ['debug_add'])
     profile[profile > 300.] = 300.
     profile[profile < Configuration['CHANNEL_WIDTH']*2.] = Configuration['CHANNEL_WIDTH']*2.
 
 
     #profile[0] = 0.
-    sf.print_log(f'''EXTRACT_VROT: Constructing the final RC
+    print_log(f'''EXTRACT_VROT: Constructing the final RC
 {'':8s} initial RC= {profile}
 {'':8s} at step width= {ring_size_req}
 ''',Configuration,case= ['debug_add'])
     return profile
 extract_vrot.__doc__ =f'''
  NAME:
     extract_vrot
@@ -276,16 +362,16 @@
     #Get the sbrs
     radi,sbr,sbr_2,systemic = sf.load_tirific(Configuration,\
         f"{Configuration['FITTING_DIR']}{Model}/{Model}.def",\
         Variables = ['RADI','SBR','SBR_2','VSYS'],array=True)
     #convert to solar_mass/pc^2
     sbr_msolar = sf.columndensity(Configuration,sbr*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
     sbr_2_msolar = sf.columndensity(Configuration,sbr_2*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
-    # interpolate these to ~1" steps
-    new_radii = np.linspace(0,radi[-1],int(radi[-1]))
+    # interpolate these to ~0.1 beam steps
+    new_radii = np.linspace(0,radi[-1],int(radi[-1]/(0.1*Configuration['BEAM'][0])+1))
     new_sbr_msolar = np.interp(new_radii,radi,sbr_msolar)
     new_sbr_2_msolar = np.interp(new_radii,radi,sbr_2_msolar)
 
     index_1 = np.where(new_sbr_msolar > 1.)[0]
     index_2 = np.where(new_sbr_2_msolar > 1.)[0]
     if index_1.size > 0 and index_2.size > 0:
         DHI = float(new_radii[index_1[-1]]+new_radii[index_2[-1]])
@@ -362,17 +448,17 @@
 '''
 
 # Function to get the PA and inclination from the moment 0 for initial estimates
 def guess_orientation(Configuration,Fits_Files, vsys = -1 ,center = None, \
             smooth = False):
     #open the moment 0
 
-    sf.print_log(f'''GUESS_ORIENTATION: starting extraction of initial parameters.
+    print_log(f'''GUESS_ORIENTATION: starting extraction of initial parameters.
 ''',Configuration, case=['debug_start','verbose'])
-    sf.update_statistic(Configuration, message= "Starting the guess orientation run")
+    update_statistics(Configuration, message= "Starting the guess orientation run")
 
     Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     map = Image[0].data
     hdr = Image[0].header
     mom0 = copy.deepcopy(Image)
     with warnings.catch_warnings():
@@ -385,15 +471,15 @@
     Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     noise_map = np.sqrt(Image[0].data)*Configuration['NOISE']*Configuration['CHANNEL_WIDTH']
 
     #these guesses get thrown off for very large galaxies so smooth when we have those:
     if smooth:
         sigma = sf.set_limits(Configuration['BEAM_IN_PIXELS'][0]*Configuration['MAX_SIZE_IN_BEAMS']/12.*2.,Configuration['BEAM_IN_PIXELS'][0],Configuration['BEAM_IN_PIXELS'][0]*5)
-        sf.print_log(f'''GUESS_ORIENTATION: We are smoothing the maps with {sigma} pixels
+        print_log(f'''GUESS_ORIENTATION: We are smoothing the maps with {sigma} pixels
 ''',Configuration,case= ['debug_add'])
         tmp =  ndimage.gaussian_filter(map, sigma=(sigma, sigma), order=0)
         tmp[map <= 0.] = 0.
         map = copy.deepcopy(tmp)
         if Configuration['DEBUG']:
             fits.writeto(f"{Configuration['LOG_DIRECTORY']}smooth_mom_map.fits",map,hdr,overwrite = True)
         tmp = ndimage.gaussian_filter(noise_map, sigma=(sigma, sigma), order=0)
@@ -417,76 +503,76 @@
     #map[0. > map ] =0
 
 
     mom0[0].data= map
 
 
     scale_factor = sf.set_limits(SNR/3.*minimum_noise_in_map/median_noise_in_map, 0.05, 1.)
-    sf.print_log(f'''GUESS_ORIENTATION: We find SNR = {SNR} and a scale factor {scale_factor} and the noise median {median_noise_in_map}
+    print_log(f'''GUESS_ORIENTATION: We find SNR = {SNR} and a scale factor {scale_factor} and the noise median {median_noise_in_map}
 {'':8s} minimum {minimum_noise_in_map}
 ''',Configuration,case= ['debug_add'])
     '''
     if np.mean(Configuration['SIZE_IN_BEAMS']) >10:
         beam_check=[Configuration['BEAM_IN_PIXELS'][0],Configuration['BEAM_IN_PIXELS'][0]/2.]
     else:
     '''
     beam_check=[Configuration['BEAM_IN_PIXELS'][0]/2.]
     center_stable = False
     checked_center = False
     center_counter = 0.
     original_center = copy.deepcopy(center)
-    sf.print_log(f'''GUESS_ORIENTATION: Looking for the center, pa and inclination
+    print_log(f'''GUESS_ORIENTATION: Looking for the center, pa and inclination
 ''',Configuration, case= ['verbose'])
 
-    sf.update_statistic(Configuration, message= "Starting the initial search for the pa, inclination and center.")
+    update_statistics(Configuration, message= "Starting the initial search for the pa, inclination and center.")
 
     while not center_stable:
-        inclination_av, pa_av, maj_extent_av = sf.get_inclination_pa(Configuration, mom0, center, cutoff = scale_factor* median_noise_in_map, figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center[0]:.2f}_{center[1]:.2f}')
+        inclination_av, pa_av, maj_extent_av =\
+            sf.get_inclination_pa(Configuration, mom0, center, cutoff = scale_factor* median_noise_in_map)
         inclination_av = [inclination_av]
         int_weight = [2.]
         pa_av = [pa_av]
         maj_extent_av = [maj_extent_av]
-        sf.print_log(f'''GUESS_ORIENTATION: From the the initial guess with center {center}.
+        print_log(f'''GUESS_ORIENTATION: From the the initial guess with center {center}.
 {'':8s} We get pa = {pa_av}, inclination = {inclination_av}, maj_extent_av {maj_extent_av}
 ''',Configuration,case= ['debug_add'])
         for mod in beam_check:
 
             for i in [[-1,-1],[-1,1],[1,-1],[1,1]]:
                 center_tmp = [center[0]+mod*i[0],center[1]+mod*i[1]]
 
-                sf.print_log(f'''GUESS_ORIENTATION: Checking at location RA = {center_tmp[0]} pix, DEC = {center_tmp[1]} pix
+                print_log(f'''GUESS_ORIENTATION: Checking at location RA = {center_tmp[0]} pix, DEC = {center_tmp[1]} pix
 ''',Configuration,case= ['debug_add'])
 
                 inclination_tmp, pa_tmp, maj_extent_tmp= \
                     sf.get_inclination_pa(Configuration, mom0, center_tmp,\
-                    cutoff = scale_factor* median_noise_in_map,\
-                    figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center_tmp[0]:.2f}_{center_tmp[1]:.2f}')
+                    cutoff = scale_factor* median_noise_in_map,)
                 inclination_av.append(inclination_tmp)
                 pa_av.append(pa_tmp)
                 int_weight.append(mod/beam_check[0]*0.25)
                 maj_extent_av.append(maj_extent_tmp)
 
         if np.isnan(np.array(inclination_av,dtype=float)).all():
-            sf.print_log(f'''GUESS_ORIENTATION: We are unable to find an  inclination.
+            print_log(f'''GUESS_ORIENTATION: We are unable to find an  inclination.
 ''',Configuration,case= ['main','screen'])
             raise BadSourceError(f'We are unable to find an initial inclination.')
 
         int_weight = np.array(int_weight)
         weight = np.array([1./x[1] for x in inclination_av],dtype= float)*int_weight
 
         inclination = np.array([np.nansum(np.array([x[0] for x in inclination_av],dtype=float)*weight)/np.nansum(weight),\
                                 np.nansum(np.array([x[1] for x in inclination_av],dtype=float)*weight)/np.nansum(weight)],dtype=float)
 
 
         if np.isnan(np.array(inclination_av,dtype=float)).all():
-            sf.print_log(f'''GUESS_ORIENTATION: We are unable to find an PA.
+            print_log(f'''GUESS_ORIENTATION: We are unable to find an PA.
 ''',Configuration,case=['main','screen'])
             raise BadSourceError(f'We are unable to find an initial PA.')
         weight = np.array([1./x[1] for x in pa_av],dtype= float)
-        sf.print_log(f'''GUESS_ORIENTATION: We find these pa and inclination
+        print_log(f'''GUESS_ORIENTATION: We find these pa and inclination
 {'':8s} pa = {' '.join([f'{float(x[0]):.2f}' for x in pa_av])}
 {'':8s} inclination = {' '.join([f'{float(x[0]):.2f}' for x in inclination_av])}
 {'':8s} int_weights = {' '.join([f'{float(x):.2f}' for x in int_weight])}
 {'':8s} weights = {' '.join([f'{float(x):.2f}' for x in weight])}
 ''',Configuration,case= ['debug_add'])
         pa = np.array([np.nansum(np.array([x[0] for x in pa_av],dtype=float)*weight)/np.nansum(weight),\
                                 np.nansum(np.array([x[1] for x in pa_av],dtype=float)*weight)/np.nansum(weight)],dtype=float)
@@ -505,22 +591,23 @@
         #    center =original_center
         #    center_stable=True
         #    break
         # For very small galaxies we do not want to correct the extend
         if maj_extent/Configuration['BEAM'][0]/3600. > 3.:
             maj_extent = maj_extent+(Configuration['BEAM'][0]/3600.*0.2/scale_factor)
 
-        sf.print_log(f'''GUESS_ORIENTATION: From the maps we find
+        print_log(f'''GUESS_ORIENTATION: From the maps we find
 {'':8s} inclination = {inclination}
 {'':8s} pa = {pa}
 {'':8s} size in beams = {maj_extent/(Configuration['BEAM'][0]/3600.)}
 ''',Configuration,case= ['debug_add'])
                 #map[3*minimum_noise_in_map > noise_map] = 0.
         # From these estimates we also get an initial SBR
         maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map, pa[0],center)
+     
         # let's get an intensity weighted center for the extracted profile.
 
         center_of_profile = np.sum(maj_profile*maj_axis)/np.sum(maj_profile)
         neg_index = np.where(maj_axis < 0.)[0]
         pos_index = np.where(maj_axis > 0.)[0]
         avg_profile = []
         neg_profile = []
@@ -529,51 +616,51 @@
         for i in range(np.nanmin([neg_index.size,pos_index.size])):
             avg_profile.append(np.nanmean([maj_profile[neg_index[neg_index.size-i-1]],maj_profile[pos_index[i]]]))
             neg_profile.append(maj_profile[neg_index[neg_index.size-i-1]])
             pos_profile.append(maj_profile[pos_index[i]])
             #diff = diff+abs(avg_profile[i]-neg_profile[i])+abs(avg_profile[i]-pos_profile[i])
             diff = diff+abs(pos_profile[-1]-neg_profile[-1])*abs(np.mean([pos_profile[-1],neg_profile[-1]]))
         diff = diff/np.nanmin([neg_index.size,pos_index.size])
-        sf.print_log(f'''GUESS_ORIENTATION:'BMAJ in pixels, center of the profile, current center, difference between pos and neg
+        print_log(f'''GUESS_ORIENTATION:'BMAJ in pixels, center of the profile, current center, difference between pos and neg
 {'':8s}{Configuration['BEAM_IN_PIXELS'][0]} {center_of_profile} {center} {diff}
 ''',Configuration,case= ['debug_add'])
 
         # if the center of the profile is more than half a beam off from the Sofia center let's see which on provides a more symmetric profile
         #if False:
         if (abs(center_of_profile/(2.*np.sin(np.radians(pa[0])))*maj_resolution) > Configuration['BEAM_IN_PIXELS'][0]*0.5 \
             or abs(center_of_profile/(2.*np.cos(np.radians(pa[0])))*maj_resolution) > Configuration['BEAM_IN_PIXELS'][0]*0.5) and SNR > 3. and not checked_center:
-            sf.print_log(f'''GUESS_ORIENTATION: The SoFiA center and that of the SBR profile are separated by more than half a beam.
+            print_log(f'''GUESS_ORIENTATION: The SoFiA center and that of the SBR profile are separated by more than half a beam.
 {'':8s}GUESS_ORIENTATION: Determining the more symmetric profile.
 ''',Configuration,case= ['debug_add'])
             # let's check against a central absorption
 
             cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}",\
                     uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
             buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/2.))
             central = cube[0].data[:,int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))]
 
             if np.count_nonzero(np.isnan(central))/central.size < 0.1:
                 center,checked_center,center_stable = sf.get_new_center(Configuration,map,inclination=inclination[0],pa=pa[0],noise=median_noise_in_map)
                 center_counter += 1
-                sf.print_log(f'''GUESS_ORIENTATION: We calculated a new center {center}.
+                print_log(f'''GUESS_ORIENTATION: We calculated a new center {center}.
 ''',Configuration,case= ['debug_add'])
             else:
                 center_stable = True
-                sf.print_log(f'''GUESS_ORIENTATION: There appears to be a central absorption source. We are relying on sofia
+                print_log(f'''GUESS_ORIENTATION: There appears to be a central absorption source. We are relying on sofia
 ''',Configuration,case= ['debug_add'])
 
         else:
-            sf.print_log(f'''GUESS_ORIENTATION: The previous center and that of the SBR profile are not separated by more than half a beam.
+            print_log(f'''GUESS_ORIENTATION: The previous center and that of the SBR profile are not separated by more than half a beam.
 {'':8s}GUESS_ORIENTATION: Keeping the last center
 ''',Configuration,case= ['debug_add'])
             center_stable = True
 
-    sf.print_log(f'''GUESS_ORIENTATION: Looking for the Initial surface brightness profile.
+    print_log(f'''GUESS_ORIENTATION: Looking for the Initial surface brightness profile.
 ''',Configuration, case= ['verbose'])
-    sf.update_statistic(Configuration, message= "Starting the initial search for the SBR and VROT.")
+    update_statistics(Configuration, message= "Starting the initial search for the SBR and VROT.")
     Configuration['SIZE_IN_BEAMS'] = np.full(2,sf.set_limits(maj_extent/(Configuration['BEAM'][0]/3600.),1.0,Configuration['MAX_SIZE_IN_BEAMS']))
 
     ring_size_req = Configuration['BEAM_IN_PIXELS'][0]/maj_resolution*Configuration['RING_SIZE']
 
     SBR_initial = avg_profile[0::int(ring_size_req)]/(np.pi*Configuration['BEAM'][0]*Configuration['BEAM'][1]/(4.*np.log(2.))) # Jy*km/s
     #deproject the SBR
     SBR_initial = SBR_initial*np.cos(np.radians(inclination[0]))
@@ -587,28 +674,28 @@
          SBR_initial.append(SBR_initial[-1])
     while len(SBR_initial) > number_of_rings:
          SBR_initial.pop()
     SBR_initial = np.array(SBR_initial,dtype=float)
     #We need to know which is the approaching side and which is receding
 
 
-    sf.print_log(f'''GUESS_ORIENTATION: Looking for the Initial Rotation Curve.
+    print_log(f'''GUESS_ORIENTATION: Looking for the Initial Rotation Curve.
 ''',Configuration,case= ['verbose'])
     Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT1']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     map = copy.deepcopy(Image[0].data)
 
     hdr = Image[0].header
-    sf.print_log(f'''GUESS_ORIENTATION: This is the amount of values we find initially {len(map[noise_map > 0.])}
+    print_log(f'''GUESS_ORIENTATION: This is the amount of values we find initially {len(map[noise_map > 0.])}
 ''',Configuration,case= ['debug_add'])
     #Image.close()
     #map[3*minimum_noise_in_map > noise_map] = float('NaN')
 
     map[3.*minimum_noise_in_map > noise_map] = float('NaN')
-    sf.print_log(f'''GUESS_ORIENTATION: This is the amount of values we find after blanking low SNR {len(map[~np.isnan(map)])}
+    print_log(f'''GUESS_ORIENTATION: This is the amount of values we find after blanking low SNR {len(map[~np.isnan(map)])}
 ''',Configuration,case= ['debug_add'])
     if vsys == -1 or center_counter > 0.:
         #As python is utterly moronic the center goes in back wards to the map
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore",message="Mean of empty slice"\
                             ,category=RuntimeWarning)
             map_vsys = np.nanmean(map[int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))])
@@ -619,15 +706,15 @@
 
 
     if len(map[~np.isnan(map)]) < 10 or np.isnan(map_vsys):
         no_values  = True
         noise_level = 2.5
         sigma = [0.5,0.5]
         while no_values:
-            sf.print_log(f'''GUESS_ORIENTATION: We smooth the velocity field to use a lower Noise threshold
+            print_log(f'''GUESS_ORIENTATION: We smooth the velocity field to use a lower Noise threshold
 ''',Configuration,case= ['debug_add'])
             tmp = copy.deepcopy(Image[0].data)
             tmp =  ndimage.gaussian_filter(Image[0].data, sigma=(sigma[1], sigma[0]), order=0)
             tmp[noise_level*minimum_noise_in_map > noise_map] =  float('NaN')
             #We need the cnter to be found else we get a crash
             if vsys == -1 or center_counter > 0.:
                 #As python is utterly moronic the center goes in back wards to the map
@@ -639,15 +726,15 @@
                     except RuntimeWarning:
                         map_vsys = vsys
 
                 if np.mean(Configuration['SIZE_IN_BEAMS']) < 10.:
                     map_vsys = (vsys+map_vsys)/2.
 
 
-            sf.print_log(f'''GUESS_ORIENTATION: We used the threshold {noise_level} and sigma = {sigma}
+            print_log(f'''GUESS_ORIENTATION: We used the threshold {noise_level} and sigma = {sigma}
 {'':8s}We find the len {len(tmp[~np.isnan(tmp)])} and the central velocity {map_vsys}
 ''',Configuration,case= ['debug_add'])
             if len(tmp[~np.isnan(tmp)]) < 10 or np.isnan(map_vsys):
                 sigma = [sigma[0]+0.5,sigma[0]+0.5]
                 noise_level -= 0.5
             else:
                 no_values = False
@@ -676,31 +763,31 @@
 
     vel_pa = sf.get_vel_pa(Configuration,map,center=center)
 
     maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map,pa[0], center=center)
     zeros = np.where(maj_profile == 0.)[0]
     maj_profile[zeros] = float('NaN')
     if all(np.isnan(maj_profile)):
-        sf.print_log(f'''GUESS_ORIENTATION: The RC extracted from the VF is all NaN's, this means something has gone very wrong.
+        print_log(f'''GUESS_ORIENTATION: The RC extracted from the VF is all NaN's, this means something has gone very wrong.
 {'':8s} Raising an error.
 ''' , Configuration,case= ['main','screen'])
         VROT_initial = [0]
         SBR_initial = [0]
         Image.close()
         return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,center[0],center[1],float('NaN'),VROT_initial
 
     loc_max = np.mean(maj_axis[np.where(maj_profile == np.nanmax(maj_profile))[0]])
     loc_min = np.mean(maj_axis[np.where(maj_profile == np.nanmin(maj_profile))[0]])
 
     if loc_max > loc_min:
         pa[0] = pa[0]+180
-        sf.print_log(f'''GUESS_ORIENTATION: We have modified the pa by 180 deg as we found the maximum velocity west of the minimum.
+        print_log(f'''GUESS_ORIENTATION: We have modified the pa by 180 deg as we found the maximum velocity west of the minimum.
 ''' , Configuration)
 
-    sf.print_log(f'''GUESS_ORIENTATION: this is the pa {pa} and the vel_pa {vel_pa}
+    print_log(f'''GUESS_ORIENTATION: this is the pa {pa} and the vel_pa {vel_pa}
 ''' , Configuration,case= ['debug_add'])
 
     if abs(pa[0]-vel_pa[0]) > 300.:
         if pa[0] > 180.:
             vel_pa[0] += 360.
         else:
             vel_pa[0] -= 360.
@@ -713,36 +800,36 @@
         if inclination[0] < 35.:
             pa[1]=abs(morph_pa[0]-vel_pa[0])
     else:
         if ~np.isnan(vel_pa[0]):
             pa = [np.nansum([vel_pa[0]/vel_pa[1],\
                 pa[0]/pa[1]])/np.nansum([1./vel_pa[1],1./pa[1]]),\
                 2.*1./np.sqrt(np.nansum([1./vel_pa[1],1./pa[1]]))]
-    sf.print_log(f'''GUESS_ORIENTATION: this is the final pa {pa}
+    print_log(f'''GUESS_ORIENTATION: this is the final pa {pa}
 ''' , Configuration,case= ['debug_add'])
 
     if smooth:
         buffer = int(Configuration['BEAM_IN_PIXELS'][0]*5.)
     else:
         buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/2.))
-    sf.print_log(f'''GUESS_ORIENTATION: We start with vsys = {vsys:.2f} km/s
+    print_log(f'''GUESS_ORIENTATION: We start with vsys = {vsys:.2f} km/s
 {'':8s}GUESS_ORIENTATION:We subtract {map_vsys:.2f} km/s from the moment 1 map to get the VROT
 ''' , Configuration,case= ['debug_add'])
 
     map = map  - map_vsys
     VROT_initial = extract_vrot(Configuration,map ,pa[0],center)
     min_RC_length= len(VROT_initial)
     if pa[1] < 10.:
         for x in [pa[0]-pa[1],pa[0]-pa[1]/2.,pa[0]+pa[1]/2.,pa[0]+pa[1]]:
             tmp  = extract_vrot(Configuration,map ,x,center)
             if len(tmp) > 0.:
                 RC_length = len(tmp)
                 if RC_length < min_RC_length:
                     min_RC_length = RC_length
-                sf.print_log(f'''GUESS_ORIENTATION: We found the lengths for the angled rotation curves:
+                print_log(f'''GUESS_ORIENTATION: We found the lengths for the angled rotation curves:
 {'':8s}GUESS_ORIENTATION: RC length = {RC_length}, min_RC length = {min_RC_length}, Vrot ini = {len(VROT_initial)}, tmnp = {len(tmp)}
 {'':8s}GUESS_ORIENTATION: Vrot {VROT_initial}
 {'':8s}GUESS_ORIENTATION: tmp {tmp}
 ''',Configuration,case= ['debug_add'])
                 VROT_initial = np.vstack((VROT_initial[:min_RC_length],tmp[:min_RC_length]))
                 VROT_initial = np.mean(VROT_initial,axis=0)
 
@@ -753,15 +840,15 @@
         VROT_initial = np.array([0.,VROT_initial[0]])
     else:
         VROT_initial[0] = 0
 
     VROT_initial = np.abs(VROT_initial/np.sin(np.radians(inclination[0])))
 
 
-    sf.print_log(f'''GUESS_ORIENTATION: We found the following initial rotation curve:
+    print_log(f'''GUESS_ORIENTATION: We found the following initial rotation curve:
 {'':8s}GUESS_ORIENTATION: RC = {VROT_initial}
 ''',Configuration,case= ['debug_add'])
     return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,center[0],center[1],map_vsys,VROT_initial
 guess_orientation.__doc__ =f'''
  NAME:
     guess_orientation
 
@@ -929,23 +1016,86 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 
 '''
+def check_parameters(Configuration,Variables,input_columns):
+     # check that we found all parameters
+    velocity ='v_app'
+    for value in Variables:
+        trig = False
+        if value.lower() in input_columns:
+            continue
+        elif value.lower() == 'v_app':
+            if 'v_rad' in input_columns:
+                Variables[Variables.index('v_app')]='v_rad'
+                velocity = 'v_rad'
+                continue
+            elif  'v_opt' in input_columns:
+                Variables[Variables.index('v_app')]='v_opt'
+                velocity = 'v_opt'
+                continue
+            else:
+                trig = True    
+        else:
+            trig = True
+
+        if trig:
+            print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
+{"":8s}SOFIA_CATALOGUE: This can happen because a) you have tampered with the sofiainput.txt file in the Support directory,
+{"":8s}SOFIA_CATALOGUE: b) you are using an updated version of SoFiA2 where the names have changed and FAT is not yet updated.'
+{"":8s}SOFIA_CATALOGUE:    In this case please file a bug report at https://github.com/PeterKamphuis/FAT/issues/'
+{"":8s}SOFIA_CATALOGUE: c) You are using pre processed SoFiA output of your own and do not have all the output'
+{"":8s}SOFIA_CATALOGUE:    Required output is {','.join(Variables)})
+''',Configuration,case= ['main','screen'])
+            raise BadCatalogueError("SOFIA_CATALOGUE: The required columns could not be found in the sofia catalogue.")
+    return velocity    
+check_parameters.__doc__ =f'''
+ NAME:
+    check_parameters(Variables,input_columns)
+
+ PURPOSE:
+    check wether all  variables are in the sofia catalogue
+ 
+ CATEGORY:
+    read_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Variable = Reguired variable
+    input_columns = found columns
+    
+
+ OPTIONAL INPUTS:
+
+
+
+ OUTPUTS:
+    velocity = the velocity found in the catalogue
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+
+'''
 
 
 # function to read the sofia catalogue
-def sofia_catalogue(Configuration,Fits_Files, Variables = None ):
+def sofia_catalogue(Configuration,Fits_Files, Variables = None ,no_edge_limit=False):
+    strip_npix= False
     if Variables is None:
         Variables =['id','x','x_min','x_max','y','y_min','y_max','z','z_min',\
                     'z_max','ra','dec','v_app','f_sum','kin_pa','w50',\
-                    'err_f_sum','err_x','err_y','err_z','rms']
-    sf.print_log(f'''SOFIA_CATALOGUE: Reading the source from the catalogue.
+                    'err_f_sum','err_x','err_y','err_z','rms','n_pix']
+        strip_npix =True
+    print_log(f'''SOFIA_CATALOGUE: Reading the source from the catalogue.
 ''',Configuration,case= ['debug_start'])
     outlist = [[] for x in Variables]
     with open(Configuration['FITTING_DIR']+'Sofia_Output/'+Configuration['BASE_NAME']+'_cat.txt') as sof_cat:
         for line in sof_cat.readlines():
             tmp =line.split()
             if line.strip() == '' or line.strip() == '#':
                 pass
@@ -954,26 +1104,16 @@
                     # get the present columns
                     input_columns  = [x.strip() for x in tmp[1:]]
                     #determin their location in the line
                     column_locations = []
                     for col in input_columns:
                         column_locations.append(line.find(col)+len(col))
                     # check that we found all parameters
-                    for value in Variables:
-                        if value.lower() in input_columns:
-                            continue
-                        else:
-                            sf.print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
-{"":8s}SOFIA_CATALOGUE: This can happen because a) you have tampered with the sofiainput.txt file in the Support directory,
-{"":8s}SOFIA_CATALOGUE: b) you are using an updated version of SoFiA2 where the names have changed and FAT is not yet updated.'
-{"":8s}SOFIA_CATALOGUE:    In this case please file a bug report at https://github.com/PeterKamphuis/FAT/issues/'
-{"":8s}SOFIA_CATALOGUE: c) You are using pre processed SoFiA output of your own and do not have all the output'
-{"":8s}SOFIA_CATALOGUE:    Required output is {','.join(Variables)})
-''',Configuration,case= ['main','screen'])
-                            raise BadCatalogueError("SOFIA_CATALOGUE: The required columns could not be found in the sofia catalogue.")
+                    velocity = check_parameters(Configuration,Variables,input_columns) 
+                    
             else:
                 for col in Variables:
                     if input_columns.index(col) == 0:
                         start = 0
                     else:
                         start = column_locations[input_columns.index(col)-1]
                     end = column_locations[input_columns.index(col)]
@@ -991,17 +1131,17 @@
                 outlist[Variables.index('f_sum')][i] = float(outlist[Variables.index('f_sum')][i])/Configuration['BEAM_IN_PIXELS'][2]*Configuration['CHANNEL_WIDTH']
         if 'err_f_sum' in Variables:
             for i in range(len(outlist[0])):
                 outlist[Variables.index('err_f_sum')][i] = float(outlist[Variables.index('err_f_sum')][i])/Configuration['BEAM_IN_PIXELS'][2]*Configuration['CHANNEL_WIDTH']
 
     # we want to fit a specific source
     if len(outlist[0]) > 1 and 'f_sum' in Variables:
-        sf.print_log(f'''SOFIA_CATALOGUE: Multiple sources were found we will try to select the correct one.
+        print_log(f'''SOFIA_CATALOGUE: Multiple sources were found we will try to select the correct one.
 ''',Configuration,case= ['debug_add'])
-        if Configuration['SOFIA_RAN']:
+        if Configuration['SOFIA_RAN'] and not no_edge_limit:
             found = False
             beam_edge=2.
             if Configuration['VEL_SMOOTH_EXTENDED'] or Configuration['CHANNEL_DEPENDENCY'].lower() == 'hanning':
                 vel_edge = 1.
                 min_vel_edge = 0.
             else:
                 vel_edge = 2.
@@ -1034,86 +1174,95 @@
                             cube= float(Configuration['NAXES'][0])*float(Configuration['NAXES'][1])* \
                                     (float(many_sources[Variables.index('z_max')][i])-float(many_sources[Variables.index('z_min')][i]))
                             source_size=(float(many_sources[Variables.index('z_max')][i])-float(many_sources[Variables.index('z_min')][i]))* \
                                         (float(many_sources[Variables.index('y_max')][i])-float(many_sources[Variables.index('y_min')][i]))* \
                                         (float(many_sources[Variables.index('x_max')][i])-float(many_sources[Variables.index('x_min')][i]))
 
                             if source_size/cube > 0.5:
-                                sf.print_log(f'''SOFIA_CATALOGUE: We discarded a very large source, so we will restore is and try for that.
+                                print_log(f'''SOFIA_CATALOGUE: We discarded a very large source, so we will restore is and try for that.
 !!!!!!!!!!!!!!!!!!!!!!!!! This means your original cube is in principle too small!!!!!!!!!!!!!!!!!!!!!!!!
 ''',Configuration)
                                 many_sources[Variables.index('f_sum')][i]=outlist[Variables.index('f_sum')][i]
                         if np.nansum(many_sources[Variables.index('f_sum')]) == 0.:
-                            sf.print_log(f'''SOFIA_CATALOGUE:The found sources are too close to the edges of the cube. And not large enough to warrant trying them.
+                            print_log(f'''SOFIA_CATALOGUE:The found sources are too close to the edges of the cube. And not large enough to warrant trying them.
 {'':8s} The edge limits were {beam_edge} beams spatially and {vel_edge} channels.
 ''',Configuration,case= ['main','screen'])
                             raise BadCatalogueError("The found sources are too close to the edges of the cube. And not large enough to warrant trying them.")
                         else:
                             found = True
                 else:
                     found = True
             # We need to check we are not throwing away a source that is infinitely brighter
             fluxes = np.array(many_sources[Variables.index('f_sum')],dtype =float)
             if np.any(fluxes == 0.):
                 no_edge_fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
                 if np.nanmax(no_edge_fluxes) > 10.* np.nanmax(fluxes):
-                    sf.print_log(f'''SOFIA_CATALOGUE: We discarded a very bright source, let's check wether it satisfies our minimum boundaries.
+                    print_log(f'''SOFIA_CATALOGUE: We discarded a very bright source, let's check wether it satisfies our minimum boundaries.
 ''',Configuration,case= ['debug_add'])
                     index = np.where(np.nanmax(no_edge_fluxes) == no_edge_fluxes)[0][0]
                     edge = check_edge_limits(float(outlist[Variables.index('x_min')][index]),
                                     float(outlist[Variables.index('x_max')][index]),
                                     float(outlist[Variables.index('y_min')][index]),
                                     float(outlist[Variables.index('y_max')][index]),
                                     float(outlist[Variables.index('z_min')][index]),
                                     float(outlist[Variables.index('z_max')][index]),
                                     Configuration,vel_edge=min_vel_edge)
                     cube= float(Configuration['NAXES'][0])*float(Configuration['NAXES'][1])
                     source_size=(float(many_sources[Variables.index('y_max')][index])-float(many_sources[Variables.index('y_min')][index]))* \
                                 (float(many_sources[Variables.index('x_max')][index])-float(many_sources[Variables.index('x_min')][index]))
 
                     if edge and source_size/cube < 0.5:
-                        sf.print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits and not more than half a channel in size.
+                        print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits and not more than half a channel in size.
 ''',Configuration)
 
                         if float(outlist[Variables.index('rms')][index])*1e6 < float(outlist[Variables.index('f_sum')][index]):
-                            sf.print_log(f'''SOFIA_CATALOGUE: There appears to be no noise in this cube. restoring the source.
+                            print_log(f'''SOFIA_CATALOGUE: There appears to be no noise in this cube. restoring the source.
 ''',Configuration)
                             many_sources  = copy.deepcopy(outlist)
                             fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
                     else:
                         if edge and source_size/cube >= 0.5:
-                            sf.print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits but spans more than half a channel so we are restoring it.
+                            print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits but spans more than half a channel so we are restoring it.
 In principle your cube is too small.
 ''',Configuration)
                         else:
-                            sf.print_log(f'''SOFIA_CATALOGUE: The bright source is acceptable, restoring its flux.
+                            print_log(f'''SOFIA_CATALOGUE: The bright source is acceptable, restoring its flux.
 ''',Configuration)
                         many_sources  = copy.deepcopy(outlist)
                         fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
-            sf.print_log(f'''SOFIA_CATALOGUE: after checking edges we find these fluxes:
+            print_log(f'''SOFIA_CATALOGUE: after checking edges we find these fluxes:
 {'':8s}{many_sources[Variables.index('f_sum')]}
 ''',Configuration,case= ['debug_add'])
         else:
-            #If we did not run SoFia we simply assume we want to fit the brightest source in the cube
+            #If we did not run SoFia or have no_edge_limit we simply assume we want to fit the brightest source in the cube
             many_sources  = copy.deepcopy(outlist)
             fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
         outlist = []
         #We want the source with the most total flux.
         index = np.where(np.nanmax(fluxes) == fluxes)[0][0]
-        sf.print_log(f'''SOFIA_CATALOGUE: We select the {index} source of this list.
+        print_log(f'''SOFIA_CATALOGUE: We select the {index} source of this list.
 ''',Configuration)
         outlist = [x[index] for x in many_sources]
         # check that our mask has the selected source
     else:
         outlist = [x[0] for x in outlist]
-
-    check_mask(Configuration,outlist[Variables.index('id')],Fits_Files)
-    sf.print_log(f'''SOFIA_CATALOGUE: we found these values:
+    if 'n_pix' in Variables:
+        #If we have the amount of pixels in the mask we calculate a SNR in Jy/beam
+        SNR=outlist[Variables.index('f_sum')]*Configuration['BEAM_IN_PIXELS'][2]/\
+            (Configuration['CHANNEL_WIDTH']*float(outlist[Variables.index('n_pix')])*\
+            Configuration['NOISE'])
+    else:
+        #if we don't know the amount of pixels we just leave the mask unmodified
+        SNR = 5
+    check_mask(Configuration,outlist[Variables.index('id')],Fits_Files,SNR=SNR)
+    print_log(f'''SOFIA_CATALOGUE: we found these values:
 {chr(10).join([f'{"":8s}{x} = {y}' for x,y in zip(Variables,outlist)])}
 ''',Configuration,case= ['debug_add'])
+    if strip_npix:
+        outlist.pop(Variables.index('n_pix'))
     return outlist
 sofia_catalogue.__doc__ =f'''
  NAME:
     sofia_catalogue
 
  PURPOSE:
        Read the sofia catalogue and extract several basic parameters from into a list.
@@ -1162,54 +1311,40 @@
 
     #Read the sofia catalogue
     with open(Configuration['CATALOGUE']) as sof_cat:
         for line in sof_cat.readlines():
             tmp =line.split()
 
             if line.strip() == '' or line.strip() == '#':
-                headerlines.append(line)
                 pass
             elif tmp[0] == '#' and len(tmp) > 1:
                 headerlines.append(line)
                 if tmp[1].strip().lower() in ['name']:
-
                     input_columns = [x.strip() for x in tmp[1:]]
                     column_locations = []
                     for col in input_columns:
                         column_locations.append(line.find(col)+len(col))
-
                     # check that we found all parameters
-                    for value in Variables:
-                        if value.lower() in input_columns:
-                            continue
-                        else:
-                            sf.print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
-{"":8s}SOFIA_CATALOGUE: This can happen because a) you have tampered with the sofiainput.txt file in the Support directory,
-{"":8s}SOFIA_CATALOGUE: b) you are using an updated version of SoFiA2 where the names have changed and FAT is not yet updated.'
-{"":8s}SOFIA_CATALOGUE:    In this case please file a bug report at https://github.com/PeterKamphuis/FAT/issues/'
-{"":8s}SOFIA_CATALOGUE: c) You are using pre processed SoFiA output of your own and do not have all the output'
-{"":8s}SOFIA_CATALOGUE:    Required output is {','.join(Variables)})
-''',Configuration,case= ['main','screen'])
-                            raise BadCatalogueError("SOFIA_CATALOGUE: The required columns could not be found in the sofia catalogue.")
+                    velocity = check_parameters(Configuration,Variables,input_columns)                   
             else:
-
                 outlist = ['' for x in input_columns]
                 for col in input_columns:
                     if input_columns.index(col) == 0:
                         start = 0
                     else:
                         start = column_locations[input_columns.index(col)-1]
                     end = column_locations[input_columns.index(col)]
                     outlist[input_columns.index(col)] = line[start:end].strip()
 
                 if not os.path.exists(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}"):
                     sf.create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}",f"{Configuration['MAIN_DIRECTORY']}")
 
                 if 'create_fat_cube' in Configuration['FITTING_STAGES']:
-                    create_fat_cube(Configuration, Fits_Files,sofia_catalogue=True,name=basename,id = outlist[input_columns.index('id')])
+                    hdr = create_fat_cube(Configuration,sofia_catalogue=True,name=basename,id = outlist[input_columns.index('id')])
+
                 else:
                     Cube = fits.open(f"{Configuration['SOFIA_DIR']}{basename}_{outlist[input_columns.index('id')]}_cube.fits",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
                     data = Cube[0].data
                     hdr = Cube[0].header
                     if hdr['NAXIS'] == 4:
                         data = data[0,:,:,:]
                         del hdr['NAXIS4']
@@ -1226,48 +1361,50 @@
                         channel-=1
                     high_chan = np.nanstd(data[channel,:,:])
 
                     hdr['FATNOISE'] = np.mean([low_chan,high_chan])
 
                     if hdr['CDELT3'] < -1:
                         raise InputError(f"Your velocity axis is declining this won't work. exiting")
+                    fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/{basename}_{outlist[input_columns.index('id')]}_FAT.fits",\
+                                 data,hdr,overwrite=True)
                     #Translate the big cube to parameters in this cube.
-                    with warnings.catch_warnings():
-                        warnings.simplefilter("ignore")
-                        coordinate_frame = WCS(hdr)
-                        x,y,z =coordinate_frame.wcs_world2pix(float(outlist[input_columns.index('ra')]),\
-                                                          float(outlist[input_columns.index('dec')]), \
-                                                          float(outlist[input_columns.index('v_app')]), 1.)
-                    shift = [int(float(outlist[input_columns.index('x')]) - x), \
-                            int(float(outlist[input_columns.index('y')]) - y),\
-                            int(float(outlist[input_columns.index('z')]) - z)]
-
-                    for i,coord in enumerate(['x','y','z']):
-                        for chang in ['','_min','_max','_peak']:
-                            val = f'{coord}{chang}'
-                            if chang == '':
-                                outlist[input_columns.index(val)] = f'{float(outlist[input_columns.index(val)])-shift[i]:.6f}'
-                            else:
-                                outlist[input_columns.index(val)] = f'{int(outlist[input_columns.index(val)])-shift[i]:d}'
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    coordinate_frame = WCS(hdr)
+                    x,y,z =coordinate_frame.wcs_world2pix(float(outlist[input_columns.index('ra')]),\
+                                                    float(outlist[input_columns.index('dec')]), \
+                                                    float(outlist[input_columns.index(velocity)]), 1.)
+                shift = [int(float(outlist[input_columns.index('x')]) - x), \
+                        int(float(outlist[input_columns.index('y')]) - y),\
+                        int(float(outlist[input_columns.index('z')]) - z)]
+
+                for i,coord in enumerate(['x','y','z']):
+                    for chang in ['','_min','_max','_peak']:
+                        val = f'{coord}{chang}'
+                        if chang == '':
+                            outlist[input_columns.index(val)] = f'{float(outlist[input_columns.index(val)])-shift[i]:.6f}'
+                        else:
+                            outlist[input_columns.index(val)] = f'{int(outlist[input_columns.index(val)])-shift[i]:d}'
 
 
-                    fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/{basename}_{outlist[input_columns.index('id')]}_FAT.fits",data,hdr,overwrite=True)
+                    
                 sf.create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/Sofia_Output",f"{Configuration['MAIN_DIRECTORY']}")
 
                 Configuration['FITTING_DIR']=f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/"
                 Configuration['SOFIA_BASENAME'] = f"{basename}_{outlist[input_columns.index('id')]}"
                 Configuration['BASE_NAME'] =  f"{basename}_{outlist[input_columns.index('id')]}_FAT"
                 sf.copy_homemade_sofia(Configuration,no_cat=True)
                 Catalogue['DISTANCE'].append(float(-1))
                 Catalogue['ID'].append(f"{outlist[input_columns.index('id')]}")
                 Catalogue['DIRECTORYNAME'].append(f"{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}")
                 Catalogue['CUBENAME'].append(f"{basename}_{outlist[input_columns.index('id')]}")
                 with open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_cat.txt",'w') as cat:
                     for hline in headerlines:
-                        cat.write(f"{hline}\n")
+                        cat.write(f"{hline}")
                     comline=''
                     for col in input_columns:
                         if input_columns.index(col) == 0:
                             start = 0
                         else:
                             start = column_locations[input_columns.index(col)-1]
                         end = column_locations[input_columns.index(col)]
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/run_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/run_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used to run external programs
 
 
 
-from pyFAT_astro.Support.clean_functions import clean_before_sofia,clean_after_sofia
-from pyFAT_astro.Support.fits_functions import cut_cubes,extract_pv,make_moments
-
+from pyFAT_astro.Support.clean_functions import clean_before_sofia,\
+    clean_after_sofia,transfer_errors,transfer_fitting_parameters
+from pyFAT_astro.Support.fits_functions import cut_cubes
+from make_moments.functions import extract_pv,moments
+from pyFAT_astro.Support.log_functions import print_log,update_statistics,enter_recovery_point
 from pyFAT_astro.Support.modify_template import write_new_to_template,\
     smooth_profile,set_cflux,fix_sbr,regularise_profile,set_fitting_parameters,\
-    check_size,no_declining_vrot,set_errors,get_warp_slope,check_angles,write_center,\
-    set_boundary_limits,regularise_warp,set_new_size
+    check_size,set_errors,get_warp_slope,check_angles,write_center,\
+    set_boundary_limits,regularise_warp,set_new_size,cut_low_rings
 from pyFAT_astro.Support.constants import H_0
 from pyFAT_astro.Support.fat_errors import FaintSourceError,BadConfigurationError,\
-                                              InclinationRunError,SofiaRunError,\
-                                              BadSourceError,TirificOutputError,ProgramError
-from pyFAT_astro.Support.tirshaker import tirshaker
-
+                                        SofiaRunError,BadSourceError,TirificOutputError
+from pyFAT_astro import Templates as templates
+from omegaconf import OmegaConf
 from astropy.wcs import WCS
 from astropy.io import fits
+from shutil import copyfile
+
 import pyFAT_astro.Support.read_functions as rf
 import pyFAT_astro.Support.support_functions as sf
 import pyFAT_astro.Support.write_functions as wf
-import pyFAT_astro
+
+try:
+    from importlib.resources import open_text as pack_open_txt
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`.
+    from importlib_resources import open_text as pack_open_txt
 
 import os
 import sys
 import copy
 
 import subprocess
 import numpy as np
@@ -35,55 +43,56 @@
 import re
 from datetime import datetime
 
 def check_angle_convergence(Configuration,Tirific_Template,\
         fit_type = 'Undefined'):
     angles= {'PA': 20., 'INCL': 10.}
     angles_ok = True
+    boundaries_ok = True
     for key in angles:
         new_angle = sf.load_tirific(Configuration,\
             f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
             Variables = [key],array=True)
         old_angle = sf.load_tirific(Configuration,\
             f"{Configuration['FITTING_DIR']}{fit_type}_In.def",\
             Variables = [key],array=True)
 
-        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: For {key} we had {old_angle[0]} which changed to {new_angle[0]}.
+        print_log(f'''CHECK_ANGLE_CONVERGENCE: For {key} we had {old_angle[0]} which changed to {new_angle[0]}.
 the maximum change is {float(Configuration['MIN_ERROR'][key][0])*float(angles[key])}
 ''',Configuration,case= ['debug_add'])
         if abs(old_angle[0]-new_angle[0]) > float(Configuration['MIN_ERROR'][key][0])*float(angles[key]):
-            sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} changed too much between iterations.
+            print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} changed too much between iterations.
 ''',Configuration)
             angles_ok = False
         if key in Configuration['FIXED_PARAMETERS'][0]:
             fixed=True
         else:
             fixed =False
         old_boun = np.array(Configuration[f'{key}_CURRENT_BOUNDARY'])
         set_boundary_limits(Configuration,Tirific_Template,key, tolerance = 0.01\
                     ,fixed = fixed)
         new_boun = np.array(Configuration[f'{key}_CURRENT_BOUNDARY'])
 
         if not np.array_equiv(old_boun,new_boun):
-            sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} boundaries changed from:
+            print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} boundaries changed from:
 {'':8s} old boundaries =  {old_boun}
 {'':8s} new boundaries =  {new_boun}
 ''',Configuration,case= ['verbose'])
-            angles_ok = False
+            boundaries_ok = False
 
-    #And we chek that the angles are well behaved
+    #And we check that the angles are well behaved
     changed_angles = check_angles(Configuration,Tirific_Template)
     if changed_angles:
-        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were modified in check_angles
+        print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were modified in check_angles
 ''',Configuration)
         angles_ok = False
     else:
-        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were unchanged in check_angles
+        print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were unchanged in check_angles
 ''',Configuration,case= ['debug_add'])
-    return angles_ok
+    return angles_ok,boundaries_ok
 check_angle_convergence.__doc__ =f'''
  NAME:
     check_angle_convergence
 
  PURPOSE:
     Check whether the inclination and PA have converged, are not hitting the boundaries and do not change too much from ring to ring.
 
@@ -110,17 +119,17 @@
 
  NOTE:
 '''
 
 def check_central_convergence(Configuration,Tirific_Template, \
         fit_type = 'Undefined'):
     #The new values are already loaded into the Tirific_Template so if we do accept we have to reset the values
-    sf.print_log(f'''CHECK_CENTRAL_CONVERGE: Starting stage {fit_type}.
+    print_log(f'''CHECK_CENTRAL_CONVERGE: Starting stage {fit_type}.
 ''',Configuration,case= ['debug_start'])
-    sf.update_statistic(Configuration, message= "Starting the central convergence run")
+    update_statistics(Configuration, message= "Starting the central convergence run")
 
     new_pos = sf.load_tirific(Configuration,\
         f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
         Variables = ['XPOS','YPOS','VSYS'],array=True)
     old_pos = sf.load_tirific(Configuration,\
         f"{Configuration['FITTING_DIR']}{fit_type}_In.def",\
         Variables = ['XPOS','YPOS','VSYS'],array=True)
@@ -144,49 +153,49 @@
 
         else:
             if Configuration['OUTER_RINGS_DOUBLED'] and Configuration['ITERATIONS'] <= 2:
                 apply_limit = Configuration['BEAM'][0]/3600.*np.mean(Configuration['SIZE_IN_BEAMS'])
             else:
                 apply_limit = Configuration['BEAM'][0]/3600.*np.mean(Configuration['SIZE_IN_BEAMS'])*0.2
         if any([True if abs(x[0]-y[0]) > apply_limit else False for x,y in zip(old_pos[:-1],new_pos[:-1]) ]):
-           sf.print_log(f'''CHECK_CONVERGENCE: The center shifted more than {apply_limit/(Configuration['BEAM'][0]/3600.)} FWHM.
+           print_log(f'''CHECK_CONVERGENCE: The center shifted more than {apply_limit/(Configuration['BEAM'][0]/3600.)} FWHM.
 {"":8s}CHECK_CONVERGENCE: Not applying this shift
 ''', Configuration,case= ['verbose'])
            write_center(Configuration,Tirific_Template, [x[0] for x in old_pos])
 
            #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template, Variables = ['VROT',
             #             'Z0', 'SBR', 'INCL','PA','SDIS','VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','SDIS_2'])
            return False
         else:
             if Configuration['ITERATIONS'] >= 3:
                 old_pos_2 = sf.load_tirific(Configuration,\
                     f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']-2}.def",\
                     Variables = ['XPOS','YPOS','VSYS'],array=True)
                 if any([True if abs(x[0]-y[0]) > lim else False for x,y,lim in zip(old_pos_2,new_pos,limits) ]):
-                    sf.print_log(f'''CHECK_CONVERGENCE: The center shifted back to the old position. Moving on to the next stage.
+                    print_log(f'''CHECK_CONVERGENCE: The center shifted back to the old position. Moving on to the next stage.
 ''', Configuration,case= ['debug_add'])
                    #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
                     return True
-            sf.print_log(f'''CHECK_CONVERGENCE: The center shifted too much trying again with new center.
+            print_log(f'''CHECK_CONVERGENCE: The center shifted too much trying again with new center.
 {outstr}''', Configuration)
             if np.sum(Configuration['SIZE_IN_BEAMS']) > 16.:
                 for i,var in enumerate(vars):
                     if  abs(new_pos[i][0] - old_pos[i][0]) < limits[i]:
-                        sf.print_log(f'''CHECK_CONVERGENCE: We are fixing the {var}.
+                        print_log(f'''CHECK_CONVERGENCE: We are fixing the {var}.
 ''', Configuration,case= ['debug_add'])
                         if var not in Configuration['CENTRAL_FIX']:
                             Configuration['CENTRAL_FIX'].append(var)
                     else:
                         if var in Configuration['CENTRAL_FIX']:
                             Configuration['CENTRAL_FIX'].remove(var)
 
             #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
             return False
     else:
-        sf.print_log(f'''CHECK_CONVERGENCE: The center is accepted. The shift is:
+        print_log(f'''CHECK_CONVERGENCE: The center is accepted. The shift is:
 {outstr}''', Configuration,case= ['verbose'])
         #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
         return True
 check_central_convergence.__doc__ =f'''
  NAME:
     check_central_convergence
 
@@ -215,25 +224,25 @@
     Unspecified
 
  NOTE:
 '''
 
 def check_inclination(Configuration,Tirific_Template,Fits_Files, \
         fit_type = 'Undefined'):
-    sf.print_log(f'''CHECK_INCLINATION: estimating whether our inclination estimate is decent.
+    print_log(f'''CHECK_INCLINATION: estimating whether our inclination estimate is decent.
 ''',Configuration,case= ['debug_start'])
-    sf.update_statistic(Configuration, message= "Starting the the inclination run")
+    update_statistics(Configuration, message= "Starting the the inclination run")
 
     to_extract=['VROT','INCL','INCL_2','PA','XPOS','YPOS']
     current = sf.load_tirific(Configuration,Tirific_Template,
                 Variables= to_extract,array=True)
 
 
     inclination = float(current[to_extract.index('INCL')][0])
-    sf.print_log(f'''CHECK_INCLINATION: This is the initial inclination {inclination}
+    print_log(f'''CHECK_INCLINATION: This is the initial inclination {inclination}
 ''',Configuration,case= ['debug_add'])
 
     if np.sum(Configuration['SIZE_IN_BEAMS']) < 10.:
         incl_to_check = np.linspace(-15.,+15.,20)
     else:
         max=inclination-10
         min=inclination-50
@@ -241,22 +250,22 @@
     # Let's make a directory to put things in
     tmp_stage = 'tmp_incl_check'
     sf.create_directory(tmp_stage,f"{Configuration['FITTING_DIR']}")
 
     other_run = [Configuration['TIRIFIC_RUNNING'],Configuration['TIRIFIC_PID']]
     Configuration['TIRIFIC_RUNNING'] = False
     #and a copy of the tirific template
-    sf.print_log(f'''CHECK_INCLINATION: python is so stupid
+    print_log(f'''CHECK_INCLINATION: python is so stupid
 {'':8s}PA = {Tirific_Template['PA']}
 ''',Configuration,case= ['debug_add'])
     Check_Template = copy.deepcopy(Tirific_Template)
     #write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Check_Template)
     Check_Template['LOOPS'] = '0'
     Check_Template['INIMODE'] = '0'
-    Check_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+    Check_Template['INSET'] = f"{Fits_Files['TIR_RUN_CUBE']}"
     current_cwd = os.getcwd()
     short_log = Configuration['LOG_DIRECTORY'].replace(Configuration['FITTING_DIR'],'')
     Check_Template['RESTARTNAME'] = f"{short_log}restart_{tmp_stage}.txt"
     #Check_Template['RESTARTNAME'] = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}restart_{tmp_stage}.txt")
     #Check_Template['RESTARTNAME'] = f"./Logs/06-09-2021/restart_tmp_incl_check.txt"
 
     #These are small galaxies make sure the VARINDX is not meesing things up
@@ -267,15 +276,15 @@
     incl_run= 'Not Initialized'
     for i,key in enumerate(out_keys):
         Check_Template[key] = f"{tmp_stage}/{tmp_stage}.{out_extensions[i]}"
 
 
     vobs = [x*np.sin(np.radians(np.mean([float(y),float(z)]))) for x,y,z in \
             zip(current[to_extract.index('VROT')][:],current[to_extract.index('INCL')][:],current[to_extract.index('INCL_2')][:])]
-    sf.print_log(f'''CHECK_INCLINATION: These are the values we get as input
+    print_log(f'''CHECK_INCLINATION: These are the values we get as input
 {'':8s}Inclination = {current[to_extract.index('INCL')][:]}, {current[to_extract.index('INCL_2')][:]}
 {'':8s}Vrot = {current[to_extract.index('VROT')][:]}
 {'':8s}Vobs = {vobs}
 {'':8s}PA = {Check_Template['PA']}
 ''',Configuration,case= ['debug_add'])
     mom_chi = []
     model_mom0 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}")
@@ -292,19 +301,27 @@
         for key in ['INCL','INCL_2']:
             Check_Template[key]= f"{' '.join([f'{x+incl:{format}}' for x in current[to_extract.index(key)][:]])}"
         format = sf.set_format('VROT')
         for key in ['VROT','VROT_2']:
             Check_Template[key]= f"{' '.join([f'{x:{format}}' for x in vrot])}"
         wf.tirific(Configuration,Check_Template,name = f'{tmp_stage}_In.def')
 
-        accepted,incl_run = sf.run_tirific(Configuration,incl_run, stage = 'incl_check', fit_type=tmp_stage)
-
-        make_moments(Configuration,Fits_Files,fit_type=tmp_stage,\
-                     moments = [0], \
-                     overwrite = True, vel_unit = 'm/s')
+        accepted,incl_run = sf.run_tirific(Configuration,incl_run, stage = 'incl_check',\
+                                fit_type=tmp_stage,\
+                                max_ini_time= int(300*(int(Check_Template['INIMODE'])+1)))
+        messages = moments(filename = f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}.fits",\
+                            mask = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}", moments = [0],\
+                            overwrite = True, map_velocity_unit= 'km/s',\
+                            debug = Configuration['DEBUG'], log=True,cube_velocity_unit='m/s',\
+                            output_directory =  f"{Configuration['FITTING_DIR']}{tmp_stage}",\
+                            output_name = tmp_stage)
+        print_log(messages,Configuration,case=['verbose'])
+        #make_moments(Configuration,Fits_Files,fit_type=tmp_stage,\
+        #             moments = [0], \
+        #             overwrite = True, vel_unit = 'm/s')
         #make_moments(filename = f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}.fits", basename = 'tmp_incl', directory = f"{Configuration['FITTING_DIR']}{tmp_stage}/",\
         #             moments = [0],level = 3.*Configuration['NOISE'], \
         #             overwrite = True, log= Configuration, vel_unit = 'm/s')
         incl_mom0 = fits.open(f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}_mom0.fits")
         if Configuration['DEBUG']:
             try:
                 os.remove(f"{Configuration['FITTING_DIR']}{tmp_stage}/tmp_{incl:.1f}_mom0.fits")
@@ -320,38 +337,38 @@
     sf.finish_current_run(Configuration, incl_run)
     Configuration['TIRIFIC_RUNNING'] = other_run[0]
     Configuration['TIRIFIC_PID'] =  other_run[1]
     low= np.where(mom_chi == np.nanmin(mom_chi))[0]
     if low.size > 1:
         low = low[0]
     new_incl = float(incl_to_check[low])
-    sf.print_log(f'''CHECK_INCLINATION: This is the new inclination {new_incl} it was {current[1][0]}.
+    print_log(f'''CHECK_INCLINATION: This is the new inclination {new_incl} it was {current[1][0]}.
 {'':8s}mom_chi = {mom_chi}
 {'':8s}low = {low}
 ''',Configuration,case= ['debug_add'])
 
 
     #exit()
     incl_err = 5.
     #np.mean(np.array([current[to_extract.index('INCL_ERR')],current[to_extract.index('INCL_2_ERR')]],dtype=float))
     if incl_err < 5.:
         incl_err = 5.
     if not current[1][0]-incl_err < new_incl < current[1][0]+incl_err:
-        sf.print_log(f'''CHECK_INCLINATION: The inclination has changed, writing to file.
+        print_log(f'''CHECK_INCLINATION: The inclination has changed, writing to file.
 ''',Configuration,case= ['debug_add'])
 
         vrot = [x/np.sin(np.radians(np.mean([float(y),float(z)])+new_incl)) for x,y,z in \
             zip(vobs,current[to_extract.index('INCL')][:],current[to_extract.index('INCL_2')][:])]
         format = sf.set_format(key)
         for key in ['INCL','INCL_2']:
             Tirific_Template[key]= f"{' '.join([f'{x+new_incl:{format}}' for x in current[to_extract.index(key)][:]])}"
         format = sf.set_format(key)
         for key in ['VROT','VROT_2']:
             Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in vrot])}"
-            sf.print_log(f'''CHECK_INCLINATION: This has gone to the template
+            print_log(f'''CHECK_INCLINATION: This has gone to the template
 {'':8s} vrot = {Tirific_Template['VROT']}
 {'':8s} incl = {Tirific_Template['INCL']}
 {'':8s} incl_2 = {Tirific_Template['INCL_2']}
 ''',Configuration,case= ['debug_add'])
 
         #Tirific_Template = copy.deepcopy(Check_Template)
         wf.tirific(Configuration,Tirific_Template,name = f"{fit_type}/{fit_type}.def")
@@ -386,91 +403,91 @@
     Unspecified
 
  NOTE: This should definitely be further explored.
 '''
 
 def check_source(Configuration, Fits_Files):
     Configuration['INITIAL_GUESSES_TIME'][0] = datetime.now()
-    sf.print_log(f'''CHECK_SOURCE: Starting.
+    print_log(f'''CHECK_SOURCE: Starting.
 ''',Configuration,case= ['debug_start'])
-    sf.update_statistic(Configuration, message= "Starting the check source run")
-
-
-    name,x,x_min,x_max,y,y_min,y_max,z,z_min,z_max,ra,dec,v_app,f_sum,kin_pa, \
-        w50,err_f_sum, err_x,err_y,err_z,source_rms= rf.sofia_catalogue(Configuration,Fits_Files)
-
-    x_min,x_max,y_min,y_max,z_min,z_max = sf.convert_type([x_min,x_max,y_min,y_max,z_min,z_max], type = 'int')
-    x,y,z,ra,dec,v_app,f_sum,kin_pa,f_sum_err , err_x,err_y,err_z= sf.convert_type([x,y,z,ra,dec,v_app,f_sum,kin_pa,err_f_sum, err_x,err_y,err_z])
-    #How does sofia 2 deal with the fully flagged channels?
-    v_app = v_app/1000.
-
-
-    # Need to check for that here if NaNs are included
-    if f_sum < 0.:
-        sf.print_log(f'''CHECK_SOURCE: This galaxy has negative total flux. That will not work. Aborting.
-''',Configuration,case=['main','screen'])
-        raise BadSourceError('We found an initial negative total flux.')
-    sf.print_log(f'''CHECK_SOURCE:  From the input we get Distance = {Configuration['DISTANCE']}
-''',Configuration,case= ['debug_add'])
-    # If the provided distance  = -1 we assume a Hubble follow
-    if float(Configuration['DISTANCE']) == -1.:
-        Configuration['DISTANCE'] = v_app/H_0
-    if float(Configuration['DISTANCE']) < 0.5:
-        Configuration['DISTANCE'] = 0.5
-    sf.print_log(f'''CHECK_SOURCE: After the checks we get Distance = {Configuration['DISTANCE']}.
-''',Configuration,case= ['debug_add'])
-    if np.sum(Configuration['Z0_INPUT_BOUNDARY']) == 0.:
-        sf.set_boundaries(Configuration,'Z0',*sf.convertskyangle(Configuration,[0.05,1.0], physical = True),input=True)
-
-    #Check whether the cube is very large, if so cut it down, Not if we are using a Sofia_Catalogue
-    if not 'sofia_catalogue' in Configuration['FITTING_STAGES']:
-        galaxy_box = [[z_min,z_max],[y_min,y_max],[x_min,x_max]]
-        new_box = cut_cubes(Configuration, Fits_Files, galaxy_box)
-
-        #update our pixel values to match the new sizes
-        for i in range(len(new_box)):
-            shift = new_box[i,0]
-            if i == 0:
-                z -= shift; z_min -= shift; z_max -= shift
-            elif i == 1:
-                y -= shift; y_min -= shift; y_max -= shift
-            elif i == 2:
-                x -= shift; x_min -= shift; x_max -= shift
+    update_statistics(Configuration, message= "Starting the check source run")
+    source_not_ok= True
+    no_edge_limit=False
+    while source_not_ok:
+        name,x,x_min,x_max,y,y_min,y_max,z,z_min,z_max,ra,dec,v_app,f_sum,kin_pa, \
+            w50,err_f_sum, err_x,err_y,err_z,source_rms= \
+            rf.sofia_catalogue(Configuration,Fits_Files,no_edge_limit=no_edge_limit)
+
+        x_min,x_max,y_min,y_max,z_min,z_max = \
+            sf.convert_type([x_min,x_max,y_min,y_max,z_min,z_max], type = 'int')
+        x,y,z,ra,dec,v_app,f_sum,kin_pa,f_sum_err , err_x,err_y,err_z= \
+            sf.convert_type([x,y,z,ra,dec,v_app,f_sum,kin_pa,err_f_sum, err_x,err_y,err_z])
+        #How does sofia 2 deal with the fully flagged channels?
+        v_app = v_app/1000.
 
-    Cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
 
+        # Need to check for that here if NaNs are included
+        if f_sum < 0.:
+            print_log(f'''CHECK_SOURCE: This galaxy has negative total flux. That will not work. Aborting.
+    ''',Configuration,case=['main','screen'])
+            raise BadSourceError('We found an initial negative total flux.')
+        print_log(f'''CHECK_SOURCE:  From the input we get Distance = {Configuration['DISTANCE']} Mpc.
+    ''',Configuration,case= ['main','screen'])
+        # If the provided distance  = -1 we assume a Hubble follow
+        if float(Configuration['DISTANCE']) == -1.:
+            Configuration['DISTANCE'] = v_app/H_0
+        if float(Configuration['DISTANCE']) < 0.5:
+            Configuration['DISTANCE'] = 0.5
+        print_log(f'''CHECK_SOURCE: After the checks we get Distance = {Configuration['DISTANCE']}.
+    ''',Configuration,case= ['debug_add'])
+        if np.sum(Configuration['Z0_INPUT_BOUNDARY']) == 0.:
+            sf.set_boundaries(Configuration,'Z0',*sf.convertskyangle(Configuration,[0.05,1.0], physical = True),input=True)
+
+        #Check whether the cube is very large, if so cut it down, Not if we are using a Sofia_Catalogue
+        if not 'sofia_catalogue' in Configuration['FITTING_STAGES']:
+            galaxy_box = [[z_min,z_max],[y_min,y_max],[x_min,x_max]]
+            new_box = cut_cubes(Configuration, Fits_Files, galaxy_box)
+
+            #update our pixel values to match the new sizes
+            for i in range(len(new_box)):
+                shift = new_box[i,0]
+                if i == 0:
+                    z -= shift; z_min -= shift; z_max -= shift
+                elif i == 1:
+                    y -= shift; y_min -= shift; y_max -= shift
+                elif i == 2:
+                    x -= shift; x_min -= shift; x_max -= shift
+
+        #We use Max_SNR later on so it always has to be defined
+        too_faint,Max_SNR = rf.check_source_brightness(Configuration,Fits_Files)
+        if too_faint and not Configuration['FORCE_FIT']:
+            too_faint,Max_moment_SNR = rf.check_source_brightness(Configuration,Fits_Files,\
+                moment=True)
+            if not too_faint and Configuration['SOFIA_THRESHOLD'] > 3 and  'run_sofia' in Configuration['FITTING_STAGES']:
+                Configuration['SOFIA_THRESHOLD']=3
+                sofia(Configuration, Fits_Files)
+                no_edge_limit = True
+            elif too_faint:
+                raise BadSourceError(f'The selected source was deemed to be too faint to process')
+            else:
+                source_not_ok = False
+        else:
+            source_not_ok = False
+     
+    Cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}"\
+        ,uint = False, do_not_scale_image_data=True,ignore_blank = True,\
+         output_verify= 'ignore')
+    Mask = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",\
+        uint = False, do_not_scale_image_data=True,ignore_blank = True, \
+        output_verify= 'ignore')
     data = Cube[0].data
-    masked_data = Cube[0].data
     header = Cube[0].header
-    Mask = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
 
-    #The following should only be run if we ran sofia
-    if 'run_sofia' in Configuration['FITTING_STAGES']:
-        #Check that the source is bright enough
-        #masked_data[Mask[0].data < 0.5] = float('NaN')
-        data_values = np.sort(masked_data[Mask[0].data > 0.5])[::-1]
-        Max_SNR = data_values[int(len(data_values)*\
-            Configuration['SOURCE_MAX_FRACTION'])]/Configuration['NOISE']
-        if Max_SNR < Configuration['SOURCE_MAX_SNR']:
-            sf.print_log(f'''CHECK_SOURCE: The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100}% of selected pixels does not always exceed {Configuration['SOURCE_MAX_SNR']}. Aborting.
-''', Configuration,case= ['main','screen'])
-            raise BadSourceError(f"The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100.}% of selected pixels does not always exceed {Configuration['SOURCE_MAX_SNR']}. Aborting.")
-        else:
-            sf.print_log(f'''CHECK_SOURCE: The SNR of brightest {Configuration['SOURCE_MAX_FRACTION']*100.}% of selected pixels always exceeds {Configuration['SOURCE_MAX_SNR']}.
-''', Configuration)
+    Mask.close()
 
-        Mean_SNR = np.nanmean(masked_data[masked_data > 0.])/Configuration['NOISE']
-        del masked_data
-        if Mean_SNR < Configuration['SOURCE_MEAN_SNR']:
-            sf.print_log(f'''CHECK_SOURCE: The mean SNR of the pixels in the mask is {Mean_SNR}, that is not enough for a fit.
-''', Configuration,case= ['main','screen'])
-            raise BadSourceError(f"The mean SNR of the pixels in the mask is {Mean_SNR}. This is too faint.")
-        else:
-            sf.print_log(f'''CHECK_SOURCE: The mean SNR of the pixels in the mask is {Mean_SNR}.
-''', Configuration)
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         cube_wcs = WCS(header)
     # convert the boundaries to real coordinates
     ralow,declow,vellow = cube_wcs.wcs_pix2world(x_min,y_min,z_min,1)
     rahigh,dechigh,velhigh = cube_wcs.wcs_pix2world(x_max,y_max,z_max,1)
@@ -479,28 +496,28 @@
     RAboun = np.sort([float(ralow),float(rahigh)])
     VELboun = np.sort([float(vellow),float(velhigh)])
     vsys_error= sf.set_limits(np.mean(np.abs(np.array(VELboun/1000.,dtype=float)-v_app))*0.05,\
                     Configuration['CHANNEL_WIDTH']*2,Configuration['CHANNEL_WIDTH']*10.)
 
     rahr,dechr = sf.convertRADEC(Configuration,ra,dec)
     # We write the results of the cut cube to the log
-    sf.print_log(f'''CHECK_SOURCE: The source finder found the following center in pixels.
+    print_log(f'''CHECK_SOURCE: The source finder found the following center in pixels.
 {"":8s}CHECK_SOURCE: RA center = {x} with boundaries {x_min}, {x_max}
 {"":8s}CHECK_SOURCE: DEC center = {y} with boundaries {y_min}, {y_max}
 {"":8s}CHECK_SOURCE: V_sys center = {z} with boundaries {z_min}, {z_max}
 {"":8s}CHECK_SOURCE: This should correspond to the WCS coordinates:
 {"":8s}CHECK_SOURCE: RA center = {ra} deg or {rahr}  with boundaries {','.join(sf.convert_type(RAboun,type='str'))}
 {"":8s}CHECK_SOURCE: DEC center = {dec} deg  or {dechr}  with boundaries {','.join(sf.convert_type(DECboun,type='str'))}
 {"":8s}CHECK_SOURCE: Sofia V_sys center = {v_app:.2f} with boundaries {','.join(sf.convert_type(VELboun/1000.,type='str'))}
 ''', Configuration)
 
     #There is a factor of two missing here but this is necessary otherwise the maxima are far to small
     Configuration['MAX_SIZE_IN_BEAMS'] = int(round(np.sqrt(((x_max-x_min)/2.)**2+((y_max-y_min)/2.)**2) \
                 /(Configuration['BEAM_IN_PIXELS'][0])+5.))
-    sf.print_log(f'''CHECK_SOURCE: From Sofia we find a max extend of {Configuration['MAX_SIZE_IN_BEAMS']}
+    print_log(f'''CHECK_SOURCE: From Sofia we find a max extend of {Configuration['MAX_SIZE_IN_BEAMS']}
 ''', Configuration,case= ['verbose'])
     if Configuration['MAX_SIZE_IN_BEAMS'] > 20.:
         smooth_field = True
     else:
         smooth_field = False
 
     pa, inclination, SBR_initial,x_new,y_new,new_vsys,VROT_initial =\
@@ -510,88 +527,88 @@
     if x_new != x or y_new != y or new_vsys != v_app:
         x,y,z_new=cube_wcs.wcs_world2pix(ra,dec,new_vsys*1000.,1)
         x=float(x_new)
         y=float(y_new)
         z=float(z_new)
         ra,dec,v_app = cube_wcs.wcs_pix2world(x,y,z,1)
         v_app = v_app/1000.
-        sf.print_log(f'''CHECK_SOURCE: The center is updated to.
+        print_log(f'''CHECK_SOURCE: The center is updated to.
 {"":8s}CHECK_SOURCE: RA center = {ra} with boundaries {','.join(sf.convert_type(RAboun,type='str'))}
 {"":8s}CHECK_SOURCE: DEC center = {dec} with boundaries {','.join(sf.convert_type(DECboun,type='str'))}
 {"":8s}CHECK_SOURCE: V_sys center = {v_app:.2f} with boundaries {','.join(sf.convert_type(VELboun/1000.,type='str'))}
 ''', Configuration)
     sf.set_boundaries(Configuration,'XPOS',*RAboun,input=True)
     sf.set_boundaries(Configuration,'YPOS',*DECboun,input=True)
     sf.set_boundaries(Configuration,'VSYS',*VELboun/1000.,input=True)
 
     if np.sum(pa) == 0. or any(np.isnan(pa)) or \
         np.sum(inclination) == 0. or any(np.isnan(inclination)) or \
         np.sum(SBR_initial) == 0. or all(np.isnan(SBR_initial)) or \
         np.sum(VROT_initial) == 0. or all(np.isnan(VROT_initial)):
-        sf.print_log(f'''CHECK_SOURCE: We could not establish proper initial estimates from the moment maps. These are what we got
+        print_log(f'''CHECK_SOURCE: We could not establish proper initial estimates from the moment maps. These are what we got
 {"":8s}CHECK_SOURCE: pa = {pa}
 {"":8s}CHECK_SOURCE: inclination = {inclination}
 {"":8s}CHECK_SOURCE: maj_extent = {Configuration['SIZE_IN_BEAMS']}
 {"":8s}CHECK_SOURCE: SBR_initial = {SBR_initial}
 {"":8s}CHECK_SOURCE: VROT_initial = {VROT_initial}
 ''', Configuration)
 
         raise BadSourceError("No initial estimates. Likely the source is too faint.")
      # Determine whether the centre is blanked or not
 
 
-    sf.print_log(f'''CHECK_SOURCE: In the center we find the vsys {new_vsys} km/s around the location:
+    print_log(f'''CHECK_SOURCE: In the center we find the vsys {new_vsys} km/s around the location:
 {"":8s}CHECK_SOURCE: x,y,z = {int(round(x))}, {int(round(y))}, {int(round(z))}.
 {'':8s}CHECK_SOURCE: we will use a systemic velocity of {v_app}
 Checking the central flux in a box with size of {Configuration['BEAM_IN_PIXELS'][0]} in pixels around the central coordinates
 ''',Configuration,case= ['debug_add'])
     Central_Flux = np.mean(data[int(round(z-1)):int(round(z+1)),\
                                 int(round(y-Configuration['BEAM_IN_PIXELS'][0]/2.)):int(round(y+Configuration['BEAM_IN_PIXELS'][0]/2.)),\
                                 int(round(x-Configuration['BEAM_IN_PIXELS'][0]/2.)):int(round(x+Configuration['BEAM_IN_PIXELS'][0]/2.))])
     del data
-    sf.print_log(f'''CHECK_SOURCE: In the center we find an average flux of  {Central_Flux} Jy/beam around the location:
+    print_log(f'''CHECK_SOURCE: In the center we find an average flux of  {Central_Flux} Jy/beam around the location:
 {"":8s}CHECK_SOURCE: x,y,z = {int(round(x))}, {int(round(y))}, {int(round(z))}.
 ''',Configuration,case= ['debug_add'])
 
     if not np.isfinite(Central_Flux):
         Configuration['EXCLUDE_CENTRAL'] = True
-        sf.print_log(f'''CHECK_SOURCE: The flux in the central part is blanked. We exclude the central rings.
+        print_log(f'''CHECK_SOURCE: The flux in the central part is blanked. We exclude the central rings.
 ''',Configuration,case=['verbose'])
     else:
         Configuration['EXCLUDE_CENTRAL'] = False
 
 
     # Size of the galaxy in beams
     if np.sum(Configuration['SIZE_IN_BEAMS']) <= 2.*Configuration['TOO_SMALL_GALAXY']:
-        sf.print_log(f'''CHECK_SOURCE: This galaxy has an estimated size of  {np.sum(Configuration['SIZE_IN_BEAMS'])} beams in diameter.
+        print_log(f'''CHECK_SOURCE: This galaxy has an estimated size of  {np.sum(Configuration['SIZE_IN_BEAMS'])} beams in diameter.
 {'':8s}This is not large enough too fit. We will exit this fit.
 ''',Configuration,case= ['main','screen'])
         raise BadSourceError('The extracted source is too small')
     ring_size, number_of_rings = sf.set_ring_size(Configuration)
     old_radii = np.linspace(0.,Configuration['BEAM'][0]*(len(SBR_initial)-1),len(SBR_initial))
     new_radii = sf.set_rings(Configuration)
     SBR_initial = np.interp(new_radii,old_radii, SBR_initial)
     old_radii = np.linspace(0.,Configuration['BEAM'][0]*(len(VROT_initial)-1),len(VROT_initial))
     VROT_initial = np.interp(new_radii,old_radii, VROT_initial)
     Configuration['OUTER_SLOPE_START'] = Configuration['NO_RINGS']
-    sf.print_log(f'''CHECK_SOURCE: Interpolating the SBR and VROT estimates to these radi.
+    print_log(f'''CHECK_SOURCE: Interpolating the SBR and VROT estimates to these radi.
 {'':8s} {new_radii}
 {'':8s} We got SBR = {SBR_initial}, VROT = {VROT_initial}
 ''',Configuration,case= ['debug_add'])
 
 
     # The extent is fairly well determined and the maximum should be no more than +3 beams and a minimum no less than 4
-    # Swithcing here from doubled outer rings causes problems though
+    # Switching here from doubled outer rings causes problems though
     SNR_range=sf.set_limits(Max_SNR,1.9, 2.6)
 
     Configuration['MAX_SIZE_IN_BEAMS'] = sf.set_limits(np.max(Configuration['SIZE_IN_BEAMS'])*3.125/SNR_range+3.,1.,Configuration['MAX_SIZE_IN_BEAMS'])
     Configuration['MIN_SIZE_IN_BEAMS'] = sf.set_limits(np.max(Configuration['SIZE_IN_BEAMS'])-3.,Configuration['TOO_SMALL_GALAXY'],np.max(Configuration['SIZE_IN_BEAMS']))
     Configuration['NO_RINGS'] = sf.calc_rings(Configuration)
     Configuration['LAST_RELIABLE_RINGS'] = [Configuration['NO_RINGS'],Configuration['NO_RINGS']]
-    sf.print_log(f'''CHECK_SOURCE: From the original Configuration and SoFiA we find:
+    print_log(f'''CHECK_SOURCE: From the original Configuration and SoFiA we find:
 {"":8s}CHECK_SOURCE: The maximum diameter we will allow  is  {2.*Configuration['MAX_SIZE_IN_BEAMS']} beams. This is based on a SNR range of {SNR_range}
 {"":8s}CHECK_SOURCE: The minimum diameter we will allow  is  {2.*Configuration['MIN_SIZE_IN_BEAMS']} beams.
 {"":8s}CHECK_SOURCE: We start with a diameter of {np.sum(Configuration['SIZE_IN_BEAMS'])} beams in the model.
 {"":8s}CHECK_SOURCE: SoFiA found a PA of {kin_pa:.2f} and we use a PA = {pa[0]:.2f} +/- {pa[1]:.2f}
 {"":8s}CHECK_SOURCE: We start with an inclination of {inclination[0]:.2f} +/- {inclination[1]:.2f}{"":8s}
 {"":8s}CHECK_SOURCE: SoFiA found a W50 of {w50:.2f} km/s
 {"":8s}CHECK_SOURCE: We will use {2.*(Configuration['NO_RINGS']-1)} rings for the model with a ring size of {Configuration['RING_SIZE']}.
@@ -622,19 +639,30 @@
               DEC=[dec,abs(err_y*header['CDELT2'])],
               VSYS =[v_app,abs(err_z*header['CDELT3']/1000.)],
               PA=pa, Inclination = inclination, Max_Vrot = [max_vrot,max_vrot_dev], Tot_Flux = [f_sum,f_sum_err], V_mask = [VELboun[1]-VELboun[0],vres],
               Distance = Configuration['DISTANCE'] , DHI = [2*Configuration['SIZE_IN_BEAMS'][0]*Configuration['BEAM'][0],Configuration['BEAM'][0]*Configuration['RING_SIZE']])
 
 
     # extract a PV-Diagram
+    messages = extract_pv(cube = Cube,\
+                overwrite = False,PA=pa[0],center=[ra,dec,v_app*1000.], map_velocity_unit ='km/s',\
+                log = True,silent = True,velocity_type = Configuration['HDR_VELOCITY'],\
+                finalsize = [int(round(Configuration['SIZE_IN_BEAMS'][0]*Configuration['BEAM'][0]/np.mean([abs(header['CDELT1']),abs(header['CDELT2'])])*1.25+header['NAXIS1']*0.2)),
+                                    int(round(z_max-z_min)+10.)],   
+                output_directory = f"{Configuration['FITTING_DIR']}Sofia_Output",\
+                output_name =f"{Configuration['SOFIA_BASENAME']}_sofia_xv.fits")
+    print_log(messages,Configuration,case=["verbose"])
+    #PV = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['SOFIA_BASENAME']}_sofia_xv.fits")
+    '''
     if not os.path.exists(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['SOFIA_BASENAME']}_sofia_xv.fits"):
         PV =extract_pv(Configuration,Cube, pa[0], center=[ra,dec,v_app*1000.], convert = 1000.,
                        finalsize = [int(round(Configuration['SIZE_IN_BEAMS'][0]*Configuration['BEAM'][0]/np.mean([abs(header['CDELT1']),abs(header['CDELT2'])])*1.25+header['NAXIS1']*0.2)),
                                     int(round(z_max-z_min)+10.)])
         fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_sofia_xv.fits",PV[0].data,PV[0].header)
+    '''
     Cube.close()
     Initial_Parameters = {}
     Initial_Parameters['XPOS'] = [ra,sf.set_limits(abs(err_x*header['CDELT1']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
     Initial_Parameters['YPOS'] = [dec,sf.set_limits(abs(err_y*header['CDELT2']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
     Initial_Parameters['VSYS'] =[v_app,vsys_error]
 
     if Configuration['OUTER_RINGS_DOUBLED']:
@@ -687,15 +715,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def check_initial_boundaries(Configuration, Initial_Parameters):
-    sf.print_log(f'''CHECK_INITIAL_BOUNDARIES: Starting Check
+    print_log(f'''CHECK_INITIAL_BOUNDARIES: Starting Check
 ''',Configuration,case= ['debug_start'])
     for parameter in Initial_Parameters:
         #some initial parameters we do not want to check as they are not in the models
         if parameter in ['FLUX']:
             continue
         if parameter in ['VROT_profile','SBR_profile']:
             stripped_parameter= parameter.split('_')[0]
@@ -709,15 +737,15 @@
                 error=0.
         else:
             stripped_parameter= parameter
             length=1
             error = sf.set_limits(abs(Initial_Parameters[parameter][1]/10.),0.,\
                 abs(Configuration[f'{stripped_parameter}_INPUT_BOUNDARY'][0][0])*1.05)
         if np.sum(Configuration[f'{stripped_parameter}_INPUT_BOUNDARY']) != 0.:
-            sf.print_log(f'''CHECK_INITIAL_BOUNDARIES: Checking {parameter}
+            print_log(f'''CHECK_INITIAL_BOUNDARIES: Checking {parameter}
 {'':8s} stripped_parameter = {stripped_parameter}
 {'':8s} boundaries = {Configuration[f'{stripped_parameter}_INPUT_BOUNDARY']}
 {'':8s} length = {length}
 {'':8s} error = {error}
 ''',Configuration,case= ['debug_add'])
             for i in range(length):
                 Initial_Parameters[parameter][i] = sf.set_limits(\
@@ -736,15 +764,15 @@
     #print(vrot,incl,incl_2)
     vobs= [[x*np.sin(np.radians(y)),x*np.sin(np.radians(z))] for x,y,z in zip(vrot,incl,incl_2)]
     delta = [[abs(x-x1),abs(y-y1),abs(z-z1)] for x,y,z,x1,y1,z1 in zip(vrot,incl,incl_2,vrot[1:],incl[1:],incl_2[1:]) ]
     #print(delta)
 
 
     for i,pair in enumerate(vobs):
-        sf.print_log(f'''CHECK_VOBS:For ring {i} we find vobs {pair}
+        print_log(f'''CHECK_VOBS:For ring {i} we find vobs {pair}
 {'':8s} And the differences {[delta[i-1] if i >0 else [0,0,0]]}.
 ''',Configuration,case= ['debug_add'])
 
     passed=True
     return passed
 
 check_vobs.__doc__='''
@@ -785,31 +813,46 @@
     if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 15:
         spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]*2.)))
     if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 30:
         spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]))*3)
     if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 45:
         spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]))*4)
 
-    sf.print_log(f'''CONSTRUCT_KERNELS: We use the following spatial_kernels
+    print_log(f'''CONSTRUCT_KERNELS: We use the following spatial_kernels
 {'':8s} spatial kernels = {spatial_kernels}
 ''', Configuration)
     velocity_kernels = [0]
+    #We want to smooth at 5 km/s,10 kms and 15 and 25 km/s andif the cube spans more than 400 km/s\
+    #also at 50 km/s
+    dispersion = [5.,10,15.,25. ,50.]
+    fact = 5.
+    for disp in dispersion:
+        kernel = int(disp/Configuration['CHANNEL_WIDTH'])
+        if disp == 50:
+            fact = 8.
+        if kernel*fact < Configuration['NAXES'][2]:
+            if fact == 8.:
+                Configuration['VEL_SMOOTH_EXTENDED'] = True
+                print_log(f'''CONSTRUCT_KERNELS: Using a very extended velocity smoothing as the cube spans more than 400 km/s.
+''', Configuration)       
+            velocity_kernels.append(kernel)
+    '''
     if Configuration['NAXES'][2] > 12:
         velocity_kernels.append(3)
     if Configuration['NAXES'][2] > 24:
         velocity_kernels.append(6)
     if Configuration['NAXES'][2] > 48:
         velocity_kernels.append(12)
     if Configuration['NAXES'][2] > 52:
         velocity_kernels.append(16)
         Configuration['VEL_SMOOTH_EXTENDED'] = True
-        sf.print_log(f'''CONSTRUCT_KERNELS: Using a very extended velocity smoothing as the cube has more than 52 channels.
-''', Configuration)
-
-    sf.print_log(f'''CONSTRUCT_KERNELS: We use the following velocity kernels
+        print_log(f''CONSTRUCT_KERNELS: Using a very extended velocity smoothing as the cube has more than 52 channels.
+'', Configuration)
+    '''
+    print_log(f'''CONSTRUCT_KERNELS: We use the following velocity kernels
 {'':8s} velocity kernels = {velocity_kernels}
 ''', Configuration)
     sofia_template['scfind.kernelsXY'] = ','.join([str(x) for x in spatial_kernels])
     sofia_template['scfind.kernelsZ'] = ','.join([str(x) for x in velocity_kernels])
     return spatial_kernels,velocity_kernels
 
 construct_kernels.__doc__ =f'''
@@ -837,39 +880,40 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 def failed_fit(Configuration,Tirific_Template,current_run, Fits_Files,\
         stage='initial', fit_type='Fit_Tirific_OSC'):
-    sf.print_log(f'''FAILED_FIT: Tirific failed to produce output in {fit_type}. It might be an unspecified crash.
+    print_log(f'''FAILED_FIT: Tirific failed to produce output in {fit_type}. It might be an unspecified crash.
 we try once more else we break off the fitting. As this sometimes happens due to a gsl interpolation error we modify the ring size by 5%
 ''',Configuration, case=['main','screen'])
     # There appears to be a case where the last ring can cause an interpolation error.
     # Deal with this we take 0.95% of the beam ring size and run again
     # I don't understand why we removed this again.
     Configuration['OLD_SIZE'].append(list(copy.deepcopy(Configuration['SIZE_IN_BEAMS'])))
     Configuration['SIZE_IN_BEAMS'] = Configuration['SIZE_IN_BEAMS']*0.95
     ring_size, number_of_rings = sf.set_ring_size(Configuration)
     set_new_size(Configuration,Tirific_Template,fit_type= fit_type\
             ,current_run = current_run)
     if stage == 'full_res':
 
         #if the crash happens when make the full resolution  we need to
         # rescale the last iteration
-        sf.print_log(f'''FAILED_FIT: We are rescaleing {Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def
+        print_log(f'''FAILED_FIT: We are rescaleing {Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def
     ''',Configuration,case=['main'])
         Last_Iteration = sf.tirific_template(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def")
         set_new_size(Configuration,Last_Iteration,fit_type= fit_type
                 ,current_run = 'Not Zed')
         wf.tirific(Configuration,Tirific_Template,name = \
             f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def",
             full_name=True)
     wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
-    accepted,current_run = sf.run_tirific(Configuration,current_run,stage = stage, fit_type = fit_type)
+    accepted,current_run = sf.run_tirific(Configuration,current_run,stage = stage, fit_type = fit_type,\
+                                max_ini_time= int(300*(int(Tirific_Template['INIMODE'])+1)))
     return accepted,current_run
 
 failed_fit.__doc__ =f'''
  NAME:
     failed_fit
 
  PURPOSE:
@@ -891,55 +935,64 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-def fitting_osc(Configuration,Fits_Files,Tirific_Template,Initial_Parameters):
+def fitting_osc(Configuration,Fits_Files,Initial_Parameters):
+    # First we want to read the template
+    Tirific_Template = sf.tirific_template()
+    # if the CTYPE3 is not 'VELO' we want to make a copy of the fitting cube that is used in tirific
+    if Configuration['HDR_VELOCITY'] != 'VELO':
+        Fits_Files = wf.create_tirific_run_cube(Configuration,Fits_Files)
     current_run = 'Not Initialized'
     Configuration['FIT_TIME'][0] = datetime.now()
     sf.create_directory(Configuration['USED_FITTING'],Configuration['FITTING_DIR'])
     wf.initialize_def_file(Configuration, Fits_Files,Tirific_Template, \
                            Initial_Parameters= Initial_Parameters, \
                            fit_type=Configuration['USED_FITTING'])
-    sf.print_log(f'''FITTING_OSC: The initial def file is written and we will now start fitting.
+    print_log(f'''FITTING_OSC: The initial def file is written and we will now start fitting.
 ''' ,Configuration)
 
         # If we have no directory to put the output we create it
 
     while not Configuration['ACCEPTED'] and Configuration['ITERATIONS'] <  Configuration['MAX_ITERATIONS']:
         Configuration['ITERATIONS'] = Configuration['ITERATIONS']+1
         # Run the step
         current_run = one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run)
 
         if (Configuration['ITERATIONS'] == 1  and np.sum(Configuration['SIZE_IN_BEAMS']) < 10.6) or  (Configuration['ACCEPTED'] and np.sum(Configuration['SIZE_IN_BEAMS']) < 6.6):
-            sf.print_log(f'''FITTING_OSC: Checking the inclination due to small galaxy size.
+            print_log(f'''FITTING_OSC: Checking the inclination due to small galaxy size.
 {'':8s}PA = {Tirific_Template['PA']}
 {'':8s}INCL = {Tirific_Template['INCL']}
 ''',Configuration,case= ['debug_add'])
             check_inclination(Configuration,Tirific_Template,Fits_Files, fit_type =Configuration['USED_FITTING'])
 
     if Configuration['ACCEPTED']:
-        sf.print_log(f'''FITTING_OSC: The model has converged in center and extent and we make a smoothed version.
+        print_log(f'''FITTING_OSC: The model has converged in center and extent and we make a smoothed version.
 ''',Configuration)
-        current_run = fit_smoothed_check(Configuration, Fits_Files,\
+        current_run = fit_smoothed(Configuration, Fits_Files,\
             Tirific_Template,current_run,stage = 'after_os',\
-             fit_type = Configuration['USED_FITTING'])
+            fit_type = Configuration['USED_FITTING'])
         if Configuration['OPTIMIZED']:
             make_full_resolution(Configuration,Tirific_Template,Fits_Files,\
                 current_run = current_run,fit_type = Configuration['USED_FITTING'])
     elif Configuration['INSTALLATION_CHECK']:
-        sf.print_log(f'''FITTING_OSC: The Installation_check has run a fit successfully.
+        print_log(f'''FITTING_OSC: The Installation_check has run a fit successfully.
 ''',Configuration)
+        fit_type = Configuration['USED_FITTING']
+        source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def")
+        target = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_1.def")
+        copyfile(source, target )
     else:
         Configuration['FINAL_COMMENT'] = 'We could not converge on the extent or centre of the galaxy'
         Configuration['OUTPUT_QUANTITY'] = 5
     Configuration['FIT_TIME'][1] = datetime.now()
-    return current_run
+    return current_run,Tirific_Template
 fitting_osc.__doc__ =f'''
  NAME:
     fitting_osc
 
  PURPOSE:
     Do the full one step convergence routines.
 
@@ -961,64 +1014,52 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This is the main fitting routine if you want to make your own start by looking here. And then add it in main.py
        This is the fitting type done for the installation check.
 '''
 
-def fit_smoothed_check(Configuration, Fits_Files,Tirific_Template,current_run, \
-            stage = 'initial',fit_type='Undefined'):
-    sf.update_statistic(Configuration, message= "Starting the smoothed check run")
-    sf.print_log(f'''FIT_SMOOTHED_CHECK: Starting stage {stage} and fit_type {fit_type}.
-''',Configuration,case= ['debug_start'])
-    if Configuration['DEBUG']:
-        sf.write_config(
-            f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Smoothing.txt', Configuration)
-        wf.tirific(Configuration,Tirific_Template, name = 'Input_to_Smooth.def')
-        os.system(f'''mv {Configuration['FITTING_DIR']}/Input_to_Smoothed_Check.def {Configuration['LOG_DIRECTORY']}''')
+def fit_smoothed(Configuration, Fits_Files,Tirific_Template,current_run, stage = 'initial', \
+                 fit_type='Undefined'):
+    #As check angles makes modifications we first want to reload the last fit into the template
+    Last_Fit_File = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def"
+    variables_to_reset =['PA','PA_2','INCL','INCL_2']
+    reset_values = sf.load_tirific(Configuration,Last_Fit_File,Variables =\
+                                 variables_to_reset,array=True)
+
+    for parameter in variables_to_reset:
+        Tirific_Template[parameter] = \
+            f"{' '.join([f'{x}' for x in reset_values[variables_to_reset.index(parameter)][:Configuration['NO_RINGS']]])}"
+
+
+    #And we create a recovery point
+    enter_recovery_point(Configuration, Fits_Files = Fits_Files, Tirific_Template= Tirific_Template,
+                         message = 'Start of fit_smoothed.',point_ID='Start_Fit_Smoothed')
 
+  
     #if we have only a few rings we only smooth. else we fit a polynomial to the RC and smooth the SBR
     #smoothed_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',hdr, min_error= np.max([float(Tirific_Template['CFLUX']),float(Tirific_Template['CFLUX_2'])]))
     fix_sbr(Configuration,Tirific_Template,smooth = True)
     if stage == 'after_cc':
         smoothed_vrot = smooth_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'])
     else:
-        min_error = []
-        pars_to_smooth = []
-        not_to_smooth = []
-        fixed_errors = []
-        for parameter in ['VROT','INCL','Z0','SDIS','PA','XPOS','YPOS','VSYS']:
-            if parameter in Configuration['FIXED_PARAMETERS'][0]:
-                not_to_smooth.append(parameter)
-            else:
-                pars_to_smooth.append(parameter)
-            min_error.append(Configuration['MIN_ERROR'][parameter])
-        warp_triggered = False
-        for key,min_err in zip(pars_to_smooth,min_error):
-                if key in ['PA','INCL']:
-                    if not warp_triggered:
-                        smoothed = regularise_warp(Configuration,Tirific_Template,\
-                            min_error = [Configuration['MIN_ERROR']['PA'],\
-                            Configuration['MIN_ERROR']['INCL']])
-                        warp_triggered = True
-                    else:
-                        pass
-                else:
-                    smoothed = regularise_profile(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter])
-                if key == 'VROT':
-                    smoothed_vrot=copy.deepcopy(smoothed)
-
-        for key,min_err in zip(not_to_smooth,fixed_errors):
-            set_errors(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter])
-    #
+      
+        for parameter in ['VROT','Z0','SDIS','XPOS','YPOS','VSYS']:
+            smoothed = regularise_profile(Configuration,Tirific_Template,\
+                        parameter)
+            if parameter == 'VROT':
+                smoothed_vrot=copy.deepcopy(smoothed)
+        #For the warp the PA and INCL we do it differently 
+        smoothed = regularise_warp(Configuration,Tirific_Template)
+                          
     if stage == 'after_cc':
 
         Tirific_Template['LOOPS'] = 1.
         if Configuration['OPTIMIZED']:
-            Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+            Tirific_Template['INSET'] = f"{Fits_Files['TIR_RUN_CUBE']}"
             Tirific_Template['INIMODE'] = "0"
             sf.finish_current_run(Configuration,current_run)
     else:
         Tirific_Template['LOOPS'] = f"{Configuration['LOOPS']}"
         xpos,ypos,vsys,pa,incl = sf.load_tirific(Configuration,\
             f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
             Variables = ['XPOS','YPOS','VSYS','PA','INCL'],array=True)
@@ -1033,50 +1074,56 @@
                 parameters_to_adjust = ['VSYS','SBR','XPOS','YPOS','PA','SDIS','VROT']
         else:
             parameters_to_adjust = ['NO_ADJUSTMENT'] #This triggers the default settings in set_fitting_parameters
 
         set_fitting_parameters(Configuration, Tirific_Template,stage = stage,\
                           initial_estimates = parameters,parameters_to_adjust = parameters_to_adjust)
 
+    
     if Configuration['DEBUG']:
         source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
-        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Last_Unsmoothed_Input.def")
+        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/Last_Unsmoothed_Input.def")
         os.system(f"cp {source} {target}")
     wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
     if Configuration['DEBUG']:
         source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
-        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Smoothed_Input.def")
+        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/Smoothed_Input.def")
         os.system(f"cp {source} {target}")
     try:
-        accepted,current_run = sf.run_tirific(Configuration,current_run, stage = stage, fit_type=fit_type)
+        accepted,current_run = sf.run_tirific(Configuration,current_run, stage = stage, fit_type=fit_type,\
+                                max_ini_time= int(300*(int(Tirific_Template['INIMODE'])+1)))
     except TirificOutputError:
         accepted,current_run = failed_fit(Configuration,Tirific_Template,current_run,\
             Fits_Files, stage=stage, fit_type=fit_type)
-
+    
     write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
+       
     if Configuration['NO_RINGS'] > 5.:
+        Configuration['FIX_RING_SIZE'] = True
+        cut_low_rings(Configuration, Tirific_Template,Fits_Files,fit_type=fit_type,current_run=current_run)
         smoothed_vrot = regularise_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'])
         set_fitting_parameters(Configuration, Tirific_Template,stage = 'final_os',\
                           initial_estimates = parameters,parameters_to_adjust  = ['VROT'])
 
         wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
         if Configuration['DEBUG']:
             source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
-            target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Second_Smoothed_Input.def")
+            target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/Second_Smoothed_Input.def")
             os.system(f"cp {source} {target}")
         try:
-            accepted,current_run = sf.run_tirific(Configuration,current_run, stage = 'final_os', fit_type=fit_type)
+            accepted,current_run = sf.run_tirific(Configuration,current_run, stage = 'final_os', fit_type=fit_type,\
+                                max_ini_time= int(300*(int(Tirific_Template['INIMODE'])+1)))
         except TirificOutputError:
             accepted,current_run = failed_fit(Configuration,Tirific_Template,\
                 current_run,Fits_Files, stage='final_os', fit_type=fit_type)
 
     return current_run
-fit_smoothed_check.__doc__ =f'''
+fit_smoothed.__doc__ =f'''
  NAME:
-    fit_smoothed_check
+    fit_smoothed
 
  PURPOSE:
     fine tune the fit after smoothing all variables.
 
  CATEGORY:
     run_functions
 
@@ -1103,33 +1150,34 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 def make_full_resolution(Configuration,Tirific_Template,Fits_Files,\
         fit_type = 'Undefined', current_run = 'Not zed'):
-    sf.update_statistic(Configuration, message= "Starting to make a full resolution model run")
+    update_statistics(Configuration, message= "Starting to make a full resolution model run")
 
-    sf.print_log(f'''MAKE_FULL_RESOLUTION: creating full resolution for stage {fit_type}.
+    print_log(f'''MAKE_FULL_RESOLUTION: creating full resolution for stage {fit_type}.
 ''',Configuration,case= ['main','debug_start'])
     write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
-    Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+    Tirific_Template['INSET'] = f"{Fits_Files['TIR_RUN_CUBE']}"
     Tirific_Template['VARY'] = f" VROT 1:3"
     Tirific_Template['VARINDX'] = f" "
     Tirific_Template['LOOPS'] = "0"
     Tirific_Template['INIMODE'] = "0"
     wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
     if Configuration['DEBUG']:
         wf.tirific(Configuration,Tirific_Template,\
             name = f'{Configuration["LOG_DIRECTORY"]}/Full_Resolution_Input.def',\
             full_name = True )
     sf.finish_current_run(Configuration,current_run)
     try:
         accepted,current_run = sf.run_tirific(Configuration,'Not zed', \
-            stage = 'full_res', fit_type=fit_type)
+            stage = 'full_res', fit_type=fit_type,\
+            max_ini_time= int(300*(int(Tirific_Template['INIMODE'])+1)))
     except TirificOutputError:
         accepted,current_run = failed_fit(Configuration,Tirific_Template,\
             'Not Zed', Fits_Files,stage='full_res', fit_type=fit_type)
 
 
     sf.finish_current_run(Configuration,current_run)
 make_full_resolution.__doc__ =f'''
@@ -1163,94 +1211,108 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run):
-
-    sf.print_log(f'''ONE_STEP_CONVERGENCE: For {Configuration['ID']} we are starting loop {Configuration['ITERATIONS']} out of maximum {Configuration['MAX_ITERATIONS']}.
+    print_log(f'''ONE_STEP_CONVERGENCE: For {Configuration['ID']} we are starting loop {Configuration['ITERATIONS']} out of maximum {Configuration['MAX_ITERATIONS']}.
 ''',Configuration, case=['main','screen','debug_start'])
+    
     fit_type = 'Fit_Tirific_OSC'
     stage = 'run_os'
     #First we run tirific
     try:
         accepted,current_run = sf.run_tirific(Configuration,current_run,\
-            stage = stage, fit_type = fit_type)
+            stage = stage, fit_type = fit_type,\
+            max_ini_time= int(300*(int(Tirific_Template['INIMODE'])+1)))
     except TirificOutputError:
+        #exit()
         accepted,current_run = failed_fit(Configuration,Tirific_Template,\
             current_run, Fits_Files,stage=stage, fit_type=fit_type)
 
 
     if not accepted:
         Configuration['ACCEPTED_TIRIFIC'] = False
         if Configuration['LOOPS'] < 20.:
-            sf.print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops ({Configuration['LOOPS']}) increasing this by 1.
+            print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops ({Configuration['LOOPS']}) increasing this by 1.
 ''',Configuration)
             Configuration['LOOPS'] += 1
     else:
         Configuration['ACCEPTED_TIRIFIC'] = True
     #Then we load the produced output into our template
     write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def" , Tirific_Template)
+    
     #Check that the centre does not deviate too much
-
     accepted_central = check_central_convergence(Configuration,Tirific_Template, fit_type = fit_type)
     if accepted_central:
         Configuration['CENTRAL_CONVERGENCE'] = True
         Configuration['CENTRAL_CONVERGENCE_COUNTER'] += 1.
         Configuration['CENTRAL_FIX'] = []
 
     # Check whether we have the correct sizes,
 
     #This currently doesn't do anything
     #accepted_proj_vrot = check_vobs(Configuration,Tirific_Template, fit_type = fit_type)
     # Check whether the central INCL and PA are stable. But only if the center is accepted
     if accepted_central:
-        accepted_angle = check_angle_convergence(Configuration,Tirific_Template, fit_type = fit_type)
+        accepted_angle,accepted_boundary = check_angle_convergence(Configuration,Tirific_Template, fit_type = fit_type)
     else:
         accepted_angle = False
-    #We only adapt the size if the other checks are ok
-    if not all(Configuration['FIX_SIZE']) and accepted_central and accepted_angle:
-        no_apply_size_change = False
-    else:
-        no_apply_size_change = True
-    accepted_size = check_size(Configuration,Tirific_Template, \
-        no_apply = no_apply_size_change, fit_type = fit_type, stage = stage, \
-        current_run = current_run,Fits_Files=Fits_Files)
+        accepted_boundary = False
+   
+    
     if all(Configuration['FIX_SIZE']):
         accepted_size = True
-    if accepted and accepted_size and accepted_central and accepted_angle: #and accepted_proj_vrot:
+    else:
+         #We only adapt the size if the other checks are ok
+        if accepted_central and accepted_angle:
+            no_apply_size_change = False
+        else:
+            no_apply_size_change = True
+        accepted_size = check_size(Configuration,Tirific_Template, \
+            no_apply = no_apply_size_change, fit_type = fit_type, stage = stage, \
+            current_run = current_run,Fits_Files=Fits_Files)
+   
+    if accepted and accepted_size and accepted_central and accepted_angle and accepted_boundary: #and accepted_proj_vrot:
         Configuration['ACCEPTED'] = True
     else:
         Configuration['ACCEPTED'] = False
         if Configuration['ITERATIONS'] > Configuration['MAX_ITERATIONS']:
-                sf.print_log(f'''ONE_STEP_CONVERGENCE: We have ran the convergence more than {Configuration['MAX_ITERATIONS']} times aborting the fit.
+                print_log(f'''ONE_STEP_CONVERGENCE: We have ran the convergence more than {Configuration['MAX_ITERATIONS']} times aborting the fit.
 ''',Configuration)
                 return current_run
         if not accepted:
-            sf.print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops hence we do not accept and we smooth and retry.
+            print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops hence we do not accept and we smooth and retry.
 ''',Configuration)
         if not accepted_central:
-            sf.print_log(f'''ONE_STEP_CONVERGENCE: The center varied too much hence we do not accept and we smooth and retry.
+            print_log(f'''ONE_STEP_CONVERGENCE: The center varied too much hence we do not accept and we smooth and retry.
+''',Configuration)
+        elif not accepted_boundary or not accepted_angle:
+            if not accepted_boundary:
+                print_log(f'''ONE_STEP_CONVERGENCE: The boundaries have been adapted.
 ''',Configuration)
-        elif not accepted_angle:
-            sf.print_log(f'''ONE_STEP_CONVERGENCE: The central disk PA or INCL have changed too much or the boundaries have been adapted.
+            if not accepted_angle:
+                print_log(f'''ONE_STEP_CONVERGENCE: The central disk PA or INCL have changed too much.
 ''',Configuration)
         elif not accepted_size:
-            sf.print_log(f'''ONE_STEP_CONVERGENCE: FAT adjusted the rings. Refitting with new settings after smoothing them.
+            print_log(f'''ONE_STEP_CONVERGENCE: FAT adjusted the rings. Refitting with new settings after smoothing them.
 ''',Configuration)
 
 
         #if not accepted_proj_vrot:
-        #    sf.print_log(f'''ONE_STEP_CONVERGENCE: The outer VROT and INCL did not converge on the minimumal change that allows for VROT*Sin(INCL)
+        #    print_log(f'''ONE_STEP_CONVERGENCE: The outer VROT and INCL did not converge on the minimumal change that allows for VROT*Sin(INCL)
 #''',Configuration)
 
 
         # First we fix the SBR we are left with also to set the reliable ring to configuration.
-        fix_sbr(Configuration,Tirific_Template,smooth = True)    # Then we determine the inner rings that should remain fixed
+          
+        fix_sbr(Configuration,Tirific_Template,smooth = True)  
+       
+        # Then we determine the inner rings that should remain fixed
 
         sf.get_inner_fix(Configuration, Tirific_Template)
 
         if all([True if x  in Configuration['FIXED_PARAMETERS'][0] else False for x in ['PA','INCL','Z0','SDIS']] ):
         #if all([Configuration['FIX_INCLINATION'][0],Configuration['FIX_PA'][0],Configuration['FIX_Z0'][0],Configuration['FIX_SDIS'][0]]):
             Configuration['WARP_SLOPE'] = [None ,None ]
         else:
@@ -1301,57 +1363,107 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This routine sets the Configuration['ACCEPTED']
 '''
 
+def set_trm_template(Configuration):
+    directory = f'{Configuration["FITTING_DIR"]}/Error_Shaker/'
+    with pack_open_txt(templates, 'TRM_errors_FAT.yml') as tmp:
+            template = tmp.readlines()
+    with open(f'{directory}/FAT_conf.yml','w') as file:
+        for line in template:
+            file.write(line)
+   
+    trm_template = OmegaConf.load(f'{directory}/FAT_conf.yml')
+    parameters = [x for x in Configuration['MIN_ERROR']]
+    for parameter in parameters:
+        setattr(trm_template.min_errors,parameter,float(Configuration['MIN_ERROR'][parameter][0]))
+    if Configuration['INSTALLATION_CHECK']:
+        trm_template.tirshaker.iterations=2
+        trm_template.tirshaker.inimode = 0
+        trm_template.tirshaker.individual_loops=1 
+        trm_template.general.verbose = True
+
+
+    trm_template.tirshaker.deffile_in = 'Error_Shaker/Error_Shaker_FAT_Start.def'
+    trm_template.general.directory = f'{Configuration["FITTING_DIR"]}'
+
+    with open(f'{directory}/FAT_conf.yml','w') as default_write:
+        default_write.write(OmegaConf.to_yaml(trm_template))
+set_trm_template.__doc__ =f'''
+ NAME:
+    set_trm_template
+
+ PURPOSE:
+    Set the proper paraemters for running TRM_errors   
+ 
+ CATEGORY:
+    run_functions
+
+ INPUTS:
+    Configuration
+
+ OPTIONAL INPUTS:
+
+
+
+ OUTPUTS:
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
 def sofia(Configuration, Fits_Files):
-    sf.print_log(f'''RUN_SOFIA: starting sofia run from the template.
+    print_log(f'''RUN_SOFIA: starting sofia run from the template.
 ''',Configuration,case= ['debug_start'])
-    sf.update_statistic(Configuration, message= "Starting the SoFiA run")
+    update_statistics(Configuration, message= "Starting the SoFiA run")
 
     sofia_template = rf.sofia_template()
     sf.create_directory('Sofia_Output',Configuration['FITTING_DIR'])
     os.chdir(Configuration['FITTING_DIR'])
-    threshold = 5.
     counter = 3
     sofia_template['input.data'] = Fits_Files['FITTING_CUBE']
     spatial_kernels,velocity_kernels = construct_kernels(Configuration,sofia_template)
 
     sofia_ok = False
     while not sofia_ok:
         clean_before_sofia(Configuration)
-        sofia_template['scfind.threshold'] = str(threshold)
+        sofia_template['scfind.threshold'] = str(Configuration['SOFIA_THRESHOLD'])
         wf.sofia(sofia_template,'sofia_input.par')
-        sf.print_log("RUN_SOFIA: Running SoFiA. \n",Configuration)
+        print_log("RUN_SOFIA: Running SoFiA. \n",Configuration)
         # Check which sofia to start
         sfrun = subprocess.Popen([Configuration['SOFIA2'],'sofia_input.par'], stdout = subprocess.PIPE, stderr = subprocess.PIPE)
         sofia_run, sofia_warnings_are_annoying = sfrun.communicate()
-        sf.print_log(sofia_run.decode("utf-8"), Configuration)
+        print_log(sofia_run.decode("utf-8"), Configuration)
 
         if sfrun.returncode == 8:
-            if threshold > 3.:
-                log_statement = f'''RUN_SOFIA: We did not find a source at a threshold of {threshold}
+            if Configuration['SOFIA_THRESHOLD'] > 3.:
+                log_statement = f'''RUN_SOFIA: We did not find a source at a threshold of {Configuration['SOFIA_THRESHOLD']}
 {"":8s} RUN_SOFIA: Lowering the threshold and trying again."
 '''
-                sf.print_log(log_statement,Configuration)
-                threshold -= 2
+                print_log(log_statement,Configuration)
+                Configuration['SOFIA_THRESHOLD'] -= 1
             else:
                 clean_after_sofia(Configuration)
-                log_statement = f'''RUN_SOFIA: We did not find a source above a threshold of {threshold}.
+                log_statement = f'''RUN_SOFIA: We did not find a source above a threshold of {Configuration['SOFIA_THRESHOLD']}.
 {"":8s}RUN_SOFIA: We cannot lower the threshold lower as the risk of fitting noise becomes too high.
 {"":8s}Continuing to the next galaxy.
 '''
-                sf.print_log(log_statement,Configuration)
+                print_log(log_statement,Configuration)
                 raise FaintSourceError("RUN_SOFIA:Sofia cannot find a source above a threshold of 3.")
         elif sfrun.returncode == 0:
             sofia_ok = True
         else:
-            sf.print_log(sofia_warnings_are_annoying.decode("utf-8"), Configuration,case=['main','screen'])
+            print_log(sofia_warnings_are_annoying.decode("utf-8"), Configuration,case=['main','screen'])
             raise SofiaRunError("RUN_SOFIA:Sofia did not execute properly. See log for details")
 
     #Move sofia output to the desired Directory
     clean_after_sofia(Configuration)
     Configuration['SOFIA_RAN'] = True
     os.chdir(Configuration['START_DIRECTORY'])
 sofia.__doc__ =f'''
@@ -1378,69 +1490,54 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-
-def tirshaker_call(Configuration):
+    
+def tirshaker_call(Configuration,Fits_Files):
     # First we make a directory to keep all contained
-    sf.update_statistic(Configuration, message= "Starting the Tirshaker call run")
+    update_statistics(Configuration, message= "Starting the Tirshaker call run")
+
+    from TRM_errors.main import main as errors_main
+
+   
     if not os.path.isdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/"):
         os.mkdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/")
 
-
     # Then we open the final file
-    filename = f"{Configuration['FITTING_DIR']}Error_Shaker/Error_Shaker_In.def"
-
+    #filename = f"{Configuration['FITTING_DIR']}Error_Shaker/Error_Shaker_In.def"
+    #Preaper the fat fitting file
+    #transfer_fitting_parameters(Configuration)    
     final_FAT_file= f"{Configuration['FITTING_DIR']}{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def"
-
-    Tirific_Template = sf.tirific_template(filename = final_FAT_file \
-                    )
+    Tirific_Template = sf.tirific_template(filename = final_FAT_file)
     #Change the name and run only 2 LOOPS
-    Tirific_Template['RESTARTNAME']= f"restart_Error_Shaker.txt"
-    Tirific_Template['INSET'] = f"../{Tirific_Template['INSET']}"
-    Tirific_Template['TIRDEF']= f"Error_Shaker_Out.def"
-    Tirific_Template['LOOPS'] = '1'
-
-    outfilename = 'Error_Shaker.def'
-    outfileprefix = 'Error_Shaker'
-
-    #This we need to remove from the actual run
-    #Configuration['NO_RINGS'] = int(Tirific_Template['NUR'])
-    #Configuration['RING_SIZE'] = 1.
-    #Configuration['SIZE_IN_BEAMS'] = Configuration['NO_RINGS']-2
+    if Configuration['OPTIMIZED']:
+        Tirific_Template['INSET'] = f"{Fits_Files['OPTIMIZED_CUBE']}"
+    else:
+        Tirific_Template['INSET'] = f"{Fits_Files['TIR_RUN_CUBE']}"
+    
     set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os')
 
     #Write it back to the file
-    wf.tirific(Configuration,Tirific_Template, name =f"Error_Shaker/Error_Shaker_In.def" )
-
-    #Determine the error block from the last fit settings.
-    parameter_groups,rings,block,variation,variation_type = sf.get_fit_groups(Configuration,Tirific_Template)
-    sf.print_log(f'''TIRSHAKER_CALL: We are shaking with the following parameters:
-{'':8s}groups = {parameter_groups}
-{'':8s}rings = {rings}
-{'':8s}block = {block}
-{'':8s}variation = {variation}
-{'':8s}variation_type = {variation_type}
-''',Configuration,case= ['debug_add'])
-
-    iterations = Configuration['SHAKER_ITERATIONS']
-    random_seed = 2
-    os.chdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/")
-    tirshaker(Configuration,Tirific_Template, outfilename = outfilename,\
-                outfileprefix = outfileprefix, parameter_groups = parameter_groups, \
-                rings = rings, block = block, variation = variation,\
-                 variation_type = variation_type, iterations = iterations,
-                 random_seed = random_seed, mode = 'mad')
-    os.chdir(f"{Configuration['START_DIRECTORY']}")
-
-    wf.tirific(Configuration,Tirific_Template,name=f"{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def")
-
+    wf.tirific(Configuration,Tirific_Template, name =f"Error_Shaker/Error_Shaker_FAT_Start.def" )
+    #setup a yaml file for TRM_errors
+    set_trm_template(Configuration)
+   
+
+    errors_main([f'configuration_file={Configuration["FITTING_DIR"]}/Error_Shaker/FAT_conf.yml'])
+    update_statistics(Configuration, message= "After the Tirshaker call run")
+
+    out_name = f"{Configuration['FITTING_DIR']}/{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def"
+    #before copying we should transfer the errors
+    transfer_errors(Configuration,fit_type=Configuration['USED_FITTING'])
+    os.rename(out_name,f"{Configuration['FITTING_DIR']}/{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}_Original_Errors.def")
+    os.rename(f"{Configuration['FITTING_DIR']}/Error_Shaker/Shaken_Errors.def",out_name)
+  
 tirshaker_call.__doc__ =f'''
  NAME:
     tirshaker
 
  PURPOSE:
     function to setup the right input for tirshaker and call it and afterwards process the results
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/support_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/support_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 # -*- coding: future_fstrings -*-
-# This module contains a set of functions and classes that are used in several different Python scripts in the Database.
-import pyFAT_astro
+
 from pyFAT_astro.Support.fat_errors import SupportRunError,SmallSourceError,\
                                               FileNotFoundError,TirificKillError,\
                                               InputError,ProgramError,DefFileError,\
-                                              BadHeaderError,FittingError,TirificOutputError
-
+                                              BadHeaderError,FittingError,TirificOutputError,\
+                                              SofiaMissingError
+from pyFAT_astro.Support.log_functions import print_log,get_usage_statistics,write_config
 from pyFAT_astro import Templates as templates
 from collections import OrderedDict #used in Proper_Dictionary
-from inspect import getframeinfo,stack
 from numpy.linalg import LinAlgError
 from scipy.optimize import curve_fit, OptimizeWarning
 from scipy import ndimage
 from scipy.signal import savgol_filter
 from astropy.wcs import WCS
 from astropy.io import fits
-from dataclasses import  asdict
+
 try:
     from importlib.resources import files as import_pack_files
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     # For Py<3.9 files is not available
     from importlib_resources import files as import_pack_files
 try:
     from importlib.resources import open_text as pack_open_txt
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     from importlib_resources import open_text as pack_open_txt
 import matplotlib.pyplot as plt
 import os
-import sys
-import inspect
 import psutil as psu
 import signal
 import time
 import traceback
 import numpy as np
 import copy
 import warnings
@@ -44,15 +41,18 @@
 from datetime import datetime
 
 # A class of ordered dictionary where keys can be inserted in at specified locations or at the end.
 class Proper_Dictionary(OrderedDict):
     def __setitem__(self, key, value):
         if key not in self:
             # If it is a new item we only allow it if it is not Configuration or Original_Cube or if we are in setup_configuration
-            function,variable,empty = traceback.format_stack()[-2].split('\n')
+            try:
+                function,variable,empty = traceback.format_stack()[-2].split('\n')
+            except ValueError: 
+                function,variable = traceback.format_stack()[-2].split('\n')
             function = function.split()[-1].strip()
             variable = variable.split('[')[0].strip()
             if variable == 'Original_Configuration' or variable == 'Configuration':
                 if function != 'setup_configuration':
                     raise ProgramError("FAT does not allow additional values to the Configuration outside the setup_configuration in support_functions.")
         OrderedDict.__setitem__(self,key, value)
     #    "what habbens now")
@@ -222,14 +222,16 @@
 
 
         if 'INCL' in Configuration['FIXED_PARAMETERS']:
             Inclination_plane =   np.zeros((len(Theta),len(Phi)))
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore",message="divide by zero encountered in true_divide"\
                                     ,category=RuntimeWarning)
+                warnings.filterwarnings("ignore",message="divide by zero encountered in divide"\
+                                    ,category=RuntimeWarning)
                 for i in range(len(Theta)):
                     Inclination_plane[:,i]= 90-np.arctan(1./(np.cos(Theta[i])*np.tan(Phi[:])))*(360./(2*np.pi))
             Inclination_plane[np.where(Inclination_plane > 90.)] = 180 - Inclination_plane[np.where(Inclination_plane > 90.)]
             Inclination_plane[np.where(Inclination_plane < 0.)] = -1 * Inclination_plane[np.where(Inclination_plane < 0.)]
             current_inclination =  90-np.arctan(1./(np.cos(Theta_in[:])*np.tan(Phi_in[:])))*(360./(2*np.pi))
             current_inclination[np.where(current_inclination > 90.)] = 180 - current_inclination[np.where(current_inclination > 90.)]
             current_inclination[np.where(current_inclination < 0.)] = -1 * current_inclination[np.where(current_inclination < 0.)]
@@ -245,14 +247,16 @@
                     Phi_out[not_flat[i]]=options_Phi[location[0]]
                     Theta_out[not_flat[i]]=options_Theta[location[0]]
         if 'PA' in Configuration['FIXED_PARAMETERS']:
             PA_plane =   np.zeros((len(Theta),len(Phi)))
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore",message="divide by zero encountered in true_divide"\
                                     ,category=RuntimeWarning)
+                warnings.filterwarnings("ignore",message="divide by zero encountered in divide"\
+                                    ,category=RuntimeWarning)
                 for i in range(len(Theta)):
                     PA_plane[:,i] = abs(np.arctan(np.sin(Theta[i])*np.tan(Phi[:]))*(360./(2*np.pi)))
 
             current_pa = abs(np.arctan(np.sin(Theta_in[:])*np.tan(Phi_in[:]))*(360./(2*np.pi)))
             current_diff = np.array([abs(x-current_pa[0]) for x in current_pa],dtype=float)
             not_flat = np.where(current_diff > 0.25)[0]
             if not_flat.size != 0:
@@ -333,99 +337,118 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+'This is for singular arrays not both sides'
+def calculate_change_angle(Configuration,Theta,Phi):
+    theta_zero = Theta[0]
+    phi_zero = Phi[0]
+       
+    theta_change= np.array([float(x-theta_zero) for x in Theta]\
+                           ,dtype=float)
+    
+    phi_change=  np.array([float(x-phi_zero) for x in Phi]\
+                           ,dtype=float)
+   
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore",message="invalid value encountered in true_divide"\
+                            ,category=RuntimeWarning)
+        #pYthon being really incredibly dumb again as changed the run time warning 
+        warnings.filterwarnings("ignore",message="invalid value encountered in divide"\
+                            ,category=RuntimeWarning)
+        theta_factor = np.sqrt(theta_change**2/(theta_change**2+phi_change**2))\
+                    *(theta_change)/abs(theta_change)
+        
+        theta_factor[np.where(np.array(theta_change) == 0.)] = 0.
+        phi_factor = np.sqrt(phi_change**2/(theta_change**2+phi_change**2))*(phi_change)/abs(phi_change)
+        phi_factor[np.where(np.array(phi_change) == 0.)] = 0.
+
+    in_zero = np.where(np.array(theta_change+phi_change) == 0.)
+    phi_factor[in_zero]=0.
+    theta_factor[in_zero]=0.
+
+    change_angle = np.sqrt(theta_change**2+phi_change**2)
+    change_angle[in_zero] =0.
+
+    return {'CHANGE_ANGLE': change_angle, 'PHI': {'ZERO': phi_zero, 'FACTOR':phi_factor},\
+                                     'THETA':{'ZERO': theta_zero, 'FACTOR':theta_factor}}
+
+def revert_change_angle(Configuration,change_angle):
+    new_theta = change_angle['THETA']['ZERO']+change_angle['CHANGE_ANGLE']\
+            *change_angle['THETA']['FACTOR']
+    new_phi =  change_angle['PHI']['ZERO']+change_angle['CHANGE_ANGLE']\
+            *change_angle['PHI']['FACTOR']
+    return new_theta,new_phi
 
 def check_angular_momentum_vector(Configuration,radius_in,pa_in,inclination_in,\
                                     modified= False,side=0):
 
     inclination = np.array(inclination_in)
     pa = np.array(pa_in)
     inclination_in = np.array(inclination_in)
     pa_in = np.array(pa_in)
     radius = np.array(radius_in,dtype=float)
     radkpc = convertskyangle(Configuration,radius)
     #radkpc = np.array([convertskyangle(Configuration,float(x)) for x in radius],dtype=float)
     #phi is dependent on theta but the max change should be the same
     max_shift = np.arctan(np.tan(Configuration['MAX_CHANGE']['INCL']*(np.pi/180.))\
                     *np.tan(Configuration['MAX_CHANGE']['PA']*(np.pi/180.)))
-    print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: The maximum allowed shift = {max_shift}.
+  
+    print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: The maximum allowed shift  = {max_shift}.
 ''',Configuration,case= ['debug_start'])
     succes = False
     counter = 0.
     while not succes:
-        print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: Calculating Phi and Theta from these PA and inclination
-PA = {pa}
-Inclination = {inclination}
-''',Configuration,case= ['debug_add'])
+        #print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: Calculating Phi and Theta from these PA and inclination
+#PA = {pa}
+#Inclination = {inclination}
+#''',Configuration,case= ['debug_add'])
         Theta,Phi,quadrant = calculate_am_vector(Configuration,pa,inclination )
-        theta_zero = Theta[0]
-        phi_zero = Phi[0]
-
-        #Let's combine the variation as fraction of the existing angle
-        theta_change= np.array([float(x-theta_zero) for x in Theta],dtype=float)
-        phi_change= np.array([float(x-phi_zero) for x in Phi],dtype=float)
-
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore",message="invalid value encountered in true_divide"\
-                                ,category=RuntimeWarning)
-            theta_factor = np.sqrt(theta_change**2/(theta_change**2+phi_change**2))\
-                        *(theta_change)/abs(theta_change)
-            theta_factor[np.where(np.array(theta_change) == 0.)] = 0.
-            phi_factor = np.sqrt(phi_change**2/(theta_change**2+phi_change**2))*(phi_change)/abs(phi_change)
-            phi_factor[np.where(np.array(phi_change) == 0.)] = 0.
-
-        in_zero = np.where(np.array(theta_change+phi_change) == 0.)
-        phi_factor[in_zero]=0.
-        theta_factor[in_zero]=0.
-
-        change_angle = np.sqrt(theta_change**2+phi_change**2)
-        change_angle[in_zero] =0.
-        new_change_angle = max_profile_change(Configuration,radkpc,change_angle,'ARBITRARY',\
-            slope = Configuration['WARP_SLOPE'][side],max_change=max_shift, kpc_radius=True )
-
-
-        new_theta_change = new_change_angle*theta_factor
-        new_phi_change = new_change_angle*phi_factor
-        new_theta = theta_zero+new_theta_change
-        new_phi = phi_zero+new_phi_change
-        print_log(f'''We put in the difference of
-phi {phi_change}, theta {theta_change}, angle {change_angle}
-new values
-phi {new_phi_change}, theta {new_theta_change}, angle {new_change_angle}
-''',Configuration,case= ['debug_add'])
-
+        change_angle = calculate_change_angle(Configuration,Theta,Phi) 
+        new_change_angle = max_profile_change(Configuration,radkpc,change_angle['CHANGE_ANGLE'],'CHANGE_ANGLE',\
+            slope = Configuration['WARP_SLOPE'][side],max_change=max_shift, kpc_radius=True, quadrant=quadrant )
+        
+        change_angle['CHANGE_ANGLE'] = new_change_angle
+        new_theta,new_phi = revert_change_angle(Configuration,change_angle)
+       
+     
         diff_phi = np.array(np.where(np.array([abs(x-y) for x,y in zip(Phi,new_phi) ],dtype=float) > 1e-6))
         diff_theta = np.array(np.where(np.array([abs(x-y) for x,y in zip(Theta,new_theta)],dtype=float) > 1e-6))
 
         if diff_phi.size != 0. or \
             diff_theta.size != 0.:
-            print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR
-{'':8s} Phi = {Phi}, new_phi = {new_phi}
-{'':8s} Phi diff = {np.array([abs(x-y) for x,y in zip(Phi,new_phi) ],dtype=float)}{'':8s}
-{'':8s} Theta = {Theta}, new_theta = {new_theta}
-{'':8s} Theta diff = {np.array([abs(x-y) for x,y in zip(Theta,new_theta) ],dtype=float)}
-''',Configuration,case= ['debug_add'])
+            #print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR
+#{'':8s} Phi = {Phi}, new_phi = {new_phi}
+#{'':8s} Phi diff = {np.array([abs(x-y) for x,y in zip(Phi,new_phi) ],dtype=float)}{'':8s}
+#{'':8s} Theta = {Theta}, new_theta = {new_theta}
+#{'':8s} Theta diff = {np.array([abs(x-y) for x,y in zip(Theta,new_theta) ],dtype=float)}
+#''',Configuration,case= ['debug_add'])
 
 
             pa,inclination = calculate_am_vector(Configuration,new_theta,new_phi,\
                                 multiple=quadrant,invert=True )
-            print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: new PA and inclination
-PA = {pa}
-Inclination = {inclination}
-''',Configuration,case= ['debug_add'])
+            # Because when the quadrant changes the PA and inclination are not checked against maximum variations 
+            # Hence this stille needs to be done
+            pa,inclination = check_quadrant_change(Configuration,pa,inclination,quadrant)
+            #for i in range(len(pa)):
+            #    print(f'PA = {pa[i]}, inclination = {inclination[i]}, quadrant = {quadrant[i]} ')
+#            print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: new PA and inclination
+#PA = {pa}
+#Inclination = {inclination}
+#''',Configuration,case= ['debug_add'])
             counter += 1
             if counter > 1000.:
                 #It is not really a succes but we have to exit the loop and one point.
                 succes = True
         else:
             succes = True
+        #exit()
 
     print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: Before checking we have modified = {modified}
 ''',Configuration,case= ['debug_add'])
     #if len(np.where(np.array([abs(x-y) for x,y in zip(pa_in,pa) ],dtype=float) != 0.)) != 0. or \
     #    len(np.where(np.array([abs(x-y) for x,y in zip(inclination_in,inclination) ],dtype=float) != 0.)) != 0.:
 
     if not np.isclose(pa_in,pa, atol=float(Configuration['MIN_ERROR']['PA'][0])*3.).any() or \
@@ -458,19 +481,61 @@
     modified = boolean indicating whether the PA and incl ave beet modfied.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
- NOTE:
+ NOTE: PA and inclination are singular sides
 '''
 
+def check_quadrant_change(Configuration,pa,inclination,quadrant):
+    diff_quadrant = [x -quadrant[0] for x in quadrant]
+    if np.sum(diff_quadrant) != 0.:
+        for i,x in enumerate(diff_quadrant):
+            if x != 0. and (1 < i <len(diff_quadrant)-1):
+                pa[i] = np.mean([pa[i-1],pa[i+1]]) 
+                inclination[i] = np.mean([inclination[i-1],inclination[i+1]])
+            elif i == len(diff_quadrant)-1:
+                pa[i] = pa[i-1]
+                inclination[i] = inclination[i-1]
+            else:
+                pass
+    return pa,inclination
+check_angular_momentum_vector.__doc__ =f'''
+ NAME:
+    check_angular_momentum_vector
 
+ PURPOSE:
+    Check the output warp by ensuring that the pa and inclination vary smoothly at the rings where the 
+    angular momentum is switching quadrants
+
+ CATEGORY:
+    support_functions
 
+ INPUTS:
+    Configuration = Standard Original FAT configuration
+    pa = PA of the model
+    inclination = inclination of the model
+    quadrants = the array that specifies the quadrants into which the am vector belongs
+
+ OPTIONAL INPUTS:
+   
+ OUTPUTS:
+    pa_new = the modfied PA
+    incl_new= the modified incl
+   
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE: PA and inclination are singular sides
+'''             
+        
 def check_sofia(Configuration,Fits_Files):
     files =['_mask.fits','_mom0.fits','_mom1.fits','_chan.fits','_mom2.fits','_cat.txt']
     for file in files:
         if os.path.exists(f'{Configuration["FITTING_DIR"]}Sofia_Output/{Configuration["BASE_NAME"]}{file}'):
             pass
         else:
             raise InputError()
@@ -559,15 +624,15 @@
 
 '''
 # clean the header
 def clean_header(Configuration,hdr_in,two_dim=False,mask_file=False):
     hdr = copy.deepcopy(hdr_in)
     print_log(f'''CLEAN_HEADER: Starting to clean the header.
 ''',Configuration,case= ['debug_start'])
-    keywords = ['CDELT','CUNIT','CRPIX','CRVAL','CTYPE']
+    keywords = ['CDELT','CUNIT','CRPIX','CRVAL','CTYPE','CROTA']
     for key in keywords:
         try:
             del hdr[f'{key}4']
         except KeyError:
             pass
     if not two_dim:
         hdr['NAXIS'] = 3
@@ -575,38 +640,64 @@
             if abs(hdr['CDELT3']) > 500:
                 hdr['CUNIT3'] = 'm/s'
             else:
                 hdr['CUNIT3'] = 'km/s'
             print_log(f'''CLEAN_HEADER:
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 Your header did not have a unit for the third axis, that is bad policy.
-{"":8s} We have set it to {hdr['CUNIT3']}. Please ensure that is correct.'
+{"":8s} We have set it to {hdr['CUNIT3']}. Please ensure that this is correct.'
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 ''',Configuration)
         if hdr['CUNIT3'].upper() == 'HZ' or hdr['CTYPE3'].upper() == 'FREQ':
             print_log('CLEAN_HEADER: FREQUENCY IS NOT A SUPPORTED VELOCITY AXIS.', Configuration, case=['main','screen'])
             raise BadHeaderError('The Cube has frequency as a velocity axis this is not supported')
 
-        vel_types = ['VELO-HEL','VELO-LSR','VELO', 'VELOCITY']
+        #vel_types = ['VELO-HEL','VELO-LSR','VELO', 'VELOCITY','VOPT','VRAD']
+        vel_types = ['VELO','VOPT','VRAD']
         if hdr['CTYPE3'].upper() not in vel_types:
             if hdr['CTYPE3'].split('-')[0].upper() in ['RA','DEC']:
                 print_log(f'''CLEAN_HEADER: Your zaxis is a spatial axis not a velocity axis.
 {"":8s}CLEAN_HEADER: Please arrange your cube logically
 ''',Configuration,case= ['main','screen'])
                 raise BadHeaderError("The Cube's third axis is not a velocity axis")
-            hdr['CTYPE3'] = 'VELO'
-            print_log(f'''CLEAN_HEADER: Your velocity projection is not standard. The keyword is changed to VELO (relativistic definition). This might be dangerous.
+            if hdr['CTYPE3'].split('-')[0].upper() == 'VELO':
+                frame = hdr['CTYPE3'].split('-')[1].upper()
+                hdr['CTYPE3'] = 'VELO'
+                if frame in ['LSR','LSRK']:
+                    hdr['SPECSYS3']='LSRK'
+                elif frame in ['HEL','HELO']:
+                    hdr['SPECSYS3']='HELIOCEN'
+            else:
+                print_log(f'''CLEAN_HEADER: Your velocity projection is not standard (CTYPE3 = {hdr["CTYPE3"]}). 
+Please note that FAT can only deal with velocity cubes, not frequency.
+''',Configuration, case=['main','screen'])
+                raise BadHeaderError(f'The Cube has a non-standard velocity projection (CTYPE3 = {hdr["CTYPE3"]})')
+        #Tirific will only run with VELO so if VRAD of VOPT then we need to run with VELO and fix it in the end
+        Configuration['HDR_VELOCITY'] = hdr['CTYPE3']
+        if  hdr['CTYPE3'].upper() in ['VRAD','VOPT']:
+            print_log(f'''CLEAN_HEADER: you are use a velocity type of {hdr['CTYPE3'].upper()} however tirific takes issue with this.
+As such we are replacing it with VELO before every tirific run. 
+!!!!!!!!!!!! ---- We are not converting anything so your fitting and all products are are of type {hdr['CTYPE3'].upper()}-------!!!!!!!!                                              
+''',Configuration)
+            #hdr['CTYPE3'] = 'VELO'
+
+        if 'SPECSYS3' not in hdr:
+            if 'SPECSYS' in hdr:
+                hdr['SPECSYS3'] = hdr['SPECSYS']
+            else:
+                print_log(f'''CLEAN_HEADER: There is no reference frame defined in your header. This is ok for FAT but WCS might complain.
 ''',Configuration)
 
         if hdr['CUNIT3'].lower() == 'km/s':
             print_log( f'''CLEAN_HEADER: The channels in your input cube are in km/s. This sometimes leads to problems with wcs lib, hence we change it to m/s.'
 ''',Configuration)
             hdr['CUNIT3'] = 'm/s'
             hdr['CDELT3'] = hdr['CDELT3']*1000.
             hdr['CRVAL3'] = hdr['CRVAL3']*1000.
+
         #because astropy is truly stupid
 
         if hdr['CUNIT3'] == 'M/S':
             hdr['CUNIT3'] = 'm/s'
 
     if not 'EPOCH' in hdr:
         if 'EQUINOX' in hdr:
@@ -635,20 +726,20 @@
             hdr['BMAJ']= hdr['BMMAJ']/3600.
         else:
             found = False
             if 'HISTORY' in hdr:
                 for line in hdr['HISTORY']:
                     tmp = [x.strip().upper() for x in line.split()]
                     if 'BMAJ=' in tmp:
-                        hdr['BMAJ'] = tmp[tmp.index('BMAJ=') + 1]
+                        hdr['BMAJ'] = float(tmp[tmp.index('BMAJ=') + 1])
                         found = True
                     if 'BMIN=' in tmp:
-                        hdr['BMIN'] = tmp[tmp.index('BMIN=') + 1]
+                        hdr['BMIN'] = float(tmp[tmp.index('BMIN=') + 1])
                     if 'BPA=' in tmp:
-                        hdr['BPA'] = tmp[tmp.index('BPA=') + 1]
+                        hdr['BPA'] = float(tmp[tmp.index('BPA=') + 1])
                     if found:
                         break
             if not found:
                 print_log(f'''CLEAN_HEADER: WE CANNOT FIND THE MAJOR AXIS FWHM IN THE HEADER
 ''',Configuration,case= ['main','screen'])
                 raise BadHeaderError("The Cube has no major axis FWHM in the header.")
     if not 'CTYPE1' in hdr or not 'CTYPE2' in hdr:
@@ -686,14 +777,21 @@
         if len(hdr['HISTORY']) > 10:
             del hdr['HISTORY']
             if Configuration:
                 print_log( f'''CLEAN_HEADER: Your cube has a significant history attached we are removing it for easier interpretation.
 ''',Configuration)
     except KeyError:
         pass
+    #The blank value only applies to integer value data
+    try:
+        if int(hdr['BITPIX']) != 16:
+            del hdr['BLANK']
+    except KeyError:
+        pass
+
     try:
         if abs(hdr['BMAJ']/hdr['CDELT1']) < 2:
             print_log( f'''CLEAN_HEADER: !!!!!!!!!!Your cube has less than two pixels per beam major axis.!!!!!!!!!!!!!!!!!
 {"":8s}CLEAN_HEADER: !!!!!!!!!!           This will lead to bad results.              !!!!!!!!!!!!!!!!'
 ''',Configuration)
 
         if abs(hdr['BMAJ']/hdr['CDELT1']) > hdr['NAXIS1']:
@@ -1261,15 +1359,15 @@
 
  NOTE:
 '''
 
 def ensure_list(variable):
     '''Make sure that variable is a list'''
     if not isinstance(variable,list):
-        if not isiterable(list1):
+        if not isiterable(variable):
             variable=[variable]
         else:
             variable=[x for x in variable]
     return variable
 ensure_list.__doc__ =f'''
  NAME:
     ensure_list
@@ -1302,15 +1400,15 @@
     while not found:
         try:
             run = subprocess.Popen([name], stdout = subprocess.PIPE, stderr = subprocess.PIPE)
             run.stdout.close()
             run.stderr.close()
             os.kill(run.pid, signal.SIGKILL)
             found = True
-        except FileNotFoundError:
+        except OSError:
             name = input(f'''You have indicated to use {name} for using {search} but it cannot be found.
 Please provide the correct name : ''')
     return name
 find_program.__doc__ =f'''
  NAME:
     find_program
 
@@ -1729,16 +1827,16 @@
 def get_fit_groups(Configuration,Tirific_Template):
     parameter_groups = []
     block = []
     rings = []
     groups = Tirific_Template['VARY'].split(',')
     variation_type = []
     variation = []
-    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
-    sbr_standard = np.mean(cut_off_limits) * 5.
+    cut_off_limits = sbr_limits(Configuration,Tirific_Template )
+    sbr_standard = np.mean(cut_off_limits) * 5. 
     paramater_standard_variation = {'PA': [10.,'a'],
                                    'INCL': [10.,'a'],
                                    'VROT': [Configuration['CHANNEL_WIDTH']*3.,'a'],
                                    'VSYS': [Configuration['CHANNEL_WIDTH'],'a'],
                                    'XPOS': [Configuration['BEAM'][0]/3600.,'a'],
                                    'YPOS': [Configuration['BEAM'][0]/3600.,'a'],
                                    'SBR': [sbr_standard,'a'],
@@ -1860,40 +1958,40 @@
     Unspecified
 
  EXAMPLE:
 
  NOTE:
 '''
 
-def get_inclination_pa(Configuration, Image, center, cutoff = 0.,\
-        figure_name = 'test'):
+def get_inclination_pa(Configuration, Image, center, cutoff = 0.):
     map = copy.deepcopy(Image[0].data)
     for i in [0,1]:
         print_log(f'''GET_INCLINATION_PA: Doing iteration {i} in the estimates
 ''',Configuration,case=['debug_start'])
         # now we need to get profiles under many angles let's say 100
         #extract the profiles under a set of angles
         angles = np.linspace(0, 360, 180)
         ratios, maj_extent = obtain_ratios(Configuration,map, center, angles,noise = cutoff)
         if np.any(np.isnan(ratios)):
             return [float('NaN'),float('NaN')],  [float('NaN'),float('NaN')],float('NaN')
         sin_ratios,sin_parameters = fit_sine(Configuration,angles,ratios)
         if np.any(np.isnan(sin_parameters)):
             return [float('NaN'),float('NaN')],  [float('NaN'),float('NaN')],float('NaN')
+        
         ratios=sin_ratios
 
         max_index = np.where(ratios == np.nanmax(ratios))[0]
         if max_index.size > 1:
             max_index =int(max_index[0])
         min_index = np.where(ratios == np.nanmin(ratios))[0]
-
         if min_index.size > 1:
             min_index =int(min_index[0])
-        max_index = set_limits(max_index,2,177)
-        min_index = set_limits(min_index,2,177)
+        #From here we know it is 1 value so lets set it to an integer    
+        max_index = set_limits(int(max_index),2,177)
+        min_index = set_limits(int(min_index),2,177)
 
         if min_index > 135 and max_index < 45:
             min_index=min_index-90
         if max_index > 135 and min_index < 45:
             max_index=max_index-90
         if i == 0:
             print_log(f'''GET_INCLINATION_PA: We initially find these indeces min {min_index } {angles[min_index]} max {max_index} {angles[max_index]}.
@@ -1907,15 +2005,15 @@
         tenp_min_index = np.where(ratios < np.nanmin(ratios)*1.1)[0]
 
         if tenp_max_index.size <= 1 and 2 <= max_index <=177 :
             tenp_max_index= [max_index-2,max_index+2]
 
         if tenp_min_index.size <= 1:
             tenp_min_index= [min_index-2,min_index+2]
-
+       
         if angles[min_index] > angles[max_index]:
             pa = float(np.nanmean(np.array([angles[min_index]-90,angles[max_index]],dtype=float)))
         else:
             pa = float(np.nanmean(np.array([angles[min_index]+90,angles[max_index]],dtype=float)))
         if 180. < pa:
             pa = pa -180
 
@@ -1932,15 +2030,15 @@
                             0.5,15.)
         ratios[ratios < 0.204] = 0.204
         ratios[1./ratios < 0.204] = 1./0.204
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             inclination = np.nanmean([np.degrees(np.arccos(np.sqrt((float(ratios[min_index])**2-0.2**2)/0.96))) \
                               ,np.degrees(np.arccos(np.sqrt(((1./float(ratios[max_index]))**2-0.2**2)/0.96))) ])
-
+          
 
         if i == 0:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 inclination_error = set_limits(np.nanmean([abs(np.degrees(np.arccos(np.sqrt((ratios[min_index]**2-0.2**2)/0.96))) - np.degrees(np.arccos(np.sqrt((ratios[tenp_min_index[0]]**2-0.2**2)/0.96)))),\
                                      abs(np.degrees(np.arccos(np.sqrt((ratios[min_index]**2-0.2**2)/0.96))) - np.degrees(np.arccos(np.sqrt((ratios[tenp_min_index[-1]]**2-0.2**2)/0.96)))),\
                                      abs(np.degrees(np.arccos(np.sqrt(((1./ratios[max_index])**2-0.2**2)/0.96))) - np.degrees(np.arccos(np.sqrt(((1./ratios[tenp_max_index[0]])**2-0.2**2)/0.96)))),\
@@ -1955,27 +2053,29 @@
                 inclination_error = float(inclination_error*0.4/(ratios[max_index]-ratios[min_index]))
         if maj_extent*3600./Configuration['BEAM'][0] < 4:
             inclination = float(inclination+(inclination/10.*np.sqrt(4./(maj_extent/Configuration['BEAM'][0]*3600.))))
             if i == 0:
                 inclination_error = float(inclination_error*4./(maj_extent*3600./Configuration['BEAM'][0]))
 
         if i == 0:
-            print_log(f'''GET_INCLINATION_PA: The initial inclination = {inclination}.
+            print_log(f'''GET_INCLINATION_PA: The initial inclination = {inclination} +- {inclination_error}.
 ''',Configuration,case=['debug_add'])
         else:
-            print_log(f'''GET_INCLINATION_PA: From the cleaned map we find inclination = {inclination}.
+            print_log(f'''GET_INCLINATION_PA: From the cleaned map we find inclination = {inclination}+- {inclination_error}.
 ''',Configuration,case=['debug_add'])
         # this leads to trouble for small sources due to uncertain PA and inclination estimates
-        if inclination < 70. and maj_extent*3600./Configuration['BEAM'][0] > 4:
+        # at low inclinations the error is too uncertain to have a proper deprojection    
+        inclination_error = inclination_error/np.sin(np.radians(inclination)) 
+        if inclination < 70. and maj_extent*3600./Configuration['BEAM'][0] > 4 and inclination_error < 10.:
             Image_clean = remove_inhomogeneities(Configuration,Image,inclination=inclination, pa = pa,iteration=i, center = center,WCS_center = False )
             map = Image_clean[0].data
             Image_clean.close()
         else:
             break
-    inclination_error = inclination_error/np.sin(np.radians(inclination))
+    
     return [inclination,inclination_error], [pa,pa_error],maj_extent
 
 get_inclination_pa.__doc__ =f'''
  NAME:
     get_inclination_pa
  PURPOSE:
     Get estimates for the PA, inclination and radius from a intensity map.
@@ -2189,66 +2289,14 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_ring_weights(Configuration,Tirific_Template):
-    print_log(f'''GET_RING_WEIGTHS: Getting the importance of the rings in terms of SBR.
-''',Configuration,case=['debug_start'])
-    sbr = load_tirific(Configuration,Tirific_Template,Variables=["SBR",f"SBR_2"],\
-                array=True )
-    print_log(f'''GET_RING_WEIGTHS: retrieve this sbr.
-{'':8s} sbr = {sbr}
-''',Configuration,case=['debug_add'])
-    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
-    print_log(f'''GET_RING_WEIGTHS: retrieved these cut_off_limits.
-{'':8s} col = {cut_off_limits}
-''',Configuration,case=['debug_add'])
-    weights= [[],[]]
-    for i in [0,1]:
-        weights[i] = [set_limits(x/y,0.1,10.) for x,y in zip(sbr[i],cut_off_limits)]
-        weights[i] = weights[i]/np.nanmax(weights[i])
-        weights[i][0:2] = np.nanmin(weights[i])
-        weights[i] = [set_limits(x,0.1,1.) for x in weights[i]]
-    print_log(f'''GET_RING_WEIGTHS: Obtained the following weights.
-{'':8s}{weights}
-''',Configuration,case=['debug_add'])
-    return np.array(weights,dtype = float)
-
-get_ring_weights.__doc__=f'''
- NAME:
-    get_ring_weights
-
- PURPOSE:
-    Get the importance of the rings based on how much the SBR lies above the noise limit for each ring
-
- CATEGORY:
-    support_functions
-
- INPUTS:
-    Configuration = Standard FAT configuration
-    Tirific_Template = Standard Tirific template containg the SBR profiles
-
- OPTIONAL INPUTS:
-
-
- OUTPUTS:
-    numpy array with the weight normalized to the the maximum.
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-    Weight 1 is most important, weight 0. least important.
-    Errors should be divided by these weights to reflect the importance
-'''
 
 def get_system_string(string):
     '''Escape any spaces in string with backlash'''
     if len(string.split()) > 1:
         string = "\ ".join(string.split())
     return string
 get_system_string.__doc__=f'''
@@ -2273,23 +2321,28 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-def get_tirific_output_names(Configuration,work_dir,deffile):
+def get_tirific_output_names(Configuration,work_dir,deffile,shaker=False):
     print_log(f'''GET_TIRIFIC_OUTPUT_NAMES: Starting the extraction of the output names in {deffile} tot be ran in {work_dir})
 ''',Configuration,case=['debug_start'])
 
     fitsfile,deffile = load_tirific(Configuration,f'{work_dir}/{deffile}' ,\
         Variables=['OUTSET','TIRDEF'])
-    output_fits = f'{work_dir}/{fitsfile[0]}'
     output_deffile = f'{work_dir}/{deffile[0]}'
+    #Tirshakerdoes not produce the fits outset
+    if not shaker:   
+        output_fits = f'{work_dir}/{fitsfile[0]}'
+    else:
+        output_fits = f'{work_dir}/{deffile[0]}'
     return output_fits,output_deffile
+    
 get_tirific_output_names.__doc__=f'''
  NAME:
     get_tirific_output_names
 
  PURPOSE:
     get the  name of the output fits file and def file as defined in the running directory + deffile
 
@@ -2313,52 +2366,14 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_usage_statistics(Configuration,process):
-    #try:
-    memory_in_mb = (process.memory_info()[0])/2**20. #psutilreturns bytes
-    cpu_percent = process.cpu_percent(interval=1)
-    #except:
-    #    cpu_percent= 0.
-    #    memory_in_mb=0.
-    return cpu_percent,memory_in_mb
-
-get_usage_statistics.__doc__ =f'''
- NAME:
-    get_usage_statistics
- PURPOSE:
-    use psutil to get the current CPU and memory usage of tirific
-
- CATEGORY:
-    support_functions
-
- INPUTS:
-    Configuration = Standard FAT configuration
-    process_id = process id of the tirific currently running.
-
- OPTIONAL INPUTS:
-
-
- OUTPUTS:
-    CPU = The current CPU usage
-    mem = current memory usage in Mb
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-    pyFAT version < 1.0.0 uses top which only works on unix and has an error in the MB calculation
-'''
-
 def get_vel_pa(Configuration,velocity_field,center= [0.,0.] ):
     print_log(f'''GET_VEL_PA: This is the center we use {center}
 ''',Configuration,case=['debug_start'])
     if center == None:
         center = [x/2. for x in velocity_field.shape]
     else:
          # because python is stupid the ceneter should be reversed to match the map
@@ -2504,87 +2519,33 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-
-
-# A simple function to return the line numbers in the stack from where the functions are called
-def linenumber(debug='short'):
-    '''get the line number of the print statement in the main.'''
-    line = []
-    for key in stack():
-        if key[1] == 'main.py':
-            break
-        if key[3] != 'linenumber' and key[3] != 'print_log' and key[3] != '<module>':
-            file = key[1].split('/')
-            to_add= f"In the function {key[3]} at line {key[2]}"
-            if debug == 'long':
-                to_add = f"{to_add} in file {file[-1]}."
-            else:
-                to_add = f"{to_add}."
-            line.append(to_add)
-    if len(line) > 0:
-        if debug == 'long':
-            line = ', '.join(line)+f'\n{"":8s}'
-        elif debug == 'short':
-            line = line[0]+f'\n{"":8s}'
-        else:
-            line = f'{"":8s}'
-    else:
-        for key in stack():
-            if key[1] == 'main.py':
-                line = f"{'('+str(key[2])+')':8s}"
-                break
-    return line
-
-linenumber.__doc__ =f'''
- NAME:
-    linenumber
-
- PURPOSE:
-    get the line number of the print statement in the main. Not sure how well this is currently working
-
- CATEGORY:
-    support_functions
-
- INPUTS:
-
- OPTIONAL INPUTS:
-
-
- OUTPUTS:
-    the line number of the print statement
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-    If debug = True the full stack of the line print will be given, in principle
-    the first debug message in every function should set this to true and later messages not.
-    !!!!Not sure whether currently the linenumber is produced due to the restructuring.
-'''
-
 #The functions load_tirifiic,load_template and get_from template were extremely similar
 #This replaces all with a single function
 def load_tirific(Configuration,def_input,Variables = None,array = False,\
-        ensure_rings = False ):
+        ensure_rings = False,brightness_check=False ):
     #Cause python is the dumbest and mutable objects in the FAT_defaults
     # such as lists transfer
     if Variables is None:
         Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI',\
                      'VROT','Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS',\
                      'SDIS','VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','XPOS_2',\
                      'YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2']
-
-
+    sbr_added =[False,False]
+    if brightness_check:
+        if 'SBR' not in Variables:
+            Variables.append('SBR')
+            sbr_added[0] =True
+        if 'SBR_2' not in Variables:
+            Variables.append('SBR_2')
+            sbr_added[1] =True
     # if the input is a string we first load the template
     if isinstance(def_input,str):
         def_input = tirific_template(filename = def_input )
 
     out = []
     for key in Variables:
         try:
@@ -2605,14 +2566,28 @@
             #or just take the longest input as the size
             length = max(map(len,out))
         #let's just order this in variable, values such that it unpacks properly into a list of variables
         out = np.zeros((len(Variables),length),dtype=float)
         for i,variable in enumerate(tmp):
             if len(variable) > 0.:
                 out[i,0:len(variable)] = variable[0:len(variable)]
+    if brightness_check:
+        for variable in Variables:
+            tmp = variable.split('_')
+            ext=''
+            if tmp[-1] == '2':
+                ext = '_2'
+            elif tmp[-1] == 'ERR':
+                if tmp[-2] == 2:
+                   ext = '_2'  
+           
+            cut = np.where(out[Variables.index(f'SBR{ext}'),:] < 1e-15)
+            if np.sum(cut) > 0.:
+                out[Variables.index(variable),cut] = float('NaN')
+        
 
     if len(Variables) == 1:
         out= out[0]
     print_log(f'''LOAD_TIRIFIC: We extracted the following profiles from the Template.
 {'':8s}Requested Variables = {Variables}
 {'':8s}Extracted = {out}
 ''',Configuration,case=['debug_start'])
@@ -2708,17 +2683,15 @@
 
 
 def make_tiltogram(Configuration,Tirific_Template):
     print_log(f'''MAKE_TILTOGRAM: Starting tiltogram.
 ''',Configuration,case=['debug_start'])
     pa_incl = load_tirific(Configuration,Tirific_Template,\
             Variables=['PA','PA_2','INCL','INCL_2'],array=True)
-    sbr = load_tirific(Configuration,Tirific_Template,Variables=["SBR",f"SBR_2"]\
-            ,array=True)
-    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
+
     add = [[],[]]
     Theta = [[],[]]
     phi = [[],[]]
     x = [[],[]]
     y = [[],[]]
     z = [[],[]]
     tiltogram = [[],[]]
@@ -2775,69 +2748,99 @@
  NOTE:
 
 '''
 
 
 
 def max_profile_change(Configuration,radius,profile,key,max_change=None,\
-                        slope = None, kpc_radius=False):
+                        slope = None, kpc_radius=False , quadrant = None):
     if not kpc_radius:
         radkpc = convertskyangle(Configuration,radius)
     else:
         radkpc = copy.deepcopy(radius)
     new_profile = copy.deepcopy(profile)
-    sm_profile = savgol_filter(profile, 3, 1)
-    if key == 'ARBITRARY' and not max_change:
-        raise InputError('For arbitrary checks you have to set the max_change.')
-    if key != 'ARBITRARY':
+  
+    sm_profile = savgol_filter(new_profile, 3, 1)
+    if key in ['ARBITRARY','CHANGE_ANGLE'] and not max_change:
+        raise InputError(f'For {key} checks you have to set the max_change.')
+    if max_change == None:
         max_change=Configuration['MAX_CHANGE'][key]
     diff_rad =  [float(y-x) for x,y in zip(radkpc,radkpc[1:])]
     diff_profile = [float(y-x) for x,y in zip(profile,profile[1:])]
     diff_sm_profile = [float(y-x) for x,y in zip(sm_profile,sm_profile[1:])]
+    if quadrant is None:
+        diff_q = np.zeros(len(diff_profile))
+    else:
+        diff_q = [float(y-x) for x,y in zip(quadrant,quadrant[1:])]
+
     print_log(f'''MAX_CHANGE_PROFILE: The profile {key} starts with.
 {'':8s} {key} = {new_profile} and max change = {max_change}
 {'':8s} smoothed {key}  = {sm_profile}
 {'':8s} diff per ring = {diff_profile}
 {'':8s} smoothed dif per ring = {diff_sm_profile}
 {'':8s} slope = {slope}
 {'':8s} diff/kpc = {[x/y for x,y in zip(diff_profile,diff_rad)]}
 ''', Configuration,case=['debug_start'])
-
+    #print(f''' For the PA and the inlcination we get a max shift per ring
+    #PA = {[Configuration['MAX_CHANGE']['PA']*y for x,y in zip(diff_profile,diff_rad)]}   
+    #INCL =  {[Configuration['MAX_CHANGE']['INCL']*y for x,y in zip(diff_profile,diff_rad)]}            
+    #          ''')
+    #    exit()
     for i,diff in enumerate(diff_profile):
-        if abs(diff)/diff_rad[i] > max_change:
+        if abs(diff)/diff_rad[i] > max_change and diff_q[i] == 0.:
+            print_log(f'''MAX_CHANGE_PROFILE: for ring {i} with {new_profile[i+1]} we find the difference {diff/diff_rad[i]}
+''', Configuration,case=['debug_add'])
             #if it is the last point we simply limit it
             if i == len(diff_profile)-1:
-                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.5*diff_rad[i])
+                new_profile[i+1] = new_profile[i]+ diff/abs(diff)*(max_change*0.5*diff_rad[i])
+                #print_log(f'''MAX_CHANGE_PROFILE: This is the last ring putting {new_profile[i+1] }.
+#''', Configuration,case=['debug_add'])
             elif i+1 == slope:
                 # if we have the start of the slope on the max_change then put it to value of the previous ring
                 new_profile[i+1] = new_profile[i]
-            elif diff_sm_profile[i]/diff_rad[i] < max_change*0.5:
+                print_log(f'''MAX_CHANGE_PROFILE: This is the start of the slope putting {new_profile[i+1] }.
+''', Configuration,case=['debug_add'])
+            elif abs(diff_sm_profile[i])/diff_rad[i] < max_change*0.5:
                 new_profile[i+1] = sm_profile[i+1]
+                print_log(f'''MAX_CHANGE_PROFILE: The smoothed profile is acceptable using {new_profile[i+1] }.
+''', Configuration,case=['debug_add'])
+                sm_profile = savgol_filter(new_profile, 3, 1)
+                diff_sm_profile = [float(y-x) for x,y in zip(sm_profile,sm_profile[1:])]
             elif diff_profile[i+1] == 0:
-                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i]) 
+                print_log(f'''MAX_CHANGE_PROFILE: The next ring is the same using {new_profile[i+1] }.
+''', Configuration,case=['debug_add'])
                 #If the change does not reverse we simply limit
             elif diff/abs(diff) == diff_profile[i+1]/abs(diff_profile[i+1]):
-                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+                new_profile[i+1] = new_profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+                print_log(f'''MAX_CHANGE_PROFILE: We are simply applying the maximum change using {new_profile[i+1] }.
+''', Configuration,case=['debug_add'])
             else:
                 if abs(diff) > abs(diff_profile[i+1]):
                     gapped_diff = radkpc[i+2] - radkpc[i]
                     if abs(new_profile[i]-new_profile[i+2])/gapped_diff < max_change:
                         new_profile[i+1] = np.mean([new_profile[i],new_profile[i+2]])
                     else:
                         new_profile[i+1] = new_profile[i]
+                    print_log(f'''MAX_CHANGE_PROFILE: Bridged the gap using {new_profile[i+1] }.
+''', Configuration,case=['debug_add'])
                 else:
 
-                    new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+                    new_profile[i+1] = new_profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
 
             if i < len(diff_profile)-1:
                 diff_profile[i+1] = float(new_profile[i+2]-new_profile[i+1])
 
     print_log(f'''MAX_CHANGE_PROFILE: The returned profile is:
 {'':8s}{key} = {new_profile}
 ''', Configuration,case=['debug_add'])
+    #for i,diff in enumerate([float(y-x) for x,y in zip(new_profile,new_profile[1:])]):
+    #    print(f'The change {diff} allowed {max_change*diff_rad[i]}')
+    #
+    #exit()
     return new_profile
 max_profile_change.__doc__ =f'''
  NAME:
      max_profile_change
 
  PURPOSE:
     Check that the profile is not change more than the maximum per kpc and correct if it does
@@ -2860,14 +2863,15 @@
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
+    Currently this function is only applied to the angular momentum vector
 
 '''
 
 
 def obtain_border_pix(Configuration,angle,center):
     rotate = False
     # only setup for 0-180 but 180.-360 is the same but -180
@@ -3018,74 +3022,14 @@
 
  PROCEDURES CALLED:
       np.mean, ndimage.map_coordinates, np.linspace, np.vstack, np.cos, np.radians, np.sin
 
  NOTE:
 '''
 
-def print_log(log_statement,Configuration, case = None):
-    if case is None:
-        case=['main']
-    if Configuration['DEBUG']:
-        if 'debug_start' in case:
-            debug = 'long'
-        else:
-            debug= 'short'
-    else:
-        debug = 'empty'
-    if Configuration['TIMING']:
-        log_statement = f"{linenumber(debug=debug)} {datetime.now()} {log_statement}"
-    else:
-        log_statement = f"{linenumber(debug=debug)}{log_statement}"
-    print_statement = False
-    if (Configuration['DEBUG'] and ('debug_start' in case or 'debug_add' in case))\
-        or ('verbose' in case and (Configuration['VERBOSE_LOG'] or Configuration['DEBUG']))\
-         or 'main' in case:
-            print_statement = True
-    if print_statement:
-        if Configuration['VERBOSE_SCREEN'] \
-            or not Configuration['OUTPUTLOG']  \
-            or 'screen' in case \
-            or (Configuration['VERBOSE_LOG'] and 'main' in case):
-            print(log_statement)
-        if Configuration['OUTPUTLOG']:
-            with open(Configuration['OUTPUTLOG'],'a') as log_file:
-                log_file.write(log_statement)
-
-print_log.__doc__ =f'''
- NAME:
-    print_log
- PURPOSE:
-    Print statements to log if existent and screen if Requested
- CATEGORY:
-    support_functions
-
- INPUTS:
-    log_statement = statement to be printed
-    Configuration = Standard FAT Configuration
-
- OPTIONAL INPUTS:
-
-
-    screen = False
-    also print the statement to the screen
-
- OUTPUTS:
-    line in the log or on the screen
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    linenumber, .write
-
- NOTE:
-    If the log is None messages are printed to the screen.
-    This is useful for testing functions.
-'''
-
 def remove_inhomogeneities(Configuration,fits_map_in,inclination=30., pa = 90.\
         ,center = None, WCS_center = True, iteration= 0 ):
     if center is None:
         center = [0.,0.]
     fits_map = copy.deepcopy(fits_map_in)
     print_log(f'''REMOVE_INHOMOGENEITIES: These are the values we get as input
 {'':8s}Inclination = {inclination}
@@ -3191,15 +3135,15 @@
                 if stage in ['run_ec','run_os','run_cc']:
                     Loopnr = f"Iteration_{Configuration['ITERATIONS']-1}"
                 elif stage in ['after_cc','after_ec','after_os'] :
                     Loopnr = f"Iteration_{Configuration['ITERATIONS']}"
                 elif fit_type == Configuration['USED_FITTING'] and stage in ['final_os']:
                     Loopnr = f"Smoothed_1"
                 else:
-                    Loopnr = 'Output_before_'+stage
+                    Loopnr = 'Output_Before_'+stage
                 if os.path.exists(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.{filetype}"):
                     target = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_{Loopnr}.{filetype}")
                     os.system(f"mv {source} {target}")
 
             elif os.path.exists(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.{filetype}"):
                 target = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Prev.{filetype}")
                 os.system(f"mv {source} {target}")
@@ -3271,16 +3215,16 @@
     Unspecified
 
  NOTE:
 '''
 
 
 def run_tirific(Configuration, current_run, stage = 'initial',\
-        fit_type = 'Undefined',deffile='Undefined'):
-    print_log(f'''RUN_TIRIFIC: For the galaxy {Configuration['ID']} in directory {Configuration['SUB_DIR']} we are starting a new TiRiFiC.
+        fit_type = 'Undefined',deffile='Undefined',max_ini_time = 600):
+    print_log(f'''RUN_TIRIFIC: For the galaxy {Configuration['ID']} in directory {Configuration['SUB_DIR']} we are starting a RUN_TIRIFIC.
 We are in in stage {stage} and fit_type {fit_type} and have done {Configuration['ITERATIONS']} loops
 ''',Configuration,case=['debug_start'])
     if deffile == 'Undefined':
         deffile=f"{fit_type}_In.def"
 
     # First move the previous fits
     rename_fit_products(Configuration,fit_type = fit_type, stage=stage )
@@ -3288,28 +3232,31 @@
     if Configuration['DEBUG']:
         if stage == 'run_os':
             write_config(
                 f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Iteration_{Configuration["ITERATIONS"]}.txt', Configuration)
     if fit_type == 'Error_Shaker':
         work_dir = os.getcwd()
         restart_file = f"restart_Error_Shaker.txt"
+        shaker = True
     else:
         restart_file = f"{Configuration['LOG_DIRECTORY']}restart_{fit_type}.txt"
         work_dir = Configuration['FITTING_DIR']
+        shaker = False
     #Get the output fits file and def file defined in workdir+ deffile
-    output_fits,output_deffile = get_tirific_output_names(Configuration,work_dir,deffile )
+    output_fits,output_deffile = get_tirific_output_names(Configuration,work_dir,deffile\
+                                ,shaker=shaker )
     # Then if already running change restart file
     if Configuration['TIRIFIC_RUNNING']:
         print_log(f'''RUN_TIRIFIC: We are using an initialized tirific in {Configuration['FITTING_DIR']} with the file {deffile}
 ''',Configuration)
 
         with open(restart_file,'a') as file:
             file.write("Restarting from previous run \n")
     else:
-        print_log(f'''RUN_TIRIFIC: We are starting a new TiRiFiC in {Configuration['FITTING_DIR']} with the file {deffile}
+        print_log(f'''RUN_TIRIFIC: We are inizializing a new TiRiFiC in {Configuration['FITTING_DIR']} with the file {deffile}
 ''',Configuration)
         with open(restart_file,'w') as file:
             file.write("Initialized a new run \n")
         current_run = subprocess.Popen([Configuration['TIRIFIC'],f"DEFFILE={deffile}","ACTION= 1"],\
                                        stdout = subprocess.PIPE, stderr = subprocess.PIPE,\
                                        cwd=work_dir,universal_newlines = True)
 
@@ -3340,36 +3287,40 @@
         counter += 1
         if (counter % 50) == 0:
             if Configuration['TIMING']:
                 with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
                     if tmp[0] == 'L' and not triggered:
                         if tmp[1] == '1':
                             file.write(f"# TIRIFIC: Started the actual fitting {datetime.now()} \n")
-                            triggered = True
                     CPU,mem = get_usage_statistics(Configuration,current_process)
                     file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for TiRiFiC \n")
         if tmp[0] == 'L':
+            if not triggered:
+                triggered = True
             if int(tmp[1]) != currentloop and Configuration['VERBOSE_SCREEN']:
                 print(f"\r{'':8s}RUN_TIRIFIC: {set_limits(float(tmp[1])-1.,0.,float(max_loop))/float(max_loop)*100.:.1f} % Completed", end =" ",flush = True)
             currentloop  = int(tmp[1])
             if max_loop == 0:
                 max_loop = int(tmp[2])
-
             Configuration['NO_POINTSOURCES'] = np.array([tmp[18],tmp[19]],dtype=float)
 
         if tmp[0].strip() == 'Finished':
             break
         if tmp[0].strip() == 'Abort':
             break
         if not triggered:
             #Check that the initialization doesn't take to long
             check = datetime.now()
             diff = (check-initialized).total_seconds()
-            if diff > 600:
-                raise TirificOutputError(f'''10 minutes after initialization the fitting has still not started.
+            if diff > max_ini_time:
+                print_log(f'''RUN_TIRIFIC: After {diff/60.} min we could not find the expected output from the tirific run. 
+running in the directory = {work_dir} 
+and the file deffile = {deffile}                         
+''',Configuration,case=['main','screen'])
+                raise TirificOutputError(f'''{diff/60.} minutes after initialization the fitting has still not started.
 We were running {deffile} and failed to find the output {output_fits} or {output_deffile}.
 ''')
     if Configuration['VERBOSE_SCREEN']:
         print(f'\n')
     if Configuration['TIMING']:
         with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
             file.write(f"# TIRIFIC: Finished this run {datetime.now()} \n")
@@ -3385,22 +3336,26 @@
         while not os.path.exists(output_fits) and wait_counter < 100.:
             time.sleep(0.3)
             wait_counter += 1
             if wait_counter/10. == int(wait_counter/10.):
                 print(f"\r Waiting for {output_fits}. \n", end = "", flush = True)
                 print_log(f'''RUN_TIRIFIC: we have waited {0.3*wait_counter} seconds for the output of tirific but it is not there yet.
 ''',Configuration)
-        if not  os.path.exists(output_fits) \
+        if not os.path.exists(output_fits) \
             or not  os.path.exists(output_deffile):
             print_log(f'''RUN_TIRIFIC: After 30 seconds we could not find the expected output from the tirific run. We are raising an error for this galaxy.
 ''',Configuration,case=['main','screen'])
             raise TirificOutputError(f'''The tirific subprocess did not produce the correct output, most likely it crashed.
 We were running {deffile} and failed to find the output {output_fits} or {output_deffile}.
 ''')
-
+    #If we are running tirific with an incorrect velocity type we should addapt the velocity type of the output
+    if Configuration['HDR_VELOCITY'] != 'VELO':
+        cube = fits.open(output_fits)
+        cube[0].header['CTYPE3'] = Configuration['HDR_VELOCITY']
+        fits.writeto(output_fits,cube[0].data,cube[0].header,overwrite=True)
     if currentloop != max_loop:
         return 1,current_run
     else:
         return 0,current_run
 run_tirific.__doc__ =f'''
  NAME:
     run_tirific
@@ -3420,14 +3375,18 @@
 
     fit_type = 'Undefined'
     type of fitting
 
     stage = 'initial'
     stage of the fitting process
 
+    max_ini_time = 600
+    maximum time it can take for tirific to initialize 
+    Higher ini times take longer
+
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
@@ -3516,16 +3475,18 @@
             Configuration['SOFIA_BASENAME'] = Configuration['BASE_NAME']
     #Add our fitting directory to the Configuration
     #Maindir always ends in slash already
     if Full_Catalogue['DIRECTORYNAME'][current_galaxy_index] == './':
         Configuration['FITTING_DIR'] = f"{Configuration['MAIN_DIRECTORY']}"
     else:
         Configuration['FITTING_DIR'] = f"{Configuration['MAIN_DIRECTORY']}{Full_Catalogue['DIRECTORYNAME'][current_galaxy_index]}/"
-
-    Configuration['INPUT_CUBE']= f"{Full_Catalogue['CUBENAME'][current_galaxy_index]}.fits"
+    if 'sofia_catalogue' in Configuration['FITTING_STAGES']:
+        Configuration['INPUT_CUBE']= f"{Full_Catalogue['CUBENAME'][current_galaxy_index]}_FAT.fits"
+    else:        
+        Configuration['INPUT_CUBE']= f"{Full_Catalogue['CUBENAME'][current_galaxy_index]}.fits"
     return(Configuration)
 set_individual_configuration.__doc__ =f'''
  NAME:
     set_individual_configuration
 
  PURPOSE:
     Fill the parameters of the configuration file that come from the catalogue
@@ -3556,18 +3517,22 @@
 
 #Function to read FAT configuration file into a dictionary
 def setup_configuration(cfg):
     if cfg.installation_check:
         cfg.fitting.fixed_parameters=['INCL','PA','SDIS']
         cfg.advanced.max_iterations= 1
         cfg.advanced.loops= 1
+        cfg.advanced.shaker_iterations = 2
         cfg.input.main_directory= f'{cfg.input.main_directory}/FAT_Installation_Check/'
         cfg.output.output_quantity = 0
-        cfg.fitting.fitting_stages = ['Create_FAT_Cube','Run_Sofia','Fit_Tirific_OSC']
+        cfg.fitting.fitting_stages = ['Create_FAT_Cube','Run_Sofia','Fit_Tirific_OSC','Tirshaker']
+        #cfg.fitting.fitting_stages = ['Create_FAT_Cube','Run_Sofia','Fit_Tirific_OSC']
         cfg.cube_name = 'NGC_2903.fits'
+        #cfg.output.debug = False
+        cfg.output.timing = True
         test_files = ['NGC_2903.fits','ModelInput.def']
         if not os.path.isdir(cfg.input.main_directory):
             os.mkdir(cfg.input.main_directory)
         else:
             for file in test_files:
                 try:
                     os.remove(f'{cfg.input.main_directory}/{file}')
@@ -3650,21 +3615,22 @@
                'SOFIA_TIME': ['Not started','Not completed'],
                'INITIAL_GUESSES_TIME': ['Not started','Not completed'],
                'FIT_TIME': ['Not started','Not completed'],
                'TIRSHAKER_TIME': ['Not started','Not completed'],
                'OUTPUTLOG': None,
                'RUN_COUNTER': 0,
                'CENTRAL_CONVERGENCE_COUNTER': 1.,
+               'RP_COUNTER': 1,
                'ITERATIONS': 0,
                'CURRENT_STAGE': 'initial', #Current stage of the fitting process, set at switiching stages
                'USED_FITTING': None,
                'TIRIFIC_PID': 'Not Initialized', #Process ID of tirific that is running
                'FAT_PID': os.getpid(), #Process ID of FAT that is running
                'FAT_PSUPROCESS': 'cant copy',
-               'FINAL_COMMENT': "This fitting stopped with an unregistered exit.", 
+               'FINAL_COMMENT': "This fitting stopped with an unregistered exit.",
 
                'MAX_SIZE_IN_BEAMS': 30, # The galaxy is not allowed to extend beyond this number of beams in radius, set in check_source
                'MIN_SIZE_IN_BEAMS': 0., # Minimum allowed radius in number of beams of the galaxy, set in check_source
                'SIZE_IN_BEAMS': np.full(2,0.,dtype=float),  #The radius of the galaxy in number of beams, adapted after running Sofia
                'NO_RINGS': 0., # The number of rings in the fit,
                'LAST_RELIABLE_RINGS': [0.,0.], # Location of the rings where the SBR drops below the cutoff limits, adapted after every run. Should only be modified in check_size
                'LIMIT_MODIFIER': [1.], #Modifier for the cutoff limits based on the inclination , adapted after every run.
@@ -3679,14 +3645,16 @@
                'RC_UNRELIABLE': 1, # Ring number from where the RC values are set flat. Should only be set in check_size
 
                'NOISE': 0. , #Noise of the input cube in Jy/beam, set in read_cube
                'SNR': 0, # the mean SNR in the moment 0 map sofia mask these are set in guess_orientation
                'BEAM_IN_PIXELS': [0.,0.,0.], #FWHM BMAJ, BMIN in pixels and total number of pixels in beam area, set in read_cube in read_functions
                'BEAM': [0.,0.,0.], #  FWHM BMAJ, BMIN in arcsec and BPA, set in main
                'BEAM_AREA': 0., #BEAM_AREA in arcsec set in main
+               'HDR_VELOCITY': 'VELO', #Track the velocity frame as tirific will only run with VELO
+               'TIR_RUN_CUBE': None, # if the type of velocity axis is not VELO we need to run on a cube with that key word adjusted.
                'NAXES': [0.,0.,0.], #  Size of the cube in pixels x,y,z arranged like sane people not python, set in main
                'MAX_ERROR': {}, #The maximum allowed errors for the parameters, set in main derived from cube
                'MIN_ERROR': {}, #The minumum allowed errors for the parameters, initially set in check_source but can be modified through out INCL,PA,SDSIS,Z0 errors change when the parameters is fixed or release
                'MAX_CHANGE': {'INCL': 6.25, 'PA': 25.}, #The maximum change in a parameter in unit/kpc
                'CHANNEL_WIDTH': 0., #Width of the channel in the cube in km/s, set in main derived from cube
                'PIXEL_SIZE': 0., #'Size of the pixels in degree'
                }
@@ -3717,14 +3685,15 @@
 
     while not os.path.isdir(Configuration['MAIN_DIRECTORY']):
         Configuration['MAIN_DIRECTORY'] = input(f'''
 Your main fitting directory ({Configuration['MAIN_DIRECTORY']}) does not exist.
 Please provide the correct directory.
 :  ''')
 
+
     if Configuration['CATALOGUE']:
         if not os.path.exists(Configuration['CATALOGUE']) and len(Configuration['CATALOGUE'].split('/')) == 1:
             Configuration['CATALOGUE']= f'''{Configuration['MAIN_DIRECTORY']}{Configuration['CATALOGUE']}'''
 
         while not os.path.exists(Configuration['CATALOGUE']):
             Configuration['CATALOGUE'] = input(f'''
 Your input catalogue ({Configuration['CATALOGUE']}) does not exist.
@@ -3753,25 +3722,37 @@
 
 
         if fit_count > 1 and 'fit_' in stage.lower():
             print(f''' FAT only supports one single fitting stage. You have already selected one and hence {stage} will be ignored.
     ''')
         else:
             approved_stages.append(stage.lower())
+    if Configuration['DEBUG']:
+        Configuration['DEBUG_FUNCTION'] = [x.upper() for x in \
+                                        Configuration['DEBUG_FUNCTION']]
 
     Configuration['FITTING_STAGES'] =approved_stages
     if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'external_sofia' in Configuration['FITTING_STAGES']:
         Configuration['FITTING_STAGES'].remove('external_sofia')
     if ('sofia_catalogue' in Configuration['FITTING_STAGES'] or 'external_sofia' in Configuration['FITTING_STAGES']) and 'run_sofia' in Configuration['FITTING_STAGES']:
         Configuration['FITTING_STAGES'].remove('run_sofia')
-    if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'create_fat_cube' in Configuration['FITTING_STAGES']:
-        Configuration['FITTING_STAGES'].remove('create_fat_cube')
+    #if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'create_fat_cube' in Configuration['FITTING_STAGES']:
+    #    Configuration['FITTING_STAGES'].remove('create_fat_cube')
+    if 'sofia_catalogue' in Configuration['FITTING_STAGES']:
+        if Configuration['SOFIA_DIR'][-1] != '/':
+            Configuration['SOFIA_DIR'] = f"{Configuration['SOFIA_DIR']}/"
+
+  
+
 
     if 'run_sofia' in Configuration['FITTING_STAGES'] and 'external_sofia' in Configuration['FITTING_STAGES']:
         raise InputError(f"You are both providing existing sofia input and ask for sofia to be ran. This won't work exiting.")
+    if 'fit_tirific_osc' in Configuration['FITTING_STAGES'] and \
+        Configuration['NUMBER_OF_DISKS'] > 2:
+        raise InputError(f"Fit_Tirific_OSC only allows for 2 or 1 disk. This won't work exiting.")
 
     #Check that the channel_dependency is acceptable
     while Configuration['CHANNEL_DEPENDENCY'].lower() not in ['sinusoidal','independent','hanning']:
         Configuration['CHANNEL_DEPENDENCY'] = input(f'''
 The channel dependency  {'CHANNEL_DEPENDENCY'} is not supported by FAT.
 Please pick one of the following {', '.join(['sinusoidal','independent','hanning'])}.
 : ''')
@@ -3793,14 +3774,20 @@
 
     if Configuration['RING_SIZE'] < 0.5:
         Configuration['RING_SIZE'] = 0.5
     if Configuration['OUTPUT_QUANTITY'] == 5:
         Configuration['OUTPUT_QUANTITY'] = 4
     if Configuration['SHAKER_ITERATIONS'] < 2:
         Configuration['SHAKER_ITERATIONS'] = 2
+    if Configuration['NCPU'] == 1:
+        if Configuration['MULTIPROCESSING']:
+             print(f'''You are only requesting 1 CPU to be used, we turn off multiprocessing.
+''')
+        Configuration['MULTIPROCESSING'] = False
+    
 
     return Configuration
 setup_configuration.__doc__ =f'''
  NAME:
     setup_configuration
 
  PURPOSE:
@@ -3826,16 +3813,19 @@
 
  NOTE: Only this function can add entries to Original_Configuration or Configuration
 '''
 
 
 
 def sbr_limits(Configuration, Tirific_Template ):
-    radii = set_rings(Configuration )
-    print_log(f'''SBR_LIMITS: Got {len(radii)} radii
+    radii = load_tirific(Configuration,Tirific_Template,Variables=['RADI'],array=True)
+    if len(radii) == 0.:
+        radii = set_rings(Configuration)
+        Tirific_Template['RADI']= ' '.join([str(x) for x in radii])
+    print_log(f'''SBR_LIMITS: Got {len(radii)} rings at the start
 ''',Configuration, case=['debug_start'])
     level = Configuration['NOISE']*1000
     noise_in_column = columndensity(Configuration,level,systemic = \
         float(load_tirific(Configuration,Tirific_Template,Variables=['VSYS'] )[0]))
     J2007col=9.61097e+19
     #J2007scl= 2. #arcsec in a sech^2 layer
     ratio=(noise_in_column/J2007col)**0.5
@@ -3863,15 +3853,15 @@
             mod_list.append(Configuration['LIMIT_MODIFIER'][-1])
         Configuration['LIMIT_MODIFIER'] = np.array(mod_list,dtype=float)
         sbr_ring_limits=[x*y for x,y in zip(sbr_ring_limits,Configuration['LIMIT_MODIFIER'])]
     print_log(f'''SBR_LIMITS: Retrieved these radii and limits:
 {'':8s}{radii}
 {'':8s}{sbr_ring_limits}
 ''',Configuration,case=['debug_add'])
-    return radii,sbr_ring_limits
+    return sbr_ring_limits
 
 sbr_limits.__doc__ =f'''
  NAME:
     sbr_limits
 
  PURPOSE:
     Calculate the sbr limits below which rings can not be trusted.
@@ -3970,16 +3960,16 @@
     Z0_kpc = convertskyangle(Configuration,Z0_av)
 
     if not isiterable(Z0_kpc):
         Z0_kpc = [Z0_kpc]
     #Scale the limits with the deviation away from 0.2 kpc as this is more or less the unmodified scale height
 
     modifier_list=[set_limits(x*(1.125-0.625*y)*set_limits(((Configuration['RING_SIZE']*Configuration['BEAM'][0])/45.)**0.25,0.75,1.25),0.5,3.) for x,y in zip(modifier_list,Z0_kpc)]
-
-    Configuration['LIMIT_MODIFIER'] = np.array(modifier_list,dtype=float)
+    #The 1.1 is emprically determined and might need modification. Lets put it in advanced configuration
+    Configuration['LIMIT_MODIFIER'] = np.array(modifier_list,dtype=float)*Configuration['LIMIT_MODIFIER_FACTOR']
     print_log(f'''SET_LIMIT_MODIFIER: Based on a Z0 in kpc {Z0_kpc}
 {'':8s} and Inclination = {Inclination}
 {'':8s} We updated the LIMIT_MODIFIER to {Configuration['LIMIT_MODIFIER']}.
 ''', Configuration,case=['debug_start'])
 
 
 set_limit_modifier.__doc__ =f'''
@@ -4050,15 +4040,15 @@
     if size_in_beams == 0.:
         size_in_beams =  np.min(Configuration['SIZE_IN_BEAMS'])
         double_size=True
     if requested_ring_size == 0.:
          requested_ring_size =  Configuration['RING_SIZE']
 
     print_log(f'''SET_RING_SIZE: Starting with the following parameters.
-{'':8s}size in beams = {size_in_beams}
+{'':8s}minimum size in beams = {size_in_beams}
 {'':8s}requested ring size = {requested_ring_size}
 ''', Configuration,case=['debug_start'])
     if not Configuration['FIX_RING_SIZE']:
         no_rings = 0.
         ring_size = 100.
         while (requested_ring_size > 0.5 and no_rings < Configuration['MINIMUM_RINGS']) or no_rings == 0.:
 
@@ -4074,14 +4064,15 @@
                 print_log(f'''SET_RING_SIZE: Because we had less than {Configuration['MINIMUM_RINGS']} rings we have reduced the requested ring size from {previous_ringsize} to {requested_ring_size}
     ''',Configuration)
 
         if double_size:
             # we had two values in the size_in beams we get the number of rings from the maximum
             #As we used the minimum to calate the ring size we need to recalculated the number of rings
             no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=np.max(Configuration['SIZE_IN_BEAMS']) )
+            size_in_beams = copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
     else:
         ring_size = requested_ring_size
         no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=np.max(Configuration['SIZE_IN_BEAMS']) )
 
     print_log(f'''SET_RING_SIZE: After checking the size we get
 {'':8s}size in beams = {size_in_beams}, ring size = {ring_size} and the number of ring = {no_rings}
 ''', Configuration,case=['debug_add'])
@@ -4291,14 +4282,15 @@
     for line in template:
         key = str(line.split('=')[0].strip().upper())
         if key == '':
             result[f'EMPTY{counter}'] = line
             counter += 1
         else:
             result[key] = str(line.split('=')[1].strip())
+   
     return result
 tirific_template.__doc__ ='''
  NAME:
     tirific_template
 
  PURPOSE:
     Read a tirific def file into a dictionary to use as a template.
@@ -4323,70 +4315,7 @@
 
  PROCEDURES CALLED:
       split, strip, open
 
  NOTE:
 '''
 
-def update_statistic(Configuration,process= None,message = None ):
-    if Configuration['TIMING']:
-        function = traceback.format_stack()[-2].split('\n')
-        function = function[0].split()[-1].strip()
-        if not process:
-            process = Configuration['FAT_PSUPROCESS']
-            program = 'pyFAT'
-        else:
-            program = 'TiRiFiC'
-
-        CPU,mem = get_usage_statistics(Configuration,process)
-        with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
-            if message:
-                file.write(f"# {function.upper()}: {message} at {datetime.now()} \n")
-            # We cannot copy the process so initialize in the configuration
-            file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for {program} \n")
-
-def write_config(file,Configuration ):
-    #be clear we are pickle dumping
-    tmp = os.path.splitext(file)
-    file = f'{tmp[0]}.pkl'
-    print_log(f'''WRITE_CONFIG: writing the configuration to {file}
-''',Configuration,case=['debug_start'])
-    # Separate the keyword names
-    #Proper dictionaries are not pickable
-
-    Pick_Configuration = {}
-    for key in Configuration:
-        Pick_Configuration[key] = Configuration[key]
-        if key == 'FAT_PSUPROCESS':
-            Pick_Configuration[key] = None
-    import pickle
-    with open(file,'wb') as tmp:
-        pickle.dump(Pick_Configuration,tmp)
-
-
-write_config.__doc__ =f'''
- NAME:
-    write_config
-
- PURPOSE:
-    Write a config file to the fitting directory.
-
- CATEGORY:
-    write_functions
-
- INPUTS:
-    file = name of the file to write to
-    Configuration = Standard FAT configuration
-
- OPTIONAL INPUTS:
-
-
- OUTPUTS:
-    A FAT config file.
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE: This doesn't work in python 3.6
-'''
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Support/write_functions.py` & `pyFAT_astro-0.1.6/pyFAT_astro/Support/write_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used to write text files to Disk
 
-
+from pyFAT_astro.Support.log_functions import print_log,extract_date
 from pyFAT_astro.Support.modify_template import set_model_parameters, set_overall_parameters,\
                                 set_fitting_parameters,get_warp_slope, update_disk_angles
-from pyFAT_astro.Support.fits_functions import extract_pv
+from make_moments.functions import extract_pv                                
 from pyFAT_astro.Support.read_functions import load_basicinfo
-from pyFAT_astro.Support.fat_errors import ProgramError
-import pyFAT_astro.Support.support_functions as sf
-import pyFAT_astro
 
+import pyFAT_astro.Support.support_functions as sf
 
 import copy
 import numpy as np
-import psutil as psu
-import time
-import warnings
-from datetime import datetime
-import traceback
 import os
+import warnings
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import matplotlib
     matplotlib.use('pdf')
     import matplotlib.pyplot as plt
     from mpl_toolkits.axes_grid1 import make_axes_locatable
@@ -156,14 +150,31 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def create_tirific_run_cube(Configuration,Fits_Files):
+    # if we have an optimized size cube this is only used in the run and we need t o change the ctyp 
+    if Configuration['OPTIMIZED']:
+        optimized_cube = f'{Configuration["FITTING_DIR"]}/{Fits_Files["OPTIMIZED_CUBE"]}'
+        cube = fits.open(optimized_cube)
+        cube[0].header['CTYPE3'] = 'VELO'
+        fits.writeto(optimized_cube,cube[0].data,cube[0].header,overwrite=True)
+    source = f'{Configuration["FITTING_DIR"]}/{Fits_Files["FITTING_CUBE"]}'
+    stripped_file_name = os.path.splitext(Fits_Files["FITTING_CUBE"])[0]
+    target = f'{Configuration["FITTING_DIR"]}/{stripped_file_name}_tirific.fits'
+    os.system(f'''cp {source} {target}''')
+    cube = fits.open(target)
+    cube[0].header['CTYPE3'] = 'VELO'
+    fits.writeto(target,cube[0].data,cube[0].header,overwrite=True)
+    Fits_Files['TIR_RUN_CUBE'] = target    
+    return Fits_Files
+
 # Function to write the first def file for a galaxy
 def initialize_def_file(Configuration, Fits_Files,Tirific_Template,\
         Initial_Parameters = None, fit_type = 'Undefined' ):
 
     if Initial_Parameters is None:
         Initial_Parameters = {}
 
@@ -243,168 +254,198 @@
 
  PROCEDURES CALLED:"/usr/share/fonts/truetype/msttcorefonts/Times_New_Roman.ttf"
     Unspecified
 
  NOTE:
 '''
 
+def beam_artist(ax,hdr,im_wcs):
+    xmin, xmax = ax.get_xlim()
+    ymin, ymax = ax.get_ylim()
+    ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
+    localoc = [float(ghxloc),float(ghyloc) ]
+    widthb = hdr['BMIN']
+    heightb = hdr['BMAJ']
+    try:
+        angleb  = hdr['BPA']
+    except KeyError:
+        angleb = 0.
+    #either the location or the beam has to be transformed 
+    beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform=ax.get_transform('world'),
+           edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
+    return beam
 
-class full_system_tracking:
-    def __init__(self,Configuration):
-        self.stop = False
-        self.pid = os.getpid()
-        self.main_pyFAT = psu.Process(self.pid)
-        self.user = self.main_pyFAT.username()
-        self.python = self.main_pyFAT.name()
-        self.tirific = Configuration['TIRIFIC']
-        self.font_file = Configuration['FONT_FILE']
-        self.sofia = Configuration['SOFIA2']
-        self.file = f"{Configuration['MAIN_DIRECTORY']}FAT_Resources_Used.txt"
-        self.plot_name= f"{Configuration['MAIN_DIRECTORY']}pyFAT_Resources_Monitor.pdf"
-        self.cpus= psu.cpu_count()
-        with open(self.file,'w') as resources:
-            resources.write("# This file contains an estimate of all resources used for a pyFAT run. \n")
-            resources.write(f"# {'Time':20s} {'Sys CPU':>10s} {'Sys RAM':>10s} {'FAT CPU':>10s} {'FAT RAM':>10s} \n")
-            resources.write(f"# {'YYYY-MM-DD hh:mm:ss':20s} {'%':>10s} {'Gb':>10s} {'%':>10s} {'Gb':>10s} \n")
-        self.interval = 60 # amount of second when to do new monitor
+beam_artist.__doc__ =f'''
+ NAME:
+    ist
 
-    def start_monitoring(self):
-        while not self.stop:
-            try:
-                self.sys_cpu= psu.cpu_percent(interval=1)
-                self.sys_ram= psu.virtual_memory().used/2**30.
-                self.CPU = 0.
-                self.RAM = 0.
-                for proc in psu.process_iter():
-                    if proc.username() == self.user \
-                        and proc.status() == 'running'\
-                        and (proc.name() == self.python or\
-                         proc.name() == self.tirific or\
-                         proc.name() == self.sofia or\
-                         proc.name() == 'python3'):
-                        try:
-                            self.CPU += proc.cpu_percent(interval=0.5)/self.cpus
-                            self.RAM += (proc.memory_info()[0])/2**30.
-                        except:
-                            pass
-                #file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Gb for TiRiFiC \n")
-                with open(self.file,'a') as resources:
-                    resources.write(f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S'):20s} {self.sys_cpu:>10.1f} {self.sys_ram:>10.2f} {self.CPU:>10.1f} {self.RAM:>10.2f} \n")
-            except Exception as e:
-                #We do not care if something goes wrong once. We don't want the monitor to crash
-                #but we would like to know what went wrong
-                traceback.print_exception(type(e),e,e.__traceback__)
-                pass
-            time.sleep(self.interval)
+ PURPOSE:
+    create a beam patch
+        
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    ax = is the axes object where the beam is intended to go
+    hdr = the image header
+    im_wcs = WCS frame of the image
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    IST
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+
+ NOTE:
+'''
+
+def create_plot_stats(Configuration,loads,labels):
+    combined_time =  np.sort(np.array(loads['Tirific']['Time']+loads['FAT']['Time'],dtype=float))
 
-    def stop_monitoring(self):
-        self.stop = True
-        loads = {'Time':[]}
-        keys=['SCPU','SRAM','FCPU','FRAM']
-        for key in keys:
-            loads[key]  = []
-        with open(self.file) as file:
-            lines = file.readlines()
-        startdate = 0
-        #load data from file into dictionary
-        for line in lines:
-            line = line.split()
-            if line[0] == '#':
-                continue
+    combined_loads ={'Tirific':{'CPU':np.interp(combined_time,np.array(loads['Tirific']['Time'],dtype=float),np.array(loads['Tirific']['CPU'],dtype=float)),\
+                                'MEM':np.interp(combined_time,np.array(loads['Tirific']['Time'],dtype=float),np.array(loads['Tirific']['MEM'],dtype=float))},\
+                    'FAT':{'CPU':np.interp(combined_time,np.array(loads['FAT']['Time'],dtype=float),np.array(loads['FAT']['CPU'],dtype=float)),\
+                                                'MEM':np.interp(combined_time,np.array(loads['FAT']['Time'],dtype=float),np.array(loads['FAT']['MEM'],dtype=float))}
+
+    }
+    comb_list= labels['Tirific']['Time']+labels['FAT']['Time']
+    comb_label = labels['Tirific']['label']+labels['FAT']['label']
+
+    labels_times=np.array([x for x, _ in sorted(zip(comb_list, comb_label))],dtype=float)
+    labels_comb = np.array([x for _, x in sorted(zip(comb_list, comb_label))],dtype=str)
+    if Configuration['MULTIPROCESSING']:
+        non_split_ct = copy.deepcopy(combined_time)
+        combined_time =[[],[]]
+        non_split_cl = copy.deepcopy(combined_loads)
+        combined_loads = [[],[]]
+        non_split_lt = copy.deepcopy(labels_times)
+        labels_times =[[],[]]
+        non_split_lc = copy.deepcopy(labels_comb)
+        labels_comb =[[],[]]
+        split_time_lab = non_split_lt[np.where(non_split_lc == 'Pausing FAT')[0]] 
+        split_time = non_split_lt[np.where(non_split_lc == 'Pausing FAT')[0]+1] 
+     
+        for i in  [0,1]:
+            if i == 0:
+                indxs = np.where(non_split_ct <= split_time)[0]
+                indxslab =  np.where(non_split_lt <= split_time_lab)[0]
+              
             else:
-                date = extract_date(f"{line[0]} {line[1]}")
-            if startdate == 0:
-                startdate = date
-            diff = date - startdate
-            time = diff.total_seconds()/(3600.)
-            loads['Time'].append(time)
-            for i,key in enumerate(keys):
-                loads[key].append(float(line[int(2+i)]))
-        #Plot the parameters
-        try:
-            mpl_fm.fontManager.addfont(self.font_file)
-            font_name = mpl_fm.FontProperties(fname=self.font_file).get_name()
-        except FileNotFoundError:
-            font_name = 'DejaVu Sans'
-        labelfont = {'family': font_name,
-                 'weight': 'normal',
-                 'size': 4}
-        fig, ax1 = plt.subplots(figsize = (8,6))
-        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.3, top = 0.7)
-        ax1.plot(loads['Time'],loads['SRAM'],'b--',lw=0.5,alpha=0.5, label='System RAM')
-        ax1.plot(loads['Time'],loads['FRAM'],'b-',lw=0.5,alpha=1.0, label='pyFAT RAM')
-        ax1.set_ylim(0,np.max(np.array(loads['SRAM']+loads['FRAM'],dtype=float))*1.1)
-        ax1.set_ylabel('RAM (Gb) ', color='b')
-        ax1.tick_params(axis='y', labelcolor='b')
-        ax1.set_xlabel('Run Duration (h)', color='k',zorder=5)
-        ax2 = ax1.twinx()
-        ax2.plot(loads['Time'],loads['SCPU'],'r--',lw=0.5,alpha=0.5, label='System CPU')
-        ax2.plot(loads['Time'],loads['FCPU'],'r-',lw=0.5,alpha=1.0, label='pyFAT CPU')
-        ax2.set_ylim(0,np.max(np.array(loads['SCPU']+loads['FCPU'],dtype=float))*1.1)
-        ax2.set_ylabel('CPUs (%)',color='r')
-        ax2.tick_params(axis='y', labelcolor='r')
-        fig.savefig(self.plot_name)
-        plt.close()
+                indxs = np.where(non_split_ct > split_time)[0]  
+                indxslab =  np.where(non_split_lt > split_time_lab)[0]
+          
+            combined_time[i] = non_split_ct[indxs]
+            labels_comb[i] = non_split_lc[indxslab]
+            labels_times[i] = non_split_lt[indxslab ]
+            combined_loads[i] = {'Tirific':{'CPU': non_split_cl['Tirific']['CPU'][indxs],\
+                                            'MEM': non_split_cl['Tirific']['MEM'][indxs] },\
+                                'FAT': {'CPU': non_split_cl['FAT']['CPU'][indxs],\
+                                        'MEM': non_split_cl['FAT']['MEM'][indxs] }}
+           
+    else:
+        combined_time = [combined_time ]
+        combined_loads = [combined_loads]
+        labels_times = [labels_times]
+        labels_comb = [labels_comb ]
+
+    return combined_time, combined_loads, labels_times, labels_comb
+
+create_plot_stats.__doc__ =f'''
+ NAME:
+    create_plot_stats(
+
+ PURPOSE:
+    create the lists and dictionaries that are required to plot a single frame in the usage plot
+    from the over loads and times dictionaries
+        
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    Configuration = is the standard FAT configuration
+    loads = is the overall loads dictionary
+    labels = the overall labels
+
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    combined_time = list with all times for individual axis object
+    combined_loads = dictionary with all loads  for individual axis object
+    labels_times = list with all label times  for individual axis object
+    labels_comb = liast with all labels  for individual axis object
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+
+ NOTE:
+'''
 
 def make_overview_plot(Configuration,Fits_Files ):
     fit_type = Configuration['USED_FITTING']
-    sf.print_log(f'''MAKE_OVERVIEW_PLOT: We are starting the overview plot.
+    print_log(f'''MAKE_OVERVIEW_PLOT: We are starting the overview plot.
 ''',Configuration,case=['debug_start'])
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         cube_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits")
         moment0_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom0.fits")
         moment1_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom1.fits")
         moment2_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom2.fits")
         cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}")
         moment0 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}")
         moment1 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT1']}")
         moment2 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT2']}")
         channels_map = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}")
         im_wcs = WCS(moment0[0].header).celestial
+   
 
     # Open the model info
-    sf.print_log(f'''MAKE_OVERVIEW_PLOT: Reading the variables from the final model
+    print_log(f'''MAKE_OVERVIEW_PLOT: Reading the variables from the final model
 ''',Configuration,case=['debug_add'])
     Vars_to_plot_short= ['RADI','XPOS','YPOS','VSYS','VROT','INCL','PA','SDIS',\
                     'SBR','Z0']
     Vars_to_plot=copy.deepcopy(Vars_to_plot_short)
     for x in Vars_to_plot_short:
         if x != 'RADI':
             Vars_to_plot.append(f'# {x}_ERR')
         if x not in ['XPOS','YPOS','VSYS']:
             Vars_to_plot.append(f'{x}_2')
             Vars_to_plot.append(f'# {x}_2_ERR')
     FAT_Model = sf.load_tirific(Configuration,\
         f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",\
-        Variables= Vars_to_plot,array=True )
+        Variables= Vars_to_plot,array=True ,brightness_check=True)
     Extra_Model_File = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def"
 
     if os.path.exists(Extra_Model_File):
         Extra_Model = sf.load_tirific(Configuration,Extra_Model_File,\
-            Variables= Vars_to_plot,array=True )
+            Variables= Vars_to_plot,array=True ,brightness_check=True)
+        
     else:
         Extra_Model = []
-    sf.print_log(f'''MAKE_OVERVIEW_PLOT: We find the following model values.
+    print_log(f'''MAKE_OVERVIEW_PLOT: We find the following model values.
 {'':8s}{[f"{x} = {FAT_Model[i,:]}" for i,x in enumerate(Vars_to_plot)]}
 ''',Configuration,case=['debug_add'])
 
     if os.path.exists(f"{Configuration['FITTING_DIR']}ModelInput.def"):
         Input_Model = sf.load_tirific(Configuration,\
             f"{Configuration['FITTING_DIR']}ModelInput.def",\
-            Variables= Vars_to_plot,array=True )
+            Variables= Vars_to_plot,array=True,brightness_check=False )
     else:
         Input_Model = []
     sof_basic_ra,sof_basic_dec, sof_basic_vsys,sof_basic_maxrot,sof_basic_pa,sof_basic_inclination,sof_basic_extent = load_basicinfo(Configuration,
         f"{Configuration['FITTING_DIR']}{Configuration['BASE_NAME']}-Basic_Info.txt",Variables=['RA','DEC','VSYS','Max VRot','PA','Inclination','D_HI'])
 
 
     #Let's start plotting
-    ysize = 23.2
+    ysize = 23.2/2.
     xsize = 0.7*ysize
     Overview = plt.figure(2, figsize=(xsize, ysize), dpi=300, facecolor='w', edgecolor='k')
 
     size_factor= ysize/11.6
     size_ratio = ysize/xsize
 
     #stupid pythonic layout for grid spec, which means it is yx instead of xy like for normal human beings
@@ -443,24 +484,23 @@
     ax_text.text(0.5,0.25,f'''The ring size used in the model is {Configuration['RING_SIZE']:.2f} x BMAJ, with BMAJ = {Configuration['BEAM'][0]:.1f} arcsec. We assumed a distance  of {Configuration['DISTANCE']:.1f} Mpc.'''
       ,rotation=0, va='top',ha='center', color='black',transform = ax_text.transAxes,
       bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
 
 
 #-----------------------------------------------------------------Moment 0 ------------------------------------------------------
     ax_moment0 = Overview.add_subplot(gs[2:8,0:6], projection=im_wcs)
-    ax_moment0.set_label('Intensity Map')
-    #Comp_ax1.set_facecolor('black')
     # we need contour levels and
     min_color = 0.
     max_color = np.nanmax(moment0[0].data)*0.8
-    moment0_plot = ax_moment0.imshow(moment0[0].data, origin='lower', alpha=1, vmin = min_color, vmax = max_color,cmap='hot_r' )
+    moment0_plot = ax_moment0.imshow(moment0[0].data, origin='lower', alpha=1,\
+        vmin = min_color, vmax = max_color,cmap='hot_r',transform=ax_moment0.get_transform(im_wcs) )
     moment0_plot.set_label('Intensity Map')
-    plt.ylabel('DEC (J2000)')
+    plt.ylabel('DEC')
     #Stupid python suddenly finds its own labels
-    plt.xlabel('RA J2000')
+    plt.xlabel('RA')
 
     median_noise_in_map = np.sqrt(np.nanmedian(channels_map[0].data[channels_map[0].data > 0.]))*Configuration['NOISE']*Configuration['CHANNEL_WIDTH']
     mindism0 = median_noise_in_map
     mindism0 = median_noise_in_map
     #"We find this {} as the minimum of the moment0 map".format(mindism0))
     if mindism0 < 0.:
         mindism0  =abs(mindism0)*2.
@@ -487,35 +527,33 @@
                levels=momlevel, colors='white',linewidths=1.5*size_factor , zorder =4)
     ax_moment0.contour(moment0[0].data, transform=ax_moment0.get_transform(im_wcs),
               levels=momlevel, colors='k',zorder=6, linewidths=1.2*size_factor)
     ax_moment0.contour(moment0_mod[0].data, transform=ax_moment0.get_transform(im_wcs),
                levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
     ax_moment0.contour(moment0_mod[0].data, transform=ax_moment0.get_transform(im_wcs),
               levels=momlevel, colors='r',zorder=8, linewidths=0.9*size_factor)
-    xmin, xmax = ax_moment0.get_xlim()
-    ymin, ymax = ax_moment0.get_ylim()
-    if xmax > ymax:
-        diff = int(xmax-ymax)/2.
-        ax_moment0.set_ylim(ymin-diff,ymax+diff)
-        ymin, ymax = ax_moment0.get_ylim()
-    else:
-        diff = int(ymax-xmax)/2.
-        ax_moment0.set_xlim(xmin-diff,xmax+diff)
-        xmin, xmax = ax_moment0.get_xlim()
-    ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
-    localoc = [float(ghxloc),float(ghyloc) ]
-    widthb = moment0[0].header['BMIN']
-    heightb = moment0[0].header['BMAJ']
-    try:
-        angleb  = moment0[0].header['BPA']
-    except KeyError:
-        angleb = 0.
-    beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform=ax_moment0.get_transform('fk4'),
-           edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
+  
+    square_plot(ax_moment0)
+    ax_moment0.grid()    
+    beam = beam_artist(ax_moment0,moment0[0].header,im_wcs)
     ax_moment0.add_patch(beam)
+    #center_x,center_y = im_wcs.wcs_world2pix(FAT_Model[Vars_to_plot.index('XPOS'),0],\
+    #                    FAT_Model[Vars_to_plot.index('YPOS'),0], 1.)
+
+    center_x = float(FAT_Model[Vars_to_plot.index('XPOS'),0])
+    center_y = float(FAT_Model[Vars_to_plot.index('YPOS'),0])
+   
+    ax_moment0.text(center_x,center_y,'X', size= 5.,va='center',ha='center', \
+                    color='white',zorder=17, transform=ax_moment0.get_transform('world'))
+    #ax_moment0.text(center_x,center_y,'X', size= 7.,va='center',ha='center', \
+     #               color='black',zorder=16, transform=ax_moment0.get_transform('world'))
+
+
+    #                ,transform = ax_moment0.transAxes,zorder=7)
+    #
     # colorbar
     divider = make_axes_locatable(ax_moment0)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment0_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
     cbar.ax.set_title(f"{moment0[0].header['BUNIT']}", y= 0.2*size_factor**2)
@@ -562,51 +600,35 @@
     inclination_correction = sf.set_limits(FAT_Model[Vars_to_plot.index('INCL'),0]+12.5,20.,90.)
     velocity_width= sf.set_limits(1.25*np.nanmax(FAT_Model[Vars_to_plot.index('VROT'),:])*np.sin(np.radians(inclination_correction)),30.,700.)
 
     max_color= FAT_Model[Vars_to_plot.index('VSYS'),0]+velocity_width
     min_color= FAT_Model[Vars_to_plot.index('VSYS'),0]-velocity_width
 
     moment1_plot = ax_moment1.imshow(moment1[0].data, cmap='rainbow', origin='lower', alpha=1, vmin = min_color, vmax = max_color )
-    plt.ylabel('DEC (J2000)')
+    plt.ylabel('DEC')
     #Stupid python suddenly finds its own labels
-    plt.xlabel('RA J2000')
+    plt.xlabel('RA')
 
     # contours
     velocity_step=sf.set_limits(int((int(max_color-min_color)*0.9)/20.),1.,30.)
     integer_array = np.linspace(0,20,21)-10
     momlevel = [FAT_Model[Vars_to_plot.index('VSYS'),0]+x*velocity_step for x in integer_array if min_color < FAT_Model[Vars_to_plot.index('VSYS'),0]+x*velocity_step < max_color]
     ax_moment1.contour(moment1[0].data, transform=ax_moment1.get_transform(im_wcs),
                levels=momlevel, colors='white',linewidths=1.5 *size_factor, zorder =4)
     ax_moment1.contour(moment1[0].data, transform=ax_moment1.get_transform(im_wcs),
               levels=momlevel, colors='k',zorder=6, linewidths=0.9*size_factor)
     ax_moment1.contour(moment1_mod[0].data, transform=ax_moment1.get_transform(im_wcs),
                levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
     #ax_moment1.contour(moment1_mod[0].data, transform=ax_moment1.get_transform(im_wcs),
     #          levels=momlevel, colors='r',zorder=8, linewidths=0.9)
-    xmin, xmax = ax_moment1.get_xlim()
-    ymin, ymax = ax_moment1.get_ylim()
-    if xmax > ymax:
-        diff = int(xmax-ymax)/2.
-        ax_moment1.set_ylim(ymin-diff,ymax+diff)
-        ymin, ymax = ax_moment1.get_ylim()
-        xmin, xmax = ax_moment1.get_xlim()
-    else:
-        diff = int(ymax-xmax)/2.
-        ax_moment1.set_xlim(xmin-diff,xmax+diff)
-    ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
-    localoc = [float(ghxloc),float(ghyloc) ]
-    widthb = moment1[0].header['BMIN']
-    heightb = moment1[0].header['BMAJ']
-    try:
-        angleb  = moment1[0].header['BPA']
-    except KeyError:
-        angleb = 0.
-    beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform=ax_moment1.get_transform('fk4'),
-           edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
+   
+    square_plot(ax_moment1)
+    beam = beam_artist(ax_moment1,moment1[0].header,im_wcs)
     ax_moment1.add_patch(beam)
+    ax_moment1.grid()
     # colorbar
     divider = make_axes_locatable(ax_moment1)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment1_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
     cbar.ax.set_title(f"{moment1[0].header['BUNIT']}", y= 0.2*size_factor**2)
@@ -629,53 +651,34 @@
     ax_moment2.set_label('Moment2')
     #Comp_ax1.set_facecolor('black')
     # we need contour levels and
     max_color= sf.set_limits(np.nanmax(moment2[0].data),15,50)
     min_color= 0.
 
     moment2_plot = ax_moment2.imshow(moment2[0].data, cmap='rainbow' ,origin='lower', alpha=1, vmin = min_color, vmax = max_color )
-    plt.ylabel('DEC (J2000)')
+    plt.ylabel('DEC')
     #Stupid python suddenly finds its own labels
-    plt.xlabel('RA J2000')
+    plt.xlabel('RA')
 
     # contours
 
     momlevel = np.linspace(min_color,max_color*0.8,5)
 
     ax_moment2.contour(moment2[0].data, transform=ax_moment2.get_transform(im_wcs),
                levels=momlevel, colors='white',linewidths=1.5*size_factor , zorder =4)
     ax_moment2.contour(moment2[0].data, transform=ax_moment2.get_transform(im_wcs),
               levels=momlevel, colors='k',zorder=6, linewidths=1.2*size_factor)
     ax_moment2.contour(moment2_mod[0].data, transform=ax_moment2.get_transform(im_wcs),
                levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
 
-    xmin, xmax = ax_moment2.get_xlim()
-    ymin, ymax = ax_moment2.get_ylim()
-    if xmax > ymax:
-        diff = int(xmax-ymax)/2.
-        ax_moment2.set_ylim(ymin-diff,ymax+diff)
-        ymin, ymax = ax_moment2.get_ylim()
-    else:
-        diff = int(ymax-xmax)/2.
-        ax_moment2.set_xlim(xmin-diff,xmax+diff)
-        xmin, xmax = ax_moment2.get_xlim()
-
-    ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
-    localoc = [float(ghxloc),float(ghyloc) ]
-    widthb = moment2[0].header['BMIN']
-    heightb = moment2[0].header['BMAJ']
-    try:
-        angleb  = moment2[0].header['BPA']
-    except KeyError:
-        angleb = 0.
-
-    beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform = ax_moment2.get_transform('fk4'),
-           edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
+   
+    square_plot(ax_moment2)
+    beam = beam_artist(ax_moment2,moment2[0].header,im_wcs)
     ax_moment2.add_patch(beam)
-
+    ax_moment2.grid()
 
     # colorbar
     divider = make_axes_locatable(ax_moment2)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment2_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
@@ -700,99 +703,42 @@
     moment2_mod.close()
 
 
 
 #__________________------------------------------------------------------------PV Diagram
 
     extract_angle = np.mean(FAT_Model[Vars_to_plot.index('PA'),0:round(len(FAT_Model[Vars_to_plot.index('PA'),:])/2.)])
-    PV = extract_pv(Configuration,cube,extract_angle, \
-                    center = [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0]),float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)], \
-                    convert=1000.)
-    if not os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/{Configuration['BASE_NAME']}_final_xv.fits"):
-        fits.writeto(f"{Configuration['FITTING_DIR']}/Finalmodel/{Configuration['BASE_NAME']}_final_xv.fits",PV[0].data,PV[0].header)
-    PV_model = extract_pv(Configuration,cube_mod,extract_angle, \
-                    center = [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0]),float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)], \
-                    convert=1000.)
-    if not os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_xv.fits"):
-        fits.writeto(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_xv.fits",PV_model[0].data,PV_model[0].header)
-    ratio=PV[0].header['NAXIS2']/PV[0].header['NAXIS1']
-    # Then we want to plot our PV-Diagram
-    '''
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        #As astropy is the dumbest piece of software ever invented and it cannot separate stray keywords from extra dimensions
-        # we need to specify we want the first two axes.
-        xv_proj = WCS(PV[0].header,naxis=[0,1])
-        xv_model_proj = WCS(PV_model[0].header,naxis=[0,1])
-    # As astropy is really a dumb piece of shit using a WCS messes up the the axes modifications
-    #ax_PV = Overview.add_subplot(gs[2:8,8:14], projection=xv_proj)
-    '''
-    ax_PV = Overview.add_subplot(gs[2:8,8:14])
-    #Comp_ax2.set_title('PV-Diagram')
-
-    maxint= np.nanmax(PV[0].data)*0.85
-    minint= np.nanmin(PV[0].data)/3.
 
-
-    PV_plot = ax_PV.imshow(PV[0].data,  cmap='hot_r', origin='lower', alpha=1, vmin=minint, vmax=maxint,aspect='auto')
-
-    xaxis = [PV[0].header['CRVAL1'] + (i - PV[0].header['CRPIX1'] + 1) * (PV[0].header['CDELT1']) for i in
-             range(PV[0].header['NAXIS1'])]
-    yaxis = [PV[0].header['CRVAL2'] + (i - PV[0].header['CRPIX2'] + 1) * (PV[0].header['CDELT2']) for i in
-             range(PV[0].header['NAXIS2'])]
-    #something is going wrong here, Fixed as usual astropy was fucking thing up
-    ax_PV.set_xticks(range(len(xaxis))[0:-1:int(len(xaxis) / 5)])
-    ax_PV.set_yticks(range(len(yaxis))[0:-1:int(len(yaxis) / 5)])
-    ax_PV.set_xticklabels(['{:10.1f}'.format(i) for i in xaxis[0:-1:int(len(xaxis) / 5)]])
-    ax_PV.set_yticklabels(['{:10.1f}'.format(i) for i in yaxis[0:-1:int(len(yaxis) / 5)]])
-
-    #Add some contours
-    neg_cont = np.array([-3,-1.5],dtype=float)*Configuration['NOISE']
-    if  np.nanmax(PV[0].data) * 0.95 < 96*Configuration['NOISE']:
-        pos_cont =  np.array([1.5,3.,6,12,24,48,96],dtype=float)*Configuration['NOISE']
-    else:
-        pos_cont =  np.array([0,1,2,3,4,5,6,7],dtype=float)*(np.nanmax(PV[0].data) * 0.95-3.*Configuration['NOISE'])/7. +3.*Configuration['NOISE']
-    pos_cont = np.array([x for x in pos_cont if x <= np.nanmax(PV[0].data) * 0.95],dtype=float)
-    sf.print_log(f'''MAKE_OVERVIEW_PLOT: postive {pos_cont}, negative {neg_cont}, noise {Configuration['NOISE']}
-''',Configuration,case=['debug_add'] )
-    if pos_cont.size == 0:
-        pos_cont = 0.5 * np.nanmax(PV[0].data) * 0.95
-
-    #ax_PV.contour(PV[0].data, levels=pos_cont, colors='k',transform=ax_PV.get_transform(xv_proj))
-    #ax_PV.contour(PV[0].data, levels=neg_cont, colors='grey',linestyles='--',transform=ax_PV.get_transform(xv_proj))
-    #ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',transform=ax_PV.get_transform(xv_model_proj),linewidths=1.)
-    ax_PV.contour(PV[0].data, levels=pos_cont,linewidths=1.*size_factor, colors='k')
-    ax_PV.contour(PV[0].data, levels=neg_cont,linewidths=1.*size_factor, colors='grey',linestyles='--')
-    ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',linewidths=1.*size_factor)
-
-    momlevel = np.hstack((neg_cont,pos_cont))
-    column_levels = ', '.join(["{:.1f}".format(x*1000.) for x in momlevel])
-    if len(momlevel) < 4:
-        info_string = f"The contours are at {column_levels} mJy/beam"
-    else:
-        info_string = f"The contours are at {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[0:4]])}"
-        counter = 5
-        while counter < len(momlevel):
-            info_string = info_string+f"\n {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[counter:counter+7]])}"
-            counter += 7
-        info_string = info_string+" mJy/beam."
-
-    divider = make_axes_locatable(ax_PV)
-    cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
-    cbar = plt.colorbar(PV_plot, cax=cax, orientation='horizontal')
-    cax.xaxis.set_ticks_position('top')
-    cbar.set_ticks([minint, maxint])
-    cbar.ax.set_title(f"{PV[0].header['BUNIT']}", y= 0.2*size_factor**2)
-
-    ax_PV.text(-0.1,-0.2,info_string, va='top',ha='left', color='black',transform = ax_PV.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7)
-
-    #cf.plot_fits(filename, Comp_ax2, cmap='hot_r', aspect=ratio, cbar ='horizontal')
-    ax_PV.set_xlabel("Offset (arcsec)")
-    ax_PV.set_ylabel("Velocity (km s$^{-1}$)")
+    messages = extract_pv(cube = cube,\
+                overwrite = False,PA=extract_angle,\
+                center=  [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),\
+                        float(FAT_Model[Vars_to_plot.index('YPOS'),0]),\
+                        float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)],\
+                map_velocity_unit= 'km/s',log = True,silent = True,\
+                output_directory = f"{Configuration['FITTING_DIR']}Finalmodel",\
+                output_name =f"{Configuration['BASE_NAME']}_final_xv.fits")
+    print_log(messages,Configuration,case=["verbose"])
+    PV = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/{Configuration['BASE_NAME']}_final_xv.fits")
+   
+    messages = extract_pv(cube = cube_mod,\
+                overwrite = False,PA=extract_angle,\
+                center=  [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),\
+                        float(FAT_Model[Vars_to_plot.index('YPOS'),0]),\
+                        float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)],\
+                cube_velocity_unit='m/s',\
+                map_velocity_unit= 'km/s',log = True,silent = True,\
+                output_directory = f"{Configuration['FITTING_DIR']}/Finalmodel/",\
+                output_name =f"Finalmodel_xv.fits")
+    print_log(messages,Configuration,case=["verbose"])
+    PV_model = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_xv.fits")
+
+
+    ax_PV = plot_PV(Configuration,image=PV, model = PV_model, figure = Overview, \
+        location = gs[2:8,8:14],size_factor = size_factor,
+        tirific_model = f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def")
     PV.close()
     PV_model.close()
 
 # ADD a legend for the plots
 
     ax_legend = Overview.add_subplot(gs[18:27,0:2],frameon = False)
     plt.tick_params(
@@ -827,37 +773,38 @@
 
     labelfont= {'family':font_name,
             'weight':'normal',
             'size':10*size_factor}
     ax_RC = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[19:22,3:9],\
                             Overview,'VROT',Input_Model = Input_Model,initial_extent= sof_basic_extent[0], \
                             initial = sof_basic_maxrot[0],Extra_Model = Extra_Model)
-    ymin =np.min([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
+    ymin =np.nanmin([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
+    ymax =np.nanmax([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
+
     if len(Extra_Model) > 0:
-        ymin2 =np.min([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
-        ymax2 =np.max([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymin2 =np.nanmin([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymax2 =np.nanmax([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
     else:
         ymin2 = ymin
         ymax2 = ymax
-    ymax =np.max([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
-
+  
     if len(Input_Model) > 0:
-        ymin3 =np.min([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
-        ymax3 =np.max([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymin3 =np.nanmin([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymax3 =np.nanmax([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
     else:
         ymin3=ymin
         ymax3= ymax
-    ymin = np.min([ymin,ymin2,ymin3])
-    ymax = np.max([ymax,ymax2,ymax3])
+    ymin = np.nanmin([ymin,ymin2,ymin3])
+    ymax = np.nanmax([ymax,ymax2,ymax3])
 
-    buffer = np.mean([ymin,ymax])/20.
+    buffer = np.nanmean([ymin,ymax])/20.
     ymin= ymin-buffer
     ymax = ymax+buffer
-
-    ax_RC.set_ylim(ymin,ymax)
+    if not np.isnan(ymin) and not np.isnan(ymax):
+        ax_RC.set_ylim(ymin,ymax)
 
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
@@ -994,15 +941,15 @@
           bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
     sec_ax = ax_SBR.twiny()
     arcmin,arcmax = ax_SBR.get_xlim()
     sec_ax.set_xticklabels([])
     sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
 
-
+#
 #----------------------------------------------Distance vs VSYS -----------------------------------------
     ax_VSYS = Overview.add_subplot(gs[2:6,16:20])
     plt.xlabel('Sys. Vel. (km s$^{-1}$)',**labelfont)
     plt.ylabel('Distance (Mpc)',**labelfont)
 
     plt.errorbar(float(FAT_Model[Vars_to_plot.index('VSYS'),0]),float(Configuration['DISTANCE'])\
                 ,xerr=float(FAT_Model[Vars_to_plot.index('# VSYS_ERR'),0]), c='k',zorder= 3,fmt="o")
@@ -1049,14 +996,16 @@
     ax_RAD.add_patch(mod_ell)
     ax_RAD.legend(loc='upper left', bbox_to_anchor=(0.0, -0.3), shadow=True, ncol=1)
     plt.xlabel('RA ($^{\circ}$)',**labelfont)
     plt.ylabel('DEC ($^{\circ}$)',**labelfont)
     cube_mod.close()
     cube.close()
     channels_map.close()
+
+    #
     plt.savefig(f"{Configuration['FITTING_DIR']}Overview.png", bbox_inches='tight')
     #plt.savefig(f"Overview_Test.png", bbox_inches='tight')
     plt.close()
 
 make_overview_plot.__doc__ =f'''
  NAME:
     make_overview_plot(Configuration,Fits_Files ):
@@ -1090,22 +1039,22 @@
         initial_extent=  None, Extra_Model = None):
     if Input_Model is None:
         Input_Model = []
     if Extra_Model is None:
         Extra_Model = []
     if legend is None:
         legend = ['Empty','Empty','Empty','Empty']
-    sf.print_log(f'''PLOT_PARAMETERS: We are starting to plot {parameter}
+    print_log(f'''PLOT_PARAMETERS: We are starting to plot {parameter}
 ''', Configuration,case=['debug_start'])
     ax = Figure.add_subplot(location)
     try:
         yerr = FAT_Model[Vars_to_plot.index(f'# {parameter}_ERR'),:]
     except ValueError:
         yerr =np.zeros(len(FAT_Model[Vars_to_plot.index('RADI'),:]))
-    sf.print_log(f'''PLOT_PARAMETERS: We found these errors {yerr}
+    print_log(f'''PLOT_PARAMETERS: We found these errors {yerr}
 ''', Configuration,case=['debug_add'])
 
     ax.errorbar(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}'),:],yerr= yerr, c ='k', label=f'{legend[0]}',zorder=3)
     ax.plot(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}'),:],'ko', ms = 3.,zorder=3)
     if np.sum(FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:]) != 0.:
         diff = np.sum(abs(FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:]-FAT_Model[Vars_to_plot.index(f'{parameter}'),:]))
         if diff != 0.:
@@ -1192,44 +1141,325 @@
 
      PROCEDURES CALLED:
         Unspecified
 
      NOTE:
 '''
 
+def plot_PV(Configuration,image=None, model = None, figure = None, \
+    location = [0.1,0.1,0.8,0.8], tirific_model=None, size_factor = 1.):
+    if image == None:
+        print('plot_PV will not work witout an image.')
+        return 'Empty'
+    else:
+        try:
+            hdr = image[0].header
+            data = image[0].data
+        except:
+            hdr = image.header
+            data = image.data
+
+    ratio=hdr['NAXIS2']/hdr['NAXIS1']
+    # Then we want to plot our PV-Diagram
+    if figure == None:
+        figure = plt.figure(2, figsize=(8, 8), dpi=300, facecolor='w', edgecolor='k')
+
+    ax = figure.add_subplot(location)
+    #Comp_ax2.set_title('PV-Diagram')
+
+    maxint= np.nanmax(data)*0.85
+    minint= np.nanmin(data)/3.
+    PV_plot = ax.imshow(data,  cmap='hot_r', origin='lower', alpha=1, \
+                            vmin=minint, vmax=maxint,aspect='auto')
+    xaxis = [hdr['CRVAL1'] + (i - hdr['CRPIX1'] + 1) \
+        * (hdr['CDELT1']) for i in range(hdr['NAXIS1'])]
+    yaxis = [hdr['CRVAL2'] + (i - hdr['CRPIX2'] + 1) * (hdr['CDELT2']) for i in
+         range(hdr['NAXIS2'])]
+    #something is going wrong here, Fixed as usual astropy was fucking thing up
+    step = int(abs((xaxis[-1]-xaxis[0])/7))
+    ticks = np.array([-3*step,-2*step,-1*step,0.,step,2*step,3*step],dtype=float)+hdr['CRVAL1']
+    pix_ticks =(ticks - hdr['CRVAL1'])/hdr['CDELT1']+(hdr['CRPIX1']-1)
+    ax.set_xticks(pix_ticks)
+    ax.set_xticklabels([f'{int(i):d}' for i in ticks],size=5,ha='center')
+    ax.set_yticks(range(len(yaxis))[0:-1:int(len(yaxis) / 5)])
+    ax.set_yticklabels(['{:.1f}'.format(i) for i in yaxis[0:-1:int(len(yaxis) / 5)]])
+    ax.grid()
+   
+    #Add some contours
+    neg_cont = np.array([-3,-1.5],dtype=float)*Configuration['NOISE']
+    if  np.nanmax(data) * 0.95 < 96*Configuration['NOISE']:
+        pos_cont =  np.array([1.5,3.,6,12,24,48,96],dtype=float)*Configuration['NOISE']
+    else:
+        pos_cont =  np.array([0,1,2,3,4,5,6,7],dtype=float)*(np.nanmax(data) * 0.95-3.*Configuration['NOISE'])/7. +3.*Configuration['NOISE']
+    pos_cont = np.array([x for x in pos_cont if x <= np.nanmax(data) * 0.95],dtype=float)
+    print_log(f'''PV_PLOT: postive {pos_cont}, negative {neg_cont}, noise {Configuration['NOISE']}
+''',Configuration,case=['debug_add'] )
+    if pos_cont.size == 0:
+        pos_cont = 0.5 * np.nanmax(data) * 0.95
+
+#ax_PV.contour(PV[0].data, levels=pos_cont, colors='k',transform=ax_PV.get_transform(xv_proj))
+#ax_PV.contour(PV[0].data, levels=neg_cont, colors='grey',linestyles='--',transform=ax_PV.get_transform(xv_proj))
+#ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',transform=ax_PV.get_transform(xv_model_proj),linewidths=1.)
+    ax.contour(data, levels=pos_cont,linewidths=1.*size_factor, colors='k')
+    ax.contour(data, levels=neg_cont,linewidths=1.*size_factor, colors='grey',linestyles='--')
+    if model != None:
+        try:
+            model_data = model[0].data
+        except:
+            model_data = model.data
+        ax.contour(model_data, levels=pos_cont, colors='b',linewidths=1.*size_factor)
+
+    momlevel = np.hstack((neg_cont,pos_cont))
+    column_levels = ', '.join(["{:.1f}".format(x*1000.) for x in momlevel])
+    if len(momlevel) < 4:
+        info_string = f"The contours are at {column_levels} mJy/beam"
+    else:
+        info_string = f"The contours are at {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[0:4]])}"
+        counter = 5
+        while counter < len(momlevel):
+            info_string = info_string+f"\n {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[counter:counter+7]])}"
+            counter += 7
+    info_string = info_string+" mJy/beam."
+
+    divider = make_axes_locatable(ax)
+    cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
+    cbar = plt.colorbar(PV_plot, cax=cax, orientation='horizontal')
+    cax.xaxis.set_ticks_position('top')
+    cbar.set_ticks([minint, maxint])
+    cbar.ax.set_title(f"{hdr['BUNIT']}", y= 0.2*size_factor**2)
+
+    ax.text(-0.1,-0.2,info_string, va='top',ha='left', color='black',transform = ax.transAxes,
+          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7)
+    if tirific_model != None:
+        parameters = sf.load_tirific(Configuration,tirific_model,\
+            Variables= ['RADI','VROT','VROT_2','INCL','INCL_2','VSYS','VSYS_2']\
+                ,array=True ,brightness_check=True)
+        if np.sum(parameters[2]) == 0.:
+            parameters[2] =   parameters[1]
+            parameters[4] =   parameters[3]
+            parameters[6] =   parameters[5]
+        if 'DRVAL1' in hdr:
+            center = [float(x) for x in hdr['DRVAL1'].split('+')]
+            model_center = [float(x[0]) for x in sf.load_tirific(Configuration,tirific_model,\
+            Variables= ['XPOS','XPOS_2','YPOS','YPOS_2'],array=True ) ]
+        if 'DRVAL2' in hdr:
+            vsys = float(hdr['DRVAL2'])
+            model_vsys = [float(x[0]) for x in sf.load_tirific(Configuration,tirific_model,\
+            Variables= ['VSYS','VSYS_2'],array=True ) ]
+
+    
+     
+                            
+        plotrc  = np.array([-1.*x*np.sin(np.radians(y))+parameters[5][0] for x,y \
+            in zip(parameters[1],parameters[3])],dtype=float)
+        plotrc2  = np.array([x*np.sin(np.radians(y))+parameters[6][0] for x,y in\
+            zip(parameters[2],parameters[4])],dtype=float)
+        # As python is a piece of shit that only does things half we need to convert to pixels
+
+        plotrc= (plotrc - hdr['CRVAL2'])/hdr['CDELT2']+(hdr['CRPIX2']-1)
+        radius = (-1.*parameters[0]-hdr['CRVAL1'])/hdr['CDELT1']+(hdr['CRPIX1']-1)
+        plotrc2= (plotrc2 - hdr['CRVAL2'])/hdr['CDELT2']+(hdr['CRPIX2']-1)
+        radius2 = (parameters[0]-hdr['CRVAL1'])/hdr['CDELT1']+(hdr['CRPIX1']-1)
+        ax.plot(radius,plotrc,'o',c='r')
+        ax.plot(radius2,plotrc2,'o',c='r')
+    #cf.plot_fits(filename, Comp_ax2, cmap='hot_r', aspect=ratio, cbar ='horizontal')
+    ax.set_xlabel("Offset (arcsec)")
+    ax.set_ylabel("Velocity (km s$^{-1}$)")
+    return ax
+plot_PV.__doc__ =f'''
+     NAME:
+        plot_PV
+
+     PURPOSE:
+        Plot the PV with th RC overlaid.
+
+     CATEGORY:
+        write_functions
+
+     INPUTS:
+        Configuration = Standard FAT configuration
+        image = fits object of the PV
+
+     OPTIONAL INPUTS:
+        model = fits object of model to overplot
+        figure = figure to plot the ax in if not defined it will be an 8 x 8 figure \
+        location = [0.1,0.1,0.8,0.8]
+            location of the ax
+        tirific_model=None
+            Model to obtain the RC from
+        size_factor = 1.
+            scaling factor for text and line widths
+
+
+
+     OUTPUTS:
+        ax object from matplot lib
+
+     OPTIONAL OUTPUTS:
+
+     PROCEDURES CALLED:
+        Unspecified
+
+     NOTE:
+'''
+
+def plot_individual_ax(Configuration,ax,combined_time,combined_loads):
+    ax.plot(combined_time,combined_loads['Tirific']['MEM'],'b-',lw=0.5)
+    ax.plot(combined_time,combined_loads['FAT']['MEM'],'b--',lw=0.5)
+    ax.set_ylim(0,np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']]) \
+                      +np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']])/10.)
+   
+   
+    ax2 = ax.twinx()
+    ax2.plot(combined_time,combined_loads['Tirific']['CPU'],'r-',lw=0.5)
+    ax2.plot(combined_time,combined_loads['FAT']['CPU'],'r--',lw=0.5)
+    return ax,ax2
+plot_individual_ax.__doc__ =f'''
+     NAME:
+        plot_individual_ax
+
+     PURPOSE:
+        setup a double plot with 2 axes 
 
+     CATEGORY:
+        write_functions
+
+     INPUTS:
+        Configuration = Standard FAT configuration
+        ax = the axis object to hold the double plot
+        combined_time = list containing the x axis
+        combined_load = dictionary that that contains the Memory (blue) and CPU (red) loads split
+                         according to tirific (solid line)  and FAT (dashed line)
+
+     OPTIONAL INPUTS:
+
+
+     OUTPUTS:
+        ax = axis object with the memory plot
+        ax2 = axis object with the CPU plot
+
+     OPTIONAL OUTPUTS:
+
+     PROCEDURES CALLED:
+        Unspecified
+
+     NOTE:
+'''
 
 def plot_usage_stats(Configuration ):
     with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt") as file:
         lines = file.readlines()
 
-    labels = {'FAT': {'label':[], 'Time':[]}, 'Tirific':{'label':[], 'Time':[]}}
-    loads = {'FAT':{'CPU':[],'MEM':[],'Time':[]},'Tirific':{'CPU':[],'MEM':[],'Time': []}}
+    
     try:
         mpl_fm.fontManager.addfont(Configuration['FONT_FILE'])
         font_name = mpl_fm.FontProperties(fname=Configuration['FONT_FILE']).get_name()
     except FileNotFoundError:
         font_name = 'DejaVu Sans'
     labelfont = {'family': font_name,
              'weight': 'normal',
              'size': 4}
+    loads,labels,maxCPU, maxMEM = read_statistics(Configuration)
+   
+    # Below thanks to P. Serra
+    # Make single-PID figures and total figure
+    #print(loads['Tirific']['Time'],loads['FAT']['Time'])
+    if len(loads['Tirific']['Time']) > 0.:
+        combined_time, combined_loads, labels_times, labels_comb = \
+                create_plot_stats(Configuration,loads,labels)
+          
+        if Configuration['MULTIPROCESSING']:
+            fig, ax = plt.subplots(1,2,sharey=True,figsize = (8,6))
+            ax[0].spines['right'].set_visible(False)
+            ax[1].spines['left'].set_visible(False)
+            ax[0].yaxis.tick_left()
+            ax[0].tick_params(labelright='off')
+            ax[1].yaxis.tick_right()
+          
+           
+            
+        else:
+            fig, ax = plt.subplots(figsize = (8,6))
+           
+            ax = [ax]
+        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.3, top = 0.7)
+        left_bottom = 0.1
+        tot_time = 0.
+        for timeone in combined_time:
+            tot_time += timeone[-1]-timeone[0]
+        normalize = tot_time/0.8
+        lengths = [np.max([(x[-1]-x[0])/normalize,0.15]) for x in combined_time]
+        lengths = np.array(lengths,dtype=float) * 0.8/np.sum(lengths) 
+        for i,axplot in enumerate(ax):
+            normalize = (labels_times[i][-1]-labels_times[i][0])/lengths[i]
+            ax_MEM,ax_CPU = plot_individual_ax(Configuration,axplot,combined_time[i],combined_loads[i])
+            ax_MEM,ax_CPU,left_bottom = set_proper_edges(Configuration, i, ax, ax_MEM,\
+                                         ax_CPU,lengths[i],left_bottom)
+            ax_CPU.set_ylim(0.,maxCPU*1.05)
+            ax_MEM.set_ylim(0.,maxMEM*1.05)
+            ax_MEM.set_xlim(combined_time[i][0],combined_time[i][-1])
+            ax_CPU.set_xlim(combined_time[i][0],combined_time[i][-1])
+                
+            ax_CPU = set_timing_labels(Configuration,ax_CPU, labels_times[i],labels_comb[i],labels,labelfont,normalize)
+        fig.text(0.5,0.25,'time (min)', va='center',ha='center',rotation= 0, color='black',
+                          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7)
+        fig.savefig(f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf")
+        plt.close()
+
+plot_usage_stats.__doc__ =f'''
+ NAME:
+    plot_usage_stats
+
+ PURPOSE:
+    Plot the RAM and CPU usage over time for the fit
+
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    ram_cpu.pdf in the Logs directory
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def read_statistics(Configuration):
+    labels = {'FAT': {'label':[], 'Time':[]}, 'Tirific':{'label':[], 'Time':[]}}
+    loads = {'FAT':{'CPU':[],'MEM':[],'Time':[]},'Tirific':{'CPU':[],'MEM':[],'Time': []}}
+    with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt") as file:
+        lines = file.readlines()
     current_stage = 'Not_Found'
-    current_module = 'Unknown'
+    #current_module = 'Unknown'
     startdate = 0
+    maxCPU = 0.
+    maxMEM= 0.
+    paused_time = 0.
+    gap_time= 0.
     for line in lines:
         line = line.strip()
         tmp = line.split(' ')
         if line[0] == '#':
             date = extract_date(f"{tmp[-2]} {tmp[-1]}")
         else:
             date = extract_date(f"{tmp[0]} {tmp[1]}")
         if startdate == 0:
             startdate = date
         diff = date - startdate
-        time = diff.total_seconds()/60.
+        time = diff.total_seconds()/60.-gap_time
+    
         if line[0] == '#':
             if tmp[1] == 'TIRIFIC:':
 
                 if tmp[2].lower() == 'initializing':
                     tmp2 = line.split('=')[1].split()
                     current_stage = tmp2[0].strip()
                     labels['Tirific']['label'].append(f'Initializing {current_stage}')
@@ -1237,174 +1467,68 @@
                 elif tmp[2].lower() == 'finished':
                     labels['Tirific']['label'].append(f'Ended {current_stage}')
                     labels['Tirific']['Time'].append(time)
                     #current_stage = 'No Tirific'
                 elif tmp[2].lower() == 'started':
                     labels['Tirific']['label'].append(f'Started {current_stage}')
                     labels['Tirific']['Time'].append(time)
+            elif tmp[1] == 'MP_FITTING_LOOP:':
+                labels['Tirific']['label'].append(f'Started {tmp[1]}')  
+                if Configuration['MULTIPROCESSING']:
+                    gap_time = time-paused_time
+                labels['Tirific']['Time'].append(time-gap_time)
             else:
-                labels['FAT']['label'].append(f'Starting {tmp[1]}')
-                labels['FAT']['Time'].append(time)
+                if tmp[2].lower() == 'pause':
+                    labels['FAT']['label'].append(f'Pausing FAT')
+                    labels['FAT']['Time'].append(time)
+                    if Configuration['MULTIPROCESSING']:
+                        '''If we are pausing due to splitting sofia and fit we subtract the pause time'''
+                        paused_time = time
+                else:
+                    labels['FAT']['label'].append(f'Starting {tmp[1]}')
+                    labels['FAT']['Time'].append(time)
         else:
             if tmp[-1].lower() == 'tirific':
                 loads['Tirific']['Time'].append(time)
                 loads['Tirific']['CPU'].append(tmp[4])
+               
                 loads['Tirific']['MEM'].append(tmp[8])
             else:
                 loads['FAT']['Time'].append(time)
                 loads['FAT']['CPU'].append(tmp[4])
                 loads['FAT']['MEM'].append(tmp[8])
-
-    # Below thanks to P. Serra
-    # Make single-PID figures and total figure
-    #print(loads['Tirific']['Time'],loads['FAT']['Time'])
-    if len(loads['Tirific']['Time']) > 0.:
-        combined_time =  np.sort(np.array(loads['Tirific']['Time']+loads['FAT']['Time'],dtype=float))
-
-        combined_loads ={'Tirific':{'CPU':np.interp(combined_time,np.array(loads['Tirific']['Time'],dtype=float),np.array(loads['Tirific']['CPU'],dtype=float)),\
-                                    'MEM':np.interp(combined_time,np.array(loads['Tirific']['Time'],dtype=float),np.array(loads['Tirific']['MEM'],dtype=float))},\
-                        'FAT':{'CPU':np.interp(combined_time,np.array(loads['FAT']['Time'],dtype=float),np.array(loads['FAT']['CPU'],dtype=float)),\
-                                                    'MEM':np.interp(combined_time,np.array(loads['FAT']['Time'],dtype=float),np.array(loads['FAT']['MEM'],dtype=float))}
-
-        }
-        comb_list= labels['Tirific']['Time']+labels['FAT']['Time']
-        comb_label = labels['Tirific']['label']+labels['FAT']['label']
-
-        labels_times=np.array([x for x, _ in sorted(zip(comb_list, comb_label))],dtype=float)
-        labels_comb = [x for _, x in sorted(zip(comb_list, comb_label))]
-
-        fig, ax1 = plt.subplots(figsize = (8,6))
-        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.3, top = 0.7)
-
-
-        ax1.plot(combined_time,combined_loads['Tirific']['MEM'],'b-',lw=0.5)
-        ax1.plot(combined_time,combined_loads['FAT']['MEM'],'b--',lw=0.5)
-        ax1.set_ylim(0,np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']]) \
-                      +np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']])/10.)
-        ax1.set_ylabel('RAM (Mb) ', color='b')
-        ax1.tick_params(axis='y', labelcolor='b')
-        ax1.set_xlabel('time (min)', color='k',zorder=5)
-        ax2 = ax1.twinx()
-        ax2.plot(combined_time,combined_loads['Tirific']['CPU'],'r-',lw=0.5)
-        ax2.plot(combined_time,combined_loads['FAT']['CPU'],'r--',lw=0.5)
-        #ax2.plot(combined_time,combined_loads['FAT']['CPU'],'r--',lw=0.5)
-        ax2.set_ylabel('CPUs (%)',color='r')
-        ax2miny,ax2maxy = ax2.get_ylim()
-        ax2.tick_params(axis='y', labelcolor='r')
-        last_label = -100
-        label_sep = combined_time[-1]/30.
-        color, linest = '0.5', '--'
-        labelfont = {'family': font_name,
-                 'weight': 'normal',
-                 'size': 6.5}
-        prev_label = ''
-
-        last_label_top = 0.
-        last_label_bottom = 0.
-        #for label,time in zip(labels['Tirific']['label'],labels['Tirific']['Time']):
-        for label,time in zip(labels_comb,labels_times):
-
-            if label in labels['Tirific']['label']:
-                offset = 20.
-                xoffset = 0.05
-                vertical_start = ax2maxy
-                va= 'bottom'
-                ha= 'left'
-                color = 'k'
-                linest = '-'
-            else:
-                offset=-50
-                xoffset = 0.025
-                vertical_start = ax2miny
-                va= 'top'
-                ha='right'
-                color = '0.5'
-                linest = '--'
-
-
-            if (prev_label == 'Initializing tmp_incl_check' or prev_label == 'Ended tmp_incl_check'):
-                if (label != 'Initializing tmp_incl_check' and label != 'Ended tmp_incl_check') or \
-                        time == labels_times[-1]    :
-
-                    if time != labels_times[-1]:
-                        ax2.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
-                        if label in labels['Tirific']['label']:
-                            last_label = last_label_top = max(prev_time,last_label_top+label_sep)
-                        else:
-                            last_label = last_label_bottom = max(prev_time,last_label_bottom+label_sep)
-                        ax2.text(last_label,vertical_start+offset,prev_label, va=va,ha=ha,rotation= 60, color='black',
-                              bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                        ax2.plot([prev_time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
-                    ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                    if label in labels['Tirific']['label']:
-                        last_label = last_label_top = max(time,last_label_top+label_sep)
-                    else:
-                        last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
-                    ax2.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
-                          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                    ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
-                else:
-                    prev_time = time
-            elif (prev_label == 'Initializing Error_Shaker' or prev_label == 'Ended Error_Shaker' or prev_label == 'Started Error_Shaker'):
-                if (label != 'Initializing Error_Shaker' and label != 'Ended Error_Shaker' and  label != 'Started Error_Shaker') or \
-                        time == labels_times[-1]:
-
-                    #ax2.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
-                    #last_label = max(prev_time,last_label+label_sep)
-                    #ax2.text(last_label,ax2maxy+20.,prev_label, va='bottom',ha='left',rotation= 60, color='black',
-                    #      bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                    #ax2.plot([prev_time,last_label+0.1],[ax2maxy,ax2maxy+20.],linest,color=color,linewidth=0.05,clip_on=False)
-                    ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                    if label in labels['Tirific']['label']:
-                        last_label = last_label_top = max(time,last_label_top+label_sep)
-                    else:
-                        last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
-                    ax2.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
-                          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                    ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
-                else:
-                    prev_label = label
-                    prev_time = time
-            else:
-                ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                if label in labels['Tirific']['label']:
-                    last_label = last_label_top = max(time,last_label_top+label_sep)
-                else:
-                    last_label = last_label_bottom= max(time,last_label_bottom+label_sep)
-                ax2.text(last_label,vertical_start+offset,label,va=va,ha=ha,rotation= 60, color='black',
-                      bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                #This should be the line to the label
-                ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
-            prev_label = label
-
-
-
-        #This is beyond stupid again, but hey it is python so needed to make things work.
-        ax2.set_ylim([ax2miny,ax2maxy])
-        fig.savefig(f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf")
-        plt.close()
-
-plot_usage_stats.__doc__ =f'''
+            if float(tmp[4]) > maxCPU:
+                    maxCPU = float(tmp[4])
+            if float(tmp[8]) > maxMEM:
+                    maxMEM = float(tmp[8])
+    return loads,labels,maxCPU,maxMEM
+read_statistics.__doc__ =f'''
  NAME:
-    plot_usage_stats
+    read_statistics
 
  PURPOSE:
-    Plot the RAM and CPU usage over time for the fit
+    Read the file Usage_Statistics.txt in the FAT log directory and transform the input into two 
+    dictionaries. In Multiprocessing the pool time is subtracted
+  
 
  CATEGORY:
     write_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
+    
 
  OPTIONAL INPUTS:
 
 
  OUTPUTS:
-    ram_cpu.pdf in the Logs directory
+    loads = dictionary with the times and Memory and CPU loads, split in system and tirific
+    labels = labels indicating specifics of what was happening at times
+    maxCPU = the max CPU load encountered
+    maxMEM = the maximum memory load encountered
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
@@ -1428,17 +1552,14 @@
             try:
                 index_no = np.where(galaxy == \
                     np.array(outputIDs))[0][0]
                 file.write(output[index_no])
             except IndexError:
                 pass
 
-
-
-
 reorder_output_catalogue.__doc__ =f'''
  NAME:
     reorder_output_catalogue
 
  PURPOSE:
     When running in multiprocessing mode the output catalogue can be
     in a different order as the input. This function makes sure the are sorted
@@ -1460,65 +1581,284 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def extract_date(string):
-    tmp = string.split(' ')
-    tmp2 = tmp[0].split('-')
-    if len(tmp2) == 3:
-        try:
-            date =  datetime.strptime(f"{tmp[0]} {tmp[1]}", '%Y-%m-%d %H:%M:%S.%f')
-        except ValueError:
-            date =  datetime.strptime(f"{tmp[0]} {tmp[1]}", '%Y-%m-%d %H:%M:%S')
+def set_proper_edges(Configuration,i,ax,ax_MEM,ax_CPU,length,left_bottom):
+    if i+1 == len(ax):
+        if i > 0:
+            ax_MEM.spines['left'].set_visible(False) 
+            ax_MEM.tick_params(axis='y', length = 0)    
+        ax_CPU.spines['left'].set_visible(False)
+        ax_CPU.set_ylabel('CPUs (%)',color='r')
+        ax_CPU.tick_params(axis='y', labelcolor='r')
     else:
-        raise ProgramError("There is no date in the provided string.")
-    return date
+        '''This currently only works with a single break'''
+        ax_CPU.spines['right'].set_visible(False)
+        ax_CPU.axis('off')    
+        ax_CPU.tick_params(labelleft='off')
+    if i == 0:
+        ax_MEM.set_ylabel('RAM (Mb) ', color='b')
+        ax_MEM.tick_params(axis='y', labelcolor='b')
+    ax_MEM.set_position([left_bottom,0.3,length,0.4])
+    ax_CPU.set_position([left_bottom,0.3,length,0.4])
+    left_bottom += length+0.01  
+
+    d =0.025
+    dx = d/(6*length)
+    kwargs = dict(transform=ax_MEM.transAxes, color='k', clip_on=False)
+    if i != 0:
+        ax_MEM.plot((-dx, dx), (1-d, 1+d), **kwargs)
+        ax_MEM.plot((-dx, dx), (-d, +d), **kwargs)
+    
+    if i+1 != len(ax):
+        ax_MEM.plot((1-dx, 1+dx), (-d, +d), **kwargs)
+        ax_MEM.plot((1-dx, 1+dx), (1-d, 1+d), **kwargs)   
+    return ax_MEM,ax_CPU,left_bottom
+set_proper_edges.__doc__ =f'''
+ NAME:
+    set_proper_edges
+
+ PURPOSE:
+    Set the proper edges form the timing plot  
+ 
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    i = index of current ax
+    ax = all axes
+    ax_MEM = the memory axis
+    ax_CPU = the CPU axis
+    length = size of the plot in fig coordinate
+    left_bottom = location of the right side of the plot in fig coordinate
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    ax_MEM = updated memory axis object
+    ax_CPU = updated CPU axis object
+    left_bottom = right hand side for next axis object
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def set_timing_labels(Configuration,ax, labels_times,labels_comb,labels,labelfont,normalize):
+    labelfont['size'] = 6
+    miny, maxy = ax.get_ylim()
+    last_label = -100
+
+    label_sep = 0.015*normalize
+    #label_sep = 0.001
+    color, linest = '0.5', '--'
+   
+    prev_label = ''
+
+    last_label_top = -100.
+    last_label_bottom = -100.
+        #for label,time in zip(labels['Tirific']['label'],labels['Tirific']['Time']):
+    for label,time in zip(labels_comb,labels_times):
+        if label in labels['Tirific']['label']:
+            offset = 20.
+            xoffset = 0.005*normalize
+            vertical_start = maxy
+            va= 'bottom'
+            ha= 'left'
+            color = 'k'
+            linest = '-'
+        else:
+            offset=-50
+            xoffset = -0.005*normalize
+            vertical_start = miny
+            va= 'top'
+            ha='right'
+            color = '0.5'
+            linest = '--'
+
+
+        if (prev_label == 'Initializing tmp_incl_check' or prev_label == 'Ended tmp_incl_check'):
+            if (label != 'Initializing tmp_incl_check' and label != 'Ended tmp_incl_check') or \
+                    time == labels_times[-1]    :
+
+                if time != labels_times[-1]:
+                    ax.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
+                    if label in labels['Tirific']['label']:
+                        last_label = last_label_top = max(prev_time,last_label_top+label_sep)
+                    else:
+                        last_label = last_label_bottom = max(prev_time,last_label_bottom+label_sep)
+                    ax.text(last_label,vertical_start+offset,prev_label, va=va,ha=ha,rotation= 60, color='black',
+                            bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
+                    ax.plot([prev_time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
+                ax.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
+                if label in labels['Tirific']['label']:
+                    last_label = last_label_top = max(time,last_label_top+label_sep)
+                else:
+                    last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
+                ax.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
+                        bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
+                ax.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
+            else:
+                prev_time = time
+        elif (prev_label == 'Initializing Error_Shaker' or prev_label == 'Ended Error_Shaker' or prev_label == 'Started Error_Shaker'):
+            if (label != 'Initializing Error_Shaker' and label != 'Ended Error_Shaker' and  label != 'Started Error_Shaker') or \
+                    time == labels_times[-1]:
+
+                    #ax2.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
+                    #last_label = max(prev_time,last_label+label_sep)
+                    #ax2.text(last_label,ax2maxy+20.,prev_label, va='bottom',ha='left',rotation= 60, color='black',
+                    #      bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
+                    #ax2.plot([prev_time,last_label+0.1],[ax2maxy,ax2maxy+20.],linest,color=color,linewidth=0.05,clip_on=False)
+                ax.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
+                if label in labels['Tirific']['label']:
+                    last_label = last_label_top = max(time,last_label_top+label_sep)
+                else:
+                    last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
+                ax.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
+                          bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
+                ax.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
+            else:
+                prev_label = label
+                prev_time = time
+        else:
+            ax.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
+          
+            if label in labels['Tirific']['label']:
+                last_label = last_label_top = max(time,last_label_top+label_sep)
+            else:
+                last_label = last_label_bottom= max(time,last_label_bottom+label_sep)
+           
+            #exit()
+            ax.text(last_label,vertical_start+offset,label,va=va,ha=ha,rotation= 60, color='black',
+                      bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
+                #This should be the line to the label
+            ax.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
+        prev_label = label
+
+    ax.set_ylim(miny,maxy)    
+    return ax
+
+set_timing_labels.__doc__ =f'''
+NAME:
+set_timing_labels
+
+PURPOSE:
+Set the timing labels for the various accournces
+
+CATEGORY:
+write_functions
+
+INPUTS:
+Configuration = Standard FAT configuration
+ax = the axis object to attach the labels to
+labels_times = list of label times
+labels_comb = list of labels
+labels = dictionary with all labels split into upper and lower 
+labelfont = label font settings
+normalize = conversion factor from image coordinate to plot
+
+OPTIONAL INPUTS:
+
+
+OUTPUTS:
+ax = label axis object
+
+OPTIONAL OUTPUTS:
+
+PROCEDURES CALLED:
+Unspecified
+
+NOTE:
+'''
 
 def sofia(template,name):
     with open(name,'w') as file:
         for key in template:
             if key[0] == 'E' or key [0] == 'H':
                 file.write(template[key])
             else:
                 file.write(f"{key} = {template[key]}\n")
 
 sofia.__doc__ =f'''
+NAME:
+sofia
+PURPOSE:
+write a sofia2 dictionary into file
+CATEGORY:
+write_functions
+
+INPUTS:
+template = sofia template
+name = name of the file to write to
+
+OPTIONAL INPUTS:
+
+OUTPUTS:
+
+OPTIONAL OUTPUTS:
+
+PROCEDURES CALLED:
+Unspecified
+
+NOTE:
+'''
+
+def square_plot(ax):
+    xmin, xmax = ax.get_xlim()
+    ymin, ymax = ax.get_ylim()
+    if xmax > ymax:
+        diff = int(xmax-ymax)/2.
+        ax.set_ylim(ymin-diff,ymax+diff)
+        ymin, ymax = ax.get_ylim()
+    else:
+        diff = int(ymax-xmax)/2.
+        ax.set_xlim(xmin-diff,xmax+diff)
+        xmin, xmax = ax.get_xlim()
+square_plot.__doc__ =f'''
  NAME:
-    sofia
+    square_plot
+
  PURPOSE:
-    write a sofia2 dictionary into file
+    square the axes object
+        
  CATEGORY:
     write_functions
 
  INPUTS:
-    template = sofia template
-    name = name of the file to write to
-
+    ax = is the axes object to be squared
+        
  OPTIONAL INPUTS:
 
- OUTPUTS:
 
+ OUTPUTS:
+    square axes
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
-    Unspecified
 
  NOTE:
 '''
 
 def tirific(Configuration,Tirific_Template, name = 'tirific.def',\
                 full_name = False  ):
     #IF we're writing we bump up the restart_ID and adjust the AZ1P angles to the current warping
     update_disk_angles(Configuration,Tirific_Template )
     try:
         Tirific_Template['RESTARTID'] = str(int(Tirific_Template['RESTARTID'])+1)
     except ValueError:
+        Tirific_Template['RESTARTID'] = 0 
+    except KeyError:
         Tirific_Template['RESTARTID'] = 0
     if full_name:
         file_name = name
     else:
         file_name = f'{Configuration["FITTING_DIR"]}{name}'
     with open(file_name, 'w') as file:
         for key in Tirific_Template:
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Templates/sofia_template.par` & `pyFAT_astro-0.1.6/pyFAT_astro/Templates/sofia_template.par`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/Templates/template.def` & `pyFAT_astro-0.1.6/pyFAT_astro/Templates/template.def`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/__init__.py` & `pyFAT_astro-0.1.6/pyFAT_astro/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # -*- coding: future_fstrings -*-
 
-import pkg_resources
+
+try:
+    from importlib.metadata import version
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`.
+    # For Py<3.9 files is not available
+    from importlib_metadata import version 
+
 import os
 import subprocess
 
 def report_version():
     # Distutils standard  way to do version numbering
     try:
-        __version__ = pkg_resources.require("pyFAT-astro")[0].version
-    except pkg_resources.DistributionNotFound:
+        __version__ = version("pyFAT-astro")
+    except:
         __version__ = "dev"
     # perhaps we are in a github with tags; in that case return describe
     path = os.path.dirname(os.path.abspath(__file__))
     try:
         # work round possible unavailability of git -C
         result = subprocess.check_output(
             'cd %s; git describe --tags' % path, shell=True, stderr=subprocess.STDOUT).rstrip().decode()
@@ -45,10 +52,10 @@
                 result=branches[i+1]
                 break
     except subprocess.CalledProcessError:
         result= None
     return result
 
 __version__ = report_version()
-__branch__ =report_branch()
+__branch__ = report_branch()
 
 #set_logger_values()
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/config/FAT_Input_Catalogue.txt` & `pyFAT_astro-0.1.6/pyFAT_astro/config/FAT_Input_Catalogue.txt`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/config/defaults.py` & `pyFAT_astro-0.1.6/pyFAT_astro/config/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 @dataclass
 class Input:
     main_directory: str = f'{os.getcwd()}'
     # 'Options are independent, sinusoidal, hanning
     channel_dependency: str = 'independent'
     catalogue: Optional[str] = None
     tirific: str = "tirific"  # Command to call tirific
-    sofia2: str = "sofia2"  # Command to call sofia 2
+    sofia2: str = "sofia"  # Command to call sofia 2
     sofia_basename: Optional[str] = None
     # Directory of the existing Sofia output. Only used if the input catalogue is sofia or pre-processed sofia is somewhere
     sofia_dir: Optional[str] = None
 
 
 @dataclass
 class Output:
@@ -77,14 +77,17 @@
     # we need at least this amount of rings (Including 0 and 1/5 beam), set here
     minimum_rings: int = 3
     too_small_galaxy: float = 1.  # if the number of beams across the major axis/2 is less than this we will not fit the galaxy, set here
     unreliable_size: float = 2.  # If the final diameter is smaller than this the fit is considered unreliable
     unreliable_inclination: float = 10.  # If the final inclination is below this the fit is considered unreliable
     shaker_iterations: int = 20
     multiprocessing: bool = True
+    number_of_disks: int = 2
+    # The whole mechanism beheind the sbr_limits (which weigh the smoothing) is emperically determined. They are multiplied with this factor to allow optimization
+    limit_modifier_factor: float = 1.05
     #We do not want to use too many cores per galaxy.
     per_galaxy_ncpu: int = 4
     catalogue_split_character: str = '|'
     # Allow for the user to set the boundaries in the fitting
     pa_input_boundary:  List = field(
         default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
     incl_input_boundary:  List = field(
@@ -102,24 +105,33 @@
     vrot_input_boundary: List = field(
         default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
     sbr_input_boundary: List = field(
         default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
     # The brightest pixels need to have a SNR above this value
     source_max_snr: float = 2.5
     # The fraction of pixels in the source that need to be above max_snr
-    source_max_fraction: float = 0.1
+    source_max_fraction: float = 0.075
     # The mean SNR required in the source
     source_mean_snr: float = 0.75
-
+    sofia_threshold: int = 5
+    #option to bypass all initial checks on the intial sofia source and simply force the TRM fitting
+    force_fit: bool = False
     # Add the channel dependency, minimum inclination,
+    debug_function: List = field(default_factory=lambda: ['ALL'] )
 
+    # If we are using a sofia catalogue and want tor overwrite the create FAT Cubes
+    sofia_overwrite: bool = False
 
 @dataclass
 class defaults:
-    ncpu: int = len(psutil.Process().cpu_affinity())
+    try:
+        ncpu: int = len(psutil.Process().cpu_affinity())
+    except AttributeError:
+        ncpu: int = psutil.cpu_count()
+
     print_examples: bool = False
     installation_check: bool = False
     cube_name: Optional[str] = None
     configuration_file: Optional[str] = None
     input: Input = Input()
     output: Output = Output()
     fitting: Fitting = Fitting()
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro/main.py` & `pyFAT_astro-0.1.6/pyFAT_astro/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- coding: future_fstrings -*-
 
 # This is the python version of FAT
-import copy
 import numpy as np
 import os
 import psutil
 import pyFAT_astro
 import pyFAT_astro.Support.support_functions as sf
 import pyFAT_astro.Support.read_functions as rf
-import pyFAT_astro.Support.write_functions as wf
 import sys
 import traceback
 import warnings
 import threading
 
 
 from datetime import datetime
 from multiprocessing import Pool,get_context,Lock,Manager
 from omegaconf import OmegaConf
 from pyFAT_astro.FAT_Galaxy_Loop import FAT_Galaxy_Loop,MP_initialize_sofia,\
                                         MP_Fitting_Loop
 from pyFAT_astro.config.defaults import defaults
-from pyFAT_astro.Support.fat_errors import ProgramError
+from pyFAT_astro.Support.fat_errors import ProgramError,BadCatalogueError
 from pyFAT_astro.Support.write_functions import reorder_output_catalogue
+from pyFAT_astro.Support.log_functions import full_system_tracking
 
 def warn_with_traceback(message, category, filename, lineno, file=None, line=None):
     log = file if hasattr(file,'write') else sys.stderr
     traceback.print_stack(file=log)
     log.write(warnings.formatwarning(message, category, filename, lineno, line))
 try:
     from importlib.resources import files as import_pack_files
@@ -58,17 +57,15 @@
         Use pyFAT in this way for batch fitting:
 
             pyFAT configuration_file=FAT_Input.yml
 
         where configuration_file specifies a yaml file with specific settings
         such as the catalog.
 
-        For fitting global screen
-    screen = False
-    global debuga single galaxy use pyFAT in this way:
+        For fitting use pyFAT in this way:
 
             pyFAT cube_name=Input_Cube.fits
 
         Where Input_Cube.fits is the observation to be fitted. In this mode
         configuration_file can still be used to specify fit settings but
         catalogue and location setting will be ignored.
 
@@ -101,15 +98,16 @@
         if cfg.ncpu == psutil.cpu_count():
             cfg.ncpu -= 1
 
         # read command line arguments anything list input should be set in '' e.g. pyROTMOD 'rotmass.MD=[1.4,True,True]'
         inputconf = OmegaConf.from_cli(argv)
         cfg_input = OmegaConf.merge(cfg,inputconf)
         if cfg_input.print_examples:
-            no_cube = OmegaConf.masked_copy(cfg, ['input','output','fitting'])
+            no_cube = OmegaConf.masked_copy(cfg, ['ncpu','input','output',\
+                'fitting','advanced'])
             with open('FAT_defaults.yml','w') as default_write:
                 default_write.write(OmegaConf.to_yaml(no_cube))
             my_resources = import_pack_files('pyFAT_astro.config')
             data = (my_resources / 'FAT_Input_Catalogue.txt').read_bytes()
             with open('FAT_Example_Catalogue.txt','w+b') as default_write:
                 default_write.write(data)
 
@@ -137,16 +135,20 @@
         cfg = OmegaConf.merge(cfg,inputconf)
 
         if not any([cfg.cube_name, cfg.configuration_file, cfg.installation_check\
                     ,cfg.print_examples,cfg.input.catalogue]):
             print(help_message)
             sys.exit()
         # if we set more cpus than available we limit to the available cpus
-        if cfg.ncpu > len(psutil.Process().cpu_affinity()):
-            cfg.ncpu  = len(psutil.Process().cpu_affinity())
+        try:
+            if cfg.ncpu > len(psutil.Process().cpu_affinity()):
+                cfg.ncpu  = len(psutil.Process().cpu_affinity())
+        except AttributeError:
+            if cfg.ncpu > psutil.cpu_count():
+                cfg.ncpu  = psutil.cpu_count()
 
         #Let's write and input example to the main directory
         if cfg.output.debug:
             with open(f'{cfg.input.main_directory}/FAT_Inputs-Run_{datetime.now().strftime("%d-%m-%Y")}.yml','w') as default_write:
                 default_write.write(OmegaConf.to_yaml(cfg))
 
 
@@ -190,15 +192,15 @@
 
         if Original_Configuration['TIMING']:
 
             with open(Original_Configuration['MAIN_DIRECTORY']+'Timing_Result.txt','w') as timing_result:
                 timing_result.write("Timing results for every section of the fit process for all galaxies.  \n")
             # If we do this we should have 1 cpu to keep going
             Original_Configuration['NCPU'] -= 1
-            system_monitor = wf.full_system_tracking(Original_Configuration)
+            system_monitor = full_system_tracking(Original_Configuration)
             fst = threading.Thread(target=system_monitor.start_monitoring)
             fst.start()
 
             print(f"We are using {Original_Configuration['NCPU']} cpus for fitting and 1 for timing.")
         else:
             print(f"We are using {Original_Configuration['NCPU']} cpus.")
         #if start_galaxy not negative then it is catalogue ID
@@ -211,15 +213,15 @@
             Original_Configuration['CATALOGUE_END_ID'] = int(len(Full_Catalogue['ID']))
             if Original_Configuration['CATALOGUE_END_ID'] == 0:
                 Original_Configuration['CATALOGUE_END_ID'] = 1
         else:
             Original_Configuration['CATALOGUE_END_ID'] = int(np.where(Original_Configuration['CATALOGUE_END_ID'] == np.array(Full_Catalogue['ID'],dtype=str))[0][0])+1
         # start the main fitting loop
         if float(Original_Configuration['CATALOGUE_START_ID']) > float(Original_Configuration['CATALOGUE_END_ID']):
-            raise CatalogError(f''' Your starting galaxy (Line nr = {Original_Configuration['CATALOGUE_START_ID']}) is listed after your ending galaxy (Line nr = {Original_Configuration['CATALOGUE_END_ID']}), maybe you have double catalogue ids?''')
+            raise BadCatalogueError(f''' Your starting galaxy (Line nr = {Original_Configuration['CATALOGUE_START_ID']}) is listed after your ending galaxy (Line nr = {Original_Configuration['CATALOGUE_END_ID']}), maybe you have double catalogue ids?''')
             sys.exit(1)
 
         if Original_Configuration['MULTIPROCESSING']:
             Original_Configuration['VERBOSE_SCREEN'] = False
             #output_catalogue = copy.deepcopy(Original_Configuration['OUTPUT_CATALOGUE'])
             #Original_Configuration['OUTPUT_CATALOGUE'] = None
             no_processes,sofia_processes = sf.calculate_number_processes(Original_Configuration)
@@ -262,14 +264,15 @@
             #        catalogue.writelines(x)
 
         else:
             Original_Configuration['PER_GALAXY_NCPU'] = sf.set_limits(Original_Configuration['NCPU'],1,20)
             for current_galaxy_index in range(Original_Configuration['CATALOGUE_START_ID'], Original_Configuration['CATALOGUE_END_ID']):
                 Configuration = sf.set_individual_configuration(current_galaxy_index,Full_Catalogue,Original_Configuration)
                 catalogue_line = FAT_Galaxy_Loop(Configuration)
+        
         if Original_Configuration['TIMING']:
             system_monitor.stop_monitoring()
             fst.join()
 
     except SystemExit:
         try:
             system_monitor.stop_monitoring()
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro.egg-info/PKG-INFO` & `pyFAT_astro-0.1.6/pyFAT_astro.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyFAT-astro
-Version: 0.1.3
+Name: pyFAT_astro
+Version: 0.1.6
 Summary: Development Status :: 4 - Beta
 Home-page: https://github.com/PeterKamphuis/pyFAT
 Author: P. Kamphuis
 Author-email: peterkamphuisastronomy@gmail.com
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -18,8 +18,11 @@
 Requires-Dist: numpy>=1.14
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: omegaconf>=2.2.2
 Requires-Dist: matplotlib
 Requires-Dist: future-fstrings
 Requires-Dist: psutil
+Requires-Dist: make-moments>=1.0.6
 Requires-Dist: importlib_resources>=3.3.0
+Requires-Dist: importlib_metadata
+Requires-Dist: TRM_errors>=0.0.5
```

### Comparing `pyFAT_astro-0.1.3/pyFAT_astro.egg-info/SOURCES.txt` & `pyFAT_astro-0.1.6/pyFAT_astro.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 pyFAT_astro/Installation_Check/__init__.py
 pyFAT_astro/Support/__init__.py
 pyFAT_astro/Support/clean_functions.py
 pyFAT_astro/Support/constants.py
 pyFAT_astro/Support/development_functions.py
 pyFAT_astro/Support/fat_errors.py
 pyFAT_astro/Support/fits_functions.py
+pyFAT_astro/Support/log_functions.py
 pyFAT_astro/Support/modify_template.py
 pyFAT_astro/Support/read_functions.py
 pyFAT_astro/Support/run_functions.py
 pyFAT_astro/Support/support_functions.py
-pyFAT_astro/Support/tirshaker.py
 pyFAT_astro/Support/write_functions.py
+pyFAT_astro/Templates/TRM_errors_FAT.yml
 pyFAT_astro/Templates/__init__.py
 pyFAT_astro/Templates/sofia_template.par
 pyFAT_astro/Templates/template.def
 pyFAT_astro/config/FAT_Input_Catalogue.txt
 pyFAT_astro/config/__init__.py
 pyFAT_astro/config/defaults.py
```

### Comparing `pyFAT_astro-0.1.3/setup.py` & `pyFAT_astro-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,22 @@
     'numpy>=1.14',
     'scipy',
     'astropy',
     'omegaconf>=2.2.2',
     'matplotlib',
     'future-fstrings',
     'psutil',
+    'make-moments>=1.0.6',
     'importlib_resources>=3.3.0',
+    'importlib_metadata',
+    'TRM_errors>=0.0.5',
 ]
 
 PACKAGE_NAME = 'pyFAT_astro'
-__version__ = 'v0.1.3'
+__version__ = 'v0.1.6'
 
 
 #with open("README.md", "r") as fh:
 #    long_description = fh.read()
 long_description = ""
 
 setup(name=PACKAGE_NAME,
```

