# Comparing `tmp/robocorp_tasks-3.0.1.tar.gz` & `tmp/robocorp_tasks-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-3.0.1.tar", max compression
+gzip compressed data, was "robocorp_tasks-3.0.2.tar", max compression
```

## Comparing `robocorp_tasks-3.0.1.tar` & `robocorp_tasks-3.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rwxr-xr-x   0        0        0     2111 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/README.md
--rw-r--r--   0        0        0     1565 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     4325 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     7959 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1494 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     8261 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    28952 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      331 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_constants.py
--rw-r--r--   0        0        0        0 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_customization/__init__.py
--rw-r--r--   0        0        0      572 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_customization/_extension_points.py
--rw-r--r--   0        0        0     9934 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      242 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     5399 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_fixtures.py
--rw-r--r--   0        0        0     2396 2024-03-19 13:07:35.889064 robocorp_tasks-3.0.1/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     7491 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     1022 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2881 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     4362 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0    13594 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_remove_refs.py
--rw-r--r--   0        0        0    10927 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     3837 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 13:07:35.893064 robocorp_tasks-3.0.1/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     3045 1970-01-01 00:00:00.000000 robocorp_tasks-3.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2189 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/README.md
+-rw-r--r--   0        0        0     1565 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4325 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     7959 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1494 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     8261 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    28952 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      331 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9934 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      242 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     5399 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_fixtures.py
+-rw-r--r--   0        0        0     2396 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     1022 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2881 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     4362 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0    13594 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_remove_refs.py
+-rw-r--r--   0        0        0    10927 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     3837 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:48.669823 robocorp_tasks-3.0.2/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 robocorp_tasks-3.0.2/PKG-INFO
```

### Comparing `robocorp_tasks-3.0.1/README.md` & `robocorp_tasks-3.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 # robocorp-tasks
 
-`robocorp-tasks` is a Python framework designed to simplify the development 
-of Python automations.
+`robocorp-tasks` is a Python framework designed to simplify the development of Python automations.
 
 ## Why
 
-While Python is widely used in the automation world, many solutions end up being 
-ad-hoc, making it difficult to navigate different projects and keep up with the
-features required for analysing the results of such automations afterwards.
+While Python is widely used in the automation world, many solutions end up being ad-hoc, making it difficult to navigate different projects and keep up with the features required for analysing the results of such automations afterwards.
 
 ## How
 
-`robocorp-tasks` provides a runner for running tasks that offers logging 
-out of the box for Python code (showing method calls, arguments, assigns, etc)
-by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
+`robocorp-tasks` provides a runner for running tasks that offers logging out of the box for Python code (showing method calls, arguments, assigns, etc) by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
 
 ## Getting started
 
-Replace the code in your `__main__` with a method that has the name of your task
-(which should not have parameters) and decorate it with the `@task` decorator, like this:
+Replace the code in your `__main__` with a method that has the name of your task (which should not have parameters) and decorate it with the `@task` decorator, like this:
 
 i.e.:
 
-
 ```
 from robocorp.tasks import task
 
 @task
 def my_task():
     ...
 ```
 
-2. Call your task using the command line below, customizing the directory and task name as needed:
-
+Call your task using the command line below, customizing the directory and task name as needed:
 
 ```
 python -m robocorp.tasks run <path/to/file.py or directory> -t <task_name>
 ```
 
 Note: if you have only one defined task in your target, the `-t <task_name>` option is not needed. 
 
 Note: the task name is the name of the method decorated with `@task`.
 
 Note: if a directory is given, only files named `*task*.py` will be used for collection.
 
-Note: in the current version only one task can be run per invocation. If more than one task 
-is found an error will be given and no tasks will be run.
+Note: in the current version only one task can be run per invocation. If more than one task is found an error will be given and no tasks will be run.
 
-3. View the log results in `output/log.html`.
+View the log results in `output/log.html`.
 
 ## Guides
 
 - [Logging customization](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/00-logging-customization.md)
 - [Output customization](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/01-output-customization.md)
+- [Setups & Teardowns](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/02-setups-teardowns.md)
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.tasks](https://github.com/robocorp/robocorp/blob/master/tasks/docs/api/robocorp.tasks.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/tasks/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/tasks/docs/CHANGELOG.md).
```

### Comparing `robocorp_tasks-3.0.1/pyproject.toml` & `robocorp_tasks-3.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "3.0.1"
+version = "3.0.2"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/__init__.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import Dict, Optional
 
 from ._fixtures import setup, teardown
 from ._protocols import ITask, Status
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(*args, **kwargs):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_callback.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_commands.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_config.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_customization/_extension_points.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_customization/_plugin_manager.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_fixtures.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_interrupts.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_interrupts.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_remove_refs.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/_task.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/src/robocorp/tasks/cli.py` & `robocorp_tasks-3.0.2/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-3.0.1/PKG-INFO` & `robocorp_tasks-3.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 3.0.1
+Version: 3.0.2
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,69 +19,61 @@
 Requires-Dist: psutil (>=5.0,<6.0)
 Requires-Dist: robocorp-log (>=2.4,<3)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
-`robocorp-tasks` is a Python framework designed to simplify the development 
-of Python automations.
+`robocorp-tasks` is a Python framework designed to simplify the development of Python automations.
 
 ## Why
 
-While Python is widely used in the automation world, many solutions end up being 
-ad-hoc, making it difficult to navigate different projects and keep up with the
-features required for analysing the results of such automations afterwards.
+While Python is widely used in the automation world, many solutions end up being ad-hoc, making it difficult to navigate different projects and keep up with the features required for analysing the results of such automations afterwards.
 
 ## How
 
-`robocorp-tasks` provides a runner for running tasks that offers logging 
-out of the box for Python code (showing method calls, arguments, assigns, etc)
-by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
+`robocorp-tasks` provides a runner for running tasks that offers logging out of the box for Python code (showing method calls, arguments, assigns, etc) by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
 
 ## Getting started
 
-Replace the code in your `__main__` with a method that has the name of your task
-(which should not have parameters) and decorate it with the `@task` decorator, like this:
+Replace the code in your `__main__` with a method that has the name of your task (which should not have parameters) and decorate it with the `@task` decorator, like this:
 
 i.e.:
 
-
 ```
 from robocorp.tasks import task
 
 @task
 def my_task():
     ...
 ```
 
-2. Call your task using the command line below, customizing the directory and task name as needed:
-
+Call your task using the command line below, customizing the directory and task name as needed:
 
 ```
 python -m robocorp.tasks run <path/to/file.py or directory> -t <task_name>
 ```
 
 Note: if you have only one defined task in your target, the `-t <task_name>` option is not needed. 
 
 Note: the task name is the name of the method decorated with `@task`.
 
 Note: if a directory is given, only files named `*task*.py` will be used for collection.
 
-Note: in the current version only one task can be run per invocation. If more than one task 
-is found an error will be given and no tasks will be run.
+Note: in the current version only one task can be run per invocation. If more than one task is found an error will be given and no tasks will be run.
 
-3. View the log results in `output/log.html`.
+View the log results in `output/log.html`.
 
 ## Guides
 
 - [Logging customization](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/00-logging-customization.md)
 - [Output customization](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/01-output-customization.md)
+- [Setups & Teardowns](https://github.com/robocorp/robocorp/blob/master/tasks/docs/guides/02-setups-teardowns.md)
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.tasks](https://github.com/robocorp/robocorp/blob/master/tasks/docs/api/robocorp.tasks.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/tasks/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/tasks/docs/CHANGELOG.md).
```

