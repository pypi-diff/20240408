# Comparing `tmp/yosemite-tools-0.0.6.tar.gz` & `tmp/yosemite-tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yosemite-tools-0.0.6.tar", last modified: Sat Apr  6 04:49:26 2024, max compression
+gzip compressed data, was "yosemite-tools-0.0.7.tar", last modified: Mon Apr  8 05:24:21 2024, max compression
```

## Comparing `yosemite-tools-0.0.6.tar` & `yosemite-tools-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:49:26.688255 yosemite-tools-0.0.6/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:49:26.687735 yosemite-tools-0.0.6/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 04:49:26.688374 yosemite-tools-0.0.6/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 04:49:19.000000 yosemite-tools-0.0.6/setup.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:49:26.680790 yosemite-tools-0.0.6/yosemite_tools/
--rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.6/yosemite_tools/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:49:26.686332 yosemite-tools-0.0.6/yosemite_tools/modules/
--rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.6/yosemite_tools/modules/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.6/yosemite_tools/modules/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     6402 2024-04-06 04:48:03.000000 yosemite-tools-0.0.6/yosemite_tools/modules/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     3943 2024-04-06 04:49:09.000000 yosemite-tools-0.0.6/yosemite_tools/modules/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.6/yosemite_tools/modules/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:49:26.687174 yosemite-tools-0.0.6/yosemite_tools.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:49:26.000000 yosemite-tools-0.0.6/yosemite_tools.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 04:49:26.000000 yosemite-tools-0.0.6/yosemite_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 04:49:26.000000 yosemite-tools-0.0.6/yosemite_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 04:49:26.000000 yosemite-tools-0.0.6/yosemite_tools.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 04:49:26.000000 yosemite-tools-0.0.6/yosemite_tools.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-08 05:24:21.102346 yosemite-tools-0.0.7/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-08 05:24:21.101021 yosemite-tools-0.0.7/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-08 05:24:21.102485 yosemite-tools-0.0.7/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-08 05:24:06.000000 yosemite-tools-0.0.7/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-08 05:24:21.089042 yosemite-tools-0.0.7/yosemite_tools/
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.7/yosemite_tools/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-08 05:24:21.099158 yosemite-tools-0.0.7/yosemite_tools/modules/
+-rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.7/yosemite_tools/modules/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.7/yosemite_tools/modules/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6419 2024-04-08 05:19:39.000000 yosemite-tools-0.0.7/yosemite_tools/modules/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2469 2024-04-08 05:23:25.000000 yosemite-tools-0.0.7/yosemite_tools/modules/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.7/yosemite_tools/modules/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-08 05:24:21.100390 yosemite-tools-0.0.7/yosemite_tools.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-08 05:24:21.000000 yosemite-tools-0.0.7/yosemite_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-08 05:24:21.000000 yosemite-tools-0.0.7/yosemite_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-08 05:24:21.000000 yosemite-tools-0.0.7/yosemite_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-08 05:24:21.000000 yosemite-tools-0.0.7/yosemite_tools.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-08 05:24:21.000000 yosemite-tools-0.0.7/yosemite_tools.egg-info/top_level.txt
```

### Comparing `yosemite-tools-0.0.6/setup.py` & `yosemite-tools-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="yosemite-tools",
-    version="0.0.06",
+    version="0.0.07",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="yosemite",
     long_description="""
 Yosemite
     """,
     packages=setuptools.find_packages(),
```

### Comparing `yosemite-tools-0.0.6/yosemite_tools/modules/inputs.py` & `yosemite-tools-0.0.7/yosemite_tools/modules/inputs.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.6/yosemite_tools/modules/logger.py` & `yosemite-tools-0.0.7/yosemite_tools/modules/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Attributes:
         logger: A logging.Logger instance for logging messages.
         log_dir: The directory where log files will be stored.
         text: A RichText instance for styled output.
         verbose: A boolean indicating whether to display verbose output.
     """
 
-    def __init__(self, name, log_dir : str ="logs", verbose : bool = False):
+    def __init__(self, name : str = "logger", log_dir : str ="logs", verbose : bool = False):
         """
         Initialize the Logger instance.
 
         Args:
             name (str): The name of the logger.
             log_dir (str, optional): The directory where log files will be stored. Defaults to "logs".
             verbose (bool, optional): Whether to display verbose output. Defaults to False.
```

### Comparing `yosemite-tools-0.0.6/yosemite_tools/modules/utils.py` & `yosemite-tools-0.0.7/yosemite_tools/modules/utils.py`

 * *Files identical despite different names*

