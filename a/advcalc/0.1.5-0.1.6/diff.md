# Comparing `tmp/advcalc-0.1.5.tar.gz` & `tmp/advcalc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.5.tar", last modified: Mon Apr  8 00:02:32 2024, max compression
+gzip compressed data, was "advcalc-0.1.6.tar", last modified: Mon Apr  8 00:10:31 2024, max compression
```

## Comparing `advcalc-0.1.5.tar` & `advcalc-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.622763 advcalc-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.581582 advcalc-0.1.5/ADVCALC/
--rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.5/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1631 2024-04-08 00:00:40.000000 advcalc-0.1.5/ADVCALC/cli.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      799 2024-04-08 00:02:32.619215 advcalc-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.616508 advcalc-0.1.5/advcalc.egg-info/
--rw-rw-rw-   0        0        0      799 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 00:02:32.622763 advcalc-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      741 2024-04-08 00:02:26.000000 advcalc-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:10:31.408624 advcalc-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:10:31.370270 advcalc-0.1.6/ADVCALC/
+-rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.6/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1631 2024-04-08 00:00:40.000000 advcalc-0.1.6/ADVCALC/cli.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      799 2024-04-08 00:10:31.407548 advcalc-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 00:10:31.403882 advcalc-0.1.6/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 00:10:31.000000 advcalc-0.1.6/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:10:31.408624 advcalc-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      741 2024-04-08 00:10:27.000000 advcalc-0.1.6/setup.py
```

### Comparing `advcalc-0.1.5/ADVCALC/__init__.py` & `advcalc-0.1.6/ADVCALC/__init__.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.5/ADVCALC/cli.py` & `advcalc-0.1.6/ADVCALC/cli.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.5/LICENSE` & `advcalc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.5/PKG-INFO` & `advcalc-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

### Comparing `advcalc-0.1.5/README.md` & `advcalc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.5/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.6/advcalc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

### Comparing `advcalc-0.1.5/setup.py` & `advcalc-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.1.5' 
+VERSION = '0.1.6' 
 DESCRIPTION = 'Advanced Python Calculator With an API'
 
 setup(
     name="advcalc", 
     version=VERSION,
     author="Zack",
     description=DESCRIPTION,
```

