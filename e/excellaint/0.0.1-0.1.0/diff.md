# Comparing `tmp/excellaint-0.0.1.tar.gz` & `tmp/excellaint-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excellaint-0.0.1.tar", last modified: Mon Apr  1 09:30:35 2024, max compression
+gzip compressed data, was "excellaint-0.1.0.tar", last modified: Mon Apr  8 13:39:18 2024, max compression
```

## Comparing `excellaint-0.0.1.tar` & `excellaint-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-01 09:30:35.713657 excellaint-0.0.1/
--rw-r--r--   0 ct6g18     (503) staff       (20)     1071 2024-04-01 08:56:49.000000 excellaint-0.0.1/LICENSE
--rw-r--r--   0 ct6g18     (503) staff       (20)      661 2024-04-01 09:30:35.713115 excellaint-0.0.1/PKG-INFO
--rw-r--r--   0 ct6g18     (503) staff       (20)      110 2024-04-01 08:56:49.000000 excellaint-0.0.1/README.md
--rw-r--r--   0 ct6g18     (503) staff       (20)       38 2024-04-01 09:30:35.713732 excellaint-0.0.1/setup.cfg
--rw-r--r--   0 ct6g18     (503) staff       (20)      830 2024-04-01 09:29:52.000000 excellaint-0.0.1/setup.py
-drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-01 09:30:35.695410 excellaint-0.0.1/src/
-drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-01 09:30:35.712510 excellaint-0.0.1/src/ExcellAint.egg-info/
--rw-r--r--   0 ct6g18     (503) staff       (20)      661 2024-04-01 09:30:35.000000 excellaint-0.0.1/src/ExcellAint.egg-info/PKG-INFO
--rw-r--r--   0 ct6g18     (503) staff       (20)      478 2024-04-01 09:30:35.000000 excellaint-0.0.1/src/ExcellAint.egg-info/SOURCES.txt
--rw-r--r--   0 ct6g18     (503) staff       (20)        1 2024-04-01 09:30:35.000000 excellaint-0.0.1/src/ExcellAint.egg-info/dependency_links.txt
--rw-r--r--   0 ct6g18     (503) staff       (20)        1 2024-04-01 09:22:54.000000 excellaint-0.0.1/src/ExcellAint.egg-info/not-zip-safe
--rw-r--r--   0 ct6g18     (503) staff       (20)       26 2024-04-01 09:30:35.000000 excellaint-0.0.1/src/ExcellAint.egg-info/requires.txt
--rw-r--r--   0 ct6g18     (503) staff       (20)       11 2024-04-01 09:30:35.000000 excellaint-0.0.1/src/ExcellAint.egg-info/top_level.txt
+drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-08 13:39:18.224675 excellaint-0.1.0/
+-rw-r--r--   0 ct6g18     (503) staff       (20)     1071 2024-04-01 08:56:49.000000 excellaint-0.1.0/LICENSE
+-rw-r--r--   0 ct6g18     (503) staff       (20)       40 2024-04-08 13:30:27.000000 excellaint-0.1.0/MANIFEST.in
+-rw-r--r--   0 ct6g18     (503) staff       (20)     4145 2024-04-08 13:39:18.224107 excellaint-0.1.0/PKG-INFO
+-rw-r--r--   0 ct6g18     (503) staff       (20)     3435 2024-04-08 13:28:12.000000 excellaint-0.1.0/README.md
+-rw-r--r--   0 ct6g18     (503) staff       (20)      831 2024-04-08 13:29:28.000000 excellaint-0.1.0/pyproject.toml
+-rw-r--r--   0 ct6g18     (503) staff       (20)       38 2024-04-08 13:39:18.224753 excellaint-0.1.0/setup.cfg
+drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-08 13:39:18.213361 excellaint-0.1.0/src/
+drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-08 13:39:18.223351 excellaint-0.1.0/src/ExcellAint.egg-info/
+-rw-r--r--   0 ct6g18     (503) staff       (20)     4145 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/PKG-INFO
+-rw-r--r--   0 ct6g18     (503) staff       (20)      519 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/SOURCES.txt
+-rw-r--r--   0 ct6g18     (503) staff       (20)        1 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/dependency_links.txt
+-rw-r--r--   0 ct6g18     (503) staff       (20)       47 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/entry_points.txt
+-rw-r--r--   0 ct6g18     (503) staff       (20)      104 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/requires.txt
+-rw-r--r--   0 ct6g18     (503) staff       (20)       11 2024-04-08 13:39:18.000000 excellaint-0.1.0/src/ExcellAint.egg-info/top_level.txt
+drwxr-xr-x   0 ct6g18     (503) staff       (20)        0 2024-04-08 13:39:18.218904 excellaint-0.1.0/src/excellaint/
+-rw-r--r--   0 ct6g18     (503) staff       (20)      199 2024-04-07 04:19:28.000000 excellaint-0.1.0/src/excellaint/__init__.py
+-rw-r--r--   0 ct6g18     (503) staff       (20)    15723 2024-04-08 13:19:43.000000 excellaint-0.1.0/src/excellaint/excellaint.py
```

### Comparing `excellaint-0.0.1/LICENSE` & `excellaint-0.1.0/LICENSE`

 * *Files identical despite different names*

