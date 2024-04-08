# Comparing `tmp/openai_cost_logger-0.0.0.tar.gz` & `tmp/openai_cost_logger-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_cost_logger-0.0.0.tar", last modified: Mon Apr  8 13:58:40 2024, max compression
+gzip compressed data, was "openai_cost_logger-0.5.0.tar", last modified: Mon Apr  8 14:24:45 2024, max compression
```

## Comparing `openai_cost_logger-0.0.0.tar` & `openai_cost_logger-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:40.174928 openai_cost_logger-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 13:58:40.174928 openai_cost_logger-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:40.174928 openai_cost_logger-0.0.0/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:40.174928 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 13:58:40.000000 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 13:58:40.000000 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:58:40.000000 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 13:58:40.000000 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 13:58:40.000000 openai_cost_logger-0.0.0/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:58:40.174928 openai_cost_logger-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 13:58:35.000000 openai_cost_logger-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 14:24:45.000000 openai_cost_logger-0.5.0/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:24:45.696762 openai_cost_logger-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 14:24:40.000000 openai_cost_logger-0.5.0/setup.py
```

### Comparing `openai_cost_logger-0.0.0/LICENSE` & `openai_cost_logger-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.0/PKG-INFO` & `openai_cost_logger-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_cost_logger
-Version: 0.0.0
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker
 Platform: UNKNOWN
```

### Comparing `openai_cost_logger-0.0.0/README.rst` & `openai_cost_logger-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.0/openai_cost_logger/constants.py` & `openai_cost_logger-0.5.0/openai_cost_logger/constants.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.0/openai_cost_logger/openai_cost_logger.py` & `openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.0/openai_cost_logger/openai_cost_logger_viz.py` & `openai_cost_logger-0.5.0/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.0/openai_cost_logger.egg-info/PKG-INFO` & `openai_cost_logger-0.5.0/openai_cost_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-cost-logger
-Version: 0.0.0
+Version: 0.5.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker
 Platform: UNKNOWN
```

### Comparing `openai_cost_logger-0.0.0/setup.py` & `openai_cost_logger-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # Read the README file (reStructuredText format)
 with open('README.rst') as f:
     long_description = f.read()
 
 # Get the version number from the environment
 version_number = os.getenv('VERSION_NUMBER')
+version_number = version_number.strip("v")
 
 setup(
     name='openai_cost_logger',
     version=version_number,
     author='Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov',
     description='OpenAI Cost Logger',
     author_email='lorenzodrudi11@gmail.com',
```

