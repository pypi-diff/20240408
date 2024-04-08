# Comparing `tmp/pulumi_venafi-1.8.0a1711781679.tar.gz` & `tmp/pulumi_venafi-1.8.0a1712403151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.8.0a1711781679.tar", last modified: Sat Mar 30 06:56:34 2024, max compression
+gzip compressed data, was "pulumi_venafi-1.8.0a1712403151.tar", last modified: Sat Apr  6 11:38:17 2024, max compression
```

## Comparing `pulumi_venafi-1.8.0a1711781679.tar` & `pulumi_venafi-1.8.0a1712403151.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    48936 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21014 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53759 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-03-30 06:56:34.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-30 06:56:34.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:56:34.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 06:56:34.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 06:56:34.000000 pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-30 06:56:28.000000 pulumi_venafi-1.8.0a1711781679/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 06:56:34.776667 pulumi_venafi-1.8.0a1711781679/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48936 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21014 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53759 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 11:38:17.000000 pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-06 11:38:09.000000 pulumi_venafi-1.8.0a1712403151/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:38:17.034040 pulumi_venafi-1.8.0a1712403151/setup.cfg
```

### Comparing `pulumi_venafi-1.8.0a1711781679/PKG-INFO` & `pulumi_venafi-1.8.0a1712403151/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.8.0a1711781679
+Version: 1.8.0a1712403151
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.8.0a1711781679/README.md` & `pulumi_venafi-1.8.0a1712403151/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/__init__.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/certificate.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/__init__.pyi` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/policy.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/provider.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.8.0a1711781679
+Version: 1.8.0a1712403151
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi,venafi
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.8.0a1711781679/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.8.0a1712403151/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.8.0a1711781679/pyproject.toml` & `pulumi_venafi-1.8.0a1712403151/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_venafi"
   description = "A Pulumi package for creating and managing venafi cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "venafi"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.8.0a1711781679"
+  version = "1.8.0a1712403151"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-venafi"
 
 [build-system]
```

