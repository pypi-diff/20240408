# Comparing `tmp/openai_cost_logger-0.0.2.tar.gz` & `tmp/openai_cost_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_cost_logger-0.0.2.tar", last modified: Mon Apr  8 09:11:46 2024, max compression
+gzip compressed data, was "openai_cost_logger-0.0.3.tar", last modified: Mon Apr  8 09:35:22 2024, max compression
```

## Comparing `openai_cost_logger-0.0.2.tar` & `openai_cost_logger-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:11:46.489593 openai_cost_logger-0.0.2/
--rw-rw-r--   0 drudao    (1000) drudao    (1000)     1070 2024-03-29 09:58:23.000000 openai_cost_logger-0.0.2/LICENSE
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      275 2024-04-08 09:11:46.489593 openai_cost_logger-0.0.2/PKG-INFO
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      663 2024-03-29 17:27:32.000000 openai_cost_logger-0.0.2/README.md
-drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:11:46.489593 openai_cost_logger-0.0.2/openai_cost_logger/
--rw-rw-r--   0 drudao    (1000) drudao    (1000)       37 2024-04-04 08:59:36.000000 openai_cost_logger-0.0.2/openai_cost_logger/__init__.py
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      597 2024-03-29 16:45:52.000000 openai_cost_logger-0.0.2/openai_cost_logger/constants.py
--rw-rw-r--   0 drudao    (1000) drudao    (1000)     3485 2024-04-08 09:01:48.000000 openai_cost_logger-0.0.2/openai_cost_logger/openai_cost_logger.py
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      396 2024-04-08 08:42:27.000000 openai_cost_logger-0.0.2/openai_cost_logger/openai_cost_logger_utils.py
--rw-rw-r--   0 drudao    (1000) drudao    (1000)     3614 2024-04-08 08:43:18.000000 openai_cost_logger-0.0.2/openai_cost_logger/openai_cost_logger_viz.py
-drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:11:46.489593 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      275 2024-04-08 09:11:46.000000 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/PKG-INFO
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      431 2024-04-08 09:11:46.000000 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 drudao    (1000) drudao    (1000)        1 2024-04-08 09:11:46.000000 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 drudao    (1000) drudao    (1000)       25 2024-04-08 09:11:46.000000 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/requires.txt
--rw-rw-r--   0 drudao    (1000) drudao    (1000)       19 2024-04-08 09:11:46.000000 openai_cost_logger-0.0.2/openai_cost_logger.egg-info/top_level.txt
--rw-rw-r--   0 drudao    (1000) drudao    (1000)       38 2024-04-08 09:11:46.489593 openai_cost_logger-0.0.2/setup.cfg
--rw-rw-r--   0 drudao    (1000) drudao    (1000)      459 2024-04-08 09:11:40.000000 openai_cost_logger-0.0.2/setup.py
+drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:35:22.547836 openai_cost_logger-0.0.3/
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)     1070 2024-03-29 09:58:23.000000 openai_cost_logger-0.0.3/LICENSE
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      287 2024-04-08 09:35:22.547836 openai_cost_logger-0.0.3/PKG-INFO
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      470 2024-04-08 09:35:05.000000 openai_cost_logger-0.0.3/README.rst
+drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:35:22.547836 openai_cost_logger-0.0.3/openai_cost_logger/
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)       37 2024-04-04 08:59:36.000000 openai_cost_logger-0.0.3/openai_cost_logger/__init__.py
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      597 2024-03-29 16:45:52.000000 openai_cost_logger-0.0.3/openai_cost_logger/constants.py
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)     3485 2024-04-08 09:01:48.000000 openai_cost_logger-0.0.3/openai_cost_logger/openai_cost_logger.py
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      396 2024-04-08 08:42:27.000000 openai_cost_logger-0.0.3/openai_cost_logger/openai_cost_logger_utils.py
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)     3614 2024-04-08 08:43:18.000000 openai_cost_logger-0.0.3/openai_cost_logger/openai_cost_logger_viz.py
+drwxrwxr-x   0 drudao    (1000) drudao    (1000)        0 2024-04-08 09:35:22.547836 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      287 2024-04-08 09:35:22.000000 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      432 2024-04-08 09:35:22.000000 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)        1 2024-04-08 09:35:22.000000 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)       25 2024-04-08 09:35:22.000000 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/requires.txt
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)       19 2024-04-08 09:35:22.000000 openai_cost_logger-0.0.3/openai_cost_logger.egg-info/top_level.txt
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)       38 2024-04-08 09:35:22.547836 openai_cost_logger-0.0.3/setup.cfg
+-rw-rw-r--   0 drudao    (1000) drudao    (1000)      494 2024-04-08 09:35:18.000000 openai_cost_logger-0.0.3/setup.py
```

### Comparing `openai_cost_logger-0.0.2/LICENSE` & `openai_cost_logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.2/openai_cost_logger/constants.py` & `openai_cost_logger-0.0.3/openai_cost_logger/constants.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.2/openai_cost_logger/openai_cost_logger.py` & `openai_cost_logger-0.0.3/openai_cost_logger/openai_cost_logger.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.0.2/openai_cost_logger/openai_cost_logger_viz.py` & `openai_cost_logger-0.0.3/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files identical despite different names*

