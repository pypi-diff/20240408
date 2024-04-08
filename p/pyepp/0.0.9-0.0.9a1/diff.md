# Comparing `tmp/pyepp-0.0.9.tar.gz` & `tmp/pyepp-0.0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepp-0.0.9.tar", last modified: Thu Nov 23 20:36:02 2023, max compression
+gzip compressed data, was "pyepp-0.0.9a1.tar", last modified: Wed Nov 22 01:57:58 2023, max compression
```

## Comparing `pyepp-0.0.9.tar` & `pyepp-0.0.9a1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 20:36:02.671070 pyepp-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-23 20:35:31.000000 pyepp-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2023-11-23 20:36:02.671070 pyepp-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-11-23 20:35:31.000000 pyepp-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 20:36:02.667070 pyepp-0.0.9/pyepp/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/base_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 20:36:02.667070 pyepp-0.0.9/pyepp/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17081 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/command_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)    13488 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/epp.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyepp/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 20:36:02.671070 pyepp-0.0.9/pyepp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-23 20:36:02.000000 pyepp-0.0.9/pyepp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-23 20:35:31.000000 pyepp-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 20:36:02.671070 pyepp-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 20:36:02.671070 pyepp-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_base_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    18250 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-11-23 20:35:31.000000 pyepp-0.0.9/tests/test_pyepp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:58.277645 pyepp-0.0.9a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2023-11-22 01:57:58.277645 pyepp-0.0.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:58.269645 pyepp-0.0.9a1/pyepp/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/base_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:58.273645 pyepp-0.0.9a1/pyepp/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17081 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/command_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13488 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/epp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyepp/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:58.273645 pyepp-0.0.9a1/pyepp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-22 01:57:58.000000 pyepp-0.0.9a1/pyepp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 01:57:58.277645 pyepp-0.0.9a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 01:57:58.273645 pyepp-0.0.9a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_base_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18250 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-11-22 01:57:11.000000 pyepp-0.0.9a1/tests/test_pyepp.py
```

### Comparing `pyepp-0.0.9/LICENSE` & `pyepp-0.0.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/PKG-INFO` & `pyepp-0.0.9a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepp
-Version: 0.0.9
+Version: 0.0.9a1
 Summary: A Python API on top of the EPP protocol.
 Author-email: InternetNZ <ehsan@internetnz.net.nz>
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/InternetNZ/pyepp
 Project-URL: Repository, https://github.com/InternetNZ/pyepp
 Keywords: epp,registry
 Classifier: Programming Language :: Python
```

### Comparing `pyepp-0.0.9/README.md` & `pyepp-0.0.9a1/README.md`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/base_command.py` & `pyepp-0.0.9a1/pyepp/base_command.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/__main__.py` & `pyepp-0.0.9a1/pyepp/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/cli.py` & `pyepp-0.0.9a1/pyepp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/contact.py` & `pyepp-0.0.9a1/pyepp/cli/contact.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/domain.py` & `pyepp-0.0.9a1/pyepp/cli/domain.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/host.py` & `pyepp-0.0.9a1/pyepp/cli/host.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/poll.py` & `pyepp-0.0.9a1/pyepp/cli/poll.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/cli/utils.py` & `pyepp-0.0.9a1/pyepp/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/command_templates.py` & `pyepp-0.0.9a1/pyepp/command_templates.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/contact.py` & `pyepp-0.0.9a1/pyepp/contact.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/domain.py` & `pyepp-0.0.9a1/pyepp/domain.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/epp.py` & `pyepp-0.0.9a1/pyepp/epp.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/helper.py` & `pyepp-0.0.9a1/pyepp/helper.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/host.py` & `pyepp-0.0.9a1/pyepp/host.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp/poll.py` & `pyepp-0.0.9a1/pyepp/poll.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyepp.egg-info/PKG-INFO` & `pyepp-0.0.9a1/pyepp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepp
-Version: 0.0.9
+Version: 0.0.9a1
 Summary: A Python API on top of the EPP protocol.
 Author-email: InternetNZ <ehsan@internetnz.net.nz>
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/InternetNZ/pyepp
 Project-URL: Repository, https://github.com/InternetNZ/pyepp
 Keywords: epp,registry
 Classifier: Programming Language :: Python
```

### Comparing `pyepp-0.0.9/pyepp.egg-info/SOURCES.txt` & `pyepp-0.0.9a1/pyepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/pyproject.toml` & `pyepp-0.0.9a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_base_command.py` & `pyepp-0.0.9a1/tests/test_base_command.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_contact.py` & `pyepp-0.0.9a1/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_domain.py` & `pyepp-0.0.9a1/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_host.py` & `pyepp-0.0.9a1/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_poll.py` & `pyepp-0.0.9a1/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyepp-0.0.9/tests/test_pyepp.py` & `pyepp-0.0.9a1/tests/test_pyepp.py`

 * *Files identical despite different names*

