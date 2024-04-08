# Comparing `tmp/foliantcontrib.checksources-1.0.0.tar.gz` & `tmp/foliantcontrib.checksources-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliantcontrib.checksources-1.0.0.tar", last modified: Sat May 28 19:10:20 2022, max compression
+gzip compressed data, was "foliantcontrib.checksources-1.0.1.tar", last modified: Mon Apr  8 19:54:08 2024, max compression
```

## Comparing `foliantcontrib.checksources-1.0.0.tar` & `foliantcontrib.checksources-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-28 19:10:20.746505 foliantcontrib.checksources-1.0.0/
--rw-r--r--   0 user       (501) staff       (20)     1068 2022-05-28 18:35:12.000000 foliantcontrib.checksources-1.0.0/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     1605 2022-05-28 19:10:20.746241 foliantcontrib.checksources-1.0.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      643 2022-05-28 18:35:12.000000 foliantcontrib.checksources-1.0.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-28 19:10:20.742704 foliantcontrib.checksources-1.0.0/foliant/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-28 19:10:20.744195 foliantcontrib.checksources-1.0.0/foliant/preprocessors/
--rw-r--r--   0 user       (501) staff       (20)     3218 2022-05-28 18:35:12.000000 foliantcontrib.checksources-1.0.0/foliant/preprocessors/checksources.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2022-05-28 19:10:20.745850 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     1605 2022-05-28 19:10:20.000000 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      318 2022-05-28 19:10:20.000000 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2022-05-28 19:10:20.000000 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       43 2022-05-28 19:10:20.000000 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2022-05-28 19:10:20.000000 foliantcontrib.checksources-1.0.0/foliantcontrib.checksources.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2022-05-28 19:10:20.746595 foliantcontrib.checksources-1.0.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)     1175 2022-05-28 19:06:56.000000 foliantcontrib.checksources-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:54:08.284880 foliantcontrib.checksources-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 19:54:04.000000 foliantcontrib.checksources-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-08 19:54:08.284880 foliantcontrib.checksources-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 19:54:04.000000 foliantcontrib.checksources-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:54:08.280881 foliantcontrib.checksources-1.0.1/foliant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:54:08.284880 foliantcontrib.checksources-1.0.1/foliant/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-08 19:54:04.000000 foliantcontrib.checksources-1.0.1/foliant/preprocessors/checksources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:54:08.284880 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-08 19:54:08.000000 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 19:54:08.000000 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:54:08.000000 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 19:54:08.000000 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 19:54:08.000000 foliantcontrib.checksources-1.0.1/foliantcontrib.checksources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:54:08.284880 foliantcontrib.checksources-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-08 19:54:04.000000 foliantcontrib.checksources-1.0.1/setup.py
```

### Comparing `foliantcontrib.checksources-1.0.0/LICENSE` & `foliantcontrib.checksources-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foliantcontrib.checksources-1.0.0/README.md` & `foliantcontrib.checksources-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![](https://img.shields.io/pypi/v/foliantcontrib.checksources.svg)](https://pypi.org/project/foliantcontrib.checksources/) [![](https://img.shields.io/github/v/tag/foliant-docs/foliantcontrib.checksources.svg?label=GitHub)](https://github.com/foliant-docs/foliantcontrib.checksources)
+
 # CheckSources
 
 CheckSources is a preprocessor that checks the project’s `chapters` for missing and unmentioned files in the sources directory.
 
 ## Installation
 
 ```bash
@@ -13,19 +15,24 @@
 To enable the preprocessor, add `checksources` to `preprocessors` section in the project config:
 
 ```yaml
 preprocessors:
     - checksources
 ```
 
-You can add a list of unmentioned files that wouldn't throw warnings by `not_in_chapters` option:
+You can add a list of unmentioned files that wouldn't throw warnings by `not_in_chapters` option.
+To perform a strict check, use the `strict_check` option:
 
 ```yaml
 preprocessors:
     - checksources:
         not_in_chapters:
           - tags.md
+        strict_check: true
 ```
 
-It is useful if you don't need to add some files to the table of contents.
+The `not_in_chapters` option is useful if you don't need to add some files to the table of contents.
+
+If the `strict_check` option is enabled, then if a critical error is detected, the build will be aborted after applying the preprocessor.
+
```

### Comparing `foliantcontrib.checksources-1.0.0/setup.py` & `foliantcontrib.checksources-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 setup(
     name='foliantcontrib.checksources',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/foliant-docs/foliantcontrib.checksources',
     packages=['foliant.preprocessors'],
     author='foliant-docs',
     author_email='foliant-shared@yandex.ru',
     license='MIT',
     platforms='any',
     install_requires=[
```

