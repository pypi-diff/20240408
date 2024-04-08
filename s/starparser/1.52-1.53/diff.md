# Comparing `tmp/starparser-1.52.tar.gz` & `tmp/starparser-1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starparser-1.52.tar", last modified: Sun Apr  7 13:19:20 2024, max compression
+gzip compressed data, was "starparser-1.53.tar", last modified: Mon Apr  8 15:18:47 2024, max compression
```

## Comparing `starparser-1.52.tar` & `starparser-1.53.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.201904 starparser-1.52/
--rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.52/LICENSE.txt
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-07 13:19:20.201774 starparser-1.52/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.52/README.md
--rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-07 13:19:20.201961 starparser-1.52/setup.cfg
--rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.52/setup.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.200818 starparser-1.52/starparser/
--rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-07 12:47:08.000000 starparser-1.52/starparser/__init__.py
--rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.52/starparser/__main__.py
--rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.52/starparser/argparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.52/starparser/columnplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.52/starparser/decisiontree.py
--rw-r--r--   0 chaaban    (501) staff       (20)    10557 2024-04-07 12:37:09.000000 starparser-1.52/starparser/fileparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)    21935 2024-04-07 12:48:19.000000 starparser-1.52/starparser/particleplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.52/starparser/plots.py
--rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.52/starparser/specialparticles.py
--rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.52/starparser/splits.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-07 13:19:20.201585 starparser-1.52/starparser.egg-info/
--rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/SOURCES.txt
--rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/dependency_links.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/entry_points.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/requires.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-07 13:19:20.000000 starparser-1.52/starparser.egg-info/top_level.txt
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.185348 starparser-1.53/
+-rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.53/LICENSE.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 15:18:47.185201 starparser-1.53/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)    36652 2024-04-07 12:48:53.000000 starparser-1.53/README.md
+-rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-08 15:18:47.185408 starparser-1.53/setup.cfg
+-rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.53/setup.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.184100 starparser-1.53/starparser/
+-rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-08 15:16:48.000000 starparser-1.53/starparser/__init__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.53/starparser/__main__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.53/starparser/argparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.53/starparser/columnplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.53/starparser/decisiontree.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.53/starparser/fileparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    21935 2024-04-07 12:48:19.000000 starparser-1.53/starparser/particleplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.53/starparser/plots.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.53/starparser/specialparticles.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.53/starparser/splits.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-08 15:18:47.184981 starparser-1.53/starparser.egg-info/
+-rw-r--r--   0 chaaban    (501) staff       (20)    36955 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/SOURCES.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/dependency_links.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/entry_points.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/requires.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-08 15:18:47.000000 starparser-1.53/starparser.egg-info/top_level.txt
```

### Comparing `starparser-1.52/LICENSE.txt` & `starparser-1.53/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starparser-1.52/PKG-INFO` & `starparser-1.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.52
+Version: 1.53
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `starparser-1.52/README.md` & `starparser-1.53/README.md`

 * *Files identical despite different names*

### Comparing `starparser-1.52/setup.py` & `starparser-1.53/setup.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/argparser.py` & `starparser-1.53/starparser/argparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/columnplay.py` & `starparser-1.53/starparser/columnplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/decisiontree.py` & `starparser-1.53/starparser/decisiontree.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/fileparser.py` & `starparser-1.53/starparser/fileparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     """
 
     """
     For the second data table, we want to know what kind of table it is
     e.g. data_particles
     """
     try:
-        starfilesplit_test[opticsheaderend:].index("#")
         starfilesplit_test[opticsheaderend:].index("loop_")
     except ValueError:
         print("\n>> Error: could not parse the star file. If it does not have an optics table, add --opticsless.\n")
         sys.exit()
 
     if versionexist:
         opticsdataend = starfilesplit_test[opticsheaderend:].index("#") + opticsheaderend
```

### Comparing `starparser-1.52/starparser/particleplay.py` & `starparser-1.53/starparser/particleplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/plots.py` & `starparser-1.53/starparser/plots.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/specialparticles.py` & `starparser-1.53/starparser/specialparticles.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser/splits.py` & `starparser-1.53/starparser/splits.py`

 * *Files identical despite different names*

### Comparing `starparser-1.52/starparser.egg-info/PKG-INFO` & `starparser-1.53/starparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.52
+Version: 1.53
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

