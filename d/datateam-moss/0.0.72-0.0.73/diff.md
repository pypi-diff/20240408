# Comparing `tmp/datateam_moss-0.0.72.tar.gz` & `tmp/datateam_moss-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datateam_moss-0.0.72.tar", last modified: Mon Apr  8 10:04:06 2024, max compression
+gzip compressed data, was "datateam_moss-0.0.73.tar", last modified: Mon Apr  8 10:19:23 2024, max compression
```

## Comparing `datateam_moss-0.0.72.tar` & `datateam_moss-0.0.73.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.791010 datateam_moss-0.0.72/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/src/datateam_moss/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/algemeen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/dimensioneel_modelleren.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/historisering.py
--rw-r--r--   0 runner    (1001) docker     (127)    23659 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/reversed_modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/src/datateam_moss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:19:23.266952 datateam_moss-0.0.73/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/src/datateam_moss/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/src/datateam_moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/src/datateam_moss/algemeen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/src/datateam_moss/dimensioneel_modelleren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/src/datateam_moss/historisering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23660 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/src/datateam_moss/reversed_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/src/datateam_moss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-04-08 10:19:23.000000 datateam_moss-0.0.73/src/datateam_moss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 10:19:23.000000 datateam_moss-0.0.73/src/datateam_moss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:19:23.000000 datateam_moss-0.0.73/src/datateam_moss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 10:19:23.000000 datateam_moss-0.0.73/src/datateam_moss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 10:19:23.000000 datateam_moss-0.0.73/src/datateam_moss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:19:23.270952 datateam_moss-0.0.73/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-08 10:19:19.000000 datateam_moss-0.0.73/tests/test.py
```

### Comparing `datateam_moss-0.0.72/LICENSE` & `datateam_moss-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.72/pyproject.toml` & `datateam_moss-0.0.73/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datateam_moss"
-version = "0.0.72"
+version = "0.0.73"
 authors = [
   { name="Robbin Breeuwer", email="r.j.breeuwer@amsterdam.nl" },
   { name="Fried Schölvinck", email="f.scholvinck@amsterdam.nl"},
   { name="Koen Hallmann", email="k.hallmann@amsterdam.nl"}
 ]
 description = "Functions needed for datateam MOSS (municipality of Amsterdam)"
 readme = "README.md"
```

### Comparing `datateam_moss-0.0.72/src/datateam_moss/algemeen.py` & `datateam_moss-0.0.73/src/datateam_moss/algemeen.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.72/src/datateam_moss/dimensioneel_modelleren.py` & `datateam_moss-0.0.73/src/datateam_moss/dimensioneel_modelleren.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.72/src/datateam_moss/historisering.py` & `datateam_moss-0.0.73/src/datateam_moss/historisering.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.72/src/datateam_moss/reversed_modeling.py` & `datateam_moss-0.0.73/src/datateam_moss/reversed_modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             'date': 'date',
             'string': 'string',
             'int': 'integer'
         }.get(type, 'string')
 
     def create_datacontract(
         self,
-        name_df: str = "Naam dataset/project"
+        name_df: str = "Naam dataset/project",
         version: str = 'v0',
         description: str = f'Description of the dataset',
         business_goal: str = 'Business goal of the dataset',
         theme: str = 'X',
         collection: str = 'X',
         datateam: str = 'MOSS',
         product_owner: str = 'x.name@amsterdam.nl',
```

### Comparing `datateam_moss-0.0.72/tests/test.py` & `datateam_moss-0.0.73/tests/test.py`

 * *Files identical despite different names*

