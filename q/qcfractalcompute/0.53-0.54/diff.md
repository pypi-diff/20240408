# Comparing `tmp/qcfractalcompute-0.53.tar.gz` & `tmp/qcfractalcompute-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcfractalcompute-0.53.tar", last modified: Tue Jan  9 21:45:31 2024, max compression
+gzip compressed data, was "qcfractalcompute-0.54.tar", last modified: Mon Apr  8 18:04:17 2024, max compression
```

## Comparing `qcfractalcompute-0.53.tar` & `qcfractalcompute-0.54.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/
--rw-r--r--   0 ben       (1000) users      (984)      653 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     1093 2023-09-20 13:55:23.000000 qcfractalcompute-0.53/pyproject.toml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.153344 qcfractalcompute-0.53/qcfractalcompute/
--rw-r--r--   0 ben       (1000) users      (984)      238 2023-09-20 13:55:23.000000 qcfractalcompute-0.53/qcfractalcompute/__init__.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/qcfractalcompute/apps/
--rw-r--r--   0 ben       (1000) users      (984)        0 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/apps/__init__.py
--rw-r--r--   0 ben       (1000) users      (984)     6741 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/apps/app_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     2016 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/apps/geometric.py
--rw-r--r--   0 ben       (1000) users      (984)     2592 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/apps/helpers.py
--rw-r--r--   0 ben       (1000) users      (984)      464 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/apps/models.py
--rw-r--r--   0 ben       (1000) users      (984)     3128 2023-11-21 21:02:10.000000 qcfractalcompute-0.53/qcfractalcompute/apps/qcengine.py
--rw-r--r--   0 ben       (1000) users      (984)     4149 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/compress.py
--rw-r--r--   0 ben       (1000) users      (984)    26322 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/compute_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     2214 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/compute_manager_cli.py
--rw-r--r--   0 ben       (1000) users      (984)     8549 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/config.py
--rw-r--r--   0 ben       (1000) users      (984)     8067 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/executors.py
--rw-r--r--   0 ben       (1000) users      (984)     1868 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/generic_wrapper.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/qcfractalcompute/run_scripts/
--rw-r--r--   0 ben       (1000) users      (984)      193 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/__init__.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/qcfractalcompute/run_scripts/__pycache__/
--rw-r--r--   0 ben       (1000) users      (984)      791 2023-10-27 15:10:21.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ben       (1000) users      (984)      729 2023-10-27 15:10:27.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 ben       (1000) users      (984)      230 2023-09-11 13:38:01.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/conda_list_env.sh
--rw-r--r--   0 ben       (1000) users      (984)     1484 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/generic_script.py
--rw-r--r--   0 ben       (1000) users      (984)     2590 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/geometric_nextchain.py
--rw-r--r--   0 ben       (1000) users      (984)     3529 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/qcengine_compute.py
--rw-r--r--   0 ben       (1000) users      (984)      644 2023-09-20 13:55:23.000000 qcfractalcompute-0.53/qcfractalcompute/run_scripts/qcengine_list.py
--rw-r--r--   0 ben       (1000) users      (984)     6273 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/test_compute_manager.py
--rw-r--r--   0 ben       (1000) users      (984)     1132 2023-11-08 15:48:56.000000 qcfractalcompute-0.53/qcfractalcompute/test_manager_config.py
--rw-r--r--   0 ben       (1000) users      (984)     6289 2023-12-05 16:08:13.000000 qcfractalcompute-0.53/qcfractalcompute/testing_helpers.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/qcfractalcompute.egg-info/
--rw-r--r--   0 ben       (1000) users      (984)      653 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     1219 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (984)        1 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (984)       88 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) users      (984)       15 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (984)       17 2024-01-09 21:45:31.000000 qcfractalcompute-0.53/qcfractalcompute.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) users      (984)       38 2024-01-09 21:45:31.156677 qcfractalcompute-0.53/setup.cfg
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/
+-rw-r--r--   0 ben       (1000) users      (984)      653 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     1093 2023-09-20 13:55:23.000000 qcfractalcompute-0.54/pyproject.toml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/qcfractalcompute/
+-rw-r--r--   0 ben       (1000) users      (984)      238 2023-09-20 13:55:23.000000 qcfractalcompute-0.54/qcfractalcompute/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/qcfractalcompute/apps/
+-rw-r--r--   0 ben       (1000) users      (984)        0 2023-09-11 13:38:01.000000 qcfractalcompute-0.54/qcfractalcompute/apps/__init__.py
+-rw-r--r--   0 ben       (1000) users      (984)     6741 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/apps/app_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     2016 2024-03-11 20:25:46.000000 qcfractalcompute-0.54/qcfractalcompute/apps/geometric.py
+-rw-r--r--   0 ben       (1000) users      (984)     2592 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/apps/helpers.py
+-rw-r--r--   0 ben       (1000) users      (984)      464 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/apps/models.py
+-rw-r--r--   0 ben       (1000) users      (984)     3128 2024-03-11 20:25:46.000000 qcfractalcompute-0.54/qcfractalcompute/apps/qcengine.py
+-rw-r--r--   0 ben       (1000) users      (984)     4149 2024-03-11 20:25:46.000000 qcfractalcompute-0.54/qcfractalcompute/compress.py
+-rw-r--r--   0 ben       (1000) users      (984)    26916 2024-04-07 13:23:41.000000 qcfractalcompute-0.54/qcfractalcompute/compute_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     2214 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/compute_manager_cli.py
+-rw-r--r--   0 ben       (1000) users      (984)     8549 2024-03-21 01:09:16.000000 qcfractalcompute-0.54/qcfractalcompute/config.py
+-rw-r--r--   0 ben       (1000) users      (984)     8054 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/executors.py
+-rw-r--r--   0 ben       (1000) users      (984)     1868 2023-09-11 13:38:01.000000 qcfractalcompute-0.54/qcfractalcompute/generic_wrapper.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/qcfractalcompute/run_scripts/
+-rw-r--r--   0 ben       (1000) users      (984)      193 2023-09-11 13:38:01.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/qcfractalcompute/run_scripts/__pycache__/
+-rw-r--r--   0 ben       (1000) users      (984)      791 2023-10-27 15:10:21.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ben       (1000) users      (984)      729 2023-10-27 15:10:27.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 ben       (1000) users      (984)      230 2023-09-11 13:38:01.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/conda_list_env.sh
+-rw-r--r--   0 ben       (1000) users      (984)     1484 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/generic_script.py
+-rw-r--r--   0 ben       (1000) users      (984)     2590 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/geometric_nextchain.py
+-rw-r--r--   0 ben       (1000) users      (984)     3529 2024-03-20 15:53:05.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/qcengine_compute.py
+-rw-r--r--   0 ben       (1000) users      (984)      644 2024-03-11 20:25:46.000000 qcfractalcompute-0.54/qcfractalcompute/run_scripts/qcengine_list.py
+-rw-r--r--   0 ben       (1000) users      (984)     7930 2024-04-07 13:23:41.000000 qcfractalcompute-0.54/qcfractalcompute/test_compute_manager.py
+-rw-r--r--   0 ben       (1000) users      (984)     1132 2023-11-08 15:48:56.000000 qcfractalcompute-0.54/qcfractalcompute/test_manager_config.py
+-rw-r--r--   0 ben       (1000) users      (984)     6420 2024-04-07 13:23:41.000000 qcfractalcompute-0.54/qcfractalcompute/testing_helpers.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/qcfractalcompute.egg-info/
+-rw-r--r--   0 ben       (1000) users      (984)      653 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     1219 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (984)        1 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (984)       88 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) users      (984)       15 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (984)       17 2024-04-08 18:04:17.000000 qcfractalcompute-0.54/qcfractalcompute.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) users      (984)       38 2024-04-08 18:04:17.023903 qcfractalcompute-0.54/setup.cfg
```

### Comparing `qcfractalcompute-0.53/PKG-INFO` & `qcfractalcompute-0.54/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractalcompute
-Version: 0.53
+Version: 0.54
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcfractalcompute-0.53/pyproject.toml` & `qcfractalcompute-0.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/apps/app_manager.py` & `qcfractalcompute-0.54/qcfractalcompute/apps/app_manager.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/apps/geometric.py` & `qcfractalcompute-0.54/qcfractalcompute/apps/geometric.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/apps/helpers.py` & `qcfractalcompute-0.54/qcfractalcompute/apps/helpers.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/apps/qcengine.py` & `qcfractalcompute-0.54/qcfractalcompute/apps/qcengine.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/compress.py` & `qcfractalcompute-0.54/qcfractalcompute/compress.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/compute_manager.py` & `qcfractalcompute-0.54/qcfractalcompute/compute_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,26 +127,41 @@
         # key = executor label, value = (key = task_id, value = parsl future)
         self._task_futures: Dict[str, Dict[int, ParslFuture]] = {exl: {} for exl in config.executors.keys()}
 
         # Mapping of task_id to record_id
         self._record_id_map: Dict[int, int] = {}
 
         self.all_queue_tags = []
-        for ex_config in config.executors.values():
+        for ex_label, ex_config in config.executors.items():
+            if len(ex_config.queue_tags) == 0:
+                raise ValueError(f"Executor {ex_label} has no queue tags")
+
             self.all_queue_tags.extend(ex_config.queue_tags)
 
+        # Merge queue tags, preserving order
+        self.all_queue_tags = list(dict.fromkeys(self.all_queue_tags))
+
         # These are more properly set up in the start() method
         self.parsl_config = None
         self.dflow_kernel = None
 
         # Set up the app manager
-        self.app_manager = AppManager(self.manager_config)
-        self.executor_programs = {
-            ex: self.app_manager.all_program_info(ex) for ex in self.manager_config.executors.keys()
-        }
+        # A bit hacky, but the app_manager may already be set if
+        # we are running in a testing environment
+        if not hasattr(self, "app_manager"):
+            self.app_manager = AppManager(self.manager_config)
+
+        self.executor_programs = {}
+        for ex in self.manager_config.executors.keys():
+            ex_programs = self.app_manager.all_program_info(ex)
+            if len(ex_programs) == 0:
+                raise ValueError(f"Executor {ex} has no available programs")
+
+            self.executor_programs[ex] = ex_programs
+
         self.all_program_info = self.app_manager.all_program_info()
 
         self.logger.info("-" * 80)
         self.logger.info("QCFractal Compute Manager:")
         self.logger.info("    Version:     {}".format(__version__))
         self.logger.info("    Base folder: {}".format(self.manager_config.base_folder))
         self.logger.info("    Cluster:     {}".format(self.name_data.cluster))
```

### Comparing `qcfractalcompute-0.53/qcfractalcompute/compute_manager_cli.py` & `qcfractalcompute-0.54/qcfractalcompute/compute_manager_cli.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/config.py` & `qcfractalcompute-0.54/qcfractalcompute/config.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/executors.py` & `qcfractalcompute-0.54/qcfractalcompute/executors.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,10 +179,9 @@
         m = importlib.import_module(executor_config.config_file)
         ex = m.get_executor()
 
         for tag in executor_config.queue_tags:
             self.tag_executor_map[tag] = ex.label
 
         self.executor_config_map[ex.label] = executor_config
-        pass
     else:
         raise ValueError("Unknown executor type: {}".format(executor_config.type))
```

### Comparing `qcfractalcompute-0.53/qcfractalcompute/generic_wrapper.py` & `qcfractalcompute-0.54/qcfractalcompute/generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-312.pyc` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/generic_script.py` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/generic_script.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/geometric_nextchain.py` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/geometric_nextchain.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/qcengine_compute.py` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/qcengine_compute.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/run_scripts/qcengine_list.py` & `qcfractalcompute-0.54/qcfractalcompute/run_scripts/qcengine_list.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/test_compute_manager.py` & `qcfractalcompute-0.54/qcfractalcompute/test_compute_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -80,14 +80,64 @@
     compute_thread.join()
 
     managers = storage_socket.managers.query(ManagerQueryFilters())
     assert len(managers) == 1
     assert set(managers[0]["tags"]) == {"tag1", "tag2", "tag3", "tag4", "*"}
 
 
+def test_manager_tags_missing(snowflake: QCATestingSnowflake, tmp_path):
+    compute_config = FractalComputeConfig(
+        base_folder=str(tmp_path),
+        cluster="testing_compute",
+        update_frequency=5,
+        server=FractalServerSettings(
+            fractal_uri=snowflake.get_uri(),
+            verify=False,
+        ),
+        executors={
+            "local": LocalExecutorConfig(
+                cores_per_worker=1,
+                memory_per_worker=1,
+                max_workers=1,
+                queue_tags=["tag1", "tag2", "*"],
+            ),
+            "local2": LocalExecutorConfig(cores_per_worker=1, memory_per_worker=1, max_workers=1, queue_tags=[]),
+        },
+    )
+
+    with pytest.raises(ValueError, match="local2 has no queue tags"):
+        ComputeManager(compute_config)
+
+
+def test_manager_tags_duplicate(snowflake: QCATestingSnowflake, tmp_path):
+    compute_config = FractalComputeConfig(
+        base_folder=str(tmp_path),
+        cluster="testing_compute",
+        update_frequency=5,
+        server=FractalServerSettings(
+            fractal_uri=snowflake.get_uri(),
+            verify=False,
+        ),
+        executors={
+            "local": LocalExecutorConfig(
+                cores_per_worker=1,
+                memory_per_worker=1,
+                max_workers=1,
+                queue_tags=["tag1", "tag2", "*"],
+            ),
+            "local2": LocalExecutorConfig(
+                cores_per_worker=1, memory_per_worker=1, max_workers=1, queue_tags=["tag2", "tag1"]
+            ),
+        },
+    )
+
+    compute = ComputeManager(compute_config)
+    assert compute.all_queue_tags == ["tag1", "tag2", "*"]
+
+
 @pytest.mark.filterwarnings("ignore:Exception in thread")
 def test_manager_claim_inactive(snowflake: QCATestingSnowflake):
     storage_socket = snowflake.get_storage_socket()
     snowflake.start_job_runner()
 
     compute = QCATestingComputeThread(snowflake._qcf_config, {})
     compute.start(manual_updates=False)
```

### Comparing `qcfractalcompute-0.53/qcfractalcompute/test_manager_config.py` & `qcfractalcompute-0.54/qcfractalcompute/test_manager_config.py`

 * *Files identical despite different names*

### Comparing `qcfractalcompute-0.53/qcfractalcompute/testing_helpers.py` & `qcfractalcompute-0.54/qcfractalcompute/testing_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 from qcfractalcompute.compress import compress_result
 from qcfractalcompute.compute_manager import ComputeManager
 from qcfractalcompute.config import FractalComputeConfig, FractalServerSettings, LocalExecutorConfig
 from qcportal.all_results import AllResultTypes
 from qcportal.record_models import PriorityEnum, RecordTask
 
 
+class MockTestingAppManager:
+    def all_program_info(self, executor_label: Optional[str] = None) -> Dict[str, List[str]]:
+        return _activated_manager_programs
+
+
 class MockTestingComputeManager(ComputeManager):
     def __init__(self, qcf_config: FractalConfig, result_data: Dict[int, AllResultTypes]):
         self._qcf_config = qcf_config
 
         host = self._qcf_config.api.host
         port = self._qcf_config.api.port
         uri = f"http://{host}:{port}"
@@ -53,18 +58,18 @@
                     memory_per_worker=1,
                     max_workers=1,
                     queue_tags=["*"],
                     scratch_directory=compute_scratch_dir,
                 )
             },
         )
-        ComputeManager.__init__(self, self._compute_config)
 
-        # overwrite the executor programs for testing
-        self.executor_programs = {"local": _activated_manager_programs}
+        # Set the app manager already
+        self.app_manager = MockTestingAppManager()
+        ComputeManager.__init__(self, self._compute_config)
 
         def cleanup(d):
             d.cleanup()
 
         weakref.finalize(self, cleanup, tmpdir)
 
         # Shorten the timeout on the client for testing
```

### Comparing `qcfractalcompute-0.53/qcfractalcompute.egg-info/PKG-INFO` & `qcfractalcompute-0.54/qcfractalcompute.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcfractalcompute
-Version: 0.53
+Version: 0.54
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcfractalcompute-0.53/qcfractalcompute.egg-info/SOURCES.txt` & `qcfractalcompute-0.54/qcfractalcompute.egg-info/SOURCES.txt`

 * *Files identical despite different names*

