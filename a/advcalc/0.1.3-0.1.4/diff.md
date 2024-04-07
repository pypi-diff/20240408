# Comparing `tmp/advcalc-0.1.3.tar.gz` & `tmp/advcalc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.3.tar", last modified: Fri Apr  5 03:57:22 2024, max compression
+gzip compressed data, was "advcalc-0.1.4.tar", last modified: Sun Apr  7 23:54:16 2024, max compression
```

## Comparing `advcalc-0.1.3.tar` & `advcalc-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.528325 advcalc-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.495987 advcalc-0.1.3/ADVCALC/
--rw-rw-rw-   0        0        0     2126 2024-04-05 03:56:50.000000 advcalc-0.1.3/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      754 2024-04-05 03:57:22.524043 advcalc-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-05 03:56:07.000000 advcalc-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 03:57:22.523634 advcalc-0.1.3/advcalc.egg-info/
--rw-rw-rw-   0        0        0      754 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 03:57:22.000000 advcalc-0.1.3/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 03:57:22.528325 advcalc-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      510 2024-04-05 03:57:16.000000 advcalc-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.077266 advcalc-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.016570 advcalc-0.1.4/ADVCALC/
+-rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.4/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1641 2024-04-07 23:50:02.000000 advcalc-0.1.4/ADVCALC/cli.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      799 2024-04-07 23:54:16.074751 advcalc-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.072381 advcalc-0.1.4/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 23:54:16.077795 advcalc-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-04-07 23:53:45.000000 advcalc-0.1.4/setup.py
```

### Comparing `advcalc-0.1.3/ADVCALC/__init__.py` & `advcalc-0.1.4/ADVCALC/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def cbrt(num):
     sum = float(num) ** (1. / 3)
     print(sum)
 
 def pow(num1, num2):
     sum = float(num1) ** float(num2)
     print(sum)
-    
+
 def getAPIKey():
     print("Your API Key is:\n")
     print(f'{apiKey}')
     
 def getCode(ApiKey):
     if str(ApiKey) == str(apiKey):
         print("""
```

### Comparing `advcalc-0.1.3/LICENSE` & `advcalc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.3/PKG-INFO` & `advcalc-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.3
-Summary: Advanced Python Calculator
+Version: 0.1.4
+Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
 
 # ADVCALC
 
 ## How to use it
 ##### First use:
 `pip instal advcalc`
 ##### Then, import it in your python file by using:
```

### Comparing `advcalc-0.1.3/README.md` & `advcalc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.3/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.4/advcalc.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.3
-Summary: Advanced Python Calculator
+Version: 0.1.4
+Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
 
 # ADVCALC
 
 ## How to use it
 ##### First use:
 `pip instal advcalc`
 ##### Then, import it in your python file by using:
```

