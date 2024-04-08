# Comparing `tmp/robocorp_workitems-1.4.4.tar.gz` & `tmp/robocorp_workitems-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-1.4.4.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.4.5.tar", max compression
```

## Comparing `robocorp_workitems-1.4.4.tar` & `robocorp_workitems-1.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     2939 2024-03-19 08:03:37.796237 robocorp_workitems-1.4.4/README.md
--rw-r--r--   0        0        0      909 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     5053 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0     2796 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/__init__.py
--rw-r--r--   0        0        0     1831 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_base.py
--rw-r--r--   0        0        0     8636 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_file.py
--rw-r--r--   0        0        0     8966 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_robocorp.py
--rw-r--r--   0        0        0     1423 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_context.py
--rw-r--r--   0        0        0     1173 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_exceptions.py
--rw-r--r--   0        0        0     6596 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_requests.py
--rw-r--r--   0        0        0     1613 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_types.py
--rw-r--r--   0        0        0     2401 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_utils.py
--rw-r--r--   0        0        0    16557 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/_workitem.py
--rw-r--r--   0        0        0        0 2024-03-19 08:03:37.800237 robocorp_workitems-1.4.4/src/robocorp/workitems/py.typed
--rw-r--r--   0        0        0     3823 1970-01-01 00:00:00.000000 robocorp_workitems-1.4.4/PKG-INFO
+-rwxr-xr-x   0        0        0     2908 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/README.md
+-rw-r--r--   0        0        0      909 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5053 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0     2796 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/__init__.py
+-rw-r--r--   0        0        0     1831 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_base.py
+-rw-r--r--   0        0        0     8636 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_file.py
+-rw-r--r--   0        0        0     8966 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_robocorp.py
+-rw-r--r--   0        0        0     1423 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0     1173 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6596 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1613 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2401 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0    16557 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:13:51.041029 robocorp_workitems-1.4.5/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 robocorp_workitems-1.4.5/PKG-INFO
```

### Comparing `robocorp_workitems-1.4.4/README.md` & `robocorp_workitems-1.4.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 # robocorp-workitems
 
-Work items are used in Robocorp Control Room for managing data that go through
-multiple steps and tasks inside a process. Each step of a process receives input
-work items from the previous step, and creates output work items for the next
-step.
+Work items are used in Robocorp Control Room for managing data that go through multiple steps and tasks inside a process. Each step of a process receives input work items from the previous step, and creates output work items for the next step.
 
 ## Getting started
 
-The library exposes two objects, `inputs` and `outputs`, which are the main way
-to interact with work item queues. The former deals with the reading input work
-items, and the latter with creating output work items.
-
-A run inside Control Room will always have at least one work item available to
-it. The simplest Robot which reads the current work item and creates an output
-can be done in the following manner:
+The library exposes two objects, `inputs` and `outputs`, which are the main way to interact with work item queues. The former deals with the reading input work items, and the latter with creating output work items.
+
+A run inside Control Room will always have at least one work item available to it. The simplest Robot which reads the current work item and creates an output can be done in the following manner:
 
 ```python
 from robocorp import workitems
 from robocorp.tasks import task
 
 @task
 def handle_item():
@@ -37,20 +30,17 @@
     for item in workitems.inputs:
         print("Received payload:", item.payload)
         workitems.outputs.create(payload={"key": "value"})
 ```
 
 ### Work item structure
 
-A work item's data payload is JSON and allows storing anything that is JSON
-serializable. By default the payload is a mapping of key-value pairs.
+A work item's data payload is JSON and allows storing anything that is JSON serializable. By default, the payload is a mapping of key-value pairs.
 
-In addition to the payload section, a work item can also contain files, which
-are stored within Robocorp Control Room. Adding and using files with work items
-requires no additional setup from the user.
+In addition to the payload section, a work item can also contain files, which are stored within Robocorp Control Room. Adding and using files with work items requires no additional setup from the user.
 
 ## Guides
 
 - [Reserving and releasing input items](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/00-reserving-inputs.md)
 - [Creating outputs](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/01-creating-outputs.md)
 - [Local development](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/02-local-development.md)
 - [Email triggering](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/03-email-triggering.md)
@@ -58,12 +48,12 @@
 - [Flow control with exceptions](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/05-input-exceptions.md)
 - [Modifying inputs](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/06-modifying-inputs.md)
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.workitems](https://github.com/robocorp/robocorp/blob/master/workitems/docs/api/robocorp.workitems.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/workitems/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/workitems/docs/CHANGELOG.md).
```

### Comparing `robocorp_workitems-1.4.4/pyproject.toml` & `robocorp_workitems-1.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-workitems"
-version = "1.4.4"
+version = "1.4.5"
 description = "Robocorp Work Items library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Cosmin P. <cosmin@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
```

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/__init__.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     BusinessException,
     EmptyQueue,
     to_exception_type,
 )
 from ._types import ExceptionType, JSONType, PathType, State
 from ._workitem import Input, Output
 
-__version__ = "1.4.4"
+__version__ = "1.4.5"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 @task_cache
 def __ctx():
```

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/__init__.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_base.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_base.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_file.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_file.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_adapters/_robocorp.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_adapters/_robocorp.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_context.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_exceptions.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_requests.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_types.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_utils.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/src/robocorp/workitems/_workitem.py` & `robocorp_workitems-1.4.5/src/robocorp/workitems/_workitem.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.4.4/PKG-INFO` & `robocorp_workitems-1.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-workitems
-Version: 1.4.4
+Version: 1.4.5
 Summary: Robocorp Work Items library
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,28 +19,21 @@
 Requires-Dist: robocorp-tasks (>=1,<4)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/robocorp/robocorp/
 Description-Content-Type: text/markdown
 
 # robocorp-workitems
 
-Work items are used in Robocorp Control Room for managing data that go through
-multiple steps and tasks inside a process. Each step of a process receives input
-work items from the previous step, and creates output work items for the next
-step.
+Work items are used in Robocorp Control Room for managing data that go through multiple steps and tasks inside a process. Each step of a process receives input work items from the previous step, and creates output work items for the next step.
 
 ## Getting started
 
-The library exposes two objects, `inputs` and `outputs`, which are the main way
-to interact with work item queues. The former deals with the reading input work
-items, and the latter with creating output work items.
-
-A run inside Control Room will always have at least one work item available to
-it. The simplest Robot which reads the current work item and creates an output
-can be done in the following manner:
+The library exposes two objects, `inputs` and `outputs`, which are the main way to interact with work item queues. The former deals with the reading input work items, and the latter with creating output work items.
+
+A run inside Control Room will always have at least one work item available to it. The simplest Robot which reads the current work item and creates an output can be done in the following manner:
 
 ```python
 from robocorp import workitems
 from robocorp.tasks import task
 
 @task
 def handle_item():
@@ -60,20 +53,17 @@
     for item in workitems.inputs:
         print("Received payload:", item.payload)
         workitems.outputs.create(payload={"key": "value"})
 ```
 
 ### Work item structure
 
-A work item's data payload is JSON and allows storing anything that is JSON
-serializable. By default the payload is a mapping of key-value pairs.
+A work item's data payload is JSON and allows storing anything that is JSON serializable. By default, the payload is a mapping of key-value pairs.
 
-In addition to the payload section, a work item can also contain files, which
-are stored within Robocorp Control Room. Adding and using files with work items
-requires no additional setup from the user.
+In addition to the payload section, a work item can also contain files, which are stored within Robocorp Control Room. Adding and using files with work items requires no additional setup from the user.
 
 ## Guides
 
 - [Reserving and releasing input items](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/00-reserving-inputs.md)
 - [Creating outputs](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/01-creating-outputs.md)
 - [Local development](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/02-local-development.md)
 - [Email triggering](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/03-email-triggering.md)
@@ -81,13 +71,13 @@
 - [Flow control with exceptions](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/05-input-exceptions.md)
 - [Modifying inputs](https://github.com/robocorp/robocorp/blob/master/workitems/docs/guides/06-modifying-inputs.md)
 
 Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
 
 ## API Reference
 
-Information on specific functions or classes: [robocorp.workitems](https://github.com/robocorp/robocorp/blob/master/workitems/docs/api/robocorp.workitems.md)
+Explore our [API](https://github.com/robocorp/robocorp/blob/master/workitems/docs/api/README.md) for extensive documentation.
 
 ## Changelog
 
 A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robocorp/blob/master/workitems/docs/CHANGELOG.md).
```

