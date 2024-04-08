# Comparing `tmp/nlit-0.0.96.tar.gz` & `tmp/nlit-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlit-0.0.96.tar", last modified: Mon Apr  8 11:55:07 2024, max compression
+gzip compressed data, was "nlit-0.0.97.tar", last modified: Mon Apr  8 11:56:36 2024, max compression
```

## Comparing `nlit-0.0.96.tar` & `nlit-0.0.97.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:55:07.464437 nlit-0.0.96/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-10-19 13:11:07.000000 nlit-0.0.96/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-10-19 13:11:07.000000 nlit-0.0.96/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2083 2024-04-08 11:55:07.464168 nlit-0.0.96/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-10-19 14:59:12.000000 nlit-0.0.96/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:55:07.462087 nlit-0.0.96/nlit/
--rw-r--r--   0 solst      (501) staff       (20)     1655 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     3196 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     5446 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/args.py
--rw-r--r--   0 solst      (501) staff       (20)      182 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     4023 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/biol.py
--rw-r--r--   0 solst      (501) staff       (20)      194 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/bkts.py
--rw-r--r--   0 solst      (501) staff       (20)     1125 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/byte.py
--rw-r--r--   0 solst      (501) staff       (20)      567 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/cell.py
--rw-r--r--   0 solst      (501) staff       (20)     8140 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/clrs.py
--rw-r--r--   0 solst      (501) staff       (20)      295 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/dict.py
--rw-r--r--   0 solst      (501) staff       (20)      524 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/docs.py
--rw-r--r--   0 solst      (501) staff       (20)     3922 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/dund.py
--rw-r--r--   0 solst      (501) staff       (20)      867 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/embs.py
--rw-r--r--   0 solst      (501) staff       (20)      435 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/errs.py
--rw-r--r--   0 solst      (501) staff       (20)     3352 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/expo.py
--rw-r--r--   0 solst      (501) staff       (20)     3504 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/exps.py
--rw-r--r--   0 solst      (501) staff       (20)     1741 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/exts.py
--rw-r--r--   0 solst      (501) staff       (20)      721 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/fmtx.py
--rw-r--r--   0 solst      (501) staff       (20)      439 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/hrdw.py
--rw-r--r--   0 solst      (501) staff       (20)      320 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/math.py
--rw-r--r--   0 solst      (501) staff       (20)      632 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/mods.py
--rw-r--r--   0 solst      (501) staff       (20)     2388 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/mthd.py
--rw-r--r--   0 solst      (501) staff       (20)      572 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/narr.py
--rw-r--r--   0 solst      (501) staff       (20)      706 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/nbks.py
--rw-r--r--   0 solst      (501) staff       (20)     1243 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/ncls.py
--rw-r--r--   0 solst      (501) staff       (20)     4328 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/path.py
--rw-r--r--   0 solst      (501) staff       (20)     1235 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/pddf.py
--rw-r--r--   0 solst      (501) staff       (20)     1310 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/pkgs.py
--rw-r--r--   0 solst      (501) staff       (20)     1399 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/plot.py
--rw-r--r--   0 solst      (501) staff       (20)      391 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/sund.py
--rw-r--r--   0 solst      (501) staff       (20)     4746 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/tens.py
--rw-r--r--   0 solst      (501) staff       (20)      204 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/text.py
--rw-r--r--   0 solst      (501) staff       (20)      229 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/tree.py
--rw-r--r--   0 solst      (501) staff       (20)     3041 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/unit.py
--rw-r--r--   0 solst      (501) staff       (20)      663 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/vals.py
--rw-r--r--   0 solst      (501) staff       (20)      615 2024-04-08 11:54:58.000000 nlit-0.0.96/nlit/vers.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:55:07.463336 nlit-0.0.96/nlit.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2083 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      723 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-19 14:57:45.000000 nlit-0.0.96/nlit.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       20 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-08 11:55:07.000000 nlit-0.0.96/nlit.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      801 2024-03-13 18:37:35.000000 nlit-0.0.96/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-08 11:55:07.464507 nlit-0.0.96/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-10-19 13:11:07.000000 nlit-0.0.96/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:56:36.188712 nlit-0.0.97/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-10-19 13:11:07.000000 nlit-0.0.97/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-10-19 13:11:07.000000 nlit-0.0.97/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2083 2024-04-08 11:56:36.188459 nlit-0.0.97/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-10-19 14:59:12.000000 nlit-0.0.97/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:56:36.186425 nlit-0.0.97/nlit/
+-rw-r--r--   0 solst      (501) staff       (20)     1655 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     3196 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     5446 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/args.py
+-rw-r--r--   0 solst      (501) staff       (20)      182 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     4037 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/biol.py
+-rw-r--r--   0 solst      (501) staff       (20)      194 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/bkts.py
+-rw-r--r--   0 solst      (501) staff       (20)     1125 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/byte.py
+-rw-r--r--   0 solst      (501) staff       (20)      567 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/cell.py
+-rw-r--r--   0 solst      (501) staff       (20)     8140 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/clrs.py
+-rw-r--r--   0 solst      (501) staff       (20)      295 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/dict.py
+-rw-r--r--   0 solst      (501) staff       (20)      524 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/docs.py
+-rw-r--r--   0 solst      (501) staff       (20)     3922 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/dund.py
+-rw-r--r--   0 solst      (501) staff       (20)      867 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/embs.py
+-rw-r--r--   0 solst      (501) staff       (20)      435 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/errs.py
+-rw-r--r--   0 solst      (501) staff       (20)     3352 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/expo.py
+-rw-r--r--   0 solst      (501) staff       (20)     3504 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/exps.py
+-rw-r--r--   0 solst      (501) staff       (20)     1741 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/exts.py
+-rw-r--r--   0 solst      (501) staff       (20)      721 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/fmtx.py
+-rw-r--r--   0 solst      (501) staff       (20)      439 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/hrdw.py
+-rw-r--r--   0 solst      (501) staff       (20)      320 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/math.py
+-rw-r--r--   0 solst      (501) staff       (20)      632 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/mods.py
+-rw-r--r--   0 solst      (501) staff       (20)     2388 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/mthd.py
+-rw-r--r--   0 solst      (501) staff       (20)      572 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/narr.py
+-rw-r--r--   0 solst      (501) staff       (20)      706 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/nbks.py
+-rw-r--r--   0 solst      (501) staff       (20)     1243 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/ncls.py
+-rw-r--r--   0 solst      (501) staff       (20)     4328 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/path.py
+-rw-r--r--   0 solst      (501) staff       (20)     1235 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/pddf.py
+-rw-r--r--   0 solst      (501) staff       (20)     1310 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/pkgs.py
+-rw-r--r--   0 solst      (501) staff       (20)     1399 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/plot.py
+-rw-r--r--   0 solst      (501) staff       (20)      391 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/sund.py
+-rw-r--r--   0 solst      (501) staff       (20)     4746 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/tens.py
+-rw-r--r--   0 solst      (501) staff       (20)      204 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/text.py
+-rw-r--r--   0 solst      (501) staff       (20)      229 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/tree.py
+-rw-r--r--   0 solst      (501) staff       (20)     3041 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/unit.py
+-rw-r--r--   0 solst      (501) staff       (20)      663 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/vals.py
+-rw-r--r--   0 solst      (501) staff       (20)      615 2024-04-08 11:56:32.000000 nlit-0.0.97/nlit/vers.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-08 11:56:36.187550 nlit-0.0.97/nlit.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2083 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      723 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-19 14:57:45.000000 nlit-0.0.97/nlit.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       20 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-08 11:56:36.000000 nlit-0.0.97/nlit.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      801 2024-04-08 11:55:50.000000 nlit-0.0.97/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-08 11:56:36.188768 nlit-0.0.97/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-10-19 13:11:07.000000 nlit-0.0.97/setup.py
```

### Comparing `nlit-0.0.96/LICENSE` & `nlit-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/PKG-INFO` & `nlit-0.0.97/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlit
-Version: 0.0.96
+Version: 0.0.97
 Summary: nlit
 Home-page: https://github.com/dsm-72/nlit
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nlit named string literal str literals
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlit-0.0.96/README.md` & `nlit-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/__init__.py` & `nlit-0.0.97/nlit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.96"
+__version__ = "0.0.97"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `nlit-0.0.96/nlit/_modidx.py` & `nlit-0.0.97/nlit/_modidx.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/args.py` & `nlit-0.0.97/nlit/args.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/biol.py` & `nlit-0.0.97/nlit/biol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/40_biol.ipynb.
 
 # %% auto 0
-__all__ = ['OBS', 'VAR', 'OBSM', 'VARM', 'OBSP', 'VARP', 'UNS', 'LAYER', 'LAYERS', 'MITO', 'RIBO', 'CELL', 'CELLS',
-           'TOTAL_COUNTS', 'BARCODE', 'BARCODES', 'GENE', 'GENES', 'N_GENES', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL',
-           'HVG', 'HIGHLY_VARIABLE', 'COUNTS', 'N_GENES_BY_COUNTS', 'LOG1P_TOTAL_COUNTS', 'ENS', 'ENSG', 'ENSEMBL',
-           'ENSEMBL_ID', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS', 'HUMAN', 'MOUSE', 'HUMAN_TF', 'MOUSE_TF',
-           'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID', 'MOUSE_ENSEMBLE_ID', 'PRENORM', 'DETECTED', 'SCALED_NORMALIZED',
-           'PCT_COUNTS', 'PCT_COUNTS_MITO', 'PCT_COUNTS_RIBO', 'X', 'X_', 'X_PRENORM', 'X_DETECTED',
-           'X_SCALED_NORMALIZED', 'PCA_HVG', 'MAGIC_HVG', 'PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY',
-           'FILTERED_MATRIX', 'SEQ', 'SEQRUN', 'SEQRUNS', 'FIRST_SENS', 'UNIQUE_SENS', 'UNIQUE_SENSITIVITY',
-           'UNIQUE_SENSITIVITIES', 'AnnPart']
+__all__ = ['OBS', 'VAR', 'OBSM', 'VARM', 'OBSP', 'VARP', 'UNS', 'LAYER', 'LAYERS', 'MITO', 'RIBO', 'CELL', 'CELLS', 'TOTAL_CELLS',
+           'BARCODE', 'BARCODES', 'GENE', 'GENES', 'N_GENES', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HVG',
+           'HIGHLY_VARIABLE', 'COUNTS', 'TOTAL_COUNTS', 'N_GENES_BY_COUNTS', 'LOG1P_TOTAL_COUNTS', 'ENS', 'ENSG',
+           'ENSEMBL', 'ENSEMBL_ID', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS', 'HUMAN', 'MOUSE', 'HUMAN_TF',
+           'MOUSE_TF', 'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID', 'MOUSE_ENSEMBLE_ID', 'PRENORM', 'DETECTED',
+           'SCALED_NORMALIZED', 'PCT_COUNTS', 'PCT_COUNTS_MITO', 'PCT_COUNTS_RIBO', 'X', 'X_', 'X_PRENORM',
+           'X_DETECTED', 'X_SCALED_NORMALIZED', 'PCA_HVG', 'MAGIC_HVG', 'PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES',
+           'SENSITIVITY', 'FILTERED_MATRIX', 'SEQ', 'SEQRUN', 'SEQRUNS', 'FIRST_SENS', 'UNIQUE_SENS',
+           'UNIQUE_SENSITIVITY', 'UNIQUE_SENSITIVITIES', 'AnnPart']
 
 # %% ../nbs/40_biol.ipynb 4
 from enum import StrEnum
 
 # %% ../nbs/40_biol.ipynb 5
 from nchr import U1
 from .args import UNIQUE
@@ -40,15 +40,15 @@
 MITO = 'mito'
 RIBO = 'ribo'
 
 # %% ../nbs/40_biol.ipynb 11
 CELL = 'cell'
 CELLS = f'{CELL}s'
 
-TOTAL_COUNTS = f'{TOTAL}{U1}{CELLS}'
+TOTAL_CELLS = f'{TOTAL}{U1}{CELLS}'
 
 # %% ../nbs/40_biol.ipynb 12
 BARCODE = 'barcode'
 BARCODES = f'{BARCODE}s'
 
 # %% ../nbs/40_biol.ipynb 14
 GENE = 'gene'
```

### Comparing `nlit-0.0.96/nlit/byte.py` & `nlit-0.0.97/nlit/byte.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/cell.py` & `nlit-0.0.97/nlit/cell.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/clrs.py` & `nlit-0.0.97/nlit/clrs.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/docs.py` & `nlit-0.0.97/nlit/docs.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/dund.py` & `nlit-0.0.97/nlit/dund.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/embs.py` & `nlit-0.0.97/nlit/embs.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/expo.py` & `nlit-0.0.97/nlit/expo.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/exps.py` & `nlit-0.0.97/nlit/exps.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/exts.py` & `nlit-0.0.97/nlit/exts.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/fmtx.py` & `nlit-0.0.97/nlit/fmtx.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/mods.py` & `nlit-0.0.97/nlit/mods.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/mthd.py` & `nlit-0.0.97/nlit/mthd.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/narr.py` & `nlit-0.0.97/nlit/narr.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/nbks.py` & `nlit-0.0.97/nlit/nbks.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/ncls.py` & `nlit-0.0.97/nlit/ncls.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/path.py` & `nlit-0.0.97/nlit/path.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/pddf.py` & `nlit-0.0.97/nlit/pddf.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/pkgs.py` & `nlit-0.0.97/nlit/pkgs.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/plot.py` & `nlit-0.0.97/nlit/plot.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/tens.py` & `nlit-0.0.97/nlit/tens.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/unit.py` & `nlit-0.0.97/nlit/unit.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/vals.py` & `nlit-0.0.97/nlit/vals.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit/vers.py` & `nlit-0.0.97/nlit/vers.py`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/nlit.egg-info/PKG-INFO` & `nlit-0.0.97/nlit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlit
-Version: 0.0.96
+Version: 0.0.97
 Summary: nlit
 Home-page: https://github.com/dsm-72/nlit
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nlit named string literal str literals
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlit-0.0.96/nlit.egg-info/SOURCES.txt` & `nlit-0.0.97/nlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlit-0.0.96/settings.ini` & `nlit-0.0.97/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = nlit
 lib_name = nlit
-version = 0.0.96
+version = 0.0.97
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = nlit
 nbs_path = nbs
 recursive = True
```

### Comparing `nlit-0.0.96/setup.py` & `nlit-0.0.97/setup.py`

 * *Files identical despite different names*

