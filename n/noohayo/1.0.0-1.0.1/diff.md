# Comparing `tmp/noohayo-1.0.0.tar.gz` & `tmp/noohayo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noohayo-1.0.0.tar", last modified: Mon Apr  8 03:27:54 2024, max compression
+gzip compressed data, was "noohayo-1.0.1.tar", last modified: Mon Apr  8 03:50:49 2024, max compression
```

## Comparing `noohayo-1.0.0.tar` & `noohayo-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:27:54.943136 noohayo-1.0.0/
--rw-rw-rw-   0        0        0       54 2024-04-08 03:27:54.942134 noohayo-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 03:27:54.918129 noohayo-1.0.0/noohayo/
--rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.0/noohayo/__init__.py
--rw-rw-rw-   0        0        0     2168 2024-04-07 23:25:21.000000 noohayo-1.0.0/noohayo/noohayo.py
-drwxrwxrwx   0        0        0        0 2024-04-08 03:27:54.941135 noohayo-1.0.0/noohayo.egg-info/
--rw-rw-rw-   0        0        0       54 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 03:27:54.000000 noohayo-1.0.0/noohayo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 03:27:54.943136 noohayo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-08 00:11:47.000000 noohayo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.916648 noohayo-1.0.1/
+-rw-rw-rw-   0        0        0       54 2024-04-08 03:50:49.915640 noohayo-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6295 2024-04-08 03:44:49.000000 noohayo-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.859741 noohayo-1.0.1/noohayo/
+-rw-rw-rw-   0        0        0        0 2024-04-07 19:19:20.000000 noohayo-1.0.1/noohayo/__init__.py
+-rw-rw-rw-   0        0        0     2128 2024-04-08 03:48:20.000000 noohayo-1.0.1/noohayo/noohayo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:50:49.913642 noohayo-1.0.1/noohayo.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 03:50:49.000000 noohayo-1.0.1/noohayo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 03:50:49.916648 noohayo-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-08 03:50:45.000000 noohayo-1.0.1/setup.py
```

### Comparing `noohayo-1.0.0/noohayo/noohayo.py` & `noohayo-1.0.1/noohayo/noohayo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import appdirs
-import noohayo.scripts.Fetch as Fetch
-from noohayo.scripts.General import General
-from noohayo.scripts.Select import Select
-from noohayo.scripts.Config import Config
-from noohayo.scripts.Help import Help
+import scripts.Fetch as Fetch
+from scripts.General import General
+from scripts.Select import Select
+from scripts.Config import Config
+from scripts.Help import Help
 
 def main():
     des = f'Description: command line interface tool that displays a banner when ever you open a new ternimal tab.'
     parser = argparse.ArgumentParser(prog="noohayo", description=des, usage="%(prog)s [option]", add_help=False)
     parser.add_argument('-h', '--help',action="store_true", help='\t\t Show this help message and exit.')
     parser.add_argument('-v','--version', action='version', version='noohayo 1.0', help="\t\t show program's version number and exit.")
     parser.add_argument('-n' ,'--new', const="", metavar="[name]" , nargs="?" ,help="Makes a new profile." )
```

