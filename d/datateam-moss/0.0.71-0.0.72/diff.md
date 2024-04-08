# Comparing `tmp/datateam_moss-0.0.71.tar.gz` & `tmp/datateam_moss-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datateam_moss-0.0.71.tar", last modified: Fri Apr  5 07:44:47 2024, max compression
+gzip compressed data, was "datateam_moss-0.0.72.tar", last modified: Mon Apr  8 10:04:06 2024, max compression
```

## Comparing `datateam_moss-0.0.71.tar` & `datateam_moss-0.0.72.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/src/datateam_moss/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/src/datateam_moss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/src/datateam_moss/algemeen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/src/datateam_moss/dimensioneel_modelleren.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/src/datateam_moss/historisering.py
--rw-r--r--   0 runner    (1001) docker     (127)    23617 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/src/datateam_moss/reversed_modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/src/datateam_moss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-05 07:44:47.000000 datateam_moss-0.0.71/src/datateam_moss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-05 07:44:47.000000 datateam_moss-0.0.71/src/datateam_moss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:44:47.000000 datateam_moss-0.0.71/src/datateam_moss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 07:44:47.000000 datateam_moss-0.0.71/src/datateam_moss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 07:44:47.000000 datateam_moss-0.0.71/src/datateam_moss.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:44:47.666128 datateam_moss-0.0.71/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 07:44:43.000000 datateam_moss-0.0.71/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.791010 datateam_moss-0.0.72/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/src/datateam_moss/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/algemeen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/dimensioneel_modelleren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/historisering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23659 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/src/datateam_moss/reversed_modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/src/datateam_moss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 10:04:06.000000 datateam_moss-0.0.72/src/datateam_moss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:04:06.795010 datateam_moss-0.0.72/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-08 10:04:00.000000 datateam_moss-0.0.72/tests/test.py
```

### Comparing `datateam_moss-0.0.71/LICENSE` & `datateam_moss-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.71/PKG-INFO` & `datateam_moss-0.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datateam_moss
-Version: 0.0.71
+Version: 0.0.72
 Summary: Functions needed for datateam MOSS (municipality of Amsterdam)
 Author-email: Robbin Breeuwer <r.j.breeuwer@amsterdam.nl>, Fried Schölvinck <f.scholvinck@amsterdam.nl>, Koen Hallmann <k.hallmann@amsterdam.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: pandas==1.4.4
```

### Comparing `datateam_moss-0.0.71/README.md` & `datateam_moss-0.0.72/README.md`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.71/pyproject.toml` & `datateam_moss-0.0.72/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datateam_moss"
-version = "0.0.71"
+version = "0.0.72"
 authors = [
   { name="Robbin Breeuwer", email="r.j.breeuwer@amsterdam.nl" },
   { name="Fried Schölvinck", email="f.scholvinck@amsterdam.nl"},
   { name="Koen Hallmann", email="k.hallmann@amsterdam.nl"}
 ]
 description = "Functions needed for datateam MOSS (municipality of Amsterdam)"
 readme = "README.md"
```

### Comparing `datateam_moss-0.0.71/src/datateam_moss/algemeen.py` & `datateam_moss-0.0.72/src/datateam_moss/algemeen.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.71/src/datateam_moss/dimensioneel_modelleren.py` & `datateam_moss-0.0.72/src/datateam_moss/dimensioneel_modelleren.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.71/src/datateam_moss/historisering.py` & `datateam_moss-0.0.72/src/datateam_moss/historisering.py`

 * *Files identical despite different names*

### Comparing `datateam_moss-0.0.71/src/datateam_moss/reversed_modeling.py` & `datateam_moss-0.0.72/src/datateam_moss/reversed_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             'date': 'date',
             'string': 'string',
             'int': 'integer'
         }.get(type, 'string')
 
     def create_datacontract(
         self,
+        name_df: str = "Naam dataset/project"
         version: str = 'v0',
         description: str = f'Description of the dataset',
         business_goal: str = 'Business goal of the dataset',
         theme: str = 'X',
         collection: str = 'X',
         datateam: str = 'MOSS',
         product_owner: str = 'x.name@amsterdam.nl',
@@ -165,15 +166,15 @@
                         }
                     } for row in group.to_dict('records')
                 ]
             } for table_name, group in pandas_df.groupby('table_name')
         ]
 
         data_contract = {
-            "Name": self.dataset,
+            "Name": name_df,
             "Version": version,
             "Description": description,
             "Business goal": business_goal,
             "Theme": theme,
             "Collection": collection,
             "Data Team": datateam,
             "Data Product Owner": product_owner,
@@ -555,8 +556,8 @@
 # DATASET = 'amis'
 
 # dataset = Dataset(
 #     spark_session=spark,
 #     catalog=CATALOG,
 #     schema=SCHEMA,
 #     dataset=DATASET,
-# )
+# )
```

### Comparing `datateam_moss-0.0.71/src/datateam_moss.egg-info/PKG-INFO` & `datateam_moss-0.0.72/src/datateam_moss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datateam_moss
-Version: 0.0.71
+Version: 0.0.72
 Summary: Functions needed for datateam MOSS (municipality of Amsterdam)
 Author-email: Robbin Breeuwer <r.j.breeuwer@amsterdam.nl>, Fried Schölvinck <f.scholvinck@amsterdam.nl>, Koen Hallmann <k.hallmann@amsterdam.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: pandas==1.4.4
```

### Comparing `datateam_moss-0.0.71/tests/test.py` & `datateam_moss-0.0.72/tests/test.py`

 * *Files identical despite different names*

