# Comparing `tmp/fremake_canopy-0.1.2.tar.gz` & `tmp/fremake_canopy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fremake_canopy-0.1.2.tar", last modified: Thu Apr  4 19:00:05 2024, max compression
+gzip compressed data, was "fremake_canopy-0.1.3.tar", last modified: Mon Apr  8 20:46:41 2024, max compression
```

## Comparing `fremake_canopy-0.1.2.tar` & `fremake_canopy-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.906262 fremake_canopy-0.1.2/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7642 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/LICENSE.md
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       59 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/MANIFEST.in
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-04 19:00:44.899171 fremake_canopy-0.1.2/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2382 2024-03-27 16:46:30.000000 fremake_canopy-0.1.2/README.md
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.879930 fremake_canopy-0.1.2/fremake_canopy.egg-info/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      280 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      469 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/SOURCES.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)        1 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/dependency_links.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       27 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/requires.txt
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       13 2024-04-04 19:00:44.000000 fremake_canopy-0.1.2/fremake_canopy.egg-info/top_level.txt
-drwxr-xr-x   0 Bennett.Chang (21243) f           (70)        0 2024-04-04 19:00:44.870793 fremake_canopy-0.1.2/gfdl_fremake/
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      173 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/__init__.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     4475 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/buildBaremetal.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7968 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/buildDocker.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     5780 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/checkout.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     7576 2024-04-04 18:35:05.000000 fremake_canopy-0.1.2/gfdl_fremake/makefilefre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     4381 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/platformfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2367 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/targetfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     2493 2024-04-04 18:35:02.000000 fremake_canopy-0.1.2/gfdl_fremake/varsfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)     6030 2024-04-04 18:57:54.000000 fremake_canopy-0.1.2/gfdl_fremake/yamlfre.py
--rw-r--r--   0 Bennett.Chang (21243) f           (70)       38 2024-04-04 19:00:44.907274 fremake_canopy-0.1.2/setup.cfg
--rw-r--r--   0 Bennett.Chang (21243) f           (70)      400 2024-04-04 18:59:35.000000 fremake_canopy-0.1.2/setup.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.294296 fremake_canopy-0.1.3/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7642 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/LICENSE.md
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       70 2024-04-08 20:46:19.000000 fremake_canopy-0.1.3/MANIFEST.in
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      208 2024-04-08 20:46:41.294286 fremake_canopy-0.1.3/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2382 2023-11-01 18:23:29.000000 fremake_canopy-0.1.3/README.md
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.259291 fremake_canopy-0.1.3/fremake_canopy.egg-info/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      208 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      640 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/SOURCES.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        1 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/dependency_links.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       27 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/requires.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       13 2024-04-08 20:46:41.000000 fremake_canopy-0.1.3/fremake_canopy.egg-info/top_level.txt
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.282295 fremake_canopy-0.1.3/gfdl_fremake/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:40:07.000000 fremake_canopy-0.1.3/gfdl_fremake/__init__.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4475 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/buildBaremetal.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7968 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/buildDocker.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     5780 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/checkout.py
+-rwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)    12023 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/fremake
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7576 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/makefilefre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4381 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/platformfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/schema.json
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2367 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/targetfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2493 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/varsfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6030 2024-04-08 18:46:00.000000 fremake_canopy-0.1.3/gfdl_fremake/yamlfre.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-08 20:46:41.291291 fremake_canopy-0.1.3/gfdl_fremake/yamls/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      231 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/am5.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     3046 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/compile.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     1144 2024-04-08 18:19:48.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/platforms.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-08 18:17:46.000000 fremake_canopy-0.1.3/gfdl_fremake/yamls/schema.json
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       38 2024-04-08 20:46:41.295293 fremake_canopy-0.1.3/setup.cfg
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      400 2024-04-08 20:43:33.000000 fremake_canopy-0.1.3/setup.py
```

### Comparing `fremake_canopy-0.1.2/LICENSE.md` & `fremake_canopy-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/README.md` & `fremake_canopy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/buildBaremetal.py` & `fremake_canopy-0.1.3/gfdl_fremake/buildBaremetal.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/buildDocker.py` & `fremake_canopy-0.1.3/gfdl_fremake/buildDocker.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/checkout.py` & `fremake_canopy-0.1.3/gfdl_fremake/checkout.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/makefilefre.py` & `fremake_canopy-0.1.3/gfdl_fremake/makefilefre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/platformfre.py` & `fremake_canopy-0.1.3/gfdl_fremake/platformfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/targetfre.py` & `fremake_canopy-0.1.3/gfdl_fremake/targetfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/varsfre.py` & `fremake_canopy-0.1.3/gfdl_fremake/varsfre.py`

 * *Files identical despite different names*

### Comparing `fremake_canopy-0.1.2/gfdl_fremake/yamlfre.py` & `fremake_canopy-0.1.3/gfdl_fremake/yamlfre.py`

 * *Files identical despite different names*

