# Comparing `tmp/monviso-0.1.2.tar.gz` & `tmp/monviso-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monviso-0.1.2.tar", last modified: Mon Apr  8 10:29:34 2024, max compression
+gzip compressed data, was "dist/monviso-0.1.2.2.tar", last modified: Mon Apr  8 14:08:31 2024, max compression
```

## Comparing `monviso-0.1.2.tar` & `monviso-0.1.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.823050 monviso-0.1.2/
--rw-r--r--   0 albani     (502) staff       (20)     2161 2024-04-08 10:24:51.000000 monviso-0.1.2/Containerfile
--rw-r--r--   0 albani     (502) staff       (20)      627 2024-04-08 10:27:45.000000 monviso-0.1.2/HISTORY.md
--rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.2/LICENSE
--rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.2/MANIFEST.in
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 10:29:34.818573 monviso-0.1.2/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.2/README.md
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.703784 monviso-0.1.2/monviso.egg-info/
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/SOURCES.txt
--rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/dependency_links.txt
--rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/entry_points.txt
--rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/requires.txt
--rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/top_level.txt
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.739113 monviso-0.1.2/monviso_reloaded/
--rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/PDB_manager.py
--rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-08 10:27:56.000000 monviso-0.1.2/monviso_reloaded/VERSION
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/__main__.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.796839 monviso-0.1.2/monviso_reloaded/__pycache__/
--rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.2/monviso_reloaded/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    11467 2024-04-08 09:23:33.000000 monviso-0.1.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/template.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.2/monviso_reloaded/base.py
--rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/cli.py
--rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/cobalt_wrapper.py
--rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.2/monviso_reloaded/database_parser.py
--rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.2/monviso_reloaded/file_handler.py
--rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.2/monviso_reloaded/gene.py
--rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.2/monviso_reloaded/input_parser.py
--rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.2/monviso_reloaded/isoform.py
--rw-r--r--   0 albani     (502) staff       (20)    13347 2024-04-08 10:25:14.000000 monviso-0.1.2/monviso_reloaded/modeller_manager.py
--rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/template.py
--rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-08 10:29:34.824515 monviso-0.1.2/setup.cfg
--rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.2/setup.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.805141 monviso-0.1.2/tests/
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/conftest.py
--rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/test_base.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:08:31.764334 monviso-0.1.2.2/
+-rw-r--r--   0 albani     (502) staff       (20)     2161 2024-04-08 14:05:56.000000 monviso-0.1.2.2/Containerfile
+-rw-r--r--   0 albani     (502) staff       (20)      650 2024-04-08 14:07:08.000000 monviso-0.1.2.2/HISTORY.md
+-rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.2.2/LICENSE
+-rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.2.2/MANIFEST.in
+-rw-r--r--   0 albani     (502) staff       (20)     2262 2024-04-08 14:08:31.763713 monviso-0.1.2.2/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.2.2/README.md
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:08:31.701909 monviso-0.1.2.2/monviso.egg-info/
+-rw-r--r--   0 albani     (502) staff       (20)     2262 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/SOURCES.txt
+-rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/dependency_links.txt
+-rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/entry_points.txt
+-rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/requires.txt
+-rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-08 14:08:31.000000 monviso-0.1.2.2/monviso.egg-info/top_level.txt
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:08:31.719226 monviso-0.1.2.2/monviso_reloaded/
+-rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/PDB_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)        8 2024-04-08 14:06:17.000000 monviso-0.1.2.2/monviso_reloaded/VERSION
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/__main__.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:08:31.759231 monviso-0.1.2.2/monviso_reloaded/__pycache__/
+-rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    11467 2024-04-08 09:23:33.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.2.2/monviso_reloaded/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.2.2/monviso_reloaded/base.py
+-rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/cli.py
+-rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/cobalt_wrapper.py
+-rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.2.2/monviso_reloaded/database_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.2.2/monviso_reloaded/file_handler.py
+-rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.2.2/monviso_reloaded/gene.py
+-rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.2.2/monviso_reloaded/input_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.2.2/monviso_reloaded/isoform.py
+-rw-r--r--   0 albani     (502) staff       (20)    13275 2024-04-08 14:05:11.000000 monviso-0.1.2.2/monviso_reloaded/modeller_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.2.2/monviso_reloaded/template.py
+-rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-08 14:08:31.764604 monviso-0.1.2.2/setup.cfg
+-rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.2.2/setup.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 14:08:31.762265 monviso-0.1.2.2/tests/
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2.2/tests/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.2.2/tests/conftest.py
+-rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.2.2/tests/test_base.py
```

### Comparing `monviso-0.1.2/Containerfile` & `monviso-0.1.2.2/Containerfile`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/HISTORY.md` & `monviso-0.1.2.2/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Changelog
 =========
 
-0.1.2 (2024-04-08)
------------------
-- Added Containerfile for Docker
+0.1.2.2 (2024-04-08)
 - Fix: Removing sorting of models in Modeller script
   makes the software compatible with the Modeller's
   version in conda
+
+0.1.2 (2024-04-08)
+-----------------
+- Added Containerfile for Docker
 - Fix: Removal of maximum 10 models reported
 
+
 0.1.1 (2024-04-02)
 ------------------
 - Fix: The model now is assigned to chain A
 - Fix: Correct residue number at chain breaks
 - Fix: Alignment, scoring, and filtering is repeated as long as
        the list of templates keeps changing
 - Fix: If mutation can be mapped on sequence, but it is not
```

### Comparing `monviso-0.1.2/LICENSE` & `monviso-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/PKG-INFO` & `monviso-0.1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.2
+Version: 0.1.2.2
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.2/README.md` & `monviso-0.1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso.egg-info/PKG-INFO` & `monviso-0.1.2.2/monviso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.2
+Version: 0.1.2.2
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.2/monviso.egg-info/SOURCES.txt` & `monviso-0.1.2.2/monviso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/PDB_manager.py` & `monviso-0.1.2.2/monviso_reloaded/PDB_manager.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/base.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/__pycache__/template.cpython-39.pyc` & `monviso-0.1.2.2/monviso_reloaded/__pycache__/template.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/base.py` & `monviso-0.1.2.2/monviso_reloaded/base.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/cli.py` & `monviso-0.1.2.2/monviso_reloaded/cli.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/cobalt_wrapper.py` & `monviso-0.1.2.2/monviso_reloaded/cobalt_wrapper.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/database_parser.py` & `monviso-0.1.2.2/monviso_reloaded/database_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/file_handler.py` & `monviso-0.1.2.2/monviso_reloaded/file_handler.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/gene.py` & `monviso-0.1.2.2/monviso_reloaded/gene.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/input_parser.py` & `monviso-0.1.2.2/monviso_reloaded/input_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/isoform.py` & `monviso-0.1.2.2/monviso_reloaded/isoform.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/monviso_reloaded/modeller_manager.py` & `monviso-0.1.2.2/monviso_reloaded/modeller_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     assess_methods=(assess.DOPE, assess.GA341))
 a.starting_model= 1
 a.ending_model  = """+str(self.num_models)+"""
 a.make()
 ok_models = filter(lambda x: x['failure'] is None, a.outputs)
 toscore = 'DOPE score'
 
-models= list(ok_models) if isinstance(ok_models, type(filter(lambda: None, []))) else ok_models
+models= list(ok_models)
 models.sort(lambda k: k[toscore])
 
 myout = open(\""""
             + output_name
             + """\", "w")
 for m in models:
         myout.write(str(m['name']) + " (DOPE SCORE: %.3f)" % (m[toscore]))
```

### Comparing `monviso-0.1.2/monviso_reloaded/template.py` & `monviso-0.1.2.2/monviso_reloaded/template.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.2/setup.py` & `monviso-0.1.2.2/setup.py`

 * *Files identical despite different names*

