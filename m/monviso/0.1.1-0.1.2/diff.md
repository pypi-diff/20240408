# Comparing `tmp/monviso-0.1.1.tar.gz` & `tmp/monviso-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monviso-0.1.1.tar", last modified: Tue Apr  2 13:10:01 2024, max compression
+gzip compressed data, was "dist/monviso-0.1.2.tar", last modified: Mon Apr  8 10:29:34 2024, max compression
```

## Comparing `monviso-0.1.1.tar` & `monviso-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.078699 monviso-0.1.1/
--rw-r--r--   0 albani     (502) staff       (20)       89 2024-02-28 10:12:03.000000 monviso-0.1.1/Containerfile
--rw-r--r--   0 albani     (502) staff       (20)      388 2024-04-02 13:03:27.000000 monviso-0.1.1/HISTORY.md
--rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.1/LICENSE
--rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.1/MANIFEST.in
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-02 13:10:01.078213 monviso-0.1.1/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.1/README.md
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.042437 monviso-0.1.1/monviso.egg-info/
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/SOURCES.txt
--rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/dependency_links.txt
--rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/entry_points.txt
--rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/requires.txt
--rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-02 13:10:00.000000 monviso-0.1.1/monviso.egg-info/top_level.txt
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.058065 monviso-0.1.1/monviso_reloaded/
--rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/PDB_manager.py
--rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-02 12:58:34.000000 monviso-0.1.1/monviso_reloaded/VERSION
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/__main__.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.074242 monviso-0.1.1/monviso_reloaded/__pycache__/
--rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.1/monviso_reloaded/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.1/monviso_reloaded/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.1/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.1/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.1/monviso_reloaded/__pycache__/gene.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.1/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.1/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    11425 2024-03-29 16:19:47.000000 monviso-0.1.1/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.1/monviso_reloaded/__pycache__/template.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.1/monviso_reloaded/base.py
--rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/cli.py
--rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/cobalt_wrapper.py
--rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.1/monviso_reloaded/database_parser.py
--rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.1/monviso_reloaded/file_handler.py
--rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.1/monviso_reloaded/gene.py
--rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.1/monviso_reloaded/input_parser.py
--rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.1/monviso_reloaded/isoform.py
--rw-r--r--   0 albani     (502) staff       (20)    13309 2024-03-29 16:18:28.000000 monviso-0.1.1/monviso_reloaded/modeller_manager.py
--rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.1/monviso_reloaded/template.py
--rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-02 13:10:01.078858 monviso-0.1.1/setup.cfg
--rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.1/setup.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-02 13:10:01.077170 monviso-0.1.1/tests/
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/conftest.py
--rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.1/tests/test_base.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.823050 monviso-0.1.2/
+-rw-r--r--   0 albani     (502) staff       (20)     2161 2024-04-08 10:24:51.000000 monviso-0.1.2/Containerfile
+-rw-r--r--   0 albani     (502) staff       (20)      627 2024-04-08 10:27:45.000000 monviso-0.1.2/HISTORY.md
+-rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.2/LICENSE
+-rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.2/MANIFEST.in
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 10:29:34.818573 monviso-0.1.2/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.2/README.md
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.703784 monviso-0.1.2/monviso.egg-info/
+-rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/SOURCES.txt
+-rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/dependency_links.txt
+-rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/entry_points.txt
+-rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/requires.txt
+-rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-08 10:29:34.000000 monviso-0.1.2/monviso.egg-info/top_level.txt
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.739113 monviso-0.1.2/monviso_reloaded/
+-rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/PDB_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-08 10:27:56.000000 monviso-0.1.2/monviso_reloaded/VERSION
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/__main__.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.796839 monviso-0.1.2/monviso_reloaded/__pycache__/
+-rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.2/monviso_reloaded/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    11467 2024-04-08 09:23:33.000000 monviso-0.1.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.2/monviso_reloaded/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.2/monviso_reloaded/base.py
+-rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/cli.py
+-rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/cobalt_wrapper.py
+-rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.2/monviso_reloaded/database_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.2/monviso_reloaded/file_handler.py
+-rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.2/monviso_reloaded/gene.py
+-rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.2/monviso_reloaded/input_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.2/monviso_reloaded/isoform.py
+-rw-r--r--   0 albani     (502) staff       (20)    13347 2024-04-08 10:25:14.000000 monviso-0.1.2/monviso_reloaded/modeller_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.2/monviso_reloaded/template.py
+-rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-08 10:29:34.824515 monviso-0.1.2/setup.cfg
+-rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.2/setup.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-08 10:29:34.805141 monviso-0.1.2/tests/
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/conftest.py
+-rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.2/tests/test_base.py
```

### Comparing `monviso-0.1.1/LICENSE` & `monviso-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/PKG-INFO` & `monviso-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.1
+Version: 0.1.2
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.1/README.md` & `monviso-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso.egg-info/PKG-INFO` & `monviso-0.1.2/monviso.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.1
+Version: 0.1.2
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
 Author: Ciskio
 License: UNKNOWN
 Description: # Monviso reloaded
         MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
```

### Comparing `monviso-0.1.1/monviso.egg-info/SOURCES.txt` & `monviso-0.1.2/monviso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/PDB_manager.py` & `monviso-0.1.2/monviso_reloaded/PDB_manager.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/base.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/cli.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/gene.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/gene.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/isoform.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/isoform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar 29 16:18:28 2024 UTC, .py size: 13309 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 d4e9 0666 fd33 0000  a..........f.3..
+00000000: 610d 0d0a 0000 0000 80b7 1366 2734 0000  a..........f'4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6403 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000060: 8302 5a06 6401 5300 2907 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da04 5061 7468 e901 0000 0029 01da  )...Path.....)..
@@ -221,495 +221,497 @@
 00000dc0: 6b6e 6f77 6e73 203d 2028 7a13 292c 0a20  knowns = (z.),. 
 00000dd0: 2020 2073 6571 7565 6e63 6520 3d20 227a     sequence = "z
 00000de0: 5922 2c0a 2020 2020 6173 7365 7373 5f6d  Y",.    assess_m
 00000df0: 6574 686f 6473 3d28 6173 7365 7373 2e44  ethods=(assess.D
 00000e00: 4f50 452c 2061 7373 6573 732e 4741 3334  OPE, assess.GA34
 00000e10: 3129 290a 612e 7374 6172 7469 6e67 5f6d  1)).a.starting_m
 00000e20: 6f64 656c 3d20 310a 612e 656e 6469 6e67  odel= 1.a.ending
-00000e30: 5f6d 6f64 656c 2020 3d20 7acb 0a61 2e6d  _model  = z..a.m
+00000e30: 5f6d 6f64 656c 2020 3d20 7af5 0a61 2e6d  _model  = z..a.m
 00000e40: 616b 6528 290a 6f6b 5f6d 6f64 656c 7320  ake().ok_models 
 00000e50: 3d20 6669 6c74 6572 286c 616d 6264 6120  = filter(lambda 
 00000e60: 783a 2078 5b27 6661 696c 7572 6527 5d20  x: x['failure'] 
 00000e70: 6973 204e 6f6e 652c 2061 2e6f 7574 7075  is None, a.outpu
 00000e80: 7473 290a 746f 7363 6f72 6520 3d20 2744  ts).toscore = 'D
-00000e90: 4f50 4520 7363 6f72 6527 0a6f 6b5f 6d6f  OPE score'.ok_mo
-00000ea0: 6465 6c73 203d 2073 6f72 7465 6428 6f6b  dels = sorted(ok
-00000eb0: 5f6d 6f64 656c 732c 206b 6579 3d6c 616d  _models, key=lam
-00000ec0: 6264 6120 6b3a 206b 5b74 6f73 636f 7265  bda k: k[toscore
-00000ed0: 5d29 0a6d 6f64 656c 7320 3d20 5b6d 2066  ]).models = [m f
-00000ee0: 6f72 206d 2069 6e20 6f6b 5f6d 6f64 656c  or m in ok_model
-00000ef0: 735b 303a 3130 5d5d 0a6d 796f 7574 203d  s[0:10]].myout =
-00000f00: 206f 7065 6e28 2261 3401 0000 222c 2022   open("a4...", "
-00000f10: 7722 290a 666f 7220 6d20 696e 206d 6f64  w").for m in mod
-00000f20: 656c 733a 0a20 2020 2020 2020 206d 796f  els:.        myo
-00000f30: 7574 2e77 7269 7465 2873 7472 286d 5b27  ut.write(str(m['
-00000f40: 6e61 6d65 275d 2920 2b20 2220 2844 4f50  name']) + " (DOP
-00000f50: 4520 5343 4f52 453a 2025 2e33 6629 2220  E SCORE: %.3f)" 
-00000f60: 2520 286d 5b74 6f73 636f 7265 5d29 290a  % (m[toscore])).
-00000f70: 656e 762e 6c69 6273 2e74 6f70 6f6c 6f67  env.libs.topolog
-00000f80: 792e 7265 6164 2866 696c 653d 2724 284c  y.read(file='$(L
-00000f90: 4942 292f 746f 705f 6865 6176 2e6c 6962  IB)/top_heav.lib
-00000fa0: 2729 0a65 6e76 2e6c 6962 732e 7061 7261  ').env.libs.para
-00000fb0: 6d65 7465 7273 2e72 6561 6428 6669 6c65  meters.read(file
-00000fc0: 3d27 2428 4c49 4229 2f70 6172 2e6c 6962  ='$(LIB)/par.lib
-00000fd0: 2729 0a6d 646c 203d 2063 6f6d 706c 6574  ').mdl = complet
-00000fe0: 655f 7064 6228 656e 762c 206d 5b27 6e61  e_pdb(env, m['na
-00000ff0: 6d65 275d 290a 7320 3d20 7365 6c65 6374  me']).s = select
-00001000: 696f 6e28 6d64 6c29 0a73 2e61 7373 6573  ion(mdl).s.asses
-00001010: 735f 646f 7065 286f 7574 7075 743d 2745  s_dope(output='E
-00001020: 4e45 5247 595f 5052 4f46 494c 4520 4e4f  NERGY_PROFILE NO
-00001030: 5f52 4550 4f52 5427 2c20 6669 6c65 3d22  _REPORT', file="
-00001040: 7a2f 222c 206e 6f72 6d61 6c69 7a65 5f70  z/", normalize_p
-00001050: 726f 6669 6c65 3d54 7275 652c 2073 6d6f  rofile=True, smo
-00001060: 6f74 6869 6e67 5f77 696e 646f 773d 3135  othing_window=15
-00001070: 2929 0e72 1300 0000 7206 0000 0072 0200  )).r....r....r..
-00001080: 0000 720d 0000 00da 086f 7574 5f70 6174  ..r......out_pat
-00001090: 68da 0974 656d 706c 6174 6573 da03 7374  h..templates..st
-000010a0: 72da 0572 616e 6765 7210 0000 0072 1100  r..ranger....r..
-000010b0: 0000 721b 0000 0072 1400 0000 7204 0000  ..r....r....r...
-000010c0: 00da 0a77 7269 7465 5f66 696c 6529 0772  ...write_file).r
-000010d0: 1500 0000 da0e 616c 6967 6e6d 656e 745f  ......alignment_
-000010e0: 6e61 6d65 5a0b 6f75 7470 7574 5f6e 616d  nameZ.output_nam
-000010f0: 65da 0b73 6372 6970 745f 7061 7468 5a0e  e..script_pathZ.
-00001100: 7465 6d70 6c61 7465 5f6e 616d 6573 da07  template_names..
-00001110: 636f 6e74 656e 74da 0266 6872 1600 0000  content..fhr....
-00001120: 7216 0000 0072 1700 0000 721e 0000 003e  r....r....r....>
-00001130: 0000 0073 5a00 0000 0001 1401 1401 0201  ...sZ...........
-00001140: 0601 12fe 0404 0602 06fe 0605 0207 16f9  ................
-00001150: 0207 02f9 0208 08f8 0208 02f8 0210 02f0  ................
-00001160: 0211 02ef 0213 06ed 0214 02ec 0216 06ea  ................
-00001170: 0217 02e9 021a 08e6 021a 02e6 0221 02df  .............!..
-00001180: 0222 02de 022a 06d6 022b 02d5 02ff 022f  ."...*...+...../
-00001190: 0801 7a1d 4d6f 6465 6c6c 6572 5f6d 616e  ..z.Modeller_man
-000011a0: 6167 6572 2e77 7269 7465 5f73 6372 6970  ager.write_scrip
-000011b0: 7429 0272 2a00 0000 7220 0000 0063 0300  t).r*...r ...c..
-000011c0: 0000 0000 0000 0000 0000 0500 0000 0400  ................
-000011d0: 0000 4300 0000 73a8 0000 007c 0164 016b  ..C...s....|.d.k
-000011e0: 0272 0c7c 0253 0074 007c 0164 0219 0083  .r.|.S.t.|.d....
-000011f0: 0164 0218 007d 037c 0374 017c 0283 016b  .d...}.|.t.|...k
-00001200: 0072 947c 037c 0264 037c 0385 0219 00a0  .r.|.|.d.|......
-00001210: 0264 04a1 0118 007d 047c 0464 0217 0074  .d.....}.|.d...t
-00001220: 007c 0164 0219 0083 016b 0272 8a7c 027c  .|.d.....k.r.|.|
-00001230: 0319 007c 0164 0519 006b 0272 8a7c 0264  ...|.d...k.r.|.d
-00001240: 037c 0385 0219 007c 0164 0619 0017 007c  .|.....|.d.....|
-00001250: 027c 0364 0217 0064 0385 0219 0017 007d  .|.d...d.......}
-00001260: 027c 0253 007c 0364 0237 007d 0371 1c74  .|.S.|.d.7.}.q.t
-00001270: 0364 077c 019b 0064 089d 0383 0101 007c  .d.|...d.......|
-00001280: 0253 0029 097a ea54 616b 6520 6120 6d75  .S.).z.Take a mu
-00001290: 7461 7469 6f6e 2069 6e20 7468 6520 666f  tation in the fo
-000012a0: 726d 6174 0a20 2020 2020 2020 205b 3120  rmat.        [1 
-000012b0: 6c65 7474 6572 2061 6d69 6e6f 2061 6369  letter amino aci
-000012c0: 642c 7265 7369 6475 6520 6e75 6d62 6572  d,residue number
-000012d0: 2c20 3120 6c65 7474 2e20 616d 696e 6f20  , 1 lett. amino 
-000012e0: 6163 6964 5d0a 2020 2020 2020 2020 616e  acid].        an
-000012f0: 6420 6170 706c 7920 6974 2074 6f20 7468  d apply it to th
-00001300: 6520 616c 6967 6e65 6420 7365 7175 656e  e aligned sequen
-00001310: 6365 2074 6f20 6d6f 6465 6c2c 0a20 2020  ce to model,.   
-00001320: 2020 2020 2074 616b 696e 6720 696e 746f       taking into
-00001330: 2061 6363 6f75 6e74 2061 6c6c 2074 6865   account all the
-00001340: 2022 2d22 2773 2e0a 0a20 2020 2020 2020   "-"'s...       
-00001350: 2052 6574 7572 6e73 2065 6469 7465 6420   Returns edited 
-00001360: 7365 7175 656e 6365 0a20 2020 2020 2020  sequence.       
-00001370: 2072 0c00 0000 7203 0000 004e fa01 2d72   r....r....N..-r
-00001380: 0100 0000 e902 0000 007a 1943 6f75 6c64  .........z.Could
-00001390: 206e 6f74 2061 7070 6c79 206d 7574 6174   not apply mutat
-000013a0: 696f 6e20 fa01 2129 0472 2700 0000 da03  ion ..!).r'.....
-000013b0: 6c65 6eda 0563 6f75 6e74 721a 0000 0029  len..countr....)
-000013c0: 0572 1500 0000 7206 0000 0072 2a00 0000  .r....r....r*...
-000013d0: 7236 0000 005a 1461 6374 7561 6c5f 7265  r6...Z.actual_re
-000013e0: 7369 6475 655f 696e 6465 7872 1600 0000  sidue_indexr....
-000013f0: 7216 0000 0072 1700 0000 da0e 5f6d 7574  r....r......_mut
-00001400: 6174 655f 7265 7369 6465 7b00 0000 7326  ate_reside{...s&
-00001410: 0000 0000 0908 0104 0310 010c 0116 0212  ................
-00001420: ff02 020e fe02 040a 0106 ff02 020e fe02  ................
-00001430: ff02 0504 010a 0210 017a 1f4d 6f64 656c  .........z.Model
-00001440: 6c65 725f 6d61 6e61 6765 722e 5f6d 7574  ler_manager._mut
-00001450: 6174 655f 7265 7369 6465 6302 0000 0000  ate_residec.....
-00001460: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
-00001470: 0000 0073 4400 0000 6700 7d02 6401 7d03  ...sD...g.}.d.}.
-00001480: 7c01 4400 5d32 7d04 7c04 6402 6b02 7228  |.D.]2}.|.d.k.r(
-00001490: 7c02 a000 6402 7c04 6702 a101 0100 710c  |...d.|.g.....q.
-000014a0: 7c02 a000 7c03 7c04 6702 a101 0100 7c03  |...|.|.g.....|.
-000014b0: 6401 3700 7d03 710c 7c02 5300 2903 7a37  d.7.}.q.|.S.).z7
-000014c0: 4672 6f6d 2061 2073 6571 7565 6e63 652c  From a sequence,
-000014d0: 2072 6574 7572 6e20 6120 3244 206c 6973   return a 2D lis
-000014e0: 7420 7769 7468 205b 7265 736e 756d 2c72  t with [resnum,r
-000014f0: 6573 6975 6465 5d72 0300 0000 7240 0000  esiude]r....r@..
-00001500: 0029 0172 2900 0000 2905 7215 0000 0072  .).r)...).r....r
-00001510: 2a00 0000 5a0c 6e75 6d62 6572 6564 5f73  *...Z.numbered_s
-00001520: 6571 7236 0000 00da 0463 6861 7272 1600  eqr6.....charr..
-00001530: 0000 7216 0000 0072 1700 0000 da17 5f61  ..r....r......_a
-00001540: 6464 5f6e 756d 6265 725f 746f 5f73 6571  dd_number_to_seq
-00001550: 7565 6e63 6599 0000 0073 1000 0000 0002  uence....s......
-00001560: 0401 0401 0801 0801 1002 0e01 0a01 7a28  ..............z(
-00001570: 4d6f 6465 6c6c 6572 5f6d 616e 6167 6572  Modeller_manager
-00001580: 2e5f 6164 645f 6e75 6d62 6572 5f74 6f5f  ._add_number_to_
-00001590: 7365 7175 656e 6365 4e29 02da 1473 6571  sequenceN)...seq
-000015a0: 7565 6e63 655f 7769 7468 5f72 6573 6e75  uence_with_resnu
-000015b0: 6d72 2000 0000 6302 0000 0000 0000 0000  mr ...c.........
-000015c0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-000015d0: 6200 0000 6401 6402 8400 7c01 4400 8301  b...d.d...|.D...
-000015e0: 7d02 7c00 6a00 a001 7c02 6403 1900 a101  }.|.j...|.d.....
-000015f0: 0100 7402 6404 7403 7c02 8301 8302 4400  ..t.d.t.|.....D.
-00001600: 5d30 7d03 7c02 7c03 1900 7c02 7c03 6404  ]0}.|.|...|.|.d.
-00001610: 1800 1900 6404 1700 6b03 722c 7c00 6a00  ....d...k.r,|.j.
-00001620: a001 7c02 7c03 1900 6404 1800 a101 0100  ..|.|...d.......
-00001630: 712c 6405 5300 2906 7aa7 4769 7665 6e20  q,d.S.).z.Given 
-00001640: 6120 7365 7175 656e 6365 2073 6176 6564  a sequence saved
-00001650: 2061 7320 6120 6c69 7374 205b 7265 736e   as a list [resn
-00001660: 756d 2c20 7265 7369 6475 655d 2c0a 2020  um, residue],.  
-00001670: 2020 2020 2020 7361 7665 2061 6c6c 2074        save all t
-00001680: 6865 2072 6573 6964 7565 206e 756d 6265  he residue numbe
-00001690: 7273 2074 6861 7420 7265 7072 6573 656e  rs that represen
-000016a0: 7420 616e 2069 6e74 6572 7275 7074 696f  t an interruptio
-000016b0: 6e0a 2020 2020 2020 2020 696e 2074 6865  n.        in the
-000016c0: 2063 6f6e 7469 6e75 6974 7920 6f66 2074   continuity of t
-000016d0: 6865 2070 726f 7465 696e 2063 6861 696e  he protein chain
-000016e0: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
-000016f0: 0000 0400 0000 5300 0000 7320 0000 0067  ......S...s ...g
-00001700: 007c 005d 187d 017c 0164 0019 0064 016b  .|.].}.|.d...d.k
-00001710: 0372 047c 0164 0019 0091 0271 0453 0029  .r.|.d.....q.S.)
-00001720: 0272 0100 0000 7240 0000 0072 1600 0000  .r....r@...r....
-00001730: 7222 0000 0072 1600 0000 7216 0000 0072  r"...r....r....r
-00001740: 1700 0000 7225 0000 00ab 0000 0072 2600  ....r%.......r&.
-00001750: 0000 7a37 4d6f 6465 6c6c 6572 5f6d 616e  ..z7Modeller_man
-00001760: 6167 6572 2e5f 7361 7665 5f63 6861 696e  ager._save_chain
-00001770: 5f73 7461 7274 732e 3c6c 6f63 616c 733e  _starts.<locals>
-00001780: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
-00001790: 7203 0000 004e 2904 7211 0000 0072 2900  r....N).r....r).
-000017a0: 0000 723a 0000 0072 4300 0000 2904 7215  ..r:...rC...).r.
-000017b0: 0000 0072 4800 0000 5a10 6669 6c74 6572  ...rH...Z.filter
-000017c0: 6564 5f6e 756d 6265 7273 7236 0000 0072  ed_numbersr6...r
-000017d0: 1600 0000 7216 0000 0072 1700 0000 da12  ....r....r......
-000017e0: 5f73 6176 655f 6368 6169 6e5f 7374 6172  _save_chain_star
-000017f0: 7473 a500 0000 730a 0000 0000 060e 0310  ts....s.........
-00001800: 0212 0118 017a 234d 6f64 656c 6c65 725f  .....z#Modeller_
-00001810: 6d61 6e61 6765 722e 5f73 6176 655f 6368  manager._save_ch
-00001820: 6169 6e5f 7374 6172 7473 2902 da09 7365  ain_starts)...se
-00001830: 7175 656e 6365 7372 2000 0000 6302 0000  quencesr ...c...
-00001840: 0000 0000 0000 0000 0009 0000 0006 0000  ................
-00001850: 0003 0000 0073 ba01 0000 6401 6402 8400  .....s....d.d...
-00001860: 7c01 4400 8301 8902 6403 6402 8400 7c01  |.D.....d.d...|.
-00001870: 4400 8301 8900 7c00 a000 8800 6404 1900  D.....|.....d...
-00001880: a101 7d02 7401 6405 6402 8400 8800 4400  ..}.t.d.d.....D.
-00001890: 8301 8301 8901 8801 7c00 6a02 6b05 9001  ........|.j.k...
-000018a0: 723e 8701 6601 6406 6402 8408 8800 6407  r>..f.d.d.....d.
-000018b0: 6408 8502 1900 4400 8301 7d03 7403 7c03  d.....D...}.t.|.
-000018c0: 8301 7404 8800 8301 6407 1800 6b02 9001  ..t.....d...k...
-000018d0: 7234 8701 6601 6409 6402 8408 8800 6407  r4..f.d.d.....d.
-000018e0: 6408 8502 1900 4400 8301 7d04 7c04 4400  d.....D...}.|.D.
-000018f0: 5d9c 8903 8701 8703 6602 640a 6402 8408  ].......f.d.d...
-00001900: 8800 6407 6408 8502 1900 4400 8301 7d05  ..d.d.....D...}.
-00001910: 7403 7c05 8301 7404 8800 8301 6407 1800  t.|...t.....d...
-00001920: 6b02 7296 7c02 6408 8803 8502 1900 7c02  k.r.|.d.......|.
-00001930: 8803 8801 1700 6408 8502 1900 1700 7d02  ......d.......}.
-00001940: 7405 8800 8301 4400 5d3a 5c02 7d06 7d07  t.....D.]:\.}.}.
-00001950: 7c07 6408 8803 8502 1900 640b 1700 7c07  |.d.......d...|.
-00001960: 8803 8801 1700 6408 8502 1900 1700 8800  ......d.........
-00001970: 7c06 3c00 7c00 0400 6a06 6407 3700 0200  |.<.|...j.d.7...
-00001980: 5f06 71ee 8801 6407 3700 8901 7196 8801  _.q...d.7...q...
-00001990: 6407 3800 8901 713c 8700 8702 6602 640c  d.8...q<....f.d.
-000019a0: 6402 8408 7407 7404 8802 8301 8301 4400  d...t.t.......D.
-000019b0: 8301 7d01 7c01 6404 1900 6407 1900 6404  ..}.|.d...d...d.
-000019c0: 1900 640b 6b02 9001 727e 640d 6402 8400  ..d.k...r~d.d...
-000019d0: 7c01 4400 8301 7d01 7c01 6404 1900 6407  |.D...}.|.d...d.
-000019e0: 1900 640e 1900 640b 6b02 9001 72a2 640f  ..d...d.k...r.d.
-000019f0: 6402 8400 7c01 4400 8301 7d01 7c00 a008  d...|.D...}.|...
-00001a00: 7c02 a101 0100 7c00 a009 7c02 a101 7d08  |.....|...|...}.
-00001a10: 7c01 5300 2910 619f 0100 0046 6f72 2061  |.S.).a....For a
-00001a20: 6c69 676e 6d65 6e74 7320 696e 2077 6869  lignments in whi
-00001a30: 6368 2074 6865 7265 2069 7320 6e6f 2063  ch there is no c
-00001a40: 6f76 6572 6167 6520 666f 7220 7365 6c66  overage for self
-00001a50: 2e6d 6f64 656c 5f63 7574 6f66 662b 0a20  .model_cutoff+. 
-00001a60: 2020 2020 2020 2072 6573 6964 7565 732c         residues,
-00001a70: 2074 6865 2073 6563 7469 6f6e 2077 6974   the section wit
-00001a80: 686f 7574 2063 6f76 6572 6167 6520 6973  hout coverage is
-00001a90: 2072 6570 6c61 6365 6420 6279 0a20 2020   replaced by.   
-00001aa0: 2020 2020 2063 6861 696e 2062 7265 616b       chain break
-00001ab0: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-00001ac0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001ad0: 7175 656e 6365 7320 286c 6973 7429 3a20  quences (list): 
-00001ae0: 4120 6c69 7374 206f 6620 5b6e 616d 652c  A list of [name,
-00001af0: 2073 6571 7565 6e63 655d 206c 6973 7473   sequence] lists
-00001b00: 2c0a 2020 2020 2020 2020 2020 2020 6f6e  ,.            on
-00001b10: 6520 666f 7220 6561 6368 2073 6571 7565  e for each seque
-00001b20: 6e63 6520 746f 2062 6520 7772 6974 7465  nce to be writte
-00001b30: 6e20 696e 2074 6865 206d 6f64 656c 6c65  n in the modelle
-00001b40: 720a 2020 2020 2020 2020 2020 2020 616c  r.            al
-00001b50: 6967 6e6d 656e 7420 696e 7075 7420 6669  ignment input fi
-00001b60: 6c65 2e0a 0a20 2020 2020 2020 2052 6574  le...        Ret
-00001b70: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00001b80: 2020 6c69 7374 3a20 5265 7475 726e 7320    list: Returns 
-00001b90: 7468 6520 7361 6d65 206c 6973 742c 2077  the same list, w
-00001ba0: 6974 6820 6368 6169 6e20 6272 6561 6b73  ith chain breaks
-00001bb0: 2e0a 2020 2020 2020 2020 6301 0000 0000  ..        c.....
-00001bc0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00001bd0: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00001be0: 7c01 6400 1900 9102 7104 5300 7221 0000  |.d.....q.S.r!..
-00001bf0: 0072 1600 0000 a902 7223 0000 00da 066f  .r......r#.....o
-00001c00: 626a 6563 7472 1600 0000 7216 0000 0072  bjectr....r....r
-00001c10: 1700 0000 7225 0000 00c3 0000 0072 2600  ....r%.......r&.
-00001c20: 0000 7a36 4d6f 6465 6c6c 6572 5f6d 616e  ..z6Modeller_man
-00001c30: 6167 6572 2e5f 6164 645f 6368 6169 6e5f  ager._add_chain_
-00001c40: 6272 6561 6b73 2e3c 6c6f 6361 6c73 3e2e  breaks.<locals>.
-00001c50: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-00001c60: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00001c70: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00001c80: 7c01 6400 1900 9102 7104 5300 2901 7203  |.d.....q.S.).r.
-00001c90: 0000 0072 1600 0000 724b 0000 0072 1600  ...r....rK...r..
-00001ca0: 0000 7216 0000 0072 1700 0000 7225 0000  ..r....r....r%..
-00001cb0: 00c4 0000 0072 2600 0000 7201 0000 0063  .....r&...r....c
-00001cc0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001cd0: 0500 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
-00001ce0: 005d 0e7d 017c 01a0 0064 00a1 0191 0271  .].}.|...d.....q
-00001cf0: 0453 00a9 0172 4000 0000 2901 7244 0000  .S...r@...).rD..
-00001d00: 00a9 0272 2300 0000 da03 7365 7172 1600  ...r#.....seqr..
-00001d10: 0000 7216 0000 0072 1700 0000 7225 0000  ..r....r....r%..
-00001d20: 00c9 0000 0072 2600 0000 6301 0000 0000  .....r&...c.....
-00001d30: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-00001d40: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
-00001d50: 6400 8800 1400 7c01 7600 9102 7104 5300  d.....|.v...q.S.
-00001d60: 724d 0000 0072 1600 0000 724e 0000 00a9  rM...r....rN....
-00001d70: 01da 0f6d 6178 5f6e 6f6e 5f63 6f76 6572  ...max_non_cover
-00001d80: 6564 7216 0000 0072 1700 0000 7225 0000  edr....r....r%..
-00001d90: 00d1 0000 0073 0200 0000 0601 7203 0000  .....s......r...
-00001da0: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00001db0: 0000 0006 0000 0013 0000 0073 1a00 0000  ...........s....
-00001dc0: 6700 7c00 5d12 7d01 7c01 a000 6400 8800  g.|.].}.|...d...
-00001dd0: 1400 a101 9102 7104 5300 724d 0000 0029  ......q.S.rM...)
-00001de0: 01da 0466 696e 6472 4e00 0000 7250 0000  ...findrN...rP..
-00001df0: 0072 1600 0000 7217 0000 0072 2500 0000  .r....r....r%...
-00001e00: da00 0000 7302 0000 0006 0163 0100 0000  ....s......c....
-00001e10: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00001e20: 1300 0000 7324 0000 0067 007c 005d 1c7d  ....s$...g.|.].}
-00001e30: 017c 0188 0188 0188 0017 0085 0219 0064  .|.............d
-00001e40: 0088 0014 006b 0291 0271 0453 0072 4d00  .....k...q.S.rM.
-00001e50: 0000 7216 0000 0072 4e00 0000 2902 7251  ..r....rN...).rQ
-00001e60: 0000 00da 0370 6f73 7216 0000 0072 1700  .....posr....r..
-00001e70: 0000 7225 0000 00de 0000 0073 0800 0000  ..r%.......s....
-00001e80: 0603 02fe 0e01 06ff fa01 2f63 0100 0000  ........../c....
-00001e90: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001ea0: 1300 0000 731c 0000 0067 007c 005d 147d  ....s....g.|.].}
-00001eb0: 0188 017c 0119 0088 007c 0119 0067 0291  ...|.....|...g..
-00001ec0: 0271 0453 0072 1600 0000 7216 0000 0072  .q.S.r....r....r
-00001ed0: 3500 0000 2902 da0b 616c 6967 6e65 645f  5...)...aligned_
-00001ee0: 7365 71da 056e 616d 6573 7216 0000 0072  seq..namesr....r
-00001ef0: 1700 0000 7225 0000 00f2 0000 0072 2600  ....r%.......r&.
-00001f00: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001f10: 0000 0006 0000 0053 0000 0073 2400 0000  .......S...s$...
-00001f20: 6700 7c00 5d1c 7d01 7c01 6400 1900 7c01  g.|.].}.|.d...|.
-00001f30: 6401 1900 6401 6402 8502 1900 6702 9102  d...d.d.....g...
-00001f40: 7104 5300 2903 7201 0000 0072 0300 0000  q.S.).r....r....
-00001f50: 4e72 1600 0000 a902 7223 0000 00da 0173  Nr......r#.....s
-00001f60: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001f70: 2500 0000 f600 0000 7226 0000 00e9 ffff  %.......r&......
-00001f80: ffff 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001f90: 0000 0006 0000 0053 0000 0073 2400 0000  .......S...s$...
-00001fa0: 6700 7c00 5d1c 7d01 7c01 6400 1900 7c01  g.|.].}.|.d...|.
-00001fb0: 6401 1900 6402 6403 8502 1900 6702 9102  d...d.d.....g...
-00001fc0: 7104 5300 2904 7201 0000 0072 0300 0000  q.S.).r....r....
-00001fd0: 4e72 5900 0000 7216 0000 0072 5700 0000  NrY...r....rW...
-00001fe0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00001ff0: 2500 0000 f800 0000 7226 0000 0029 0a72  %.......r&...).r
-00002000: 4700 0000 da03 6d61 7872 0800 0000 da03  G.....maxr......
-00002010: 7375 6d72 4300 0000 da09 656e 756d 6572  sumrC.....enumer
-00002020: 6174 6572 1000 0000 723a 0000 0072 4900  ater....r:...rI.
-00002030: 0000 722b 0000 0029 0972 1500 0000 724a  ..r+...).r....rJ
-00002040: 0000 005a 0e6e 756d 5f74 6172 6765 745f  ...Z.num_target_
-00002050: 7365 71da 0e63 6865 636b 5f70 7265 7365  seq..check_prese
-00002060: 6e63 65da 0970 6f73 6974 696f 6e73 da0e  nce..positions..
-00002070: 6368 6563 6b5f 706f 7369 7469 6f6e 7236  check_positionr6
-00002080: 0000 0072 4f00 0000 722f 0000 0072 1600  ...rO...r/...r..
-00002090: 0000 2904 7255 0000 0072 5100 0000 7256  ..).rU...rQ...rV
-000020a0: 0000 0072 5300 0000 7217 0000 00da 115f  ...rS...r......_
-000020b0: 6164 645f 6368 6169 6e5f 6272 6561 6b73  add_chain_breaks
-000020c0: b400 0000 7344 0000 0000 0f0e 010e 030e  ....sD..........
-000020d0: 0212 040c 040a 010a ff06 0316 060a 010a  ................
-000020e0: ff06 0308 010c 030a fd06 0514 041c 0110  ................
-000020f0: 021e ff06 0210 0202 0102 ff06 030a 021c  ................
-00002100: 0316 010e 0116 010e 020a 030a 027a 224d  .............z"M
-00002110: 6f64 656c 6c65 725f 6d61 6e61 6765 722e  odeller_manager.
-00002120: 5f61 6464 5f63 6861 696e 5f62 7265 616b  _add_chain_break
-00002130: 7363 0100 0000 0000 0000 0000 0000 0a00  sc..............
-00002140: 0000 0800 0000 4300 0000 737e 0100 0064  ......C...s~...d
-00002150: 0164 02a0 007c 006a 01a1 0117 0064 0317  .d...|.j.....d..
-00002160: 007d 0174 027c 006a 036a 047c 0183 027d  .}.t.|.j.j.|...}
-00002170: 0267 007d 0374 0583 008f 487d 0474 027c  .g.}.t....H}.t.|
-00002180: 006a 036a 0464 0483 027d 057c 04a0 067c  .j.j.d...}.|...|
-00002190: 05a1 017d 067c 06a0 0764 05a1 0164 0664  ...}.|...d...d.d
-000021a0: 0085 0219 007d 0764 0764 0884 007c 0744  .....}.d.d...|.D
-000021b0: 0083 017d 0357 0064 0004 0004 0083 0301  ...}.W.d........
-000021c0: 006e 1031 0073 7a30 0001 0001 0001 0059  .n.1.sz0.......Y
-000021d0: 0001 007c 00a0 087c 006a 017c 0364 0919  ...|...|.j.|.d..
-000021e0: 0064 0619 00a1 027c 0364 0919 0064 063c  .d.....|.d...d.<
-000021f0: 007c 00a0 097c 03a1 017d 0364 027d 087c  .|...|...}.d.}.|
-00002200: 0864 0a7c 006a 036a 0a17 0064 0b17 0037  .d.|.j.j...d...7
-00002210: 007d 087c 0864 0c7c 006a 036a 0a17 0064  .}.|.d.|.j.j...d
-00002220: 0d17 0037 007d 087c 087c 0364 0919 0064  ...7.}.|.|.d...d
-00002230: 0619 0064 0e17 0037 007d 087c 0364 0664  ...d...7.}.|.d.d
-00002240: 0085 0219 0044 005d 447d 097c 0864 0a7c  .....D.]D}.|.d.|
-00002250: 0964 0919 0017 0064 0f17 0064 0b17 0037  .d.....d...d...7
-00002260: 007d 087c 0864 107c 0964 0919 0017 0064  .}.|.d.|.d.....d
-00002270: 0f17 0064 0d17 0037 007d 087c 087c 0964  ...d...7.}.|.|.d
-00002280: 0619 0064 0e17 0037 007d 0871 f87c 006a  ...d...7.}.q.|.j
-00002290: 0b90 0172 7a74 0583 008f 1c7d 047c 04a0  ...rzt.....}.|..
-000022a0: 0c7c 027c 08a1 0201 0057 0064 0004 0004  .|.|.....W.d....
-000022b0: 0083 0301 006e 1231 0090 0173 7030 0001  .....n.1...sp0..
-000022c0: 0001 0001 0059 0001 0064 0053 0029 114e  .....Y...d.S.).N
-000022d0: 5a0f 6d6f 6465 6c6c 6572 5f69 6e70 7574  Z.modeller_input
-000022e0: 5f72 0b00 0000 722c 0000 007a 1774 656d  _r....r,...z.tem
-000022f0: 706c 6174 6573 5f61 6c69 676e 6564 2e66  plates_aligned.f
-00002300: 6173 7461 fa01 3e72 0300 0000 6301 0000  asta..>r....c...
-00002310: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00002320: 0053 0000 0073 3a00 0000 6700 7c00 5d32  .S...s:...g.|.]2
-00002330: 7d01 7c01 a000 6400 a101 6401 1900 a000  }.|...d...d.....
-00002340: a100 6402 1900 6403 a001 7c01 a000 6400  ..d...d...|...d.
-00002350: a101 6404 6405 8502 1900 a101 6702 9102  ..d.d.......g...
-00002360: 7104 5300 2906 da01 0a72 0100 0000 7259  q.S.)....r....rY
-00002370: 0000 0072 0b00 0000 7203 0000 004e 2902  ...r....r....N).
-00002380: da05 7370 6c69 7472 1300 0000 2902 7223  ..splitr....).r#
-00002390: 0000 00da 0178 7216 0000 0072 1600 0000  .....xr....r....
-000023a0: 7217 0000 0072 2500 0000 0b01 0000 7226  r....r%.......r&
-000023b0: 0000 007a 344d 6f64 656c 6c65 725f 6d61  ...z4Modeller_ma
-000023c0: 6e61 6765 722e 7772 6974 655f 616c 6967  nager.write_alig
-000023d0: 6e6d 656e 742e 3c6c 6f63 616c 733e 2e3c  nment.<locals>.<
-000023e0: 6c69 7374 636f 6d70 3e72 0100 0000 7a04  listcomp>r....z.
-000023f0: 3e50 313b 7262 0000 007a 0973 6571 7565  >P1;rb...z.seque
-00002400: 6e63 653a 7a0d 3a2e 3a2e 3a2e 3a2e 3a3a  nce:z.:.:.:.:.::
-00002410: 3a3a 0a7a 022a 0a72 3000 0000 7a0b 7374  ::.z.*.r0...z.st
-00002420: 7275 6374 7572 6558 3a29 0d72 1300 0000  ructureX:).r....
-00002430: 7206 0000 0072 0200 0000 720d 0000 0072  r....r....r....r
-00002440: 3700 0000 7204 0000 00da 0972 6561 645f  7...r......read_
-00002450: 6669 6c65 7263 0000 0072 4500 0000 7260  filerc...rE...r`
-00002460: 0000 0072 1b00 0000 7212 0000 0072 3b00  ...r....r....r;.
-00002470: 0000 290a 7215 0000 0072 3c00 0000 da0b  ..).r....r<.....
-00002480: 6f75 7470 7574 5f70 6174 6872 4a00 0000  output_pathrJ...
-00002490: 723f 0000 00da 0966 696c 655f 7061 7468  r?.....file_path
-000024a0: 5a15 616c 6967 6e65 645f 7365 7175 656e  Z.aligned_sequen
-000024b0: 6365 5f66 696c 655a 1161 6c69 676e 6564  ce_fileZ.aligned
-000024c0: 5f73 6571 7565 6e63 6573 723e 0000 00da  _sequencesr>....
-000024d0: 1174 656d 706c 6174 655f 7365 7175 656e  .template_sequen
-000024e0: 6365 7216 0000 0072 1600 0000 7217 0000  cer....r....r...
-000024f0: 0072 1d00 0000 0101 0000 733a 0000 0000  .r........s:....
-00002500: 0214 010e 0204 0108 010e 010a 0112 012c  ...............,
-00002510: 031e 030a 0404 0114 0114 0114 0310 0118  ................
-00002520: 0102 0102 0106 ff02 0202 fe02 0302 fd02  ................
-00002530: ff04 0612 0508 0108 017a 204d 6f64 656c  .........z Model
-00002540: 6c65 725f 6d61 6e61 6765 722e 7772 6974  ler_manager.writ
-00002550: 655f 616c 6967 6e6d 656e 7463 0100 0000  e_alignmentc....
-00002560: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-00002570: 4300 0000 7302 0100 007c 006a 0064 016b  C...s....|.j.d.k
-00002580: 0272 4674 0164 0264 03a0 027c 006a 03a1  .rFt.d.d...|.j..
-00002590: 0117 0064 0417 007c 006a 046a 0517 0064  ...d...|.j.j...d
-000025a0: 0517 007c 006a 046a 0617 0064 0617 0083  ...|.j.j...d....
-000025b0: 0101 007c 00a0 07a1 0001 0064 0053 0074  ...|.......d.S.t
-000025c0: 087c 006a 046a 097c 006a 046a 0564 0717  .|.j.j.|.j.j.d..
-000025d0: 0064 03a0 027c 006a 03a1 0117 0064 0817  .d...|.j.....d..
-000025e0: 0083 027d 0174 0a83 008f 1a7d 027c 02a0  ...}.t.....}.|..
-000025f0: 0b7c 01a1 0101 0057 0064 0004 0004 0083  .|.....W.d......
-00002600: 0301 006e 1031 0073 9230 0001 0001 0001  ...n.1.s.0......
-00002610: 0059 0001 0074 0ca0 0da1 007d 0374 0ca0  .Y...t.....}.t..
-00002620: 0e74 0f7c 0183 01a1 0101 0064 0964 03a0  .t.|.......d.d..
-00002630: 027c 006a 03a1 0117 0064 0a17 007d 047c  .|.j.....d...}.|
-00002640: 006a 109b 0064 0574 0f7c 0483 019b 009d  .j...d.t.|......
-00002650: 037d 0574 116a 127c 0564 0b64 0b64 0b64  .}.t.j.|.d.d.d.d
-00002660: 0c8d 0401 0074 0ca0 0e7c 03a1 0101 007c  .....t...|.....|
-00002670: 00a0 07a1 0001 0064 0053 0029 0d4e 467a  .......d.S.).NFz
-00002680: 164d 6f64 656c 6c69 6e67 206f 6620 6d75  .Modelling of mu
-00002690: 7461 7469 6f6e 2072 0b00 0000 7a12 2077  tation r....z. w
-000026a0: 6173 2065 6578 636c 7564 6564 206f 6e20  as eexcluded on 
-000026b0: 7219 0000 007a 1920 6475 6520 746f 206d  r....z. due to m
-000026c0: 6973 7369 6e67 2063 6f76 6572 6167 652e  issing coverage.
-000026d0: 722f 0000 005a 065f 6d6f 6465 6c7a 102e  r/...Z._modelz..
-000026e0: 2e2f 7275 6e5f 6d6f 6465 6c6c 6572 5f72  ./run_modeller_r
-000026f0: 2e00 0000 5429 03da 0573 6865 6c6c da12  ....T)...shell..
-00002700: 756e 6976 6572 7361 6c5f 6e65 776c 696e  universal_newlin
-00002710: 6573 da05 6368 6563 6b29 1372 1200 0000  es..check).r....
-00002720: 721a 0000 0072 1300 0000 7206 0000 0072  r....r....r....r
-00002730: 0d00 0000 721b 0000 0072 1c00 0000 da0d  ....r....r......
-00002740: 6c6f 6164 5f6c 6f67 5f66 696c 6572 0200  load_log_filer..
-00002750: 0000 7237 0000 0072 0400 0000 da10 6372  ..r7...r......cr
-00002760: 6561 7465 5f64 6972 6563 746f 7279 da02  eate_directory..
-00002770: 6f73 da06 6765 7463 7764 da05 6368 6469  os..getcwd..chdi
-00002780: 7272 3900 0000 7207 0000 00da 0a73 7562  rr9...r......sub
-00002790: 7072 6f63 6573 73da 0372 756e 2906 7215  process..run).r.
-000027a0: 0000 005a 0a6d 6f64 656c 5f70 6174 6872  ...Z.model_pathr
-000027b0: 3f00 0000 5a16 686f 6d65 5f77 6f72 6b69  ?...Z.home_worki
-000027c0: 6e67 5f64 6972 6563 746f 7279 723d 0000  ng_directoryr=..
-000027d0: 00da 0763 6f6d 6d61 6e64 7216 0000 0072  ...commandr....r
-000027e0: 1600 0000 7217 0000 0072 7200 0000 2c01  ....r....rr...,.
-000027f0: 0000 733a 0000 0000 020a 0110 0102 ff02  ..s:............
-00002800: 0106 ff02 0102 ff02 0206 fe02 0202 fe06  ................
-00002810: 0308 0104 0202 0106 011a fe04 0408 0128  ...............(
-00002820: 0108 010e 0114 0114 0104 0108 ff06 030a  ................
-00002830: 017a 144d 6f64 656c 6c65 725f 6d61 6e61  .z.Modeller_mana
-00002840: 6765 722e 7275 6e63 0100 0000 0000 0000  ger.runc........
-00002850: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
-00002860: 7394 0000 007c 006a 0072 8874 0183 008f  s....|.j.r.t....
-00002870: 6a7d 0174 027c 006a 036a 0464 0164 02a0  j}.t.|.j.j.d.d..
-00002880: 057c 006a 06a1 0117 0064 0317 0083 027d  .|.j.....d.....}
-00002890: 027c 01a0 077c 02a1 01a0 08a1 007d 037c  .|...|.......}.|
-000028a0: 03a0 0964 04a1 017d 047c 047c 037c 0464  ...d...}.|.|.|.d
-000028b0: 0585 0219 00a0 0964 02a1 0117 007d 057c  .......d.....}.|
-000028c0: 037c 047c 0585 0219 007c 005f 0a57 0064  .|.|.....|._.W.d
-000028d0: 0504 0004 0083 0301 0071 9031 0073 7c30  .........q.1.s|0
-000028e0: 0001 0001 0001 0059 0001 006e 0864 0667  .......Y...n.d.g
-000028f0: 017c 005f 0a64 0553 0029 0761 1801 0000  .|._.d.S.).a....
-00002900: 204f 7065 6e20 7468 6520 6c6f 6720 6669   Open the log fi
-00002910: 6c65 2061 6674 6572 2074 6865 2072 756e  le after the run
-00002920: 206f 6620 6d6f 6465 6c6c 6572 2e0a 2020   of modeller..  
-00002930: 2020 2020 2020 4c6f 6f6b 2066 6f72 2074        Look for t
-00002940: 6865 2074 6162 6c65 2077 6974 6820 7468  he table with th
-00002950: 6520 444f 5045 2073 636f 7265 732e 0a20  e DOPE scores.. 
-00002960: 2020 2020 2020 2053 6176 6520 6974 2061         Save it a
-00002970: 7320 6174 7472 6962 7574 6520 286c 6973  s attribute (lis
-00002980: 7429 2e0a 2020 2020 2020 2020 0a20 2020  t)..        .   
-00002990: 2020 2020 2042 7574 2069 6620 7468 6520       But if the 
-000029a0: 6d75 7461 7469 6f6e 2069 7320 6e6f 7420  mutation is not 
-000029b0: 6d6f 6465 6c6c 6162 6c65 2c20 6475 6520  modellable, due 
-000029c0: 746f 206d 6973 7369 6e67 2074 656d 706c  to missing templ
-000029d0: 6174 650a 2020 2020 2020 2020 636f 6e76  ate.        conv
-000029e0: 6572 6167 652c 206a 7573 7420 7361 7665  erage, just save
-000029f0: 2061 2077 6172 6e69 6e67 2073 7472 696e   a warning strin
-00002a00: 6720 6173 2061 7474 7269 6275 7465 2e0a  g as attribute..
-00002a10: 2020 2020 2020 2020 722d 0000 0072 0b00          r-...r..
-00002a20: 0000 7a04 2e6c 6f67 7a46 4669 6c65 6e61  ..z..logzFFilena
-00002a30: 6d65 2020 2020 2020 2020 2020 2020 2020  me              
-00002a40: 2020 2020 2020 2020 2020 2020 6d6f 6c70              molp
-00002a50: 6466 2020 2020 2044 4f50 4520 7363 6f72  df     DOPE scor
-00002a60: 6520 2020 2047 4133 3431 2073 636f 7265  e    GA341 score
-00002a70: 4e7a 4a21 2054 6865 206d 7574 6174 696f  NzJ! The mutatio
-00002a80: 6e20 7761 7320 6e6f 7420 6d6f 6465 6c6c  n was not modell
-00002a90: 6564 2c20 6475 6520 746f 206d 6973 7369  ed, due to missi
-00002aa0: 6e67 2074 656d 706c 6174 6573 2066 6f72  ng templates for
-00002ab0: 2074 6861 7420 7265 6769 6f6e 2e29 0b72   that region.).r
-00002ac0: 1200 0000 7204 0000 0072 0200 0000 720d  ....r....r....r.
-00002ad0: 0000 0072 3700 0000 7213 0000 0072 0600  ...r7...r....r..
-00002ae0: 0000 7265 0000 00da 0a73 706c 6974 6c69  ..re.....splitli
-00002af0: 6e65 73da 0569 6e64 6578 720f 0000 0029  nes..indexr....)
-00002b00: 0672 1500 0000 723f 0000 005a 086c 6f67  .r....r?...Z.log
-00002b10: 5f70 6174 685a 046c 6f67 735a 1174 6162  _pathZ.logsZ.tab
-00002b20: 6c65 5f73 7461 7274 5f69 6e64 6578 5a0f  le_start_indexZ.
-00002b30: 7461 626c 655f 656e 645f 696e 6465 7872  table_end_indexr
-00002b40: 1600 0000 7216 0000 0072 1700 0000 726c  ....r....r....rl
-00002b50: 0000 0045 0100 0073 1000 0000 0008 0601  ...E...s........
-00002b60: 0801 1e01 0e02 0a01 1602 2e02 7a1e 4d6f  ............z.Mo
-00002b70: 6465 6c6c 6572 5f6d 616e 6167 6572 2e6c  deller_manager.l
-00002b80: 6f61 645f 6c6f 675f 6669 6c65 2912 da08  oad_log_file)...
-00002b90: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00002ba0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00002bb0: 5f5f da04 6c69 7374 7239 0000 0072 2700  __..listr9...r'.
-00002bc0: 0000 7218 0000 0072 1f00 0000 da04 626f  ..r....r......bo
-00002bd0: 6f6c 722b 0000 0072 1e00 0000 7245 0000  olr+...r....rE..
-00002be0: 0072 4700 0000 7249 0000 0072 6000 0000  .rG...rI...r`...
-00002bf0: 721d 0000 0072 7200 0000 726c 0000 0072  r....rr...rl...r
-00002c00: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
-00002c10: 0000 0072 0500 0000 0800 0000 731a 0000  ...r........s...
-00002c20: 0008 0106 0104 ff0c 1008 090e 1c08 3d10  ..............=.
-00002c30: 1e10 0c10 0f10 4d08 2b0e 1972 0500 0000  ......M.+..r....
-00002c40: 2907 726e 0000 0072 7100 0000 da07 7061  ).rn...rq.....pa
-00002c50: 7468 6c69 6272 0200 0000 da0c 6669 6c65  thlibr......file
-00002c60: 5f68 616e 646c 6572 7204 0000 0072 0500  _handlerr....r..
-00002c70: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002c80: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002c90: 0100 0000 7308 0000 0008 0108 010c 020c  ....s...........
-00002ca0: 03                                       .
+00000e90: 4f50 4520 7363 6f72 6527 0a0a 6d6f 6465  OPE score'..mode
+00000ea0: 6c73 3d20 6c69 7374 286f 6b5f 6d6f 6465  ls= list(ok_mode
+00000eb0: 6c73 2920 6966 2069 7369 6e73 7461 6e63  ls) if isinstanc
+00000ec0: 6528 6f6b 5f6d 6f64 656c 732c 2074 7970  e(ok_models, typ
+00000ed0: 6528 6669 6c74 6572 286c 616d 6264 613a  e(filter(lambda:
+00000ee0: 204e 6f6e 652c 205b 5d29 2929 2065 6c73   None, []))) els
+00000ef0: 6520 6f6b 5f6d 6f64 656c 730a 6d6f 6465  e ok_models.mode
+00000f00: 6c73 2e73 6f72 7428 6b65 793d 6c61 6d62  ls.sort(key=lamb
+00000f10: 6461 206b 3a20 6b5b 746f 7363 6f72 655d  da k: k[toscore]
+00000f20: 290a 0a6d 796f 7574 203d 206f 7065 6e28  )..myout = open(
+00000f30: 2261 3401 0000 222c 2022 7722 290a 666f  "a4...", "w").fo
+00000f40: 7220 6d20 696e 206d 6f64 656c 733a 0a20  r m in models:. 
+00000f50: 2020 2020 2020 206d 796f 7574 2e77 7269         myout.wri
+00000f60: 7465 2873 7472 286d 5b27 6e61 6d65 275d  te(str(m['name']
+00000f70: 2920 2b20 2220 2844 4f50 4520 5343 4f52  ) + " (DOPE SCOR
+00000f80: 453a 2025 2e33 6629 2220 2520 286d 5b74  E: %.3f)" % (m[t
+00000f90: 6f73 636f 7265 5d29 290a 656e 762e 6c69  oscore])).env.li
+00000fa0: 6273 2e74 6f70 6f6c 6f67 792e 7265 6164  bs.topology.read
+00000fb0: 2866 696c 653d 2724 284c 4942 292f 746f  (file='$(LIB)/to
+00000fc0: 705f 6865 6176 2e6c 6962 2729 0a65 6e76  p_heav.lib').env
+00000fd0: 2e6c 6962 732e 7061 7261 6d65 7465 7273  .libs.parameters
+00000fe0: 2e72 6561 6428 6669 6c65 3d27 2428 4c49  .read(file='$(LI
+00000ff0: 4229 2f70 6172 2e6c 6962 2729 0a6d 646c  B)/par.lib').mdl
+00001000: 203d 2063 6f6d 706c 6574 655f 7064 6228   = complete_pdb(
+00001010: 656e 762c 206d 5b27 6e61 6d65 275d 290a  env, m['name']).
+00001020: 7320 3d20 7365 6c65 6374 696f 6e28 6d64  s = selection(md
+00001030: 6c29 0a73 2e61 7373 6573 735f 646f 7065  l).s.assess_dope
+00001040: 286f 7574 7075 743d 2745 4e45 5247 595f  (output='ENERGY_
+00001050: 5052 4f46 494c 4520 4e4f 5f52 4550 4f52  PROFILE NO_REPOR
+00001060: 5427 2c20 6669 6c65 3d22 7a2f 222c 206e  T', file="z/", n
+00001070: 6f72 6d61 6c69 7a65 5f70 726f 6669 6c65  ormalize_profile
+00001080: 3d54 7275 652c 2073 6d6f 6f74 6869 6e67  =True, smoothing
+00001090: 5f77 696e 646f 773d 3135 2929 0e72 1300  _window=15)).r..
+000010a0: 0000 7206 0000 0072 0200 0000 720d 0000  ..r....r....r...
+000010b0: 00da 086f 7574 5f70 6174 68da 0974 656d  ...out_path..tem
+000010c0: 706c 6174 6573 da03 7374 72da 0572 616e  plates..str..ran
+000010d0: 6765 7210 0000 0072 1100 0000 721b 0000  ger....r....r...
+000010e0: 0072 1400 0000 7204 0000 00da 0a77 7269  .r....r......wri
+000010f0: 7465 5f66 696c 6529 0772 1500 0000 da0e  te_file).r......
+00001100: 616c 6967 6e6d 656e 745f 6e61 6d65 5a0b  alignment_nameZ.
+00001110: 6f75 7470 7574 5f6e 616d 65da 0b73 6372  output_name..scr
+00001120: 6970 745f 7061 7468 5a0e 7465 6d70 6c61  ipt_pathZ.templa
+00001130: 7465 5f6e 616d 6573 da07 636f 6e74 656e  te_names..conten
+00001140: 74da 0266 6872 1600 0000 7216 0000 0072  t..fhr....r....r
+00001150: 1700 0000 721e 0000 003e 0000 0073 5a00  ....r....>...sZ.
+00001160: 0000 0001 1401 1401 0201 0601 12fe 0404  ................
+00001170: 0602 06fe 0605 0207 16f9 0207 02f9 0208  ................
+00001180: 08f8 0208 02f8 0210 02f0 0211 02ef 0213  ................
+00001190: 06ed 0214 02ec 0216 06ea 0217 02e9 021a  ................
+000011a0: 08e6 021a 02e6 0223 02dd 0224 02dc 022c  .......#...$...,
+000011b0: 06d4 022d 02d3 02ff 0231 0801 7a1d 4d6f  ...-.....1..z.Mo
+000011c0: 6465 6c6c 6572 5f6d 616e 6167 6572 2e77  deller_manager.w
+000011d0: 7269 7465 5f73 6372 6970 7429 0272 2a00  rite_script).r*.
+000011e0: 0000 7220 0000 0063 0300 0000 0000 0000  ..r ...c........
+000011f0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00001200: 73a8 0000 007c 0164 016b 0272 0c7c 0253  s....|.d.k.r.|.S
+00001210: 0074 007c 0164 0219 0083 0164 0218 007d  .t.|.d.....d...}
+00001220: 037c 0374 017c 0283 016b 0072 947c 037c  .|.t.|...k.r.|.|
+00001230: 0264 037c 0385 0219 00a0 0264 04a1 0118  .d.|.......d....
+00001240: 007d 047c 0464 0217 0074 007c 0164 0219  .}.|.d...t.|.d..
+00001250: 0083 016b 0272 8a7c 027c 0319 007c 0164  ...k.r.|.|...|.d
+00001260: 0519 006b 0272 8a7c 0264 037c 0385 0219  ...k.r.|.d.|....
+00001270: 007c 0164 0619 0017 007c 027c 0364 0217  .|.d.....|.|.d..
+00001280: 0064 0385 0219 0017 007d 027c 0253 007c  .d.......}.|.S.|
+00001290: 0364 0237 007d 0371 1c74 0364 077c 019b  .d.7.}.q.t.d.|..
+000012a0: 0064 089d 0383 0101 007c 0253 0029 097a  .d.......|.S.).z
+000012b0: ea54 616b 6520 6120 6d75 7461 7469 6f6e  .Take a mutation
+000012c0: 2069 6e20 7468 6520 666f 726d 6174 0a20   in the format. 
+000012d0: 2020 2020 2020 205b 3120 6c65 7474 6572         [1 letter
+000012e0: 2061 6d69 6e6f 2061 6369 642c 7265 7369   amino acid,resi
+000012f0: 6475 6520 6e75 6d62 6572 2c20 3120 6c65  due number, 1 le
+00001300: 7474 2e20 616d 696e 6f20 6163 6964 5d0a  tt. amino acid].
+00001310: 2020 2020 2020 2020 616e 6420 6170 706c          and appl
+00001320: 7920 6974 2074 6f20 7468 6520 616c 6967  y it to the alig
+00001330: 6e65 6420 7365 7175 656e 6365 2074 6f20  ned sequence to 
+00001340: 6d6f 6465 6c2c 0a20 2020 2020 2020 2074  model,.        t
+00001350: 616b 696e 6720 696e 746f 2061 6363 6f75  aking into accou
+00001360: 6e74 2061 6c6c 2074 6865 2022 2d22 2773  nt all the "-"'s
+00001370: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00001380: 6e73 2065 6469 7465 6420 7365 7175 656e  ns edited sequen
+00001390: 6365 0a20 2020 2020 2020 2072 0c00 0000  ce.        r....
+000013a0: 7203 0000 004e fa01 2d72 0100 0000 e902  r....N..-r......
+000013b0: 0000 007a 1943 6f75 6c64 206e 6f74 2061  ...z.Could not a
+000013c0: 7070 6c79 206d 7574 6174 696f 6e20 fa01  pply mutation ..
+000013d0: 2129 0472 2700 0000 da03 6c65 6eda 0563  !).r'.....len..c
+000013e0: 6f75 6e74 721a 0000 0029 0572 1500 0000  ountr....).r....
+000013f0: 7206 0000 0072 2a00 0000 7236 0000 005a  r....r*...r6...Z
+00001400: 1461 6374 7561 6c5f 7265 7369 6475 655f  .actual_residue_
+00001410: 696e 6465 7872 1600 0000 7216 0000 0072  indexr....r....r
+00001420: 1700 0000 da0e 5f6d 7574 6174 655f 7265  ......_mutate_re
+00001430: 7369 6465 7d00 0000 7326 0000 0000 0908  side}...s&......
+00001440: 0104 0310 010c 0116 0212 ff02 020e fe02  ................
+00001450: 040a 0106 ff02 020e fe02 ff02 0504 010a  ................
+00001460: 0210 017a 1f4d 6f64 656c 6c65 725f 6d61  ...z.Modeller_ma
+00001470: 6e61 6765 722e 5f6d 7574 6174 655f 7265  nager._mutate_re
+00001480: 7369 6465 6302 0000 0000 0000 0000 0000  sidec...........
+00001490: 0005 0000 0005 0000 0043 0000 0073 4400  .........C...sD.
+000014a0: 0000 6700 7d02 6401 7d03 7c01 4400 5d32  ..g.}.d.}.|.D.]2
+000014b0: 7d04 7c04 6402 6b02 7228 7c02 a000 6402  }.|.d.k.r(|...d.
+000014c0: 7c04 6702 a101 0100 710c 7c02 a000 7c03  |.g.....q.|...|.
+000014d0: 7c04 6702 a101 0100 7c03 6401 3700 7d03  |.g.....|.d.7.}.
+000014e0: 710c 7c02 5300 2903 7a37 4672 6f6d 2061  q.|.S.).z7From a
+000014f0: 2073 6571 7565 6e63 652c 2072 6574 7572   sequence, retur
+00001500: 6e20 6120 3244 206c 6973 7420 7769 7468  n a 2D list with
+00001510: 205b 7265 736e 756d 2c72 6573 6975 6465   [resnum,resiude
+00001520: 5d72 0300 0000 7240 0000 0029 0172 2900  ]r....r@...).r).
+00001530: 0000 2905 7215 0000 0072 2a00 0000 5a0c  ..).r....r*...Z.
+00001540: 6e75 6d62 6572 6564 5f73 6571 7236 0000  numbered_seqr6..
+00001550: 00da 0463 6861 7272 1600 0000 7216 0000  ...charr....r...
+00001560: 0072 1700 0000 da17 5f61 6464 5f6e 756d  .r......_add_num
+00001570: 6265 725f 746f 5f73 6571 7565 6e63 659b  ber_to_sequence.
+00001580: 0000 0073 1000 0000 0002 0401 0401 0801  ...s............
+00001590: 0801 1002 0e01 0a01 7a28 4d6f 6465 6c6c  ........z(Modell
+000015a0: 6572 5f6d 616e 6167 6572 2e5f 6164 645f  er_manager._add_
+000015b0: 6e75 6d62 6572 5f74 6f5f 7365 7175 656e  number_to_sequen
+000015c0: 6365 4e29 02da 1473 6571 7565 6e63 655f  ceN)...sequence_
+000015d0: 7769 7468 5f72 6573 6e75 6d72 2000 0000  with_resnumr ...
+000015e0: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+000015f0: 0005 0000 0043 0000 0073 6200 0000 6401  .....C...sb...d.
+00001600: 6402 8400 7c01 4400 8301 7d02 7c00 6a00  d...|.D...}.|.j.
+00001610: a001 7c02 6403 1900 a101 0100 7402 6404  ..|.d.......t.d.
+00001620: 7403 7c02 8301 8302 4400 5d30 7d03 7c02  t.|.....D.]0}.|.
+00001630: 7c03 1900 7c02 7c03 6404 1800 1900 6404  |...|.|.d.....d.
+00001640: 1700 6b03 722c 7c00 6a00 a001 7c02 7c03  ..k.r,|.j...|.|.
+00001650: 1900 6404 1800 a101 0100 712c 6405 5300  ..d.......q,d.S.
+00001660: 2906 7aa7 4769 7665 6e20 6120 7365 7175  ).z.Given a sequ
+00001670: 656e 6365 2073 6176 6564 2061 7320 6120  ence saved as a 
+00001680: 6c69 7374 205b 7265 736e 756d 2c20 7265  list [resnum, re
+00001690: 7369 6475 655d 2c0a 2020 2020 2020 2020  sidue],.        
+000016a0: 7361 7665 2061 6c6c 2074 6865 2072 6573  save all the res
+000016b0: 6964 7565 206e 756d 6265 7273 2074 6861  idue numbers tha
+000016c0: 7420 7265 7072 6573 656e 7420 616e 2069  t represent an i
+000016d0: 6e74 6572 7275 7074 696f 6e0a 2020 2020  nterruption.    
+000016e0: 2020 2020 696e 2074 6865 2063 6f6e 7469      in the conti
+000016f0: 6e75 6974 7920 6f66 2074 6865 2070 726f  nuity of the pro
+00001700: 7465 696e 2063 6861 696e 2e63 0100 0000  tein chain.c....
+00001710: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001720: 5300 0000 7320 0000 0067 007c 005d 187d  S...s ...g.|.].}
+00001730: 017c 0164 0019 0064 016b 0372 047c 0164  .|.d...d.k.r.|.d
+00001740: 0019 0091 0271 0453 0029 0272 0100 0000  .....q.S.).r....
+00001750: 7240 0000 0072 1600 0000 7222 0000 0072  r@...r....r"...r
+00001760: 1600 0000 7216 0000 0072 1700 0000 7225  ....r....r....r%
+00001770: 0000 00ad 0000 0072 2600 0000 7a37 4d6f  .......r&...z7Mo
+00001780: 6465 6c6c 6572 5f6d 616e 6167 6572 2e5f  deller_manager._
+00001790: 7361 7665 5f63 6861 696e 5f73 7461 7274  save_chain_start
+000017a0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+000017b0: 636f 6d70 3e72 0100 0000 7203 0000 004e  comp>r....r....N
+000017c0: 2904 7211 0000 0072 2900 0000 723a 0000  ).r....r)...r:..
+000017d0: 0072 4300 0000 2904 7215 0000 0072 4800  .rC...).r....rH.
+000017e0: 0000 5a10 6669 6c74 6572 6564 5f6e 756d  ..Z.filtered_num
+000017f0: 6265 7273 7236 0000 0072 1600 0000 7216  bersr6...r....r.
+00001800: 0000 0072 1700 0000 da12 5f73 6176 655f  ...r......_save_
+00001810: 6368 6169 6e5f 7374 6172 7473 a700 0000  chain_starts....
+00001820: 730a 0000 0000 060e 0310 0212 0118 017a  s..............z
+00001830: 234d 6f64 656c 6c65 725f 6d61 6e61 6765  #Modeller_manage
+00001840: 722e 5f73 6176 655f 6368 6169 6e5f 7374  r._save_chain_st
+00001850: 6172 7473 2902 da09 7365 7175 656e 6365  arts)...sequence
+00001860: 7372 2000 0000 6302 0000 0000 0000 0000  sr ...c.........
+00001870: 0000 0009 0000 0006 0000 0003 0000 0073  ...............s
+00001880: ba01 0000 6401 6402 8400 7c01 4400 8301  ....d.d...|.D...
+00001890: 8902 6403 6402 8400 7c01 4400 8301 8900  ..d.d...|.D.....
+000018a0: 7c00 a000 8800 6404 1900 a101 7d02 7401  |.....d.....}.t.
+000018b0: 6405 6402 8400 8800 4400 8301 8301 8901  d.d.....D.......
+000018c0: 8801 7c00 6a02 6b05 9001 723e 8701 6601  ..|.j.k...r>..f.
+000018d0: 6406 6402 8408 8800 6407 6408 8502 1900  d.d.....d.d.....
+000018e0: 4400 8301 7d03 7403 7c03 8301 7404 8800  D...}.t.|...t...
+000018f0: 8301 6407 1800 6b02 9001 7234 8701 6601  ..d...k...r4..f.
+00001900: 6409 6402 8408 8800 6407 6408 8502 1900  d.d.....d.d.....
+00001910: 4400 8301 7d04 7c04 4400 5d9c 8903 8701  D...}.|.D.].....
+00001920: 8703 6602 640a 6402 8408 8800 6407 6408  ..f.d.d.....d.d.
+00001930: 8502 1900 4400 8301 7d05 7403 7c05 8301  ....D...}.t.|...
+00001940: 7404 8800 8301 6407 1800 6b02 7296 7c02  t.....d...k.r.|.
+00001950: 6408 8803 8502 1900 7c02 8803 8801 1700  d.......|.......
+00001960: 6408 8502 1900 1700 7d02 7405 8800 8301  d.......}.t.....
+00001970: 4400 5d3a 5c02 7d06 7d07 7c07 6408 8803  D.]:\.}.}.|.d...
+00001980: 8502 1900 640b 1700 7c07 8803 8801 1700  ....d...|.......
+00001990: 6408 8502 1900 1700 8800 7c06 3c00 7c00  d.........|.<.|.
+000019a0: 0400 6a06 6407 3700 0200 5f06 71ee 8801  ..j.d.7..._.q...
+000019b0: 6407 3700 8901 7196 8801 6407 3800 8901  d.7...q...d.8...
+000019c0: 713c 8700 8702 6602 640c 6402 8408 7407  q<....f.d.d...t.
+000019d0: 7404 8802 8301 8301 4400 8301 7d01 7c01  t.......D...}.|.
+000019e0: 6404 1900 6407 1900 6404 1900 640b 6b02  d...d...d...d.k.
+000019f0: 9001 727e 640d 6402 8400 7c01 4400 8301  ..r~d.d...|.D...
+00001a00: 7d01 7c01 6404 1900 6407 1900 640e 1900  }.|.d...d...d...
+00001a10: 640b 6b02 9001 72a2 640f 6402 8400 7c01  d.k...r.d.d...|.
+00001a20: 4400 8301 7d01 7c00 a008 7c02 a101 0100  D...}.|...|.....
+00001a30: 7c00 a009 7c02 a101 7d08 7c01 5300 2910  |...|...}.|.S.).
+00001a40: 619f 0100 0046 6f72 2061 6c69 676e 6d65  a....For alignme
+00001a50: 6e74 7320 696e 2077 6869 6368 2074 6865  nts in which the
+00001a60: 7265 2069 7320 6e6f 2063 6f76 6572 6167  re is no coverag
+00001a70: 6520 666f 7220 7365 6c66 2e6d 6f64 656c  e for self.model
+00001a80: 5f63 7574 6f66 662b 0a20 2020 2020 2020  _cutoff+.       
+00001a90: 2072 6573 6964 7565 732c 2074 6865 2073   residues, the s
+00001aa0: 6563 7469 6f6e 2077 6974 686f 7574 2063  ection without c
+00001ab0: 6f76 6572 6167 6520 6973 2072 6570 6c61  overage is repla
+00001ac0: 6365 6420 6279 0a20 2020 2020 2020 2063  ced by.        c
+00001ad0: 6861 696e 2062 7265 616b 732e 0a0a 2020  hain breaks...  
+00001ae0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00001af0: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
+00001b00: 7320 286c 6973 7429 3a20 4120 6c69 7374  s (list): A list
+00001b10: 206f 6620 5b6e 616d 652c 2073 6571 7565   of [name, seque
+00001b20: 6e63 655d 206c 6973 7473 2c0a 2020 2020  nce] lists,.    
+00001b30: 2020 2020 2020 2020 6f6e 6520 666f 7220          one for 
+00001b40: 6561 6368 2073 6571 7565 6e63 6520 746f  each sequence to
+00001b50: 2062 6520 7772 6974 7465 6e20 696e 2074   be written in t
+00001b60: 6865 206d 6f64 656c 6c65 720a 2020 2020  he modeller.    
+00001b70: 2020 2020 2020 2020 616c 6967 6e6d 656e          alignmen
+00001b80: 7420 696e 7075 7420 6669 6c65 2e0a 0a20  t input file... 
+00001b90: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00001ba0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00001bb0: 3a20 5265 7475 726e 7320 7468 6520 7361  : Returns the sa
+00001bc0: 6d65 206c 6973 742c 2077 6974 6820 6368  me list, with ch
+00001bd0: 6169 6e20 6272 6561 6b73 2e0a 2020 2020  ain breaks..    
+00001be0: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+00001bf0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00001c00: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+00001c10: 9102 7104 5300 7221 0000 0072 1600 0000  ..q.S.r!...r....
+00001c20: a902 7223 0000 00da 066f 626a 6563 7472  ..r#.....objectr
+00001c30: 1600 0000 7216 0000 0072 1700 0000 7225  ....r....r....r%
+00001c40: 0000 00c5 0000 0072 2600 0000 7a36 4d6f  .......r&...z6Mo
+00001c50: 6465 6c6c 6572 5f6d 616e 6167 6572 2e5f  deller_manager._
+00001c60: 6164 645f 6368 6169 6e5f 6272 6561 6b73  add_chain_breaks
+00001c70: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001c80: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00001c90: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00001ca0: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+00001cb0: 9102 7104 5300 2901 7203 0000 0072 1600  ..q.S.).r....r..
+00001cc0: 0000 724b 0000 0072 1600 0000 7216 0000  ..rK...r....r...
+00001cd0: 0072 1700 0000 7225 0000 00c6 0000 0072  .r....r%.......r
+00001ce0: 2600 0000 7201 0000 0063 0100 0000 0000  &...r....c......
+00001cf0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+00001d00: 0000 7316 0000 0067 007c 005d 0e7d 017c  ..s....g.|.].}.|
+00001d10: 01a0 0064 00a1 0191 0271 0453 00a9 0172  ...d.....q.S...r
+00001d20: 4000 0000 2901 7244 0000 00a9 0272 2300  @...).rD.....r#.
+00001d30: 0000 da03 7365 7172 1600 0000 7216 0000  ....seqr....r...
+00001d40: 0072 1700 0000 7225 0000 00cb 0000 0072  .r....r%.......r
+00001d50: 2600 0000 6301 0000 0000 0000 0000 0000  &...c...........
+00001d60: 0002 0000 0004 0000 0013 0000 0073 1800  .............s..
+00001d70: 0000 6700 7c00 5d10 7d01 6400 8800 1400  ..g.|.].}.d.....
+00001d80: 7c01 7600 9102 7104 5300 724d 0000 0072  |.v...q.S.rM...r
+00001d90: 1600 0000 724e 0000 00a9 01da 0f6d 6178  ....rN.......max
+00001da0: 5f6e 6f6e 5f63 6f76 6572 6564 7216 0000  _non_coveredr...
+00001db0: 0072 1700 0000 7225 0000 00d3 0000 0073  .r....r%.......s
+00001dc0: 0200 0000 0601 7203 0000 004e 6301 0000  ......r....Nc...
+00001dd0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001de0: 0013 0000 0073 1a00 0000 6700 7c00 5d12  .....s....g.|.].
+00001df0: 7d01 7c01 a000 6400 8800 1400 a101 9102  }.|...d.........
+00001e00: 7104 5300 724d 0000 0029 01da 0466 696e  q.S.rM...)...fin
+00001e10: 6472 4e00 0000 7250 0000 0072 1600 0000  drN...rP...r....
+00001e20: 7217 0000 0072 2500 0000 dc00 0000 7302  r....r%.......s.
+00001e30: 0000 0006 0163 0100 0000 0000 0000 0000  .....c..........
+00001e40: 0000 0200 0000 0600 0000 1300 0000 7324  ..............s$
+00001e50: 0000 0067 007c 005d 1c7d 017c 0188 0188  ...g.|.].}.|....
+00001e60: 0188 0017 0085 0219 0064 0088 0014 006b  .........d.....k
+00001e70: 0291 0271 0453 0072 4d00 0000 7216 0000  ...q.S.rM...r...
+00001e80: 0072 4e00 0000 2902 7251 0000 00da 0370  .rN...).rQ.....p
+00001e90: 6f73 7216 0000 0072 1700 0000 7225 0000  osr....r....r%..
+00001ea0: 00e0 0000 0073 0800 0000 0603 02fe 0e01  .....s..........
+00001eb0: 06ff fa01 2f63 0100 0000 0000 0000 0000  ..../c..........
+00001ec0: 0000 0200 0000 0500 0000 1300 0000 731c  ..............s.
+00001ed0: 0000 0067 007c 005d 147d 0188 017c 0119  ...g.|.].}...|..
+00001ee0: 0088 007c 0119 0067 0291 0271 0453 0072  ...|...g...q.S.r
+00001ef0: 1600 0000 7216 0000 0072 3500 0000 2902  ....r....r5...).
+00001f00: da0b 616c 6967 6e65 645f 7365 71da 056e  ..aligned_seq..n
+00001f10: 616d 6573 7216 0000 0072 1700 0000 7225  amesr....r....r%
+00001f20: 0000 00f4 0000 0072 2600 0000 6301 0000  .......r&...c...
+00001f30: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001f40: 0053 0000 0073 2400 0000 6700 7c00 5d1c  .S...s$...g.|.].
+00001f50: 7d01 7c01 6400 1900 7c01 6401 1900 6401  }.|.d...|.d...d.
+00001f60: 6402 8502 1900 6702 9102 7104 5300 2903  d.....g...q.S.).
+00001f70: 7201 0000 0072 0300 0000 4e72 1600 0000  r....r....Nr....
+00001f80: a902 7223 0000 00da 0173 7216 0000 0072  ..r#.....sr....r
+00001f90: 1600 0000 7217 0000 0072 2500 0000 f800  ....r....r%.....
+00001fa0: 0000 7226 0000 00e9 ffff ffff 6301 0000  ..r&........c...
+00001fb0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00001fc0: 0053 0000 0073 2400 0000 6700 7c00 5d1c  .S...s$...g.|.].
+00001fd0: 7d01 7c01 6400 1900 7c01 6401 1900 6402  }.|.d...|.d...d.
+00001fe0: 6403 8502 1900 6702 9102 7104 5300 2904  d.....g...q.S.).
+00001ff0: 7201 0000 0072 0300 0000 4e72 5900 0000  r....r....NrY...
+00002000: 7216 0000 0072 5700 0000 7216 0000 0072  r....rW...r....r
+00002010: 1600 0000 7217 0000 0072 2500 0000 fa00  ....r....r%.....
+00002020: 0000 7226 0000 0029 0a72 4700 0000 da03  ..r&...).rG.....
+00002030: 6d61 7872 0800 0000 da03 7375 6d72 4300  maxr......sumrC.
+00002040: 0000 da09 656e 756d 6572 6174 6572 1000  ....enumerater..
+00002050: 0000 723a 0000 0072 4900 0000 722b 0000  ..r:...rI...r+..
+00002060: 0029 0972 1500 0000 724a 0000 005a 0e6e  .).r....rJ...Z.n
+00002070: 756d 5f74 6172 6765 745f 7365 71da 0e63  um_target_seq..c
+00002080: 6865 636b 5f70 7265 7365 6e63 65da 0970  heck_presence..p
+00002090: 6f73 6974 696f 6e73 da0e 6368 6563 6b5f  ositions..check_
+000020a0: 706f 7369 7469 6f6e 7236 0000 0072 4f00  positionr6...rO.
+000020b0: 0000 722f 0000 0072 1600 0000 2904 7255  ..r/...r....).rU
+000020c0: 0000 0072 5100 0000 7256 0000 0072 5300  ...rQ...rV...rS.
+000020d0: 0000 7217 0000 00da 115f 6164 645f 6368  ..r......_add_ch
+000020e0: 6169 6e5f 6272 6561 6b73 b600 0000 7344  ain_breaks....sD
+000020f0: 0000 0000 0f0e 010e 030e 0212 040c 040a  ................
+00002100: 010a ff06 0316 060a 010a ff06 0308 010c  ................
+00002110: 030a fd06 0514 041c 0110 021e ff06 0210  ................
+00002120: 0202 0102 ff06 030a 021c 0316 010e 0116  ................
+00002130: 010e 020a 030a 027a 224d 6f64 656c 6c65  .......z"Modelle
+00002140: 725f 6d61 6e61 6765 722e 5f61 6464 5f63  r_manager._add_c
+00002150: 6861 696e 5f62 7265 616b 7363 0100 0000  hain_breaksc....
+00002160: 0000 0000 0000 0000 0a00 0000 0800 0000  ................
+00002170: 4300 0000 737e 0100 0064 0164 02a0 007c  C...s~...d.d...|
+00002180: 006a 01a1 0117 0064 0317 007d 0174 027c  .j.....d...}.t.|
+00002190: 006a 036a 047c 0183 027d 0267 007d 0374  .j.j.|...}.g.}.t
+000021a0: 0583 008f 487d 0474 027c 006a 036a 0464  ....H}.t.|.j.j.d
+000021b0: 0483 027d 057c 04a0 067c 05a1 017d 067c  ...}.|...|...}.|
+000021c0: 06a0 0764 05a1 0164 0664 0085 0219 007d  ...d...d.d.....}
+000021d0: 0764 0764 0884 007c 0744 0083 017d 0357  .d.d...|.D...}.W
+000021e0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+000021f0: 7a30 0001 0001 0001 0059 0001 007c 00a0  z0.......Y...|..
+00002200: 087c 006a 017c 0364 0919 0064 0619 00a1  .|.j.|.d...d....
+00002210: 027c 0364 0919 0064 063c 007c 00a0 097c  .|.d...d.<.|...|
+00002220: 03a1 017d 0364 027d 087c 0864 0a7c 006a  ...}.d.}.|.d.|.j
+00002230: 036a 0a17 0064 0b17 0037 007d 087c 0864  .j...d...7.}.|.d
+00002240: 0c7c 006a 036a 0a17 0064 0d17 0037 007d  .|.j.j...d...7.}
+00002250: 087c 087c 0364 0919 0064 0619 0064 0e17  .|.|.d...d...d..
+00002260: 0037 007d 087c 0364 0664 0085 0219 0044  .7.}.|.d.d.....D
+00002270: 005d 447d 097c 0864 0a7c 0964 0919 0017  .]D}.|.d.|.d....
+00002280: 0064 0f17 0064 0b17 0037 007d 087c 0864  .d...d...7.}.|.d
+00002290: 107c 0964 0919 0017 0064 0f17 0064 0d17  .|.d.....d...d..
+000022a0: 0037 007d 087c 087c 0964 0619 0064 0e17  .7.}.|.|.d...d..
+000022b0: 0037 007d 0871 f87c 006a 0b90 0172 7a74  .7.}.q.|.j...rzt
+000022c0: 0583 008f 1c7d 047c 04a0 0c7c 027c 08a1  .....}.|...|.|..
+000022d0: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+000022e0: 1231 0090 0173 7030 0001 0001 0001 0059  .1...sp0.......Y
+000022f0: 0001 0064 0053 0029 114e 5a0f 6d6f 6465  ...d.S.).NZ.mode
+00002300: 6c6c 6572 5f69 6e70 7574 5f72 0b00 0000  ller_input_r....
+00002310: 722c 0000 007a 1774 656d 706c 6174 6573  r,...z.templates
+00002320: 5f61 6c69 676e 6564 2e66 6173 7461 fa01  _aligned.fasta..
+00002330: 3e72 0300 0000 6301 0000 0000 0000 0000  >r....c.........
+00002340: 0000 0002 0000 0008 0000 0053 0000 0073  ...........S...s
+00002350: 3a00 0000 6700 7c00 5d32 7d01 7c01 a000  :...g.|.]2}.|...
+00002360: 6400 a101 6401 1900 a000 a100 6402 1900  d...d.......d...
+00002370: 6403 a001 7c01 a000 6400 a101 6404 6405  d...|...d...d.d.
+00002380: 8502 1900 a101 6702 9102 7104 5300 2906  ......g...q.S.).
+00002390: da01 0a72 0100 0000 7259 0000 0072 0b00  ...r....rY...r..
+000023a0: 0000 7203 0000 004e 2902 da05 7370 6c69  ..r....N)...spli
+000023b0: 7472 1300 0000 2902 7223 0000 00da 0178  tr....).r#.....x
+000023c0: 7216 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+000023d0: 2500 0000 0d01 0000 7226 0000 007a 344d  %.......r&...z4M
+000023e0: 6f64 656c 6c65 725f 6d61 6e61 6765 722e  odeller_manager.
+000023f0: 7772 6974 655f 616c 6967 6e6d 656e 742e  write_alignment.
+00002400: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00002410: 6d70 3e72 0100 0000 7a04 3e50 313b 7262  mp>r....z.>P1;rb
+00002420: 0000 007a 0973 6571 7565 6e63 653a 7a0d  ...z.sequence:z.
+00002430: 3a2e 3a2e 3a2e 3a2e 3a3a 3a3a 0a7a 022a  :.:.:.:.::::.z.*
+00002440: 0a72 3000 0000 7a0b 7374 7275 6374 7572  .r0...z.structur
+00002450: 6558 3a29 0d72 1300 0000 7206 0000 0072  eX:).r....r....r
+00002460: 0200 0000 720d 0000 0072 3700 0000 7204  ....r....r7...r.
+00002470: 0000 00da 0972 6561 645f 6669 6c65 7263  .....read_filerc
+00002480: 0000 0072 4500 0000 7260 0000 0072 1b00  ...rE...r`...r..
+00002490: 0000 7212 0000 0072 3b00 0000 290a 7215  ..r....r;...).r.
+000024a0: 0000 0072 3c00 0000 da0b 6f75 7470 7574  ...r<.....output
+000024b0: 5f70 6174 6872 4a00 0000 723f 0000 00da  _pathrJ...r?....
+000024c0: 0966 696c 655f 7061 7468 5a15 616c 6967  .file_pathZ.alig
+000024d0: 6e65 645f 7365 7175 656e 6365 5f66 696c  ned_sequence_fil
+000024e0: 655a 1161 6c69 676e 6564 5f73 6571 7565  eZ.aligned_seque
+000024f0: 6e63 6573 723e 0000 00da 1174 656d 706c  ncesr>.....templ
+00002500: 6174 655f 7365 7175 656e 6365 7216 0000  ate_sequencer...
+00002510: 0072 1600 0000 7217 0000 0072 1d00 0000  .r....r....r....
+00002520: 0301 0000 733a 0000 0000 0214 010e 0204  ....s:..........
+00002530: 0108 010e 010a 0112 012c 031e 030a 0404  .........,......
+00002540: 0114 0114 0114 0310 0118 0102 0102 0106  ................
+00002550: ff02 0202 fe02 0302 fd02 ff04 0612 0508  ................
+00002560: 0108 017a 204d 6f64 656c 6c65 725f 6d61  ...z Modeller_ma
+00002570: 6e61 6765 722e 7772 6974 655f 616c 6967  nager.write_alig
+00002580: 6e6d 656e 7463 0100 0000 0000 0000 0000  nmentc..........
+00002590: 0000 0600 0000 0800 0000 4300 0000 7302  ..........C...s.
+000025a0: 0100 007c 006a 0064 016b 0272 4674 0164  ...|.j.d.k.rFt.d
+000025b0: 0264 03a0 027c 006a 03a1 0117 0064 0417  .d...|.j.....d..
+000025c0: 007c 006a 046a 0517 0064 0517 007c 006a  .|.j.j...d...|.j
+000025d0: 046a 0617 0064 0617 0083 0101 007c 00a0  .j...d.......|..
+000025e0: 07a1 0001 0064 0053 0074 087c 006a 046a  .....d.S.t.|.j.j
+000025f0: 097c 006a 046a 0564 0717 0064 03a0 027c  .|.j.j.d...d...|
+00002600: 006a 03a1 0117 0064 0817 0083 027d 0174  .j.....d.....}.t
+00002610: 0a83 008f 1a7d 027c 02a0 0b7c 01a1 0101  .....}.|...|....
+00002620: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00002630: 0073 9230 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
+00002640: 0ca0 0da1 007d 0374 0ca0 0e74 0f7c 0183  .....}.t...t.|..
+00002650: 01a1 0101 0064 0964 03a0 027c 006a 03a1  .....d.d...|.j..
+00002660: 0117 0064 0a17 007d 047c 006a 109b 0064  ...d...}.|.j...d
+00002670: 0574 0f7c 0483 019b 009d 037d 0574 116a  .t.|.......}.t.j
+00002680: 127c 0564 0b64 0b64 0b64 0c8d 0401 0074  .|.d.d.d.d.....t
+00002690: 0ca0 0e7c 03a1 0101 007c 00a0 07a1 0001  ...|.....|......
+000026a0: 0064 0053 0029 0d4e 467a 164d 6f64 656c  .d.S.).NFz.Model
+000026b0: 6c69 6e67 206f 6620 6d75 7461 7469 6f6e  ling of mutation
+000026c0: 2072 0b00 0000 7a12 2077 6173 2065 6578   r....z. was eex
+000026d0: 636c 7564 6564 206f 6e20 7219 0000 007a  cluded on r....z
+000026e0: 1920 6475 6520 746f 206d 6973 7369 6e67  . due to missing
+000026f0: 2063 6f76 6572 6167 652e 722f 0000 005a   coverage.r/...Z
+00002700: 065f 6d6f 6465 6c7a 102e 2e2f 7275 6e5f  ._modelz.../run_
+00002710: 6d6f 6465 6c6c 6572 5f72 2e00 0000 5429  modeller_r....T)
+00002720: 03da 0573 6865 6c6c da12 756e 6976 6572  ...shell..univer
+00002730: 7361 6c5f 6e65 776c 696e 6573 da05 6368  sal_newlines..ch
+00002740: 6563 6b29 1372 1200 0000 721a 0000 0072  eck).r....r....r
+00002750: 1300 0000 7206 0000 0072 0d00 0000 721b  ....r....r....r.
+00002760: 0000 0072 1c00 0000 da0d 6c6f 6164 5f6c  ...r......load_l
+00002770: 6f67 5f66 696c 6572 0200 0000 7237 0000  og_filer....r7..
+00002780: 0072 0400 0000 da10 6372 6561 7465 5f64  .r......create_d
+00002790: 6972 6563 746f 7279 da02 6f73 da06 6765  irectory..os..ge
+000027a0: 7463 7764 da05 6368 6469 7272 3900 0000  tcwd..chdirr9...
+000027b0: 7207 0000 00da 0a73 7562 7072 6f63 6573  r......subproces
+000027c0: 73da 0372 756e 2906 7215 0000 005a 0a6d  s..run).r....Z.m
+000027d0: 6f64 656c 5f70 6174 6872 3f00 0000 5a16  odel_pathr?...Z.
+000027e0: 686f 6d65 5f77 6f72 6b69 6e67 5f64 6972  home_working_dir
+000027f0: 6563 746f 7279 723d 0000 00da 0763 6f6d  ectoryr=.....com
+00002800: 6d61 6e64 7216 0000 0072 1600 0000 7217  mandr....r....r.
+00002810: 0000 0072 7200 0000 2e01 0000 733a 0000  ...rr.......s:..
+00002820: 0000 020a 0110 0102 ff02 0106 ff02 0102  ................
+00002830: ff02 0206 fe02 0202 fe06 0308 0104 0202  ................
+00002840: 0106 011a fe04 0408 0128 0108 010e 0114  .........(......
+00002850: 0114 0104 0108 ff06 030a 017a 144d 6f64  ...........z.Mod
+00002860: 656c 6c65 725f 6d61 6e61 6765 722e 7275  eller_manager.ru
+00002870: 6e63 0100 0000 0000 0000 0000 0000 0600  nc..............
+00002880: 0000 0800 0000 4300 0000 7394 0000 007c  ......C...s....|
+00002890: 006a 0072 8874 0183 008f 6a7d 0174 027c  .j.r.t....j}.t.|
+000028a0: 006a 036a 0464 0164 02a0 057c 006a 06a1  .j.j.d.d...|.j..
+000028b0: 0117 0064 0317 0083 027d 027c 01a0 077c  ...d.....}.|...|
+000028c0: 02a1 01a0 08a1 007d 037c 03a0 0964 04a1  .......}.|...d..
+000028d0: 017d 047c 047c 037c 0464 0585 0219 00a0  .}.|.|.|.d......
+000028e0: 0964 02a1 0117 007d 057c 037c 047c 0585  .d.....}.|.|.|..
+000028f0: 0219 007c 005f 0a57 0064 0504 0004 0083  ...|._.W.d......
+00002900: 0301 0071 9031 0073 7c30 0001 0001 0001  ...q.1.s|0......
+00002910: 0059 0001 006e 0864 0667 017c 005f 0a64  .Y...n.d.g.|._.d
+00002920: 0553 0029 0761 1801 0000 204f 7065 6e20  .S.).a.... Open 
+00002930: 7468 6520 6c6f 6720 6669 6c65 2061 6674  the log file aft
+00002940: 6572 2074 6865 2072 756e 206f 6620 6d6f  er the run of mo
+00002950: 6465 6c6c 6572 2e0a 2020 2020 2020 2020  deller..        
+00002960: 4c6f 6f6b 2066 6f72 2074 6865 2074 6162  Look for the tab
+00002970: 6c65 2077 6974 6820 7468 6520 444f 5045  le with the DOPE
+00002980: 2073 636f 7265 732e 0a20 2020 2020 2020   scores..       
+00002990: 2053 6176 6520 6974 2061 7320 6174 7472   Save it as attr
+000029a0: 6962 7574 6520 286c 6973 7429 2e0a 2020  ibute (list)..  
+000029b0: 2020 2020 2020 0a20 2020 2020 2020 2042        .        B
+000029c0: 7574 2069 6620 7468 6520 6d75 7461 7469  ut if the mutati
+000029d0: 6f6e 2069 7320 6e6f 7420 6d6f 6465 6c6c  on is not modell
+000029e0: 6162 6c65 2c20 6475 6520 746f 206d 6973  able, due to mis
+000029f0: 7369 6e67 2074 656d 706c 6174 650a 2020  sing template.  
+00002a00: 2020 2020 2020 636f 6e76 6572 6167 652c        converage,
+00002a10: 206a 7573 7420 7361 7665 2061 2077 6172   just save a war
+00002a20: 6e69 6e67 2073 7472 696e 6720 6173 2061  ning string as a
+00002a30: 7474 7269 6275 7465 2e0a 2020 2020 2020  ttribute..      
+00002a40: 2020 722d 0000 0072 0b00 0000 7a04 2e6c    r-...r....z..l
+00002a50: 6f67 7a46 4669 6c65 6e61 6d65 2020 2020  ogzFFilename    
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a70: 2020 2020 2020 6d6f 6c70 6466 2020 2020        molpdf    
+00002a80: 2044 4f50 4520 7363 6f72 6520 2020 2047   DOPE score    G
+00002a90: 4133 3431 2073 636f 7265 4e7a 4a21 2054  A341 scoreNzJ! T
+00002aa0: 6865 206d 7574 6174 696f 6e20 7761 7320  he mutation was 
+00002ab0: 6e6f 7420 6d6f 6465 6c6c 6564 2c20 6475  not modelled, du
+00002ac0: 6520 746f 206d 6973 7369 6e67 2074 656d  e to missing tem
+00002ad0: 706c 6174 6573 2066 6f72 2074 6861 7420  plates for that 
+00002ae0: 7265 6769 6f6e 2e29 0b72 1200 0000 7204  region.).r....r.
+00002af0: 0000 0072 0200 0000 720d 0000 0072 3700  ...r....r....r7.
+00002b00: 0000 7213 0000 0072 0600 0000 7265 0000  ..r....r....re..
+00002b10: 00da 0a73 706c 6974 6c69 6e65 73da 0569  ...splitlines..i
+00002b20: 6e64 6578 720f 0000 0029 0672 1500 0000  ndexr....).r....
+00002b30: 723f 0000 005a 086c 6f67 5f70 6174 685a  r?...Z.log_pathZ
+00002b40: 046c 6f67 735a 1174 6162 6c65 5f73 7461  .logsZ.table_sta
+00002b50: 7274 5f69 6e64 6578 5a0f 7461 626c 655f  rt_indexZ.table_
+00002b60: 656e 645f 696e 6465 7872 1600 0000 7216  end_indexr....r.
+00002b70: 0000 0072 1700 0000 726c 0000 0047 0100  ...r....rl...G..
+00002b80: 0073 1000 0000 0008 0601 0801 1e01 0e02  .s..............
+00002b90: 0a01 1602 2e02 7a1e 4d6f 6465 6c6c 6572  ......z.Modeller
+00002ba0: 5f6d 616e 6167 6572 2e6c 6f61 645f 6c6f  _manager.load_lo
+00002bb0: 675f 6669 6c65 2912 da08 5f5f 6e61 6d65  g_file)...__name
+00002bc0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00002bd0: 5f5f 7175 616c 6e61 6d65 5f5f da04 6c69  __qualname__..li
+00002be0: 7374 7239 0000 0072 2700 0000 7218 0000  str9...r'...r...
+00002bf0: 0072 1f00 0000 da04 626f 6f6c 722b 0000  .r......boolr+..
+00002c00: 0072 1e00 0000 7245 0000 0072 4700 0000  .r....rE...rG...
+00002c10: 7249 0000 0072 6000 0000 721d 0000 0072  rI...r`...r....r
+00002c20: 7200 0000 726c 0000 0072 1600 0000 7216  r...rl...r....r.
+00002c30: 0000 0072 1600 0000 7217 0000 0072 0500  ...r....r....r..
+00002c40: 0000 0800 0000 731a 0000 0008 0106 0104  ......s.........
+00002c50: ff0c 1008 090e 1c08 3f10 1e10 0c10 0f10  ........?.......
+00002c60: 4d08 2b0e 1972 0500 0000 2907 726e 0000  M.+..r....).rn..
+00002c70: 0072 7100 0000 da07 7061 7468 6c69 6272  .rq.....pathlibr
+00002c80: 0200 0000 da0c 6669 6c65 5f68 616e 646c  ......file_handl
+00002c90: 6572 7204 0000 0072 0500 0000 7216 0000  err....r....r...
+00002ca0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002cb0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00002cc0: 0000 0008 0108 010c 020c 03              ...........
```

### Comparing `monviso-0.1.1/monviso_reloaded/__pycache__/template.cpython-39.pyc` & `monviso-0.1.2/monviso_reloaded/__pycache__/template.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/base.py` & `monviso-0.1.2/monviso_reloaded/base.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/cli.py` & `monviso-0.1.2/monviso_reloaded/cli.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/cobalt_wrapper.py` & `monviso-0.1.2/monviso_reloaded/cobalt_wrapper.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/database_parser.py` & `monviso-0.1.2/monviso_reloaded/database_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/file_handler.py` & `monviso-0.1.2/monviso_reloaded/file_handler.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/gene.py` & `monviso-0.1.2/monviso_reloaded/gene.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/input_parser.py` & `monviso-0.1.2/monviso_reloaded/input_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/isoform.py` & `monviso-0.1.2/monviso_reloaded/isoform.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/monviso_reloaded/modeller_manager.py` & `monviso-0.1.2/monviso_reloaded/modeller_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,18 @@
             + """\",
     assess_methods=(assess.DOPE, assess.GA341))
 a.starting_model= 1
 a.ending_model  = """+str(self.num_models)+"""
 a.make()
 ok_models = filter(lambda x: x['failure'] is None, a.outputs)
 toscore = 'DOPE score'
-ok_models = sorted(ok_models, key=lambda k: k[toscore])
-models = [m for m in ok_models[0:10]]
+
+models= list(ok_models) if isinstance(ok_models, type(filter(lambda: None, []))) else ok_models
+models.sort(lambda k: k[toscore])
+
 myout = open(\""""
             + output_name
             + """\", "w")
 for m in models:
         myout.write(str(m['name']) + " (DOPE SCORE: %.3f)" % (m[toscore]))
 env.libs.topology.read(file='$(LIB)/top_heav.lib')
 env.libs.parameters.read(file='$(LIB)/par.lib')
```

### Comparing `monviso-0.1.1/monviso_reloaded/template.py` & `monviso-0.1.2/monviso_reloaded/template.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.1/setup.py` & `monviso-0.1.2/setup.py`

 * *Files identical despite different names*

