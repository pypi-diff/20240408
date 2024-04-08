# Comparing `tmp/whiffle_client-0.3.0.tar.gz` & `tmp/whiffle_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.3.0.tar", last modified: Fri Mar  8 10:41:04 2024, max compression
+gzip compressed data, was "whiffle_client-0.3.1.tar", last modified: Mon Apr  8 08:35:39 2024, max compression
```

## Comparing `whiffle_client-0.3.0.tar` & `whiffle_client-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.897558 whiffle_client-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     2951 2024-03-08 10:41:04.897558 whiffle_client-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2231 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 10:41:04.897558 whiffle_client-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.889558 whiffle_client-0.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4791 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.890558 whiffle_client-0.3.0/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.893558 whiffle_client-0.3.0/whiffle_client/analysis/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6719 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/io.py
--rw-rw-rw-   0 root         (0) root         (0)    16419 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     4854 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/scatter.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/skill.py
--rw-rw-rw-   0 root         (0) root         (0)     3231 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/analysis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.894558 whiffle_client-0.3.0/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/resources/example_yaml_include.yaml
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/resources/example_yaml_include_metmasts.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.895558 whiffle_client-0.3.0/whiffle_client/wind/
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10808 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.896558 whiffle_client-0.3.0/whiffle_client/wind/components/
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/components/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/components/geometries.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/components/metmast.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/components/turbine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.896558 whiffle_client-0.3.0/whiffle_client/wind/loaders/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/loaders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-03-08 10:41:01.000000 whiffle_client-0.3.0/whiffle_client/wind/wind_simulation_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 10:41:04.897558 whiffle_client-0.3.0/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2951 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-08 10:41:04.000000 whiffle_client-0.3.0/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     3326 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 08:35:39.320943 whiffle_client-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.312943 whiffle_client-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4791 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.313943 whiffle_client-0.3.1/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.315943 whiffle_client-0.3.1/whiffle_client/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    16419 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     4854 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/scatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4957 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/skill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3231 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/analysis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.316943 whiffle_client-0.3.1/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include_metmasts.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.317943 whiffle_client-0.3.1/whiffle_client/wind/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.318943 whiffle_client-0.3.1/whiffle_client/wind/components/
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/geometries.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/metmast.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/components/turbine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.318943 whiffle_client-0.3.1/whiffle_client/wind/loaders/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/loaders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-08 08:35:36.000000 whiffle_client-0.3.1/whiffle_client/wind/wind_simulation_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 08:35:39.319943 whiffle_client-0.3.1/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3326 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-08 08:35:39.000000 whiffle_client-0.3.1/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.3.0/LICENCE.txt` & `whiffle_client-0.3.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/PKG-INFO` & `whiffle_client-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: click~=8.0.4
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: pyyaml-include~=1.3.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: xarray
-Requires-Dist: netcdf4
-Requires-Dist: matplotlib
-Requires-Dist: hvplot
 Requires-Dist: jupyter
+Provides-Extra: analysis
+Requires-Dist: numpy; extra == "analysis"
+Requires-Dist: pandas; extra == "analysis"
+Requires-Dist: scipy; extra == "analysis"
+Requires-Dist: scikit-learn; extra == "analysis"
+Requires-Dist: xarray; extra == "analysis"
+Requires-Dist: netcdf4; extra == "analysis"
+Requires-Dist: matplotlib; extra == "analysis"
+Requires-Dist: hvplot; extra == "analysis"
 
 # Whiffle client
 
+## Quickstart
+
+`whiffle-client` can be installed with `pip` as follows:
+
+`pip install whiffle-client` or `pip install "whiffle-client[analysis]"` to include data-analysis packages.
+
 This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config edit user.token <your_token>`
 
 You can create a new task by executing,
```

### Comparing `whiffle_client-0.3.0/README.md` & `whiffle_client-0.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Whiffle client
 
+## Installation
+
+`whiffle-client` can be installed with pip in editable mode:
+
+`pip install -e .`
+
+If extra dependencies are needed, they can be installed as follows:
+
+`pip install -e ".[analysis]"`
+
 ## Command line interface
 
 ### List config
 
 `whiffle config-list`
 
 ### Add token to config
```

### Comparing `whiffle_client-0.3.0/USER_README.md` & `whiffle_client-0.3.1/USER_README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Whiffle client
 
+## Quickstart
+
+`whiffle-client` can be installed with `pip` as follows:
+
+`pip install whiffle-client` or `pip install "whiffle-client[analysis]"` to include data-analysis packages.
+
 This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config edit user.token <your_token>`
 
 You can create a new task by executing,
```

### Comparing `whiffle_client-0.3.0/pyproject.toml` & `whiffle_client-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 
 dependencies = [
     "click~=8.0.4",
     "PyYAML~=6.0",
     "pyyaml-include~=1.3.1",
     "platformdirs~=4.0.0",
     "requests",
+    "jupyter"
+]
+
+dynamic = ["version"]
+
+[project.optional-dependencies]
+analysis = [
     "numpy",
     "pandas",
     "scipy",
     "scikit-learn",
     "xarray",
     "netcdf4",
     "matplotlib",
-    "hvplot",
-    "jupyter"
+    "hvplot"
 ]
 
-dynamic = ["version"]
+[project.scripts]
+whiffle = "whiffle_client.entrypoints:whiffle"
 
 [tool.setuptools]
 package-dir = {"whiffle_client" = "whiffle_client"}
 
-[project.scripts]
-whiffle = "whiffle_client.entrypoints:whiffle"
-
 [tool.setuptools.package-data]
 whiffle_client = [
     "resources/whiffle_config.yaml", 
     "resources/example_generic_params.json", 
     "resources/example_yaml_include.yaml",
     "resources/example_yaml_include_metmasts.yaml",
     ]
```

### Comparing `whiffle_client-0.3.0/tests/test_client.py` & `whiffle_client-0.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/analysis/io.py` & `whiffle_client-0.3.1/whiffle_client/analysis/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/analysis/plot.py` & `whiffle_client-0.3.1/whiffle_client/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/analysis/scatter.py` & `whiffle_client-0.3.1/whiffle_client/analysis/scatter.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/analysis/skill.py` & `whiffle_client-0.3.1/whiffle_client/analysis/skill.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/analysis/utils.py` & `whiffle_client-0.3.1/whiffle_client/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/client.py` & `whiffle_client-0.3.1/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/entrypoints.py` & `whiffle_client-0.3.1/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/io.py` & `whiffle_client-0.3.1/whiffle_client/io.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.3.1/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/resources/example_yaml_include.yaml` & `whiffle_client-0.3.1/whiffle_client/resources/example_yaml_include.yaml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/wind/client.py` & `whiffle_client-0.3.1/whiffle_client/wind/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/wind/loaders/csv.py` & `whiffle_client-0.3.1/whiffle_client/wind/loaders/csv.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client/wind/wind_simulation_task.py` & `whiffle_client-0.3.1/whiffle_client/wind/wind_simulation_task.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.3.0/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.3.1/whiffle_client.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: click~=8.0.4
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: pyyaml-include~=1.3.1
 Requires-Dist: platformdirs~=4.0.0
 Requires-Dist: requests
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: xarray
-Requires-Dist: netcdf4
-Requires-Dist: matplotlib
-Requires-Dist: hvplot
 Requires-Dist: jupyter
+Provides-Extra: analysis
+Requires-Dist: numpy; extra == "analysis"
+Requires-Dist: pandas; extra == "analysis"
+Requires-Dist: scipy; extra == "analysis"
+Requires-Dist: scikit-learn; extra == "analysis"
+Requires-Dist: xarray; extra == "analysis"
+Requires-Dist: netcdf4; extra == "analysis"
+Requires-Dist: matplotlib; extra == "analysis"
+Requires-Dist: hvplot; extra == "analysis"
 
 # Whiffle client
 
+## Quickstart
+
+`whiffle-client` can be installed with `pip` as follows:
+
+`pip install whiffle-client` or `pip install "whiffle-client[analysis]"` to include data-analysis packages.
+
 This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config edit user.token <your_token>`
 
 You can create a new task by executing,
```

### Comparing `whiffle_client-0.3.0/whiffle_client.egg-info/SOURCES.txt` & `whiffle_client-0.3.1/whiffle_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

