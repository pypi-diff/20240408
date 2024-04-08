# Comparing `tmp/nablachem-24.5.tar.gz` & `tmp/nablachem-24.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nablachem-24.5.tar", max compression
+gzip compressed data, was "nablachem-24.6.tar", max compression
```

## Comparing `nablachem-24.5.tar` & `nablachem-24.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.5/LICENSE
--rw-r--r--   0        0        0      559 2024-01-22 10:02:27.526533 nablachem-24.5/README.md
--rw-r--r--   0        0        0      553 2024-04-07 14:07:11.586964 nablachem-24.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.5/src/nablachem/__init__.py
--rw-r--r--   0        0        0    16621 2024-04-07 14:00:22.947057 nablachem-24.5/src/nablachem/alchemy.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nablachem-24.5/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-01-21 09:39:54.867938 nablachem-24.6/LICENSE
+-rw-r--r--   0        0        0      559 2024-01-22 10:02:27.526533 nablachem-24.6/README.md
+-rw-r--r--   0        0        0      553 2024-04-08 10:33:59.743816 nablachem-24.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-21 09:41:21.927909 nablachem-24.6/src/nablachem/__init__.py
+-rw-r--r--   0        0        0    16629 2024-04-08 10:33:43.953820 nablachem-24.6/src/nablachem/alchemy.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nablachem-24.6/PKG-INFO
```

### Comparing `nablachem-24.5/LICENSE` & `nablachem-24.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nablachem-24.5/README.md` & `nablachem-24.6/README.md`

 * *Files identical despite different names*

### Comparing `nablachem-24.5/pyproject.toml` & `nablachem-24.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nablachem"
-version = "24.5"
+version = "24.6"
 description = "Easy access to research code."
 authors = ["von Rudorff, Guido Falk <vonrudorff@uni-kassel.de>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://nablachem.org/code"
 repository = "https://github.com/NablaChem/nablachem"
```

### Comparing `nablachem-24.5/src/nablachem/alchemy.py` & `nablachem-24.6/src/nablachem/alchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,20 +254,20 @@
             for i in range(len(indices)):
                 if indices[i] > 0 and i not in non_zero_columns:
                     abort_mask = True
                     break
             if abort_mask:
                 continue
 
-            indices = tuple([indices[_] for _ in non_zero_columns])
+            mod_indices = tuple([indices[_] for _ in non_zero_columns])
 
             subset_offsets = tuple(map(tuple, subset_offsets))
             try:
                 stencil = findiff.stencils.Stencil(
-                    subset_offsets, partials={indices: 1}, spacings=1
+                    subset_offsets, partials={mod_indices: 1}, spacings=1
                 )
             except:
                 # Numerical issue -> next try
                 continue
             # Did not find a stencil -> next try
             if len(stencil.values) == 0:
                 continue
```

### Comparing `nablachem-24.5/PKG-INFO` & `nablachem-24.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nablachem
-Version: 24.5
+Version: 24.6
 Summary: Easy access to research code.
 Home-page: https://nablachem.org/code
 License: LGPL
 Author: von Rudorff, Guido Falk
 Author-email: vonrudorff@uni-kassel.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

