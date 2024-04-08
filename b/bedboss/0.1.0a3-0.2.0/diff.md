# Comparing `tmp/bedboss-0.1.0a3.tar.gz` & `tmp/bedboss-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedboss-0.1.0a3.tar", last modified: Mon Oct  2 19:23:20 2023, max compression
+gzip compressed data, was "bedboss-0.2.0.tar", last modified: Mon Apr  8 17:58:14 2024, max compression
```

## Comparing `bedboss-0.1.0a3.tar` & `bedboss-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedboss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss/bedmaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedmaker/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21126 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedmaker/bedmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss/bedqc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedqc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3283 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedqc/bedqc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedqc/est_line.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss/bedstat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedstat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8952 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedstat/bedstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedstat/pep_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss/bedstat/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/bedstat/tools/regionstat.R
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/bedboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/bedboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-02 19:23:20.000000 bedboss-0.1.0a3/bedboss.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 19:23:20.664072 bedboss-0.1.0a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2023-10-02 19:23:09.000000 bedboss-0.1.0a3/test/test_bedboss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-08 17:58:05.000000 bedboss-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 17:58:05.000000 bedboss-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 17:58:14.470189 bedboss-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 17:58:05.000000 bedboss-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.462189 bedboss-0.2.0/bedboss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedboss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedbuncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/bedbuncher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedbuncher/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5113 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/tools/bedsetStat.R
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedclassifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedclassifier/bedclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14256 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/bedmaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3354 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/bedqc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/est_line.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedstat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6020 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/bedstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedstat/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/tools/regionstat.R
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/qdrant_index/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/qdrant_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/qdrant_index/qdrant_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3999 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/requirements_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/bedboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:58:14.470189 bedboss-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-08 17:58:05.000000 bedboss-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedbuncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedmaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedstat.py
```

### Comparing `bedboss-0.1.0a3/LICENSE` & `bedboss-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bedboss-0.1.0a3/bedboss/bedqc/bedqc.py` & `bedboss-0.2.0/bedboss/bedqc/bedqc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 def bedqc(
     bedfile: str,
     outfolder: str,
     max_file_size: int = MAX_FILE_SIZE,
     max_region_number: int = MAX_REGION_NUMBER,
     min_region_width: int = MIN_REGION_WIDTH,
     pm: pypiper.PipelineManager = None,
-    **kwargs,
 ) -> bool:
     """
     Perform quality checks on a BED file.
 
     :param bedfile: path to the bed file
     :param outfolder: path to the folder where to store information about pipeline and logs
     :param max_file_size: Maximum file size threshold to pass the quality check.
     :param max_region_number: Maximum number of regions threshold to pass the quality check.
     :param min_region_width: Minimum region width threshold to pass the quality check.
     :param pm: Pypiper object for managing pipeline operations.
     :return: True if the file passes the quality check.
+    :raises QualityException: if the file does not pass the quality
     """
     _LOGGER.info("Running bedqc...")
-    _LOGGER.warning(f"Unused arguments: {kwargs}")
 
-    output_file = os.path.join(outfolder, "flagged_bed.csv")
+    output_file = os.path.join(outfolder, "failed_qc.csv")
     bedfile_name = os.path.basename(bedfile)
     input_extension = os.path.splitext(bedfile_name)[1]
 
-    file_exists = os.path.isfile(bedfile)
+    # file_exists = os.path.isfile(bedfile)
+    if not os.path.exists(outfolder):
+        os.makedirs(outfolder)
 
     # to execute bedqc from inside Python (without using cli) Pypiper is set to default:
     if not pm:
         pm = pypiper.PipelineManager(
             name="bedQC-pipeline", outfolder=outfolder, recover=True, multi=True
         )
 
@@ -94,14 +95,14 @@
     if len(detail) > 0:
         _LOGGER.info("file_name: ", bedfile_name)
         if os.path.exists(output_file):
             with open(output_file, "a") as f:
                 f.write(f"{bedfile_name}\t{detail} \n")
         else:
             with open(output_file, "w") as f:
-                f.write(f"file_name\tdetail \n")
+                f.write("file_name\tdetail \n")
                 f.write(f"{bedfile_name}\t{detail} \n")
 
         raise QualityException(f"{str(detail)}")
 
     _LOGGER.info(f"File ({file}) has passed Quality Control!")
     return True
```

### Comparing `bedboss-0.1.0a3/bedboss/bedstat/bedstat.py` & `bedboss-0.2.0/bedboss/bedbuncher/bedbuncher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,249 @@
-from hashlib import md5
-from typing import NoReturn
-import json
-import yaml
+from geniml.io import BedSet
+from geniml.bbclient import BBClient
+
 import os
-import requests
-import gzip
-import pypiper
-import bbconf
+import json
+import subprocess
+from typing import Union, List
+import peppy
+import pephubclient
+from pephubclient.helpers import is_registry_path
 import logging
 
-_LOGGER = logging.getLogger("bedboss")
+from bbconf import BedBaseAgent
+from bbconf.models.base_models import FileModel
+from bbconf.models.bedset_models import BedSetPlots
+
 
-SCHEMA_PATH_BEDSTAT = os.path.join(
-    os.path.dirname(os.path.realpath(__file__)), "pep_schema.yaml"
-)
+from bedboss.exceptions import BedBossException
 
 
-def digest_bedfile(filepath: str) -> str:
+_LOGGER = logging.getLogger("bedboss")
+
+
+def create_bed_list_file(bedset: BedSet, file_path: str) -> None:
     """
-    Generate digest for bedfile
+    Create a file with bed_set_list (Later this file is used in R script)
 
-    :param str filepath: path to the bed file
-    :return str: digest of the files
+    :param bedset: bed_set object
+    :param file_path: path to the file
+    :return: None
     """
-    with gzip.open(filepath, "rb") as f:
-        # concate column values
-        chrs = ",".join([row.split()[0].decode("utf-8") for row in f])
-        starts = ",".join([row.split()[1].decode("utf-8") for row in f])
-        ends = ",".join([row.split()[2].decode("utf-8") for row in f])
-        # hash column values
-        chr_digest = md5(chrs.encode("utf-8")).hexdigest()
-        start_digest = md5(starts.encode("utf-8")).hexdigest()
-        end_digest = md5(ends.encode("utf-8")).hexdigest()
-        # hash column digests
-        bed_digest = md5(
-            ",".join([chr_digest, start_digest, end_digest]).encode("utf-8")
-        ).hexdigest()
+    list_of_samples = [sample.path for sample in bedset]
 
-        return bed_digest
+    with open(file_path, "w") as f:
+        for sample in list_of_samples:
+            f.write(sample + "\n")
 
+    return None
 
-def convert_unit(size_in_bytes: int) -> str:
+
+def create_plots(
+    bedset: List[str],
+    output_folder: str,
+) -> dict:
     """
-    Convert the size from bytes to other units like KB, MB or GB
-    :param int size_in_bytes: size in bytes
-    :return str: File size as string in different units
+    Create plots for a bedset (commonality region plot)
+
+    :param bedset: list of bedfiles ids
+    :param output_folder: path to the output folder
+    :return: dict with information about crated plots
     """
-    if size_in_bytes < 1024:
-        return str(size_in_bytes) + "bytes"
-    elif size_in_bytes in range(1024, 1024 * 1024):
-        return str(round(size_in_bytes / 1024, 2)) + "KB"
-    elif size_in_bytes in range(1024 * 1024, 1024 * 1024 * 1024):
-        return str(round(size_in_bytes / (1024 * 1024))) + "MB"
-    elif size_in_bytes >= 1024 * 1024 * 1024:
-        return str(round(size_in_bytes / (1024 * 1024 * 1024))) + "GB"
+    bbclient_obj = BBClient()
 
+    bed_set_object = BedSet()
+    for bed_id in bedset:
+        bed_set_object.add(bbclient_obj.load_bed(bed_id))
 
-def bedstat(
-    bedfile: str,
-    bedbase_config: str,
-    genome: str,
-    outfolder: str,
-    ensdb: str = None,
-    open_signal_matrix: str = None,
-    bigbed: str = None,
-    sample_yaml: str = None,
-    just_db_commit: bool = False,
-    no_db_commit: bool = False,
+    bedset_md5sum = bed_set_object.identifier
+
+    # if output folder doesn't exist create it
+    if not os.path.exists(output_folder):
+        os.makedirs(output_folder)
+    bedset_list_path = os.path.join(output_folder, f"{bedset_md5sum}_bedset.txt")
+    create_bed_list_file(bed_set_object, bedset_list_path)
+    rscript_path = os.path.join(
+        os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
+        "bedbuncher",
+        "tools",
+        "bedsetStat.R",
+    )
+    assert os.path.exists(rscript_path), FileNotFoundError(
+        f"'{rscript_path}' script not found"
+    )
+
+    json_file_path = os.path.join(output_folder, bedset_md5sum + ".json")
+    command = (
+        f"Rscript {rscript_path} --outputfolder={output_folder} "
+        f"--bedfilelist={bedset_list_path} --id={bedset_md5sum} "
+        f"--json={json_file_path}"
+    )
+
+    subprocess.run(command, shell=True)
+
+    with open(json_file_path, "r", encoding="utf-8") as f:
+        bedset_summary_info = json.loads(f.read())
+
+    os.remove(bedset_list_path)
+    os.remove(json_file_path)
+
+    _LOGGER.info("Plots were created successfully and mediated files were removed")
+    return bedset_summary_info["plots"][0]
+
+
+def run_bedbuncher(
+    bedbase_config: Union[str, BedBaseAgent],
+    record_id: str,
+    bed_set: List[str],
+    output_folder: str,
+    name: str = None,
+    description: str = None,
+    heavy: bool = False,
+    upload_pephub: bool = False,
+    upload_s3: bool = False,
+    no_fail: bool = False,
     force_overwrite: bool = False,
-    skip_qdrant: bool = False,
-    pm: pypiper.PipelineManager = None,
-    **kwargs,
-) -> NoReturn:
-    """
-    Run bedstat pipeline - pipeline for obtaining statistics about bed files
-        and inserting them into the database
-
-    :param str bedfile: the full path to the bed file to process
-    :param str bigbed: the full path to the bigbed file. Defaults to None.
-        (bigbed won't be created and some producing of some statistics will
-        be skipped.)
-    :param str bedbase_config: The path to the bedbase configuration file.
-    :param str open_signal_matrix: a full path to the openSignalMatrix
-        required for the tissue specificity plots
-    :param str outfolder: The folder for storing the pipeline results.
-    :param str genome: genome assembly of the sample
-    :param str ensdb: a full path to the ensdb gtf file required for genomes
-        not in GDdata
-    :param str sample_yaml: a yaml config file with sample attributes to pass
-        on more metadata
-        into the database
-    :param bool just_db_commit: whether just to commit the JSON to the database
-    :param bool no_db_commit: whether the JSON commit to the database should be
-        skipped
-    :param skip_qdrant: whether to skip qdrant indexing
-    :param bool force_overwrite: whether to overwrite the existing record
-    :param pm: pypiper object
-    """
-    # TODO why are we no longer using bbconf to get the output path?
-    # outfolder_stats = bbc.get_bedstat_output_path()
-    outfolder_stats = os.path.join(outfolder, "output", "bedstat_output")
-    try:
-        os.makedirs(outfolder_stats)
-    except FileExistsError:
-        pass
-    bbc = bbconf.BedBaseConf(config_path=bedbase_config, database_only=True)
-
-    bed_digest = md5(open(bedfile, "rb").read()).hexdigest()
-    bedfile_name = os.path.split(bedfile)[1]
-
-    fileid = os.path.splitext(os.path.splitext(bedfile_name)[0])[0]
-    outfolder = os.path.abspath(os.path.join(outfolder_stats, bed_digest))
-    try:
-        os.makedirs(outfolder)
-    except FileExistsError:
-        pass
-    json_file_path = os.path.abspath(os.path.join(outfolder, fileid + ".json"))
-    json_plots_file_path = os.path.abspath(
-        os.path.join(outfolder, fileid + "_plots.json")
-    )
-    bed_relpath = os.path.relpath(
-        bedfile,
-        os.path.abspath(os.path.join(outfolder_stats, os.pardir, os.pardir)),
-    )
-    bigbed_relpath = os.path.relpath(
-        os.path.join(bigbed, fileid + ".bigBed"),
-        os.path.abspath(os.path.join(outfolder_stats, os.pardir, os.pardir)),
-    )
-    if not just_db_commit:
-        if force_overwrite:
-            new_start = True
-
-        if not pm:
-            pm = pypiper.PipelineManager(
-                name="bedstat-pipeline",
-                outfolder=outfolder,
-            )
-
-        rscript_path = os.path.join(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
-            "bedstat",
-            "tools",
-            "regionstat.R",
-        )
-        assert os.path.exists(rscript_path), FileNotFoundError(
-            f"'{rscript_path}' script not found"
-        )
-        command = (
-            f"Rscript {rscript_path} --bedfilePath={bedfile} "
-            f"--fileId={fileid} --openSignalMatrix={open_signal_matrix} "
-            f"--outputFolder={outfolder} --genome={genome} "
-            f"--ensdb={ensdb} --digest={bed_digest}"
-        )
+) -> None:
+    """
+    Add bedset to the database
 
-        pm.run(cmd=command, target=json_file_path)
+    :param bedbase_config: BedBaseConf object
+    :param record_id: record identifier or name to be used in database
+    :param name: name of the bedset
+    :param output_folder: path to the output folder
+    :param bed_set: Bedset object or list of bedfiles ids
+    :param description: Bedset description
+    :param heavy: whether to use heavy processing (add all columns to the database).
+        if False -> R-script won't be executed, only basic statistics will be calculated
+    :param no_fail: whether to raise an error if bedset was not added to the database
+    :param upload_pephub: whether to create a view in pephub
+    :param upload_s3: whether to upload files to s3
+    :param force_overwrite: whether to overwrite the record in the database
+    # TODO: force_overwrite is not working!!! Fix it!
+    :return:
+    """
+    _LOGGER.info(f"Adding bedset { record_id} to the database")
+
+    if isinstance(bedbase_config, str):
+        bbagent = BedBaseAgent(bedbase_config)
+    else:
+        bbagent = bedbase_config
+
+    if not record_id:
+        raise BedBossException(
+            "bedset_name was not provided correctly. Please provide it in pep name or as argument"
+        )
+
+    output_folder = os.path.join(
+        output_folder,
+        "bedsets",
+    )
 
-    # commit to the database if no_db_commit is not set
-    if not no_db_commit:
-        data = {}
-        if os.path.exists(json_file_path):
-            with open(json_file_path, "r", encoding="utf-8") as f:
-                data = json.loads(f.read())
-        if os.path.exists(json_plots_file_path):
-            with open(json_plots_file_path, "r", encoding="utf-8") as f_plots:
-                plots = json.loads(f_plots.read())
-        else:
-            plots = []
-        if sample_yaml and os.path.exists(sample_yaml):
-            # get the sample-specific metadata from the sample yaml representation
-            y = yaml.safe_load(open(sample_yaml, "r"))
-            # if schema and os.path.exists(schema):
-            schema = yaml.safe_load(open(SCHEMA_PATH_BEDSTAT, "r"))
-            schema = schema["properties"]["samples"]["items"]["properties"]
-
-            for key in list(y):
-                if key in schema:
-                    if not schema[key]["db_commit"]:
-                        y.pop(key, None)
-                elif key in [
-                    "bedbase_config",
-                    "pipeline_interfaces",
-                    "yaml_file",
-                ]:
-                    y.pop(key, None)
-            data.update({"other": y})
-        # unlist the data, since the output of regionstat.R is a dict of lists of
-        # length 1 and force keys to lower to correspond with the
-        # postgres column identifiers
-        data = {k.lower(): v[0] if isinstance(v, list) else v for k, v in data.items()}
-        data.update(
-            {
-                "bedfile": {
-                    "path": bed_relpath,
-                    "size": os.path.getsize(bedfile),
-                    "title": "Path to the BED file",
-                }
-            }
-        )
+    if heavy:
+        _LOGGER.info("Heavy processing is True. Calculating plots...")
+        plot_value = create_plots(
+            bedset=bed_set,
+            output_folder=output_folder,
+        )
+        plots = BedSetPlots(region_commonality=FileModel(**plot_value))
+    else:
+        _LOGGER.info("Heavy processing is False. Plots won't be calculated")
+        plots = None
+
+    bbagent.bedset.create(
+        identifier=record_id,
+        name=name,
+        bedid_list=bed_set,
+        statistics=True,
+        description=description,
+        upload_pephub=upload_pephub,
+        upload_s3=upload_s3,
+        plots=plots.model_dump(exclude_none=True, exclude_unset=True),
+        local_path=output_folder,
+        no_fail=no_fail,
+    )
 
-        if os.path.exists(os.path.join(bigbed, fileid + ".bigBed")):
-            data.update(
-                {
-                    "bigbedfile": {
-                        "path": bigbed_relpath,
-                        "size": os.path.getsize(
-                            os.path.join(bigbed, fileid + ".bigBed")
-                        ),
-                        "title": "Path to the big BED file",
-                    }
-                }
-            )
-
-            if not os.path.islink(os.path.join(bigbed, fileid + ".bigBed")):
-                digest = requests.get(
-                    f"http://refgenomes.databio.org/genomes/genome_digest/{genome}"
-                ).text.strip('""')
-
-                data.update(
-                    {
-                        "genome": {
-                            "alias": genome,
-                            "digest": digest,
-                        }
-                    }
-                )
+
+def run_bedbuncher_form_pep(
+    bedbase_config: str,
+    bedset_pep: Union[str, peppy.Project],
+    output_folder: str,
+    bedset_name: str = None,
+    heavy: bool = False,
+    upload_pephub: bool = False,
+    upload_s3: bool = False,
+    no_fail: bool = False,
+    force_overwrite: bool = False,
+) -> str:
+    """
+    Create bedset from pep and add it to the database
+
+    :param bedbase_config: BedBaseConf object or path to the config file
+    :param bedset_pep: path to the pep file or pephub registry path
+    :param bedset_name: name of the bedset
+    :param output_folder: path to the output folder
+    :param heavy: whether to use heavy processing (add all columns to the database).
+        if False -> R-script won't be executed, only basic statistics will be calculated
+    :param upload_pephub: whether to create a view in pephub
+    :param upload_s3: whether to upload files to s3
+    :param no_fail: whether to raise an error if bedset was not added to the database
+    :param force_overwrite: whether to overwrite the record in the database
+
+    return bedset_name
+    """
+    if isinstance(bedset_pep, peppy.Project):
+        pep_of_bed = bedset_pep
+    elif isinstance(bedset_pep, str):
+        if is_registry_path(bedset_pep):
+            pep_of_bed = pephubclient.PEPHubClient().load_project(bedset_pep)
         else:
-            data.update(
-                {
-                    "genome": {
-                        "alias": genome,
-                        "digest": "",
-                    }
-                }
-            )
-
-        for plot in plots:
-            plot_id = plot["name"]
-            del plot["name"]
-            data.update({plot_id: plot})
-        bbc.bed.report(
-            sample_name=bed_digest,
-            values=data,
-            force_overwrite=force_overwrite,
-        )
+            pep_of_bed = peppy.Project(bedset_pep)
+    else:
+        raise ValueError(
+            "bedset_pep should be either path to the pep file or pephub registry path"
+        )
+
+    bedfiles_list = [
+        bedfile_id.get("record_identifier") or bedfile_id.sample_name
+        for bedfile_id in pep_of_bed.samples
+    ]
+
+    run_bedbuncher(
+        bedbase_config=bedbase_config,
+        record_id=bedset_name or pep_of_bed.name,
+        bed_set=bedfiles_list,
+        output_folder=output_folder,
+        name=bedset_name or pep_of_bed.name,
+        description=pep_of_bed.description,
+        heavy=heavy,
+        upload_pephub=upload_pephub,
+        upload_s3=upload_s3,
+        no_fail=no_fail,
+        force_overwrite=force_overwrite,
+    )
+    return bedset_name
 
-    if not skip_qdrant:
-        bbc.add_bed_to_qdrant(
-            bed_id=bed_digest,
-            bed_file_path=bedfile,
-            payload={"fileid": fileid},
-        )
+
+# if __name__ == "__main__":
+#     run_bedbuncher(
+#         "/home/bnt4me/virginia/repos/bbuploader/config_db_local.yaml",
+#         record_id="test_bedset",
+#         name="This is a name",
+#         bed_set=[
+#             "bbad85f21962bb8d972444f7f9a3a932",
+#             "0dcdf8986a72a3d85805bbc9493a1302",
+#         ],
+#         output_folder="/home/bnt4me/virginia/",
+#         description="This is a description",
+#         upload_s3=True,
+#         no_fail=True,
+#         upload_pephub=True,
+#         heavy=True,
+#     )
+
+# run_bedbuncher_form_pep(
+#     "/home/bnt4me/virginia/repos/bbuploader/config_db_local.yaml",
+#     bedset_name="pephub_test",
+#     bedset_pep="khoroshevskyi/bedbunch:default",
+#     upload_pephub=True,
+# )
```

### Comparing `bedboss-0.1.0a3/bedboss/bedstat/tools/regionstat.R` & `bedboss-0.2.0/bedboss/bedstat/tools/regionstat.R`

 * *Files 1% similar despite different names*

```diff
@@ -137,18 +137,18 @@
           tss <- list(median_TSS_dist = signif(median(abs(TSSdist), na.rm=TRUE), digits = 4))
           bedmeta = append(bedmeta, tss)
         }
         plots = rbind(plots, getPlotReportDF("tssdist", "Region-TSS distance distribution"))
         message("Successfully calculated and plot TSS distance.")
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: TSS distance plot!')
         print(e)
       }
-    ) 
+    )
   }
   
   
   
   # Chromosomes region distribution plot
   if (!exists("bedmeta") ){
     tryCatch(
@@ -161,15 +161,15 @@
           plotBoth("chrombins", plotChromBins(calcChromBinsRef(query, genome)))
         }
         
         plots = rbind(plots, getPlotReportDF("chrombins", "Regions distribution over chromosomes"))
         message("Successfully calculated and plot chromosomes region distribution.")
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Chromosomes region distribution plot!')
         print(e)
       }
     ) 
   }
   
   
   
@@ -203,15 +203,15 @@
             gc_content <- list(gc_content = signif(mean(gcvec), digits = 4))
             bedmeta = append(bedmeta, gc_content)
           }
           plots = rbind(plots, getPlotReportDF("gccontent", "GC content"))
           message("Successfully calculated and plot GC content.")
         },
         error = function(e){
-          message('Caught an error!')
+          message('Caught an error in creating: GC content plot!')
           print(e, gcvec)
         }
       ) 
     }
   }
   
   
@@ -230,21 +230,21 @@
     tryCatch(
       expr = {
         if (!(genome %in% c("hg19", "hg38", "mm10")) && gtffile == "None"){
           message("Ensembl annotation gtf file not provided. Skipping partition plot ... ")
         } else {
           if (genome %in% c("hg19", "hg38", "mm10")) {
             gp = calcPartitionsRef(query, genome)
-            plotBoth("paritions", plotPartitions(gp))
+            plotBoth("partitions", plotPartitions(gp))
           } else {
             partitionList = myPartitionList(gtffile)
             gp = calcPartitions(query, partitionList)
-            plotBoth("paritions", plotPartitions(gp))
+            plotBoth("partitions", plotPartitions(gp))
           }
-          plots = rbind(plots, getPlotReportDF("paritions", "Regions distribution over genomic partitions"))
+          plots = rbind(plots, getPlotReportDF("partitions", "Regions distribution over genomic partitions"))
           # flatten the result returned by the function above
           partiotionNames = as.vector(gp[,"partition"])
           partitionsList = list()
           for(i in seq_along(partiotionNames)){
             partitionsList[[paste0(partiotionNames[i], "_frequency")]] = 
               as.vector(gp[,"Freq"])[i]
             partitionsList[[paste0(partiotionNames[i], "_percentage")]] = 
@@ -253,15 +253,15 @@
           if (exists("bedmeta")){
             bedmeta = append(bedmeta, partitionsList)
           }
           message("Successfully calculated and plot regions distribution over genomic partitions.")
         }
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Partition plot!')
         print(e)
       }
     ) 
   }
  
   
   # Expected partition plots
@@ -280,15 +280,15 @@
             plotBoth("expected_partitions", plotExpectedPartitions(calcExpectedPartitions(query, partitionList, genomeSize)))
           }
           plots = rbind(plots, getPlotReportDF("expected_partitions", "Expected distribution over genomic partitions"))
           message("Successfully calculated and plot expected distribution over genomic partitions.")
         }
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Expected partition plot!')
         print(e)
       }
     ) 
   }
  
   # Cumulative partition plots
   if (!exists("bedmeta") ){
@@ -304,15 +304,15 @@
             plotBoth("cumulative_partitions", plotCumulativePartitions(calcCumulativePartitions(query, partitionList)))
           }
           plots = rbind(plots, getPlotReportDF("cumulative_partitions", "Cumulative distribution over genomic partitions"))
           message("Successfully calculated and plot cumulative distribution over genomic partitions.")
         }
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Cumulative partition plot!')
         print(e)
       }
     ) 
   }
   
   # QThist plot
   if (exists("bedmeta")){
@@ -334,30 +334,30 @@
           mean_region_width <- list(mean_region_width = signif(mean(widths), digits = 4))
           bedmeta = append(bedmeta, mean_region_width)
         }
         plots = rbind(plots, getPlotReportDF("widths_histogram", "Quantile-trimmed histogram of widths"))
         message("Successfully calculated and plot quantile-trimmed histogram of widths.")
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Quantile-trimmed histogram of widths plot!')
         print(e, widths)
       }
     ) 
   }
   
   # Neighbor regions distance plots
   if (!exists("bedmeta") ){
     tryCatch(
       expr = {
         plotBoth("neighbor_distances", plotNeighborDist(calcNeighborDist(query)))
         plots = rbind(plots, getPlotReportDF("neighbor_distances", "Distance between neighbor regions"))
         message("Successfully calculated and plot distance between neighbor regions.")
       },
       error = function(e){
-        message('Caught an error!')
+        message('Caught an error in creating: Distance between neighbor regions plot!')
         print(e)
       }
     ) 
   }
   
   
   # Tissue specificity plot if open signal matrix is provided
@@ -368,15 +368,15 @@
       tryCatch(
         expr = {
           plotBoth("open_chromatin", plotSummarySignal(calcSummarySignal(query, data.table::fread(cellMatrix))))
           plots = rbind(plots, getPlotReportDF("open_chromatin", "Cell specific enrichment for open chromatin"))
           message("Successfully calculated and plot cell specific enrichment for open chromatin.")
         },
         error = function(e){
-          message('Caught an error!')
+          message('Caught an error in creating: Cell specific enrichment for open chromatin plot!')
           print(e)
         }
       ) 
     }
   }
  
   
@@ -417,29 +417,31 @@
 outfolder = opt$outputFolder
 genome = opt$genome
 cellMatrix = opt$openSignalMatrix
 gtffile = opt$ensdb
 
 
 # build BSgenome package ID to check whether it's installed
-if (genome == "T2T"){
+if ( startsWith(genome, "T2T")){
   BSg = "BSgenome.Hsapiens.NCBI.T2T.CHM13v2.0"
 } else {
   if (startsWith(genome, "hg") | startsWith(genome, "grch")) {
-  orgName = "Hsapiens"
+    orgName = "Hsapiens"
   } else if (startsWith(genome, "mm") | startsWith(genome, "grcm")){
-  orgName = "Mmusculus"
+    orgName = "Mmusculus"
   } else if (startsWith(genome, "dm")){
-  orgName = "Dmelanogaster"
+    orgName = "Dmelanogaster"
   } else if (startsWith(genome, "ce")){
-  orgName = "Celegans"
+    orgName = "Celegans"
   } else if (startsWith(genome, "danRer")){
-  orgName = "Drerio"
+    orgName = "Drerio"
   }  else if (startsWith(genome, "TAIR")){
     orgName = "Athaliana"
+  } else {
+    orgName = "Undefined"
   }
   BSg = paste0("BSgenome.", orgName , ".UCSC.", genome)
 }
 
 BSgm = paste0(BSg, ".masked")
 
 # read bed file and run doitall()
```

### Comparing `bedboss-0.1.0a3/bedboss/exceptions.py` & `bedboss-0.2.0/bedboss/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,62 @@
-class OpenSignalMatrixException(Exception):
+class BedBossException(BaseException):
+    """Exception, when bedboss fails."""
+
+    def __init__(self, reason: str = ""):
+        """
+        Optionally provide explanation for exceptional condition.
+
+        :param str reason: some context why error occurred while
+        using BedBoss
+        """
+        super(BedBossException, self).__init__(reason)
+
+
+class OpenSignalMatrixException(BedBossException):
     """Exception when Open Signal Matrix does not exist."""
 
     def __init__(self, reason: str = ""):
         """
         Optionally provide explanation for exceptional condition.
 
         :param str reason: some context why error occurred while
         using Open Signal Matrix
         """
         super(OpenSignalMatrixException, self).__init__(reason)
 
 
-class QualityException(Exception):
+class QualityException(BedBossException):
     """Exception, when quality test of the bed file didn't pass."""
 
     def __init__(self, reason: str = ""):
         """
         Optionally provide explanation for exceptional condition.
 
         :param str reason: reason why quality control wasn't successful
         """
+        self.reason = reason
         super(QualityException, self).__init__(reason)
 
 
-class RequirementsException(Exception):
+class RequirementsException(BedBossException):
     """Exception, when requirement packages are not installed."""
 
     def __init__(self, reason: str = ""):
         """
         Optionally provide explanation for exceptional condition.
 
         :param str reason: additional info about requirements exception
         """
         super(RequirementsException, self).__init__(reason)
+
+
+class BedTypeException(BedBossException):
+    """Exception when Bed Type could not be determined."""
+
+    def __init__(self, reason: str = ""):
+        """
+        Optionally provide explanation for exceptional condition.
+
+        :param str reason: some context why error occurred while
+        using Open Signal Matrix
+        """
+        super(BedTypeException, self).__init__(reason)
```

### Comparing `bedboss-0.1.0a3/setup.py` & `bedboss-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 with open(f"{PACKAGE_NAME}/_version.py", "r") as versionfile:
     __version__ = versionfile.readline().split()[-1].strip("\"'\n")
 
 
 def read_reqs(reqs_name):
     deps = []
-    with open(os.path.join(REQDIR, f"requirements-{reqs_name}.txt"), "r") as f:
-        for l in f:
-            if not l.strip():
+    with open(os.path.join(REQDIR, f"requirements-{reqs_name}.txt"), "r") as file:
+        for line in file:
+            if not line.strip():
                 continue
-            deps.append(l)
+            deps.append(line)
     return deps
 
 
 DEPENDENCIES = read_reqs("all")
 extra["install_requires"] = DEPENDENCIES
 
 scripts = None
@@ -46,30 +46,30 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="project, bioinformatics, sequencing, ngs, workflow",
-    url=f"https://github.com/databio/{PACKAGE_NAME}/",
+    url="https://databio.org",
     authors=[
         "Oleksandr Khoroshevskyi",
         "Michal Stolarczyk",
         "Ognen Duzlevski",
         "Jose Verdezoto",
         "Bingjie Xue",
     ],
+    author_email="khorosh@virginia.edu",
     license="BSD2",
     entry_points={
         "console_scripts": [
             "bedboss = bedboss.__main__:main",
         ],
     },
     package_data={PACKAGE_NAME: ["templates/*"]},
-    scripts=scripts,
     include_package_data=True,
     test_suite="tests",
     tests_require=read_reqs("dev"),
     setup_requires=(
         ["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []
     ),
     **extra,
```

