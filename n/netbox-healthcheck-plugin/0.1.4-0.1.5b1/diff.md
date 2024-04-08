# Comparing `tmp/netbox-healthcheck-plugin-0.1.4.tar.gz` & `tmp/netbox-healthcheck-plugin-0.1.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-healthcheck-plugin-0.1.4.tar", last modified: Mon Apr  8 18:00:06 2024, max compression
+gzip compressed data, was "netbox-healthcheck-plugin-0.1.5b1.tar", last modified: Mon Apr  8 18:58:43 2024, max compression
```

## Comparing `netbox-healthcheck-plugin-0.1.4.tar` & `netbox-healthcheck-plugin-0.1.5b1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.653684 netbox-healthcheck-plugin-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-08 18:00:06.653684 netbox-healthcheck-plugin-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.649685 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.649685 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.649685 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.649685 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-08 18:00:06.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 18:00:06.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:00:06.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 18:00:06.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:00:06.000000 netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:00:06.653684 netbox-healthcheck-plugin-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:00:06.649685 netbox-healthcheck-plugin-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 18:00:02.000000 netbox-healthcheck-plugin-0.1.4/tests/test_netbox_healthcheck_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 18:58:43.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 18:58:42.000000 netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:58:43.014374 netbox-healthcheck-plugin-0.1.5b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:58:43.010374 netbox-healthcheck-plugin-0.1.5b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 18:58:38.000000 netbox-healthcheck-plugin-0.1.5b1/tests/test_netbox_healthcheck_plugin.py
```

### Comparing `netbox-healthcheck-plugin-0.1.4/CONTRIBUTING.md` & `netbox-healthcheck-plugin-0.1.5b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.4/LICENSE` & `netbox-healthcheck-plugin-0.1.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.4/PKG-INFO` & `netbox-healthcheck-plugin-0.1.5b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.4
+Version: 0.1.5b1
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 # NetBox HealthCheck Plugin
 
 NetBox plugin for HealthCheck.
 
 NetBox provides health check monitors that can be queried to make sure that the service is running in good condition.  
 
-NetBox exposes metrics at the `/healthcheck` HTTP endpoint, e.g. `https://netbox.local/healthcheck`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
+NetBox exposes metrics at the `/healthcheck` HTTP endpoint under the plugin, e.g. `https://netbox.local/plugins/netbox_healthcheck_plugin/healthcheck/`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
 
 * Free software: Apache-2.0
 * Documentation: https://netbox-community.github.io/netbox-healthcheck-plugin/
 
 
 ## Features
```

### Comparing `netbox-healthcheck-plugin-0.1.4/README.md` & `netbox-healthcheck-plugin-0.1.5b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # NetBox HealthCheck Plugin
 
 NetBox plugin for HealthCheck.
 
 NetBox provides health check monitors that can be queried to make sure that the service is running in good condition.  
 
-NetBox exposes metrics at the `/healthcheck` HTTP endpoint, e.g. `https://netbox.local/healthcheck`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
+NetBox exposes metrics at the `/healthcheck` HTTP endpoint under the plugin, e.g. `https://netbox.local/plugins/netbox_healthcheck_plugin/healthcheck/`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
 
 * Free software: Apache-2.0
 * Documentation: https://netbox-community.github.io/netbox-healthcheck-plugin/
 
 
 ## Features
```

### Comparing `netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/__init__.py` & `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Top-level package for NetBox HealthCheck Plugin."""
 
 __author__ = """Arthur Hanson"""
 __email__ = 'ahanson@netboxlabs.com'
-__version__ = '0.1.4'
+__version__ = '0.1.5b1'
 
 
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 
 
 class HealthCheckConfig(PluginConfig):
     name = 'netbox_healthcheck_plugin'
     verbose_name = 'NetBox HealthCheck Plugin'
     description = 'NetBox plugin for HealthCheck.'
     version = 'version'
     base_url = 'netbox_healthcheck_plugin'
     django_apps = [
         'health_check',
         'health_check.db',
         'health_check.contrib.migrations',
         'health_check.contrib.redis',
     ]
-
+    min_version = "v4.0-beta1"
 
 config = HealthCheckConfig
```

### Comparing `netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html` & `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin/templates/netbox_healthcheck_plugin/healthcheck.html`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/PKG-INFO` & `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-healthcheck-plugin
-Version: 0.1.4
+Version: 0.1.5b1
 Summary: NetBox plugin for HealthCheck.
 Author-email: Arthur Hanson <ahanson@netboxlabs.com>
 Project-URL: Documentation, https://github.com/netbox-community/netbox-healthcheck-plugin/blob/main/README.md
 Project-URL: Source, https://github.com/netbox-community/netbox-healthcheck-plugin
 Project-URL: Tracker, https://github.com/netbox-community/netbox-healthcheck-plugin/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 # NetBox HealthCheck Plugin
 
 NetBox plugin for HealthCheck.
 
 NetBox provides health check monitors that can be queried to make sure that the service is running in good condition.  
 
-NetBox exposes metrics at the `/healthcheck` HTTP endpoint, e.g. `https://netbox.local/healthcheck`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
+NetBox exposes metrics at the `/healthcheck` HTTP endpoint under the plugin, e.g. `https://netbox.local/plugins/netbox_healthcheck_plugin/healthcheck/`. It allows monitor conditions via HTTP(S), with responses available in HTML and JSON formats.
 
 * Free software: Apache-2.0
 * Documentation: https://netbox-community.github.io/netbox-healthcheck-plugin/
 
 
 ## Features
```

### Comparing `netbox-healthcheck-plugin-0.1.4/netbox_healthcheck_plugin.egg-info/SOURCES.txt` & `netbox-healthcheck-plugin-0.1.5b1/netbox_healthcheck_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-healthcheck-plugin-0.1.4/pyproject.toml` & `netbox-healthcheck-plugin-0.1.5b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name =  "netbox-healthcheck-plugin"
-version = "0.1.4"
+version = "0.1.5b1"
 authors = [
     {name = "Arthur Hanson", email = "ahanson@netboxlabs.com"},
 ]
 description = "NetBox plugin for HealthCheck."
 readme = "README.md"
 
 classifiers=[
```

