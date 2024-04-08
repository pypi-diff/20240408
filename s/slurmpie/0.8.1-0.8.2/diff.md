# Comparing `tmp/slurmpie-0.8.1.tar.gz` & `tmp/slurmpie-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slurmpie-0.8.1.tar", last modified: Wed Apr  3 13:48:01 2024, max compression
+gzip compressed data, was "dist/slurmpie-0.8.2.tar", last modified: Mon Apr  8 13:58:25 2024, max compression
```

## Comparing `slurmpie-0.8.1.tar` & `slurmpie-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 13:47:37.000000 slurmpie-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 13:48:01.000000 slurmpie-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 13:47:37.000000 slurmpie-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 13:48:01.000000 slurmpie-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-03 13:47:37.000000 slurmpie-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:47:37.000000 slurmpie-0.8.1/slurmpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-04-03 13:47:37.000000 slurmpie-0.8.1/slurmpie/slurmpie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 13:48:01.000000 slurmpie-0.8.1/slurmpie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:48:01.000000 slurmpie-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-03 13:47:37.000000 slurmpie-0.8.1/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 13:58:03.000000 slurmpie-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 13:58:25.000000 slurmpie-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 13:58:03.000000 slurmpie-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 13:58:25.000000 slurmpie-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 13:58:03.000000 slurmpie-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:03.000000 slurmpie-0.8.2/slurmpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-04-08 13:58:03.000000 slurmpie-0.8.2/slurmpie/slurmpie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 13:58:25.000000 slurmpie-0.8.2/slurmpie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:25.000000 slurmpie-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-08 13:58:03.000000 slurmpie-0.8.2/tests/test_pipeline.py
```

### Comparing `slurmpie-0.8.1/LICENSE` & `slurmpie-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.1/PKG-INFO` & `slurmpie-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.1/README.md` & `slurmpie-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.1/setup.py` & `slurmpie-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="slurmpie",
-    version="0.8.1",
+    version="0.8.2",
     author="Sebastian van der Voort",
     author_email="Svdvoort@users.noreply.github.com",
     description="Package to interact with SLURM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/svdvoort/slurmpie",
     packages=setuptools.find_packages(),
```

### Comparing `slurmpie-0.8.1/slurmpie/slurmpie.py` & `slurmpie-0.8.2/slurmpie/slurmpie.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,17 +422,15 @@
 
         stdout, stderr = sbatch_process.communicate()
 
         if sbatch_process.returncode != 0 or "error" in stdout.decode("utf-8").lower():
             submitted_command = " ".join(sbatch_command)
             err_msg = "Sbatch job submission failed with follow error:\n{msg}\nSubmitted using the following command:\n{submitted_command}"
             raise RuntimeError(
-                err_msg.format(
-                    msg=stderr, sbatch_submitted_commandcommand=submitted_command
-                )
+                err_msg.format(msg=stderr, submitted_command=submitted_command)
             )
         else:
             job_number = stdout.decode("utf-8").strip().split(":")[0]
         return job_number
 
 
 class Pipeline:
```

### Comparing `slurmpie-0.8.1/slurmpie.egg-info/PKG-INFO` & `slurmpie-0.8.2/slurmpie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.8.1/tests/test_jobs.py` & `slurmpie-0.8.2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `slurmpie-0.8.1/tests/test_pipeline.py` & `slurmpie-0.8.2/tests/test_pipeline.py`

 * *Files identical despite different names*

