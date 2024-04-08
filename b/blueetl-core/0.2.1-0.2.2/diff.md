# Comparing `tmp/blueetl-core-0.2.1.tar.gz` & `tmp/blueetl-core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueetl-core-0.2.1.tar", last modified: Fri Apr  5 12:45:47 2024, max compression
+gzip compressed data, was "blueetl-core-0.2.2.tar", last modified: Mon Apr  8 13:23:03 2024, max compression
```

## Comparing `blueetl-core-0.2.1.tar` & `blueetl-core-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.040930 blueetl-core-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.032930 blueetl-core-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.032930 blueetl-core-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-05 12:45:47.040930 blueetl-core-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.032930 blueetl-core-0.2.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.036930 blueetl-core-0.2.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.036930 blueetl-core-0.2.1/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/source/_images/BlueETL.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:45:47.040930 blueetl-core-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.032930 blueetl-core-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.036930 blueetl-core-0.2.1/src/blueetl_core/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 12:45:46.000000 blueetl-core-0.2.1/src/blueetl_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/src/blueetl_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.036930 blueetl-core-0.2.1/src/blueetl_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-05 12:45:47.000000 blueetl-core-0.2.1/src/blueetl_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-05 12:45:47.000000 blueetl-core-0.2.1/src/blueetl_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:45:47.000000 blueetl-core-0.2.1/src/blueetl_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 12:45:47.000000 blueetl-core-0.2.1/src/blueetl_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 12:45:47.000000 blueetl-core-0.2.1/src/blueetl_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:47.036930 blueetl-core-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_etl_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_etl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_etl_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-05 12:45:41.000000 blueetl-core-0.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.523795 blueetl-core-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/_images/BlueETL.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.523795 blueetl-core-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.527795 blueetl-core-0.2.2/src/blueetl_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/src/blueetl_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/src/blueetl_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 13:23:03.000000 blueetl-core-0.2.2/src/blueetl_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:23:03.531795 blueetl-core-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_etl_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-08 13:22:57.000000 blueetl-core-0.2.2/tox.ini
```

### Comparing `blueetl-core-0.2.1/.github/workflows/publish-sdist.yml` & `blueetl-core-0.2.2/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/.github/workflows/run-tox.yml` & `blueetl-core-0.2.2/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/CHANGELOG.rst` & `blueetl-core-0.2.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+Version 0.2.2
+-------------
+
+Improvements
+~~~~~~~~~~~~
+
+- In ``blueetl_core.parallel.isolated()``, execute the function in the same process if ``BLUEETL_JOBLIB_JOBS`` is set to ``1``.
+
 Version 0.2.1
 -------------
 
 New Features
 ~~~~~~~~~~~~
 
 - Add ``blueetl_core.parallel.isolated()`` to execute a function in a separate subprocess.
```

### Comparing `blueetl-core-0.2.1/LICENSE.txt` & `blueetl-core-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/PKG-INFO` & `blueetl-core-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.1/README.rst` & `blueetl-core-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/doc/Makefile` & `blueetl-core-0.2.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/doc/source/_images/BlueETL.jpeg` & `blueetl-core-0.2.2/doc/source/_images/BlueETL.jpeg`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/doc/source/conf.py` & `blueetl-core-0.2.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/pyproject.toml` & `blueetl-core-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/src/blueetl_core/constants.py` & `blueetl-core-0.2.2/src/blueetl_core/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,13 +2,14 @@
 
 # Constants that can be set as environment variables to modify the behaviour of parallelization.
 
 # If more than 10, all iterations are printed to stderr. Above 50, the output is sent to stdout.
 # If not overridden, the value depends on logging: 0 if loglevel >= logging.WARNING else 10
 BLUEETL_JOBLIB_VERBOSE = "BLUEETL_JOBLIB_VERBOSE"
 # Number of concurrent jobs. If not overridden, it uses by default: os.cpu_count() // 2
+# If 1, do not use subprocesses (mainly for testing or debugging).
 BLUEETL_JOBLIB_JOBS = "BLUEETL_JOBLIB_JOBS"
 # JobLib backend (loky, multiprocessing, threading). If not overridden, it uses by default: loky
 BLUEETL_JOBLIB_BACKEND = "BLUEETL_JOBLIB_BACKEND"
 # Logging level to be configured in subprocesses.
 # If empty or not defined, use the effective log level of the parent process (recommended).
 BLUEETL_SUBPROCESS_LOGGING_LEVEL = "BLUEETL_SUBPROCESS_LOGGING_LEVEL"
```

### Comparing `blueetl-core-0.2.1/src/blueetl_core/etl.py` & `blueetl-core-0.2.2/src/blueetl_core/etl.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/src/blueetl_core/parallel.py` & `blueetl-core-0.2.2/src/blueetl_core/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,17 @@
         task = Task(partial(func, *args, **kwargs))
         ctx = TaskContext(
             task_id=0,
             loglevel=L.getEffectiveLevel(),
             seed=None,
             ppid=os.getpid(),
         )
+        if os.getenv(BLUEETL_JOBLIB_JOBS) == "1":
+            # execute the task in the current process and return the result
+            return task(ctx)
         executor = get_reusable_executor(max_workers=1, reuse=False)
         try:
             future = executor.submit(task, ctx)
             return future.result()
         finally:
             executor.shutdown(wait=True)
```

### Comparing `blueetl-core-0.2.1/src/blueetl_core/utils.py` & `blueetl-core-0.2.2/src/blueetl_core/utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/src/blueetl_core.egg-info/PKG-INFO` & `blueetl-core-0.2.2/src/blueetl_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
```

### Comparing `blueetl-core-0.2.1/src/blueetl_core.egg-info/SOURCES.txt` & `blueetl-core-0.2.2/src/blueetl_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tests/conftest.py` & `blueetl-core-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tests/test_etl_dataframe.py` & `blueetl-core-0.2.2/tests/test_etl_dataframe.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tests/test_etl_index.py` & `blueetl-core-0.2.2/tests/test_etl_index.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tests/test_etl_series.py` & `blueetl-core-0.2.2/tests/test_etl_series.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tests/test_utils.py` & `blueetl-core-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.2.1/tox.ini` & `blueetl-core-0.2.2/tox.ini`

 * *Files identical despite different names*

