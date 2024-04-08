# Comparing `tmp/noohayo-1.0.3.tar.gz` & `tmp/noohayo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noohayo-1.0.3.tar", last modified: Mon Apr  8 04:17:51 2024, max compression
+gzip compressed data, was "noohayo-1.0.4.tar", last modified: Mon Apr  8 05:26:34 2024, max compression
```

## Comparing `noohayo-1.0.3.tar` & `noohayo-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 04:17:51.353959 noohayo-1.0.3/
--rw-rw-rw-   0        0        0       54 2024-04-08 04:17:51.352967 noohayo-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6295 2024-04-08 03:44:49.000000 noohayo-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 04:17:51.284390 noohayo-1.0.3/noohayo/
--rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.3/noohayo/__init__.py
--rw-rw-rw-   0        0        0     2168 2024-04-08 04:16:47.000000 noohayo-1.0.3/noohayo/noohayo.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:17:51.351961 noohayo-1.0.3/noohayo/scripts/
--rw-rw-rw-   0        0        0      665 2024-04-06 21:14:24.000000 noohayo-1.0.3/noohayo/scripts/Colorer.py
--rw-rw-rw-   0        0        0     2997 2024-04-08 00:18:51.000000 noohayo-1.0.3/noohayo/scripts/Config.py
--rw-rw-rw-   0        0        0     2381 2024-04-08 04:16:38.000000 noohayo-1.0.3/noohayo/scripts/Fetch.py
--rw-rw-rw-   0        0        0     2842 2024-04-08 04:16:40.000000 noohayo-1.0.3/noohayo/scripts/General.py
--rw-rw-rw-   0        0        0      753 2024-04-08 00:09:33.000000 noohayo-1.0.3/noohayo/scripts/Help.py
--rw-rw-rw-   0        0        0      998 2024-04-08 04:16:43.000000 noohayo-1.0.3/noohayo/scripts/Select.py
--rw-rw-rw-   0        0        0        0 2024-04-08 04:13:02.000000 noohayo-1.0.3/noohayo/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 04:17:51.318966 noohayo-1.0.3/noohayo.egg-info/
--rw-rw-rw-   0        0        0       54 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 04:17:51.000000 noohayo-1.0.3/noohayo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 04:17:51.353959 noohayo-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-08 04:16:34.000000 noohayo-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 05:26:34.363985 noohayo-1.0.4/
+-rw-rw-rw-   0        0        0     6489 2024-04-08 05:26:34.362983 noohayo-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6290 2024-04-08 05:19:17.000000 noohayo-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 05:26:34.329693 noohayo-1.0.4/noohayo/
+-rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.4/noohayo/__init__.py
+-rw-rw-rw-   0        0        0     2168 2024-04-08 04:16:47.000000 noohayo-1.0.4/noohayo/noohayo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 05:26:34.361980 noohayo-1.0.4/noohayo/scripts/
+-rw-rw-rw-   0        0        0      665 2024-04-06 21:14:24.000000 noohayo-1.0.4/noohayo/scripts/Colorer.py
+-rw-rw-rw-   0        0        0     2997 2024-04-08 00:18:51.000000 noohayo-1.0.4/noohayo/scripts/Config.py
+-rw-rw-rw-   0        0        0     2381 2024-04-08 04:16:38.000000 noohayo-1.0.4/noohayo/scripts/Fetch.py
+-rw-rw-rw-   0        0        0     2842 2024-04-08 04:16:40.000000 noohayo-1.0.4/noohayo/scripts/General.py
+-rw-rw-rw-   0        0        0      814 2024-04-08 05:25:04.000000 noohayo-1.0.4/noohayo/scripts/Help.py
+-rw-rw-rw-   0        0        0      998 2024-04-08 04:16:43.000000 noohayo-1.0.4/noohayo/scripts/Select.py
+-rw-rw-rw-   0        0        0        0 2024-04-08 04:13:02.000000 noohayo-1.0.4/noohayo/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 05:26:34.351697 noohayo-1.0.4/noohayo.egg-info/
+-rw-rw-rw-   0        0        0     6489 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 05:26:34.000000 noohayo-1.0.4/noohayo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 05:26:34.363985 noohayo-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-04-08 05:26:26.000000 noohayo-1.0.4/setup.py
```

### Comparing `noohayo-1.0.3/README.md` & `noohayo-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 ## ScreenShots -
 <div style="display: flex;"><img src="https://raw.githubusercontent.com/BreakRyo/noohayo/main/screenshots/1.png" style="Height:500px"/>
 <img src="https://raw.githubusercontent.com/BreakRyo/noohayo/main/screenshots/2.png" style="Height:500px;margin-left:10px"/></div>
 
 ## Usage -
 
-### 1. Installation :
+### 1 Installation 
 You can install it via pip :
 ``` pip install noohayo ```
-### 2. Create a profile  :
+### 2 Create a profile  
 - when you first install the tool you will find no profile, to create one :
     ``` noohayo -n ProfileName ```
 - if the profile is created successfully run this command to see all the profiles you have :
 ``` noohayo -s ```
 - to select a profile as the default one run this command :
 ``` noohayo -s ProfileName ```
 - if you want to locate the profiles folder for [Customization](#customization) run this command :
   ``` noohayo -l ```
 - for more information about the command run this command :
 ``` noohayo -h ```    
 
-## Customization -
+## Customization 
 
 - All what's being displayed in the banned is customizable, to start Customizing :
     ``` 
     Ryu@suke ~/⮞  noohayo -l
         C:\Users\user\AppData\Local\BreakRyo\noohayo\Profiles 
     ```
     after running ```noohayo -l``` you will get the location of the profiles, if you didn't find the profiles folder follow these steps first [Create a profile](#2-create-a-profile)
```

### Comparing `noohayo-1.0.3/noohayo/noohayo.py` & `noohayo-1.0.4/noohayo/noohayo.py`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.3/noohayo/scripts/Colorer.py` & `noohayo-1.0.4/noohayo/scripts/Colorer.py`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.3/noohayo/scripts/Config.py` & `noohayo-1.0.4/noohayo/scripts/Config.py`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.3/noohayo/scripts/Fetch.py` & `noohayo-1.0.4/noohayo/scripts/Fetch.py`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.3/noohayo/scripts/General.py` & `noohayo-1.0.4/noohayo/scripts/General.py`

 * *Files identical despite different names*

### Comparing `noohayo-1.0.3/noohayo/scripts/Help.py` & `noohayo-1.0.4/noohayo/scripts/Help.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,10 +11,11 @@
     print(f"\n Usage : \033[38;2;70;167;226mnoohayo\033[0m [\033[38;2;232;157;30moption\033[0m]")
     print(f"\n {des}")
     print(f"\n \033[38;2;232;157;30mOptions\033[0m :\n")
     for action in parser :
         name = action.dest
         met = (f" {action.metavar}" if action.metavar is not None else "")
         print(f"\t -{name[0]}{met}, --{name}{met} \t\t {action.help}")
+    print("\nGithub : https://github.com/BreakRyo/noohayo")
     print()
```

### Comparing `noohayo-1.0.3/noohayo/scripts/Select.py` & `noohayo-1.0.4/noohayo/scripts/Select.py`

 * *Files identical despite different names*

