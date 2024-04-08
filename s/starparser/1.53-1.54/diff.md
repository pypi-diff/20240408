# Comparing `tmp/starparser-1.53.tar.gz` & `tmp/starparser-1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starparser-1.53.tar", last modified: Mon Apr  8 15:18:47 2024, max compression
+gzip compressed data, was "starparser-1.54.tar", last modified: Mon Apr  8 18:32:49 2024, max compression
```

## Comparing `starparser-1.53.tar` & `starparser-1.54.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.185348 starparser-1.53/
--rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.53/LICENSE.txt
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 15:18:47.185201 starparser-1.53/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.53/README.md
--rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-08 15:18:47.185408 starparser-1.53/setup.cfg
--rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.53/setup.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.184100 starparser-1.53/starparser/
--rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-08 15:16:48.000000 starparser-1.53/starparser/__init__.py
--rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.53/starparser/__main__.py
--rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.53/starparser/argparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.53/starparser/columnplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.53/starparser/decisiontree.py
--rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.53/starparser/fileparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)    21935 2024-04-07 12:48:19.000000 starparser-1.53/starparser/particleplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.53/starparser/plots.py
--rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.53/starparser/specialparticles.py
--rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.53/starparser/splits.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.184981 starparser-1.53/starparser.egg-info/
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/SOURCES.txt
--rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/dependency_links.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/entry_points.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/requires.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/top_level.txt
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 18:32:49.872923 starparser-1.54/
+-rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.54/LICENSE.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 18:32:49.872805 starparser-1.54/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.54/README.md
+-rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-08 18:32:49.872976 starparser-1.54/setup.cfg
+-rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.54/setup.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 18:32:49.871718 starparser-1.54/starparser/
+-rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-08 18:32:17.000000 starparser-1.54/starparser/__init__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.54/starparser/__main__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.54/starparser/argparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.54/starparser/columnplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.54/starparser/decisiontree.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.54/starparser/fileparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    22917 2024-04-08 18:31:32.000000 starparser-1.54/starparser/particleplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.54/starparser/plots.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.54/starparser/specialparticles.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.54/starparser/splits.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 18:32:49.872610 starparser-1.54/starparser.egg-info/
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/SOURCES.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/dependency_links.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/entry_points.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/requires.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-08 18:32:49.000000 starparser-1.54/starparser.egg-info/top_level.txt
```

### Comparing `starparser-1.53/LICENSE.txt` & `starparser-1.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starparser-1.53/PKG-INFO` & `starparser-1.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.53
+Version: 1.54
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `starparser-1.53/README.md` & `starparser-1.54/README.md`

 * *Files identical despite different names*

### Comparing `starparser-1.53/setup.py` & `starparser-1.54/setup.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/argparser.py` & `starparser-1.54/starparser/argparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/columnplay.py` & `starparser-1.54/starparser/columnplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/decisiontree.py` & `starparser-1.54/starparser/decisiontree.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/fileparser.py` & `starparser-1.54/starparser/fileparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/particleplay.py` & `starparser-1.54/starparser/particleplay.py`

 * *Files 5% similar despite different names*

```diff
@@ -279,21 +279,34 @@
     lookup_dict = importfrom_particles.set_index('_rlnImageName')[columnstoswap].to_dict('index')
 
     # Check for duplicates in importfrom_particles
     if importfrom_particles['_rlnImageName'].duplicated().any():
         print("\n>> Error: Duplicate entries found in the star file.\n")
         sys.exit()
 
-    # Perform the swapping of values
+    original_particles['_rlnMatched'] = original_particles['_rlnImageName'].apply(lambda x: x in lookup_dict)
+
+    matched_count = original_particles['_rlnMatched'].sum()    
+
+    if matched_count == 0:
+        print("\n>> Error: could not match any particles to the second file.\n")
+        sys.exit()
+
+    if matched_count != len(original_particles.index):
+        print(f"\n!! Warning: Could not match {len(original_particles.index)-matched_count} particles. Their original values have been kept.\n")
+
+
+    # Perform the swap
     for c in columnstoswap:
-        # Map each value, checking if it exists in the dictionary
-        original_particles[c] = original_particles['_rlnImageName'].apply(
-            lambda x: lookup_dict[x][c] if x in lookup_dict else sys.exit(f"\n>> Error: {x} not found in file that you are importing from.")
+        original_particles[c] = original_particles.apply(
+            lambda row: lookup_dict[row['_rlnImageName']]['_rlnOpticsGroup'] if row['_rlnMatched'] else row[c], axis=1
         )
 
+    original_particles.drop("_rlnMatched", axis=1, inplace=True)
+
     return(original_particles)
 
 """
 --import_mic_values
 """
 def importmicvalues(importedparticles, importfrom_particles, column):
     # Extract the simple micrograph name if necessary
@@ -306,21 +319,32 @@
         importfrom_particles["_rlnMicrographNameSimple"] = importfrom_particles['_rlnMicrographName'].str.split('/').str[-1]
     else:
         importfrom_particles["_rlnMicrographNameSimple"] = importfrom_particles['_rlnMicrographName']
 
     # Create a lookup dictionary from importfrom_particles
     lookup_dict = importfrom_particles.set_index('_rlnMicrographNameSimple')[column].to_dict()
 
-    # Update values in importedparticles using lookup_dict, with error reporting
-    importedparticles[column] = importedparticles['_rlnMicrographNameSimple'].apply(
-        lambda x: lookup_dict[x] if x in lookup_dict else sys.exit(f"\n>> Error: Micrograph {x} not found in original file.")
+    importedparticles['_rlnMatched'] = importedparticles['_rlnMicrographNameSimple'].apply(lambda x: x in lookup_dict)
+    matched_count = importedparticles['_rlnMatched'].sum() 
+
+    if matched_count == 0:
+        print("\n>> Error: could not match any micrographs to the second file.\n")
+        sys.exit()
+
+    if matched_count != len(importedparticles.index):
+        print(f"\n!! Warning: Could not match the micrographs of {len(importedparticles.index)-matched_count} particles. Their original values in {column} have been kept.\n")
+
+    # Update values in importedparticles using lookup_dict
+    importedparticles[column] = importedparticles.apply(
+        lambda row: lookup_dict[row['_rlnMicrographNameSimple']] if row['_rlnMatched'] else row[column], axis=1
     )
 
     # Drop the temporary '_rlnMicrographNameSimple' column
     importedparticles.drop("_rlnMicrographNameSimple", axis=1, inplace=True)
+    importedparticles.drop("_rlnMatched", axis=1, inplace=True)
 
     return(importedparticles)
 
 """
 --expand_optics
 """
 
@@ -417,15 +441,15 @@
 
     #print(newdata)
 
     ####
 
     #print(original_particles["_rlnOpticsGroup"].head())
 
-    expandedparticles = columnplay.importmicvalues(original_particles, newdata, "_rlnOpticsGroup")
+    expandedparticles = importmicvalues(original_particles, newdata, "_rlnOpticsGroup")
 
     totaldifferent = 0
     for i, j in zip(original_particles.iterrows(), expandedparticles.iterrows()):
         if i[1]["_rlnOpticsGroup"] != j[1]["_rlnOpticsGroup"]:
             totaldifferent += 1
 
     print("\n>> The number of particles that have acquired a new optics group number = " + str(totaldifferent) + "\n")
```

### Comparing `starparser-1.53/starparser/plots.py` & `starparser-1.54/starparser/plots.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/specialparticles.py` & `starparser-1.54/starparser/specialparticles.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser/splits.py` & `starparser-1.54/starparser/splits.py`

 * *Files identical despite different names*

### Comparing `starparser-1.53/starparser.egg-info/PKG-INFO` & `starparser-1.54/starparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.53
+Version: 1.54
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

