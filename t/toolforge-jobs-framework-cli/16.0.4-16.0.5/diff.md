# Comparing `tmp/toolforge-jobs-framework-cli-16.0.4.tar.gz` & `tmp/toolforge-jobs-framework-cli-16.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-jobs-framework-cli-16.0.4.tar", last modified: Wed Apr  3 17:16:41 2024, max compression
+gzip compressed data, was "toolforge-jobs-framework-cli-16.0.5.tar", last modified: Mon Apr  8 08:51:44 2024, max compression
```

## Comparing `toolforge-jobs-framework-cli-16.0.4.tar` & `toolforge-jobs-framework-cli-16.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.444186 toolforge-jobs-framework-cli-16.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 17:16:41.444186 toolforge-jobs-framework-cli-16.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_dump.py
--rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tests/test_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/tjf_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/api.py
--rw-rw-rw-   0 root         (0) root         (0)    31930 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-03 17:16:36.000000 toolforge-jobs-framework-cli-16.0.4/tjf_cli/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:16:41.440186 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-03 17:16:41.000000 toolforge-jobs-framework-cli-16.0.4/toolforge_jobs_framework_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35120 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.105943 toolforge-jobs-framework-cli-16.0.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2651 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     6173 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tests/test_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/tjf_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    32109 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2024-04-08 08:51:39.000000 toolforge-jobs-framework-cli-16.0.5/tjf_cli/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:51:44.109943 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      355 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 08:51:44.000000 toolforge-jobs-framework-cli-16.0.5/toolforge_jobs_framework_cli.egg-info/top_level.txt
```

### Comparing `toolforge-jobs-framework-cli-16.0.4/LICENSE` & `toolforge-jobs-framework-cli-16.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/README.md` & `toolforge-jobs-framework-cli-16.0.5/README.md`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tests/test_api.py` & `toolforge-jobs-framework-cli-16.0.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tests/test_dump.py` & `toolforge-jobs-framework-cli-16.0.5/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tests/test_loader.py` & `toolforge-jobs-framework-cli-16.0.5/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tjf_cli/api.py` & `toolforge-jobs-framework-cli-16.0.5/tjf_cli/api.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tjf_cli/cli.py` & `toolforge-jobs-framework-cli-16.0.5/tjf_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,16 +376,19 @@
         job.pop("schedule", None)
     elif cont is not None:
         job["type"] = "continuous"
         job.pop("continuous", None)
     else:
         job["type"] = "one-off"
 
-    filelog = job.get("filelog", "false")
-    if filelog == "True":
+    filelog = job.get("filelog", False)
+    # We are currently sending a stringified boolean, remove str support once
+    # https://gitlab.wikimedia.org/repos/cloud/toolforge/jobs-api/-/merge_requests/70
+    # is in
+    if str(filelog) == "True":
         job["filelog"] = "yes"
     else:
         job["filelog"] = "no"
 
     if retry == 0:
         job["retry"] = "no"
     else:
```

### Comparing `toolforge-jobs-framework-cli-16.0.4/tjf_cli/errors.py` & `toolforge-jobs-framework-cli-16.0.5/tjf_cli/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-jobs-framework-cli-16.0.4/tjf_cli/loader.py` & `toolforge-jobs-framework-cli-16.0.5/tjf_cli/loader.py`

 * *Files identical despite different names*

