# Comparing `tmp/psrdb-3.0.2.tar.gz` & `tmp/psrdb-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psrdb-3.0.2.tar", max compression
+gzip compressed data, was "psrdb-3.0.3.tar", max compression
```

## Comparing `psrdb-3.0.2.tar` & `psrdb-3.0.3.tar`

### file list

```diff
@@ -1,30 +1,38 @@
--rw-r--r--   0        0        0    35149 2023-05-30 05:15:57.018989 psrdb-3.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-30 05:15:57.018989 psrdb-3.0.2/psrdb/__init__.py
--rw-r--r--   0        0        0     2714 2023-11-16 01:56:57.824868 psrdb-3.0.2/psrdb/graphql_client.py
--rw-r--r--   0        0        0     9377 2023-11-16 01:56:57.824868 psrdb-3.0.2/psrdb/graphql_table.py
--rw-r--r--   0        0        0        0 2023-06-02 01:54:24.872472 psrdb-3.0.2/psrdb/scripts/__init__.py
--rw-r--r--   0        0        0     7036 2023-11-23 06:54:49.415087 psrdb-3.0.2/psrdb/scripts/generate_meerkat_json.py
--rwxr-xr-x   0        0        0     4446 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/scripts/ingest_obs.py
--rwxr-xr-x   0        0        0     2539 2023-11-30 03:08:39.588898 psrdb-3.0.2/psrdb/scripts/psrdb.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.331662 psrdb-3.0.2/psrdb/tables/__init__.py
--rw-r--r--   0        0        0     6182 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/calibration.py
--rw-r--r--   0        0        0    10082 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/ephemeris.py
--rw-r--r--   0        0        0     5761 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/main_project.py
--rw-r--r--   0        0        0    30567 2023-11-30 03:08:39.592898 psrdb-3.0.2/psrdb/tables/observation.py
--rw-r--r--   0        0        0     4779 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/pipeline_image.py
--rw-r--r--   0        0        0    17605 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/pipeline_run.py
--rw-r--r--   0        0        0     7390 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/project.py
--rw-r--r--   0        0        0     6119 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/pulsar.py
--rw-r--r--   0        0        0     7640 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/pulsar_fold_result.py
--rw-r--r--   0        0        0     6425 2023-11-30 03:08:39.592898 psrdb-3.0.2/psrdb/tables/residual.py
--rw-r--r--   0        0        0     5190 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/telescope.py
--rw-r--r--   0        0        0     5419 2023-11-16 01:56:57.828868 psrdb-3.0.2/psrdb/tables/template.py
--rw-r--r--   0        0        0    13910 2023-11-30 03:08:39.592898 psrdb-3.0.2/psrdb/tables/toa.py
--rw-r--r--   0        0        0        0 2023-11-07 08:06:24.335662 psrdb-3.0.2/psrdb/utils/__init__.py
--rw-r--r--   0        0        0     2345 2023-11-07 08:06:35.143673 psrdb-3.0.2/psrdb/utils/ephemeris.py
--rw-r--r--   0        0        0     4697 2023-11-07 08:06:35.143673 psrdb-3.0.2/psrdb/utils/header.py
--rw-r--r--   0        0        0     3928 2023-11-07 08:06:24.335662 psrdb-3.0.2/psrdb/utils/other.py
--rw-r--r--   0        0        0     1318 2023-11-07 08:06:24.335662 psrdb-3.0.2/psrdb/utils/residual.py
--rw-r--r--   0        0        0     1374 2023-11-07 08:06:24.335662 psrdb-3.0.2/psrdb/utils/toa.py
--rw-r--r--   0        0        0      891 2023-11-30 03:08:39.592898 psrdb-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 05:15:57.018989 psrdb-3.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-30 05:15:57.018989 psrdb-3.0.3/psrdb/__init__.py
+-rw-r--r--   0        0        0    14969 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/data/l_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     3147 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/data/molonglo_phasing.txt
+-rw-r--r--   0        0        0     1782 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/data/polarisation_calibrators.csv
+-rw-r--r--   0        0        0     5680 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/data/s_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     5441 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/data/uhf_band_gain_calibrators.csv
+-rw-r--r--   0        0        0     2714 2024-04-08 03:59:36.344737 psrdb-3.0.3/psrdb/graphql_client.py
+-rw-r--r--   0        0        0     9359 2024-04-08 03:59:36.344737 psrdb-3.0.3/psrdb/graphql_table.py
+-rw-r--r--   0        0        0      924 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/load_data.py
+-rw-r--r--   0        0        0        0 2023-06-02 01:54:24.872472 psrdb-3.0.3/psrdb/scripts/__init__.py
+-rw-r--r--   0        0        0     6338 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/scripts/generate_meerkat_json.py
+-rw-r--r--   0        0        0     3764 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/scripts/generate_molonglo_json.py
+-rwxr-xr-x   0        0        0     4446 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/scripts/ingest_obs.py
+-rwxr-xr-x   0        0        0     2539 2024-04-08 03:59:36.348736 psrdb-3.0.3/psrdb/scripts/psrdb.py
+-rw-r--r--   0        0        0        0 2023-11-07 08:06:24.331662 psrdb-3.0.3/psrdb/tables/__init__.py
+-rw-r--r--   0        0        0     6182 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/calibration.py
+-rw-r--r--   0        0        0    10082 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/ephemeris.py
+-rw-r--r--   0        0        0     5761 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/main_project.py
+-rw-r--r--   0        0        0    30656 2024-04-08 03:59:36.348736 psrdb-3.0.3/psrdb/tables/observation.py
+-rw-r--r--   0        0        0     4779 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/pipeline_image.py
+-rw-r--r--   0        0        0    17605 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/pipeline_run.py
+-rw-r--r--   0        0        0     7390 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/project.py
+-rw-r--r--   0        0        0     6119 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/pulsar.py
+-rw-r--r--   0        0        0     7640 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/pulsar_fold_result.py
+-rw-r--r--   0        0        0     6495 2024-04-08 03:59:36.348736 psrdb-3.0.3/psrdb/tables/residual.py
+-rw-r--r--   0        0        0     5190 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/telescope.py
+-rw-r--r--   0        0        0     5419 2023-11-16 01:56:57.828868 psrdb-3.0.3/psrdb/tables/template.py
+-rw-r--r--   0        0        0    13910 2024-04-08 03:59:36.348736 psrdb-3.0.3/psrdb/tables/toa.py
+-rw-r--r--   0        0        0        0 2023-11-07 08:06:24.335662 psrdb-3.0.3/psrdb/utils/__init__.py
+-rw-r--r--   0        0        0     2345 2023-11-07 08:06:35.143673 psrdb-3.0.3/psrdb/utils/ephemeris.py
+-rw-r--r--   0        0        0     5879 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/utils/header.py
+-rw-r--r--   0        0        0     3928 2024-04-08 03:59:36.352734 psrdb-3.0.3/psrdb/utils/other.py
+-rw-r--r--   0        0        0     1318 2023-11-07 08:06:24.335662 psrdb-3.0.3/psrdb/utils/residual.py
+-rw-r--r--   0        0        0     1374 2024-04-08 03:59:36.352734 psrdb-3.0.3/psrdb/utils/toa.py
+-rw-r--r--   0        0        0      806 2024-03-21 03:33:05.768496 psrdb-3.0.3/psrdb/utils/upload.py
+-rw-r--r--   0        0        0     1006 2024-04-08 03:59:36.352734 psrdb-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 psrdb-3.0.3/PKG-INFO
```

### Comparing `psrdb-3.0.2/LICENSE` & `psrdb-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/graphql_client.py` & `psrdb-3.0.3/psrdb/graphql_client.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/graphql_table.py` & `psrdb-3.0.3/psrdb/graphql_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,12 +234,12 @@
 
     @classmethod
     def get_default_parser(cls, desc=""):
         from argparse import ArgumentParser
         from os import environ
 
         parser = ArgumentParser(description=desc)
-        parser.add_argument("-t", "--token", nargs=1, default=environ.get("PSRDB_TOKEN"), help="JWT token")
-        parser.add_argument("-u", "--url", nargs=1, default=environ.get("PSRDB_URL", "https://pulsars.org.au/api/"), help="GraphQL URL")
+        parser.add_argument("-t", "--token", default=environ.get("PSRDB_TOKEN"), help="JWT token")
+        parser.add_argument("-u", "--url", default=environ.get("PSRDB_URL", "https://pulsars.org.au/api/"), help="GraphQL URL")
         parser.add_argument("-q", "--quiet", action="store_true", default=False, help="Return ID only")
         parser.add_argument("-v", "--verbose", action="store_true", default=False, help="Increase verbosity")
         return parser
```

### Comparing `psrdb-3.0.2/psrdb/scripts/generate_meerkat_json.py` & `psrdb-3.0.3/psrdb/scripts/generate_meerkat_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,34 +6,24 @@
 import json
 import shlex
 import logging
 import subprocess
 from decouple import config
 from datetime import datetime
 
-import psrchive as psr
-
 from psrdb.utils import header
+from psrdb.utils.upload import generate_obs_length, get_archive_ephemeris
 
 
 CALIBRATIONS_DIR = config("CALIBRATIONS_DIR", "/fred/oz005/users/aparthas/reprocessing_MK/poln_calibration")
 RESULTS_DIR = config("RESULTS_DIR", "/fred/oz005/kronos")
 FOLDING_DIR = config("FOLDING_DIR", "/fred/oz005/timing")
 SEARCH_DIR  = config("SEARCH_DIR",  "/fred/oz005/search")
 
 
-def generate_obs_length(archive):
-    """
-    Determine the length of the observation from the input archive file
-    """
-
-    ar = psr.Archive_load(archive)
-    ar = ar.total()
-    return ar.get_first_Integration().get_duration()
-
 def get_sf_length(sf_files):
     """
     Determine the length of input sf files with the vap command
     """
     comm = f"vap -c length {' '.join(sf_files)}"
     args = shlex.split(comm)
     proc = subprocess.Popen(args, stdout=subprocess.PIPE, text=True, bufsize=1)
@@ -76,29 +66,14 @@
         cal_epoch_dt = datetime.strptime(cal_epoch, "%Y-%m-%d-%H:%M:%S")
         if cal_epoch_dt < utc_start_dt:
             return ("post", cal)
 
     raise RuntimeError(f"Could not find calibration file for utc_start={utc_start}")
 
 
-def get_archive_ephemeris(freq_summed_archive):
-    """
-    Get the ephemeris from the archive file using the vap command.
-    """
-    comm = "vap -E {0}".format(freq_summed_archive)
-    args = shlex.split(comm)
-    proc = subprocess.Popen(args,stdout=subprocess.PIPE)
-    proc.wait()
-    ephemeris_text = proc.stdout.read().decode("utf-8")
-
-    if ephemeris_text.startswith('\n'):
-        # Remove newline character at start of output
-        ephemeris_text = ephemeris_text.lstrip('\n')
-    return ephemeris_text
-
 def main():
     import argparse
 
     parser = argparse.ArgumentParser(description="Ingest PTUSE fold mode observation")
     parser.add_argument("obs_header", type=str, help="obs.header file location")
     parser.add_argument("beam", type=int, help="beam number of the observation")
     parser.add_argument(
```

### Comparing `psrdb-3.0.2/psrdb/scripts/ingest_obs.py` & `psrdb-3.0.3/psrdb/scripts/ingest_obs.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/scripts/psrdb.py` & `psrdb-3.0.3/psrdb/scripts/psrdb.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/calibration.py` & `psrdb-3.0.3/psrdb/tables/calibration.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/ephemeris.py` & `psrdb-3.0.3/psrdb/tables/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/main_project.py` & `psrdb-3.0.3/psrdb/tables/main_project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/observation.py` & `psrdb-3.0.3/psrdb/tables/observation.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     def list(
         self,
         id=None,
         pulsar_name=None,
         telescope_name=None,
         project_id=None,
         project_short=None,
+        main_project="All",
         utcs=None,
         utce=None,
         obs_type='fold',
         unprocessed=None,
         incomplete=None,
     ):
         """Return a list of Observation information based on the `self.field_names` and filtered by the parameters.
@@ -99,14 +100,15 @@
         """Return a list of records matching the id and/or any of the arguments."""
         filters = [
             {"field": "id", "value": id},
             {"field": "pulsar_Name", "value": pulsar_name},
             {"field": "telescope_Name", "value": telescope_name},
             {"field": "project_Id", "value": project_id},
             {"field": "project_Short", "value": project_short},
+            {"field": "mainProject", "value": main_project},
             {"field": "utcStartGte", "value": utcs},
             {"field": "utcStartLte", "value": utce},
             {"field": "obsType", "value": obs_type},
         ]
         if unprocessed is not None:
             filters.append({"field": "unprocessed", "value": unprocessed})
         if incomplete is not None:
```

### Comparing `psrdb-3.0.2/psrdb/tables/pipeline_image.py` & `psrdb-3.0.3/psrdb/tables/pipeline_image.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/pipeline_run.py` & `psrdb-3.0.3/psrdb/tables/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/project.py` & `psrdb-3.0.3/psrdb/tables/project.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/pulsar.py` & `psrdb-3.0.3/psrdb/tables/pulsar.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/pulsar_fold_result.py` & `psrdb-3.0.3/psrdb/tables/pulsar_fold_result.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/residual.py` & `psrdb-3.0.3/psrdb/tables/residual.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,28 +110,31 @@
                     id,
                 }
             }
         }
         """
         # Loop over the lines and grab the important info to reduce upload size
         residual_line_info = []
-        for residual_line in residual_lines[1:]:
+        for residual_line in residual_lines:
             residual_line = residual_line.rstrip("\n")
             # Loop over residual lines and turn into a dict
             residual_dict = residual_line_to_dict(residual_line)
             # return only important info as a comma sperated string
             residual_line_info.append(f"{decode_id(residual_dict['id'])},{residual_dict['mjd']},{residual_dict['residual']},{residual_dict['residual_error']},{residual_dict['residual_phase']}")
         # Upload the residuals 1000 at a time
         responses = []
         for residual_chunk in chunk_list(residual_line_info, 1000):
             self.variables = {
                 'residualLines': residual_chunk,
             }
             responses.append(self.mutation_graphql())
-        return responses[-1]
+        if len(responses) == 0:
+            return None
+        else:
+            return responses[-1]
 
     def process(self, args):
         """Parse the arguments collected by the CLI."""
         self.print_stdout = True
         if args.subcommand == "create":
             with open(args.residual_path, "r") as f:
                 residual_lines = f.readlines()
```

### Comparing `psrdb-3.0.2/psrdb/tables/telescope.py` & `psrdb-3.0.3/psrdb/tables/telescope.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/template.py` & `psrdb-3.0.3/psrdb/tables/template.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/tables/toa.py` & `psrdb-3.0.3/psrdb/tables/toa.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/utils/ephemeris.py` & `psrdb-3.0.3/psrdb/utils/ephemeris.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/utils/header.py` & `psrdb-3.0.3/psrdb/utils/header.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import re
+import csv
 import json
 
+from psrdb.load_data import LBAND_CALIBRATORS, UHFBAND_CALIBRATORS, SBAND_CALIBRATORS, POLARISATION_CALIBRATORS
+
 
 class KeyValueStore:
     def __init__(self, fname):
         self.cfg = {}
         self.read_file(fname)
 
     def read_file(self, fname):
@@ -32,14 +35,18 @@
     def __init__(self, fname):
         KeyValueStore.__init__(self, fname)
 
     def parse(self):
         self.source = self.cfg["SOURCE"]
         self.utc_start = self.cfg["UTC_START"]
         self.telescope = self.cfg["TELESCOPE"]
+        if "BEAM" in self.cfg.keys():
+            self.beam = self.cfg["BEAM"]
+        else:
+            self.beam = None
         if "DELAYCAL_ID" in self.cfg.keys():
             self.delaycal_id = self.cfg["DELAYCAL_ID"]
         else:
             self.delaycal_id = None
         if "PHASEUP_ID" in self.cfg.keys():
             self.phaseup_id  = self.cfg["PHASEUP_ID"]
         else:
@@ -76,40 +83,53 @@
     def parse(self):
         Header.parse(self)
 
         self.proposal_id = self.get("PROPOSAL_ID")
 
         self.nant = len(self.get("ANTENNAE").split(","))
 
-        h_weights = self.get("WEIGHTS_POLH").split(",")
-        v_weights = self.get("WEIGHTS_POLV").rstrip(",").split(",")
         if self.get("WEIGHTS_POLH") == "Unknown" or self.get("WEIGHTS_POLV") == "Unknown":
             self.nant_eff = self.nant
         else:
-            nant_eff_h = 0
-            nant_eff_v = 0
-            for w in h_weights:
-                nant_eff_h += float(w)
-            for w in v_weights:
-                nant_eff_v += float(w)
-            self.nant_eff = int((nant_eff_h + nant_eff_v) / 2)
+            h_weights = self.get("WEIGHTS_POLH")
+            v_weights = self.get("WEIGHTS_POLV")
+            if h_weights == "None" or v_weights == "None":
+                # No weights given so return None
+                self.nant_eff = None
+            else:
+                nant_eff_h = 0
+                nant_eff_v = 0
+                for w in h_weights.split(","):
+                    nant_eff_h += float(w)
+                for w in v_weights.rstrip(",").split(","):
+                    nant_eff_v += float(w)
+                self.nant_eff = int((nant_eff_h + nant_eff_v) / 2)
         self.configuration = json.dumps(self.cfg)
 
         self.machine = "PTUSE"
         self.machine_version = "1.0"
         machine_config = {"machine": "PTUSE", "version": 1.0}
         self.machine_config = json.dumps(machine_config)
 
         if self.get("PERFORM_FOLD") == "1":
             self.fold_dm = float(self.get("FOLD_DM"))
             self.fold_nchan = int(self.get("FOLD_OUTNCHAN"))
-            self.fold_npol = int(self.get("FOLD_OUTNPOL"))
+            if self.get("FOLD_OUTNPOL") != "None":
+                self.fold_npol = int(self.get("FOLD_OUTNPOL"))
             self.fold_nbin = int(self.get("FOLD_OUTNBIN"))
             self.fold_tsubint = int(self.get("FOLD_OUTTSUBINT"))
-            if self.source.endswith(("_N", "_S", "_O")):
+
+            # Get all calibrator names from data files
+            calibrator_names = ("J1939-6342", "J0408-6545")# Flux and bandpass calibration https://skaafrica.atlassian.net/wiki/spaces/ESDKB/pages/1481408634/Flux+and+bandpass+calibration
+            for cal_file in [LBAND_CALIBRATORS, UHFBAND_CALIBRATORS, SBAND_CALIBRATORS, POLARISATION_CALIBRATORS]:
+                with open(cal_file, 'r') as csv_file:
+                    csv_reader = csv.reader(csv_file)
+                    calibrator_names += tuple(row[0] for row in csv_reader)
+            # Ends with are labels for calibrations and starts with are calibrator source names
+            if self.source.endswith(("_N", "_S", "_O")) or self.source.endswith(calibrator_names):
                 self.obs_type = "cal"
             else:
                 self.obs_type = "fold"
         else:
             self.fold_dm = None
             self.fold_nchan = None
             self.fold_npol = None
```

### Comparing `psrdb-3.0.2/psrdb/utils/other.py` & `psrdb-3.0.3/psrdb/utils/other.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/utils/residual.py` & `psrdb-3.0.3/psrdb/utils/residual.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/psrdb/utils/toa.py` & `psrdb-3.0.3/psrdb/utils/toa.py`

 * *Files identical despite different names*

### Comparing `psrdb-3.0.2/pyproject.toml` & `psrdb-3.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "psrdb"
-version = "3.0.2"
+version = "3.0.3"
 description = "CLI for pulsars.org.au"
 authors = ["GWDC"]
 license = "MIT"
 packages = [{include = "psrdb"}]
+include = ["psrdb/data/molonglo_phasing.txt"]
 
 [tool.poetry.scripts]
 psrdb = "psrdb.scripts.psrdb:main"
 generate_meerkat_json = "psrdb.scripts.generate_meerkat_json:main"
+generate_molonglo_json = "psrdb.scripts.generate_molonglo_json:main"
 ingest_obs = "psrdb.scripts.ingest_obs:main"
 remove_fluxcals = "psrdb.scripts.remove_fluxcals:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.25.1"
 python-decouple = "^3.8"
```

### Comparing `psrdb-3.0.2/PKG-INFO` & `psrdb-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrdb
-Version: 3.0.2
+Version: 3.0.3
 Summary: CLI for pulsars.org.au
 License: MIT
 Author: GWDC
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

