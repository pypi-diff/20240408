# Comparing `tmp/fbnconfig-0.0.36.tar.gz` & `tmp/fbnconfig-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbnconfig-0.0.36.tar", max compression
+gzip compressed data, was "fbnconfig-0.0.37.tar", max compression
```

## Comparing `fbnconfig-0.0.36.tar` & `fbnconfig-0.0.37.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      176 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/__init__.py
--rw-r--r--   0        0        0     6600 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/access.py
--rw-r--r--   0        0        0     6513 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/configuration.py
--rw-r--r--   0        0        0     4113 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/deploy.py
--rw-r--r--   0        0        0     8124 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/drive.py
--rw-r--r--   0        0        0     7488 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/identity.py
--rw-r--r--   0        0        0     1057 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/load_module.py
--rw-r--r--   0        0        0     9681 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/log.py
--rw-r--r--   0        0        0     8126 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/main.py
--rw-r--r--   0        0        0      771 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/resource_abc.py
--rw-r--r--   0        0        0    14699 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig/scheduler.py
--rw-r--r--   0        0        0     7913 2024-03-25 10:13:58.000000 fbnconfig-0.0.36/fbnconfig.md
--rw-r--r--   0        0        0     1070 2024-03-25 10:17:24.404688 fbnconfig-0.0.36/pyproject.toml
--rw-r--r--   0        0        0     8445 1970-01-01 00:00:00.000000 fbnconfig-0.0.36/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/access.py
+-rw-r--r--   0        0        0     6513 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/configuration.py
+-rw-r--r--   0        0        0     4113 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/deploy.py
+-rw-r--r--   0        0        0     8124 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/drive.py
+-rw-r--r--   0        0        0     7488 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/identity.py
+-rw-r--r--   0        0        0     1057 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/load_module.py
+-rw-r--r--   0        0        0     9681 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/log.py
+-rw-r--r--   0        0        0     8126 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/main.py
+-rw-r--r--   0        0        0      771 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/resource_abc.py
+-rw-r--r--   0        0        0    14708 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/scheduler.py
+-rw-r--r--   0        0        0     8107 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig.md
+-rw-r--r--   0        0        0     1070 2024-04-08 09:09:43.374110 fbnconfig-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0     8639 1970-01-01 00:00:00.000000 fbnconfig-0.0.37/PKG-INFO
```

### Comparing `fbnconfig-0.0.36/fbnconfig/access.py` & `fbnconfig-0.0.37/fbnconfig/access.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/configuration.py` & `fbnconfig-0.0.37/fbnconfig/configuration.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/deploy.py` & `fbnconfig-0.0.37/fbnconfig/deploy.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/drive.py` & `fbnconfig-0.0.37/fbnconfig/drive.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/identity.py` & `fbnconfig-0.0.37/fbnconfig/identity.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/load_module.py` & `fbnconfig-0.0.37/fbnconfig/load_module.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/log.py` & `fbnconfig-0.0.37/fbnconfig/log.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/main.py` & `fbnconfig-0.0.37/fbnconfig/main.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/resource_abc.py` & `fbnconfig-0.0.37/fbnconfig/resource_abc.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.36/fbnconfig/scheduler.py` & `fbnconfig-0.0.37/fbnconfig/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,16 @@
             raise (RuntimeError("Cannot change identifier on job. Create a new one"))
         self.read(client, old_state)
         remote = copy.deepcopy(self.remote)
         desired = self.model_dump(mode="json", exclude_none=True, exclude={"jobId"})
         effective = remote | desired
         remoteArgs = remote["argumentDefinitions"]
         effectiveArgs = {
-            argKey: remoteArgs[argKey] | argValue
-            for argKey,argValue in desired["argumentDefinitions"].items()
+            argKey: remoteArgs.get(argKey, {}) | argValue
+            for argKey, argValue in desired["argumentDefinitions"].items()
         }
         effective["argumentDefinitions"] = effectiveArgs
         if effective == remote:
             return None
         client.put(f"/scheduler2/api/jobs/{self.scope}/{self.code}", json=desired)
         new_state = JobState(
             id=self.id,
```

### Comparing `fbnconfig-0.0.36/fbnconfig.md` & `fbnconfig-0.0.37/fbnconfig.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # fbnconfig
+[![pypi](https://img.shields.io/pypi/v/fbnconfig)](https://pypi.org/project/fbnconfig/)
+[![python](https://img.shields.io/pypi/pyversions/fbnconfig.svg)](https://pypi.python.org/pypi/fbnconfig)
 
 fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID
 environment setup. It allows you to specify the desired state and, when you deploy, it will converge
 the LUSID env to that state by creating, updating or deleting entities within lusid so that the
 lusid environment and the desired state match.
 
 ## Getting started
```

### Comparing `fbnconfig-0.0.36/pyproject.toml` & `fbnconfig-0.0.37/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbnconfig"
-version = "0.0.36"
+version = "0.0.37"
 description = "fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment"
 authors = ["FINBOURNE Technology <engineering@finbourne.com>"]
 readme = "fbnconfig.md"
 
 [tool.poetry.scripts]
 fbnconfig = 'fbnconfig.main:cli'
```

### Comparing `fbnconfig-0.0.36/PKG-INFO` & `fbnconfig-0.0.37/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: fbnconfig
-Version: 0.0.36
+Version: 0.0.37
 Summary: fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment
 Author: FINBOURNE Technology
 Author-email: engineering@finbourne.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.25.2,<0.26.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # fbnconfig
+[![pypi](https://img.shields.io/pypi/v/fbnconfig)](https://pypi.org/project/fbnconfig/)
+[![python](https://img.shields.io/pypi/pyversions/fbnconfig.svg)](https://pypi.python.org/pypi/fbnconfig)
 
 fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID
 environment setup. It allows you to specify the desired state and, when you deploy, it will converge
 the LUSID env to that state by creating, updating or deleting entities within lusid so that the
 lusid environment and the desired state match.
 
 ## Getting started
```

