# Comparing `tmp/advcalc-0.1.4.tar.gz` & `tmp/advcalc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.4.tar", last modified: Sun Apr  7 23:54:16 2024, max compression
+gzip compressed data, was "advcalc-0.1.5.tar", last modified: Mon Apr  8 00:02:32 2024, max compression
```

## Comparing `advcalc-0.1.4.tar` & `advcalc-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.077266 advcalc-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.016570 advcalc-0.1.4/ADVCALC/
--rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.4/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1641 2024-04-07 23:50:02.000000 advcalc-0.1.4/ADVCALC/cli.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      799 2024-04-07 23:54:16.074751 advcalc-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 23:54:16.072381 advcalc-0.1.4/advcalc.egg-info/
--rw-rw-rw-   0        0        0      799 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 23:54:15.000000 advcalc-0.1.4/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 23:54:16.077795 advcalc-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-04-07 23:53:45.000000 advcalc-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.622763 advcalc-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.581582 advcalc-0.1.5/ADVCALC/
+-rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.5/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1631 2024-04-08 00:00:40.000000 advcalc-0.1.5/ADVCALC/cli.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      799 2024-04-08 00:02:32.619215 advcalc-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 00:02:32.616508 advcalc-0.1.5/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 00:02:32.000000 advcalc-0.1.5/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:02:32.622763 advcalc-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      741 2024-04-08 00:02:26.000000 advcalc-0.1.5/setup.py
```

### Comparing `advcalc-0.1.4/ADVCALC/__init__.py` & `advcalc-0.1.5/ADVCALC/__init__.py`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.4/ADVCALC/cli.py` & `advcalc-0.1.5/ADVCALC/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def getAPIKey():
     print("Your API Key is:\n")
     print(f'{apiKey}')
 
 def getCode():
     ApiKey = input("Enter API Key: ")
-    if str(ApiKey) == str(apiKey):
+    if ApiKey == apiKey:
         print("""
 def advcalc(equation):
     print(eval(equation))
     
 def add(num1, num2):
     sum = float(num1) + float(num2)
     print(sum)
```

### Comparing `advcalc-0.1.4/LICENSE` & `advcalc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.4/PKG-INFO` & `advcalc-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

### Comparing `advcalc-0.1.4/README.md` & `advcalc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.4/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.5/advcalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

