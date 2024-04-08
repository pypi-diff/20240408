# Comparing `tmp/netbox-healthcheck-plugin-0.1.2.tar.gz` & `tmp/netbox-healthcheck-plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-healthcheck-plugin-0.1.2.tar", last modified: Fri Apr  5 22:44:18 2024, max compression
+gzip compressed data, was "netbox-healthcheck-plugin-0.1.3.tar", last modified: Mon Apr  8 17:14:15 2024, max compression
```

## Comparing `netbox-healthcheck-plugin-0.1.2.tar` & `netbox-healthcheck-plugin-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:44:18.414945 netbox-healthcheck-plugin-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-05 22:44:18.414945 netbox-healthcheck-plugin-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:44:18.410945 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:44:18.410945 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-05 22:44:18.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-05 22:44:18.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:44:18.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 22:44:18.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 22:44:18.000000 netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:44:18.414945 netbox-healthcheck-plugin-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:44:18.410945 netbox-healthcheck-plugin-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 22:44:14.000000 netbox-healthcheck-plugin-0.1.2/tests/test_netbox_healthcheck_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:15.221078 netbox-healthcheck-plugin-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-08 17:14:15.221078 netbox-healthcheck-plugin-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:15.217078 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:15.217078 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-08 17:14:15.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-08 17:14:15.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:14:15.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 17:14:15.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 17:14:15.000000 netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:14:15.221078 netbox-healthcheck-plugin-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:14:15.217078 netbox-healthcheck-plugin-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 17:14:08.000000 netbox-healthcheck-plugin-0.1.3/tests/test_netbox_healthcheck_plugin.py
```

### Comparing `netbox-healthcheck-plugin-0.1.2/CONTRIBUTING.md` & `netbox-healthcheck-plugin-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.2/LICENSE` & `netbox-healthcheck-plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.2/PKG-INFO` & `netbox-healthcheck-plugin-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django-health-check<4,>=3
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: flake8-pyproject; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
@@ -43,14 +44,15 @@
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
+|   3.4 - 3.7    |      0.1.3     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.2/README.md` & `netbox-healthcheck-plugin-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
+|   3.4 - 3.7    |      0.1.3     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin/__init__.py` & `netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for NetBox HealthCheck Plugin."""
 
 __author__ = """Arthur Hanson"""
 __email__ = 'ahanson@netboxlabs.com'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 
 from extras.plugins import PluginConfig
 
 
 class HealthCheckConfig(PluginConfig):
     name = 'netbox_healthcheck_plugin'
```

### Comparing `netbox-healthcheck-plugin-0.1.2/netbox_healthcheck_plugin.egg-info/PKG-INFO` & `netbox-healthcheck-plugin-0.1.3/netbox_healthcheck_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django-health-check<4,>=3
 Provides-Extra: test
 Requires-Dist: black==24.3.0; extra == "test"
 Requires-Dist: check-manifest==0.49; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: flake8-pyproject; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
@@ -43,14 +44,15 @@
 
 ## Compatibility
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
 |   3.4 - 3.7    |      0.1.0     |
 |   3.4 - 3.7    |      0.1.2     |
+|   3.4 - 3.7    |      0.1.3     |
 
 ## Installing
 
 For adding to a NetBox Docker setup see
 [the general instructions for using netbox-docker with plugins](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins).
 
 While this is still in development and not yet on pypi you can install with pip:
```

### Comparing `netbox-healthcheck-plugin-0.1.2/pyproject.toml` & `netbox-healthcheck-plugin-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-healthcheck-plugin"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for HealthCheck."
 readme = "README.md"
 
 classifiers=[
@@ -23,14 +23,18 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 requires-python = ">=3.8.1"
 
+dependencies = [
+    'django-health-check >= 3,<4'
+]
+
 [project.optional-dependencies]
 test = [
     "black==24.3.0",
     "check-manifest==0.49",
     "flake8",
     "flake8-pyproject",
     "pre-commit==3.7.0",
```

