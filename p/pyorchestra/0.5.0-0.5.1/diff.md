# Comparing `tmp/pyorchestra-0.5.0.tar.gz` & `tmp/pyorchestra-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.5.0.tar", max compression
+gzip compressed data, was "pyorchestra-0.5.1.tar", max compression
```

## Comparing `pyorchestra-0.5.0.tar` & `pyorchestra-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/LICENSE
--rwxr-xr-x   0        0        0    25622 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/README.md
--rwxr-xr-x   0        0        0       62 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      655 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1294 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/main.py
--rwxr-xr-x   0        0        0    10221 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      519 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/backend.py
--rwxr-xr-x   0        0        0    19474 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/formatting.py
--rwxr-xr-x   0        0        0      168 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/job.py
--rwxr-xr-x   0        0        0     1575 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/models.py
--rwxr-xr-x   0        0        0    10720 2024-04-05 14:15:22.444179 pyorchestra-0.5.0/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-05 14:15:22.448179 pyorchestra-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-08 09:10:23.346701 pyorchestra-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0    25622 2024-04-08 09:10:23.346701 pyorchestra-0.5.1/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      655 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1294 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/main.py
+-rwxr-xr-x   0        0        0    10221 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      531 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/backend.py
+-rwxr-xr-x   0        0        0    19474 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/core.py
+-rwxr-xr-x   0        0        0      873 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/formatting.py
+-rwxr-xr-x   0        0        0      168 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/job.py
+-rwxr-xr-x   0        0        0     1575 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/models.py
+-rwxr-xr-x   0        0        0    10720 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-08 09:10:23.350700 pyorchestra-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    26496 1970-01-01 00:00:00.000000 pyorchestra-0.5.1/PKG-INFO
```

### Comparing `pyorchestra-0.5.0/LICENSE` & `pyorchestra-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/README.md` & `pyorchestra-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/dto/job.py` & `pyorchestra-0.5.1/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/dto/run.py` & `pyorchestra-0.5.1/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/dto/schedule_definition.py` & `pyorchestra-0.5.1/orchestra/api/dto/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/dto/task.py` & `pyorchestra-0.5.1/orchestra/api/dto/task.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/main.py` & `pyorchestra-0.5.1/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/routers/jobs.py` & `pyorchestra-0.5.1/orchestra/api/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/api/routers/tasks.py` & `pyorchestra-0.5.1/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/backend.py` & `pyorchestra-0.5.1/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/core.py` & `pyorchestra-0.5.1/orchestra/core.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/formatting.py` & `pyorchestra-0.5.1/orchestra/formatting.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/models.py` & `pyorchestra-0.5.1/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/orchestra/scheduling.py` & `pyorchestra-0.5.1/orchestra/scheduling.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.0/pyproject.toml` & `pyorchestra-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.5.0"
+version = "0.5.1"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.5.0/PKG-INFO` & `pyorchestra-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorchestra
-Version: 0.5.0
+Version: 0.5.1
 Summary: Orchestra is a job scheduler on top of Celery
 Home-page: https://github.com/vidosits/orchestra
 License: LGPLv3
 Author: András Vidosits
 Author-email: andras@hyperplane.hu
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: License :: Other/Proprietary License
```

