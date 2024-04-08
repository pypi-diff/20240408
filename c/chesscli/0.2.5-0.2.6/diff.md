# Comparing `tmp/chesscli-0.2.5.tar.gz` & `tmp/chesscli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscli-0.2.5.tar", last modified: Mon Apr  8 02:51:48 2024, max compression
+gzip compressed data, was "chesscli-0.2.6.tar", last modified: Mon Apr  8 03:12:51 2024, max compression
```

## Comparing `chesscli-0.2.5.tar` & `chesscli-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.079363 chesscli-0.2.5/
--rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:51:48.078371 chesscli-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.5/README.md
--rw-rw-rw-   0        0        0      615 2024-04-08 02:51:33.000000 chesscli-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 02:51:48.079363 chesscli-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      502 2024-04-08 02:51:36.000000 chesscli-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.052020 chesscli-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.059312 chesscli-0.2.5/src/chesscli/
--rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.5/src/chesscli/__init__.py
--rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.5/src/chesscli/__main__.py
--rw-rw-rw-   0        0        0     3123 2024-04-08 02:34:37.000000 chesscli-0.2.5/src/chesscli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:51:48.076363 chesscli-0.2.5/src/chesscli.egg-info/
--rw-rw-rw-   0        0        0     2503 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-08 02:51:48.000000 chesscli-0.2.5/src/chesscli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 02:51:47.000000 chesscli-0.2.5/src/chesscli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.246160 chesscli-0.2.6/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 02:36:45.000000 chesscli-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      245 2024-04-08 03:12:51.244782 chesscli-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1944 2024-04-07 23:49:46.000000 chesscli-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 03:12:51.246160 chesscli-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      502 2024-04-08 03:11:23.000000 chesscli-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.222037 chesscli-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.230076 chesscli-0.2.6/src/chesscli/
+-rw-rw-rw-   0        0        0        0 2024-04-08 02:03:35.000000 chesscli-0.2.6/src/chesscli/__init__.py
+-rw-rw-rw-   0        0        0       64 2024-04-08 01:53:52.000000 chesscli-0.2.6/src/chesscli/__main__.py
+-rw-rw-rw-   0        0        0     3123 2024-04-08 02:34:37.000000 chesscli-0.2.6/src/chesscli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 03:12:51.243779 chesscli-0.2.6/src/chesscli.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 03:12:51.000000 chesscli-0.2.6/src/chesscli.egg-info/top_level.txt
```

### Comparing `chesscli-0.2.5/LICENSE` & `chesscli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chesscli-0.2.5/PKG-INFO` & `chesscli-0.2.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: chesscli
-Version: 0.2.5
-Summary: A CLI for chess application development.
-Author: Neel Patel
-Author-email: Neel Patel <patel.neel5@northeastern.edu>
-Project-URL: Homepage, https://github.com/neelthepatel8/chesscli
-Project-URL: Issues, https://github.com/neelthepatel8/chesscli/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChessCLI
 
 ChessCLI is a command-line interface (CLI) tool designed to streamline the development environment for a chess game project. It automates tasks such as setting up the project, opening the codebase in Visual Studio Code, and managing Docker containers.
 
 ## Features
 
 - **Easy Configuration**: Quickly configure the path to your chess game project repository.
```

### Comparing `chesscli-0.2.5/src/chesscli/main.py` & `chesscli-0.2.6/src/chesscli/main.py`

 * *Files identical despite different names*

