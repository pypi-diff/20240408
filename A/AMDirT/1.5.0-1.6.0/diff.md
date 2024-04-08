# Comparing `tmp/AMDirT-1.5.0.tar.gz` & `tmp/AMDirT-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AMDirT-1.5.0.tar", last modified: Thu Feb 15 12:41:02 2024, max compression
+gzip compressed data, was "AMDirT-1.6.0.tar", last modified: Mon Apr  8 11:47:33 2024, max compression
```

## Comparing `AMDirT-1.5.0.tar` & `AMDirT-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.711138 AMDirT-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/assets/tables.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/autofill/
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/autofill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/core/
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/core/ena.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/merge/
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/merge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/validate/application/
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/validate/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/validate/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/validate/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/validate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-02-15 12:41:00.000000 AMDirT-1.5.0/AMDirT/viewer/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 12:41:02.707138 AMDirT-1.5.0/AMDirT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-15 12:41:02.000000 AMDirT-1.5.0/AMDirT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-15 12:41:00.000000 AMDirT-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-02-15 12:41:02.711138 AMDirT-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-02-15 12:41:00.000000 AMDirT-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 12:41:02.711138 AMDirT-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-15 12:41:00.000000 AMDirT-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/assets/tables.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/autofill/
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/autofill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    15915 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/core/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/core/ena.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/AMDirT/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/merge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/AMDirT/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/AMDirT/validate/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/validate/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/AMDirT/validate/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/validate/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/validate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.752009 AMDirT-1.6.0/AMDirT/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-04-08 11:47:31.000000 AMDirT-1.6.0/AMDirT/viewer/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:47:33.748009 AMDirT-1.6.0/AMDirT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:47:33.000000 AMDirT-1.6.0/AMDirT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 11:47:31.000000 AMDirT-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-08 11:47:33.752009 AMDirT-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-08 11:47:31.000000 AMDirT-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:47:33.752009 AMDirT-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-08 11:47:31.000000 AMDirT-1.6.0/setup.py
```

### Comparing `AMDirT-1.5.0/AMDirT/assets/tables.json` & `AMDirT-1.6.0/AMDirT/assets/tables.json`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/autofill/__init__.py` & `AMDirT-1.6.0/AMDirT/autofill/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/cli.py` & `AMDirT-1.6.0/AMDirT/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import click
 from AMDirT import __version__
 
 from AMDirT.validate import run_validation
 from AMDirT.viewer import run_app
 from AMDirT.convert import run_convert
-from AMDirT.core import get_json_path
+from AMDirT.core import get_json_path, get_amdir_tags, get_latest_tag
 from AMDirT.autofill import run_autofill
 from AMDirT.merge import merge_new_df
+from AMDirT.download import download as download_amdir
 from json import load
 
 
 class MutuallyExclusiveOption(click.Option):
     # Credits goes to Stan Chang for this code snippet
     # https://gist.github.com/stanchan/bce1c2d030c76fe9223b5ff6ad0f03db
 
@@ -290,9 +291,49 @@
     \b
 
     DATASET: path to tsv file of new dataset to merge
     """
     merge_new_df(**kwargs, **ctx.obj)
 
 
+@cli.command()
+@click.option(
+    "-t",
+    "--table",
+    help="AncientMetagenomeDir table to download",
+    type=click.Choice(get_table_list()),
+    default="ancientmetagenome-hostassociated",
+    show_default=True,
+)
+@click.option(
+    "-y",
+    "--table_type",
+    help="Type of table to download",
+    type=click.Choice(["samples", "libraries"]),
+    default="samples",
+    show_default=True,
+)
+@click.option(
+    "-r",
+    "--release",
+    help="Release tag to download",
+    type=click.Choice(get_amdir_tags()),
+    default=get_latest_tag(get_amdir_tags()),
+    show_default=True,
+)
+@click.option(
+    "-o",
+    "--output",
+    help="Output directory",
+    type=click.Path(writable=True),
+    default=".",
+    show_default=True,
+)
+def download(no_args_is_help=True, **kwargs):
+    """\b
+    Download a table from the AMDirT repository
+    """
+    download_amdir(**kwargs)
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `AMDirT-1.5.0/AMDirT/convert/__init__.py` & `AMDirT-1.6.0/AMDirT/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/core/__init__.py` & `AMDirT-1.6.0/AMDirT/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Tuple, Iterable
 from pathlib import Path
 import requests
 from numpy import where
 import pandas as pd
 import streamlit as st
 from packaging import version
+from packaging.version import InvalidVersion
 from importlib.resources import files as get_module_dir
 import os
 import logging
 import colorlog
 from json import load
 
 
@@ -61,15 +62,42 @@
     if r.status_code == 200:
         return [
             tag["name"]
             for tag in r.json()
             if version.parse(tag["name"]) >= version.parse("v22.09")
         ]
     else:
-        return []
+        logger.warning(
+            "Could not fetch tags from AncientMetagenomeDir. Defaulting to master. Metadata may not yet be officially released."
+        )
+        return ["master"]
+
+
+@st.cache_data
+def get_latest_tag(tags):
+    try:
+        return sorted(tags, key=lambda x: version.Version(x))[-1]
+    except InvalidVersion:
+        if "master" in tags:
+            return "master"
+        else:
+            raise InvalidVersion("No valid tags found")
+
+
+def check_allowed_values(ref: list, test: str):
+    """
+    Check if test is in ref
+    Args:
+        ref(list): List of allowed values
+        test(str): value to check
+    """
+
+    if test in ref:
+        return True
+    return False
 
 
 def get_colour_chemistry(instrument: str) -> int:
     """
     Get number of colours used in sequencing chemistry
     Args:
         instrument(str): Name of the instrument
```

### Comparing `AMDirT-1.5.0/AMDirT/core/diff.py` & `AMDirT-1.6.0/AMDirT/core/diff.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/core/ena.py` & `AMDirT-1.6.0/AMDirT/core/ena.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/merge/__init__.py` & `AMDirT-1.6.0/AMDirT/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/validate/__init__.py` & `AMDirT-1.6.0/AMDirT/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/validate/application/__init__.py` & `AMDirT-1.6.0/AMDirT/validate/application/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/validate/domain/__init__.py` & `AMDirT-1.6.0/AMDirT/validate/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/validate/exceptions.py` & `AMDirT-1.6.0/AMDirT/validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/viewer/__init__.py` & `AMDirT-1.6.0/AMDirT/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT/viewer/streamlit.py` & `AMDirT-1.6.0/AMDirT/viewer/streamlit.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/AMDirT.egg-info/PKG-INFO` & `AMDirT-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1
-Name: AMDirT
-Version: 1.5.0
-Summary: AMDirT: AncientMetagenomeDir Toolkit
-Home-page: https://github.com/SPAAM-community/AMDirT
-License: GNU-GPLv3
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular.png#gh-light-mode-only) 
-
-</div>
-
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_dark.png#gh-dark-mode-only)
-
-</div>
+  <picture>
+    <img alt="AMDirT Logo" src="https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_transparent.png">
+  </picture>
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
-AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
+AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes.
+
+This tool provides ways to explore and download sequencing data for ancient microbial and environmental (meta)genomes, automatically prepare input samplesheets for a range of bioinformatic processing pipelines, and to validate AncientMetagenomeDir submissions.
 
 For documentation on using the tool, please see [How Tos](https://amdirt.readthedocs.io/en/latest/how_to/index.html), [Tutorials](https://amdirt.readthedocs.io/en/latest/tutorials/index.html) and/or [Quick Reference](https://amdirt.readthedocs.io/en/latest/reference.html).
 
 ## Install
 
+AMDirT has been tested on different Unix systems (macOS and Ubuntu) using Intel and AMD chips. If you suspect that AMDirT isn't working properly because you use a different hardware/OS, please open an [issue on GitHub](https://github.com/SPAAM-community/AMDirT/issues).
+
 ### 1. With [pip](https://pip.pypa.io/en/stable/getting-started/)
 
 ```bash
 pip install amdirt
 ```
 
 ### 2. With conda
@@ -73,9 +58,7 @@
 
 ## More information
 
 For more information, please see the AMDirT Documentation
 
 - Stable: [amdirt.readthedocs.io/en/latest/](https://amdirt.readthedocs.io/en/latest/)
 - Development version: [amdirt.readthedocs.io/en/dev/](https://amdirt.readthedocs.io/en/dev/)
-
-
```

### Comparing `AMDirT-1.5.0/AMDirT.egg-info/SOURCES.txt` & `AMDirT-1.6.0/AMDirT.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 AMDirT/assets/__init__.py
 AMDirT/assets/tables.json
 AMDirT/autofill/__init__.py
 AMDirT/convert/__init__.py
 AMDirT/core/__init__.py
 AMDirT/core/diff.py
 AMDirT/core/ena.py
+AMDirT/download/__init__.py
 AMDirT/merge/__init__.py
 AMDirT/validate/__init__.py
 AMDirT/validate/exceptions.py
 AMDirT/validate/application/__init__.py
 AMDirT/validate/domain/__init__.py
 AMDirT/viewer/__init__.py
 AMDirT/viewer/streamlit.py
```

### Comparing `AMDirT-1.5.0/LICENSE` & `AMDirT-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AMDirT-1.5.0/PKG-INFO` & `AMDirT-1.6.0/AMDirT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.5.0
+Version: 1.6.0
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular.png#gh-light-mode-only) 
-
-</div>
-
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_dark.png#gh-dark-mode-only)
-
-</div>
+  <picture>
+    <img alt="AMDirT Logo" src="https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_transparent.png">
+  </picture>
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
-AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
+AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes.
+
+This tool provides ways to explore and download sequencing data for ancient microbial and environmental (meta)genomes, automatically prepare input samplesheets for a range of bioinformatic processing pipelines, and to validate AncientMetagenomeDir submissions.
 
 For documentation on using the tool, please see [How Tos](https://amdirt.readthedocs.io/en/latest/how_to/index.html), [Tutorials](https://amdirt.readthedocs.io/en/latest/tutorials/index.html) and/or [Quick Reference](https://amdirt.readthedocs.io/en/latest/reference.html).
 
 ## Install
 
+AMDirT has been tested on different Unix systems (macOS and Ubuntu) using Intel and AMD chips. If you suspect that AMDirT isn't working properly because you use a different hardware/OS, please open an [issue on GitHub](https://github.com/SPAAM-community/AMDirT/issues).
+
 ### 1. With [pip](https://pip.pypa.io/en/stable/getting-started/)
 
 ```bash
 pip install amdirt
 ```
 
 ### 2. With conda
```

### Comparing `AMDirT-1.5.0/README.md` & `AMDirT-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
-
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular.png#gh-light-mode-only) 
+Metadata-Version: 2.1
+Name: AMDirT
+Version: 1.6.0
+Summary: AMDirT: AncientMetagenomeDir Toolkit
+Home-page: https://github.com/SPAAM-community/AMDirT
+License: GNU-GPLv3
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-</div>
-
-<div align="center">
-  
-![AMDirT](https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_dark.png#gh-dark-mode-only)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4003825.svg)](https://doi.org/10.5281/zenodo.4003825) [![PyPI version](https://badge.fury.io/py/AMDirT.svg)](https://pypi.org/project/AMDirT) [![Documentation Status](https://readthedocs.org/projects/amdirt/badge/?version=dev)](https://amdirt.readthedocs.io/en/dev/?badge=dev) [![AMDirT-CI](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml/badge.svg)](https://github.com/SPAAM-community/AMDirT/actions/workflows/ci_test.yml)
 
-</div>
+  <picture>
+    <img alt="AMDirT Logo" src="https://raw.githubusercontent.com/SPAAM-community/AMDirT/master/assets/logo_rectangular_transparent.png">
+  </picture>
 
 **AMDirT**: [**A**ncient**M**etagenome**Dir**](https://github.com/SPAAM-community/ancientmetagenomedir) **T**oolkit
 
-AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes. This tool provides ways to validate AncientMetagenomeDir submissions, explore and download sequencing data for ancient microbial and environmental (meta)genomes, and automatically prepare input samplesheets for a range of bioinformatic processing pipelines.
+AMDirT is a toolkit for interacting with the AncientMetagenomeDir metadata repository of ancient metagenomic samples and ancient microbial genomes.
+
+This tool provides ways to explore and download sequencing data for ancient microbial and environmental (meta)genomes, automatically prepare input samplesheets for a range of bioinformatic processing pipelines, and to validate AncientMetagenomeDir submissions.
 
 For documentation on using the tool, please see [How Tos](https://amdirt.readthedocs.io/en/latest/how_to/index.html), [Tutorials](https://amdirt.readthedocs.io/en/latest/tutorials/index.html) and/or [Quick Reference](https://amdirt.readthedocs.io/en/latest/reference.html).
 
 ## Install
 
+AMDirT has been tested on different Unix systems (macOS and Ubuntu) using Intel and AMD chips. If you suspect that AMDirT isn't working properly because you use a different hardware/OS, please open an [issue on GitHub](https://github.com/SPAAM-community/AMDirT/issues).
+
 ### 1. With [pip](https://pip.pypa.io/en/stable/getting-started/)
 
 ```bash
 pip install amdirt
 ```
 
 ### 2. With conda
@@ -62,7 +69,9 @@
 
 ## More information
 
 For more information, please see the AMDirT Documentation
 
 - Stable: [amdirt.readthedocs.io/en/latest/](https://amdirt.readthedocs.io/en/latest/)
 - Development version: [amdirt.readthedocs.io/en/dev/](https://amdirt.readthedocs.io/en/dev/)
+
+
```

### Comparing `AMDirT-1.5.0/setup.py` & `AMDirT-1.6.0/setup.py`

 * *Files identical despite different names*

