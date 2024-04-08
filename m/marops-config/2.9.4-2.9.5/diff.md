# Comparing `tmp/marops_config-2.9.4.tar.gz` & `tmp/marops_config-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marops_config-2.9.4.tar", last modified: Fri Oct  6 07:08:28 2023, max compression
+gzip compressed data, was "marops_config-2.9.5.tar", last modified: Thu Oct 12 22:27:12 2023, max compression
```

## Comparing `marops_config-2.9.4.tar` & `marops_config-2.9.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:28.616651 marops_config-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-10-06 07:08:28.616651 marops_config-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-06 07:07:51.000000 marops_config-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:28.612651 marops_config-2.9.4/marops_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-10-06 07:07:51.000000 marops_config-2.9.4/marops_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-06 07:07:51.000000 marops_config-2.9.4/marops_config/generate_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:28.616651 marops_config-2.9.4/marops_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-06 07:07:51.000000 marops_config-2.9.4/marops_config/schemas/marops.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:28.616651 marops_config-2.9.4/marops_config/test/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 07:07:51.000000 marops_config-2.9.4/marops_config/test/marops_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 07:08:28.612651 marops_config-2.9.4/marops_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 07:08:28.000000 marops_config-2.9.4/marops_config.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-06 07:08:28.616651 marops_config-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 07:07:51.000000 marops_config-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:12.340208 marops_config-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-10-12 22:27:12.340208 marops_config-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-12 22:26:32.000000 marops_config-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:12.340208 marops_config-2.9.5/marops_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-10-12 22:26:32.000000 marops_config-2.9.5/marops_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-12 22:26:32.000000 marops_config-2.9.5/marops_config/generate_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:12.340208 marops_config-2.9.5/marops_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-12 22:26:32.000000 marops_config-2.9.5/marops_config/schemas/marops.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:12.340208 marops_config-2.9.5/marops_config/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-12 22:26:32.000000 marops_config-2.9.5/marops_config/test/marops_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 22:27:12.340208 marops_config-2.9.5/marops_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 22:27:12.000000 marops_config-2.9.5/marops_config.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-12 22:27:12.340208 marops_config-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 22:26:32.000000 marops_config-2.9.5/setup.py
```

### Comparing `marops_config-2.9.4/PKG-INFO` & `marops_config-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marops_config
-Version: 2.9.4
+Version: 2.9.5
 Summary: A library for reading / writing MarOps config files
 Home-page: https://github.com/Greenroom-Robotics/marops
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `marops_config-2.9.4/README.md` & `marops_config-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `marops_config-2.9.4/marops_config/__init__.py` & `marops_config-2.9.5/marops_config/__init__.py`

 * *Files identical despite different names*

### Comparing `marops_config-2.9.4/marops_config/schemas/marops.schema.json` & `marops_config-2.9.5/marops_config/schemas/marops.schema.json`

 * *Files identical despite different names*

### Comparing `marops_config-2.9.4/marops_config.egg-info/PKG-INFO` & `marops_config-2.9.5/marops_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marops-config
-Version: 2.9.4
+Version: 2.9.5
 Summary: A library for reading / writing MarOps config files
 Home-page: https://github.com/Greenroom-Robotics/marops
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `marops_config-2.9.4/setup.cfg` & `marops_config-2.9.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = marops_config
-version = 2.9.4
+version = 2.9.5
 url = https://github.com/Greenroom-Robotics/marops
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

