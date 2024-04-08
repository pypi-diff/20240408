# Comparing `tmp/yuezhlib-0.1.0.tar.gz` & `tmp/yuezhlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuezhlib-0.1.0.tar", last modified: Mon Apr  8 04:34:16 2024, max compression
+gzip compressed data, was "yuezhlib-0.1.1.tar", last modified: Mon Apr  8 06:08:24 2024, max compression
```

## Comparing `yuezhlib-0.1.0.tar` & `yuezhlib-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 adv        (503) staff       (20)        0 2024-04-08 04:34:16.105216 yuezhlib-0.1.0/
--rw-r--r--   0 adv        (503) staff       (20)      654 2024-04-08 04:34:16.104971 yuezhlib-0.1.0/PKG-INFO
--rw-r--r--   0 adv        (503) staff       (20)       38 2024-04-08 04:34:16.105303 yuezhlib-0.1.0/setup.cfg
--rw-r--r--   0 adv        (503) staff       (20)     1003 2024-04-08 04:31:36.000000 yuezhlib-0.1.0/setup.py
-drwxr-xr-x   0 adv        (503) staff       (20)        0 2024-04-08 04:34:16.104671 yuezhlib-0.1.0/yuezhlib.egg-info/
--rw-r--r--   0 adv        (503) staff       (20)      654 2024-04-08 04:34:16.000000 yuezhlib-0.1.0/yuezhlib.egg-info/PKG-INFO
--rw-r--r--   0 adv        (503) staff       (20)      167 2024-04-08 04:34:16.000000 yuezhlib-0.1.0/yuezhlib.egg-info/SOURCES.txt
--rw-r--r--   0 adv        (503) staff       (20)        1 2024-04-08 04:34:16.000000 yuezhlib-0.1.0/yuezhlib.egg-info/dependency_links.txt
--rw-r--r--   0 adv        (503) staff       (20)       36 2024-04-08 04:34:16.000000 yuezhlib-0.1.0/yuezhlib.egg-info/requires.txt
--rw-r--r--   0 adv        (503) staff       (20)        1 2024-04-08 04:34:16.000000 yuezhlib-0.1.0/yuezhlib.egg-info/top_level.txt
+drwxr-xr-x   0 adv        (503) staff       (20)        0 2024-04-08 06:08:24.218650 yuezhlib-0.1.1/
+-rw-r--r--   0 adv        (503) staff       (20)      654 2024-04-08 06:08:24.218448 yuezhlib-0.1.1/PKG-INFO
+-rw-r--r--   0 adv        (503) staff       (20)       38 2024-04-08 06:08:24.218735 yuezhlib-0.1.1/setup.cfg
+-rw-r--r--   0 adv        (503) staff       (20)     1003 2024-04-08 06:02:52.000000 yuezhlib-0.1.1/setup.py
+drwxr-xr-x   0 adv        (503) staff       (20)        0 2024-04-08 06:08:24.216816 yuezhlib-0.1.1/yuezhlib/
+-rw-r--r--   0 adv        (503) staff       (20)       41 2024-04-08 06:04:01.000000 yuezhlib-0.1.1/yuezhlib/__init__.py
+-rw-r--r--   0 adv        (503) staff       (20)     5859 2024-04-08 06:07:15.000000 yuezhlib-0.1.1/yuezhlib/cantonese_tokenizer.py
+drwxr-xr-x   0 adv        (503) staff       (20)        0 2024-04-08 06:08:24.218137 yuezhlib-0.1.1/yuezhlib.egg-info/
+-rw-r--r--   0 adv        (503) staff       (20)      654 2024-04-08 06:08:24.000000 yuezhlib-0.1.1/yuezhlib.egg-info/PKG-INFO
+-rw-r--r--   0 adv        (503) staff       (20)      220 2024-04-08 06:08:24.000000 yuezhlib-0.1.1/yuezhlib.egg-info/SOURCES.txt
+-rw-r--r--   0 adv        (503) staff       (20)        1 2024-04-08 06:08:24.000000 yuezhlib-0.1.1/yuezhlib.egg-info/dependency_links.txt
+-rw-r--r--   0 adv        (503) staff       (20)       36 2024-04-08 06:08:24.000000 yuezhlib-0.1.1/yuezhlib.egg-info/requires.txt
+-rw-r--r--   0 adv        (503) staff       (20)        9 2024-04-08 06:08:24.000000 yuezhlib-0.1.1/yuezhlib.egg-info/top_level.txt
```

### Comparing `yuezhlib-0.1.0/PKG-INFO` & `yuezhlib-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuezhlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for preprocessing Cantonese and Written Chinese
 Home-page: https://github.com/shivanraptor/yuezhlib
 Author: Raptor K
 Author-email: findme@raptor.hk
 License: UNKNOWN
 Keywords: Cantonese,preprocess
 Platform: UNKNOWN
```

### Comparing `yuezhlib-0.1.0/setup.py` & `yuezhlib-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Library for preprocessing Cantonese and Written Chinese'
 LONG_DESCRIPTION = 'Library for preprocessing Cantonese and Written Chinese'
 
 setup(
         name='yuezhlib',
         version=VERSION,
         python_requires='>=3.9.7',
```

### Comparing `yuezhlib-0.1.0/yuezhlib.egg-info/PKG-INFO` & `yuezhlib-0.1.1/yuezhlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuezhlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for preprocessing Cantonese and Written Chinese
 Home-page: https://github.com/shivanraptor/yuezhlib
 Author: Raptor K
 Author-email: findme@raptor.hk
 License: UNKNOWN
 Keywords: Cantonese,preprocess
 Platform: UNKNOWN
```

