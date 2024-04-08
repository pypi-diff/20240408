# Comparing `tmp/stock-hexagonal-app-0.0.0.tar.gz` & `tmp/stock-hexagonal-app-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock-hexagonal-app-0.0.0.tar", last modified: Sun Apr  7 16:19:36 2024, max compression
+gzip compressed data, was "stock-hexagonal-app-0.1.3.tar", last modified: Mon Apr  8 06:18:01 2024, max compression
```

## Comparing `stock-hexagonal-app-0.0.0.tar` & `stock-hexagonal-app-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.914379 stock-hexagonal-app-0.0.0/
--rw-r--r--   0 macuj      (502) staff       (20)       58 2024-04-07 07:05:10.000000 stock-hexagonal-app-0.0.0/.gitattributes
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.900565 stock-hexagonal-app-0.0.0/.github/
--rw-r--r--   0 macuj      (502) staff       (20)       20 2024-04-06 05:56:05.000000 stock-hexagonal-app-0.0.0/.github/CODEOWNERS
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.901264 stock-hexagonal-app-0.0.0/.github/workflows/
--rw-r--r--   0 macuj      (502) staff       (20)      527 2024-04-07 07:06:21.000000 stock-hexagonal-app-0.0.0/.github/workflows/qa.yml
--rw-r--r--   0 macuj      (502) staff       (20)       28 2024-04-07 15:45:55.000000 stock-hexagonal-app-0.0.0/.gitignore
--rw-r--r--   0 macuj      (502) staff       (20)     1038 2024-04-06 10:11:55.000000 stock-hexagonal-app-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 macuj      (502) staff       (20)        5 2024-04-07 07:05:10.000000 stock-hexagonal-app-0.0.0/CHANGELOG.md
--rw-r--r--   0 macuj      (502) staff       (20)      929 2024-04-07 16:19:28.000000 stock-hexagonal-app-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 macuj      (502) staff       (20)     1064 2024-04-07 07:05:10.000000 stock-hexagonal-app-0.0.0/LICENSE
--rw-r--r--   0 macuj      (502) staff       (20)     2378 2024-04-07 16:19:36.913740 stock-hexagonal-app-0.0.0/PKG-INFO
--rw-r--r--   0 macuj      (502) staff       (20)      532 2024-04-06 10:16:12.000000 stock-hexagonal-app-0.0.0/README.md
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.901752 stock-hexagonal-app-0.0.0/docs/
--rw-r--r--   0 macuj      (502) staff       (20)       19 2024-04-07 07:05:10.000000 stock-hexagonal-app-0.0.0/docs/index.md
--rw-r--r--   0 macuj      (502) staff       (20)      244 2024-04-07 07:05:10.000000 stock-hexagonal-app-0.0.0/mkdocs.yml
--rw-r--r--   0 macuj      (502) staff       (20)      905 2024-04-07 16:19:23.000000 stock-hexagonal-app-0.0.0/pyproject.toml
--rw-r--r--   0 macuj      (502) staff       (20)       52 2024-04-06 06:13:22.000000 stock-hexagonal-app-0.0.0/requirements-dev.txt
--rw-r--r--   0 macuj      (502) staff       (20)       14 2024-04-06 14:15:25.000000 stock-hexagonal-app-0.0.0/requirements.txt
--rw-r--r--   0 macuj      (502) staff       (20)       38 2024-04-07 16:19:36.914469 stock-hexagonal-app-0.0.0/setup.cfg
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.902256 stock-hexagonal-app-0.0.0/src/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 14:05:01.000000 stock-hexagonal-app-0.0.0/src/__init__.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.903180 stock-hexagonal-app-0.0.0/src/adapters/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:17:38.000000 stock-hexagonal-app-0.0.0/src/adapters/__init__.py
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 05:10:44.000000 stock-hexagonal-app-0.0.0/src/adapters/alpha_vantage_adapter.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.904504 stock-hexagonal-app-0.0.0/src/domain/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:17:34.000000 stock-hexagonal-app-0.0.0/src/domain/__init__.py
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 05:12:06.000000 stock-hexagonal-app-0.0.0/src/domain/prepare_data.py
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 05:12:16.000000 stock-hexagonal-app-0.0.0/src/domain/statistics.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.905605 stock-hexagonal-app-0.0.0/src/entrypoints/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:52:05.000000 stock-hexagonal-app-0.0.0/src/entrypoints/__init__.py
--rw-r--r--   0 macuj      (502) staff       (20)     1437 2024-04-07 15:50:00.000000 stock-hexagonal-app-0.0.0/src/entrypoints/cli_entrypoint.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.906759 stock-hexagonal-app-0.0.0/src/helpers/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:54:23.000000 stock-hexagonal-app-0.0.0/src/helpers/__init__.py
--rw-r--r--   0 macuj      (502) staff       (20)      307 2024-04-07 15:50:08.000000 stock-hexagonal-app-0.0.0/src/helpers/logger.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.907838 stock-hexagonal-app-0.0.0/src/ports/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:17:52.000000 stock-hexagonal-app-0.0.0/src/ports/__init__.py
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 14:01:15.000000 stock-hexagonal-app-0.0.0/src/ports/stock_data_provider.py
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.912305 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/
--rw-r--r--   0 macuj      (502) staff       (20)     2378 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/PKG-INFO
--rw-r--r--   0 macuj      (502) staff       (20)      837 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/SOURCES.txt
--rw-r--r--   0 macuj      (502) staff       (20)        1 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/dependency_links.txt
--rw-r--r--   0 macuj      (502) staff       (20)       65 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/entry_points.txt
--rw-r--r--   0 macuj      (502) staff       (20)       83 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/requires.txt
--rw-r--r--   0 macuj      (502) staff       (20)       42 2024-04-07 16:19:36.000000 stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/top_level.txt
-drwxr-xr-x   0 macuj      (502) staff       (20)        0 2024-04-07 16:19:36.911527 stock-hexagonal-app-0.0.0/tests/
--rw-r--r--   0 macuj      (502) staff       (20)        0 2024-04-06 10:17:46.000000 stock-hexagonal-app-0.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.084722 stock-hexagonal-app-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.github/workflows/qa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-08 06:18:01.084722 stock-hexagonal-app-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:18:01.084722 stock-hexagonal-app-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/adapters/alpha_vantage_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/domain/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/domain/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/entrypoints/cli_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/helpers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/src/ports/stock_data_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-08 06:18:01.000000 stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:18:01.080722 stock-hexagonal-app-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:17:40.000000 stock-hexagonal-app-0.1.3/tests/__init__.py
```

### Comparing `stock-hexagonal-app-0.0.0/.github/workflows/qa.yml` & `stock-hexagonal-app-0.1.3/.github/workflows/qa.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: quality-assurance
 
 on:
   push:
 
 jobs:
-  pre-commit:
+  qa:
     runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v4
 
 # Instead of setup Python and pip install there should be Docker container pulled with preinstalled deps
       - name: Set up Python
```

### Comparing `stock-hexagonal-app-0.0.0/.pre-commit-config.yaml` & `stock-hexagonal-app-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.0.0/CONTRIBUTING.md` & `stock-hexagonal-app-0.1.3/CONTRIBUTING.md`

 * *Files 20% similar despite different names*

```diff
@@ -34,20 +34,35 @@
 
 ## Install package in development mode
 
 ```sh
 python -m pip install --editable .
 ```
 
-## Build package source and built distribution
+## Build package source (.tar.gz) and built (.whl) distribution
 
 ```sh
 python -m build
 ```
 
+## Upload package discribution to pypi
+
+```sh
+export TWINE_USERNAME=__token__
+export TWINE_PASSWORD=<my-twine-api-token>
+twine upload dist/*
+```
+
+## New git tag
+
+```sh
+git tag -a <version> -m <message>
+git push origin <tag-version>
+```
+
 ## Run CLI app
 
 ```sh
 stock-cli-app --help
 ```
 
 ## Run pre-commit
```

### Comparing `stock-hexagonal-app-0.0.0/LICENSE` & `stock-hexagonal-app-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.0.0/PKG-INFO` & `stock-hexagonal-app-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-hexagonal-app
-Version: 0.0.0
+Version: 0.1.3
 Summary: Python tool for analyzing stock data build on hexagonal architecture.
 Author-email: Jeremiasz Macura <jeremiaszmacura99@gmail.com>
 License: Copyright 2024 Jeremiasz Macura
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,14 +20,15 @@
 License-File: LICENSE
 Requires-Dist: typer==0.12.1
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Provides-Extra: qa
 Requires-Dist: pre-commit==3.7.0; extra == "qa"
 Provides-Extra: upload
+Requires-Dist: build==1.2.1; extra == "upload"
 Requires-Dist: twine==5.0.0; extra == "upload"
 
 # Python CLI tool to analyze stock data
 
 ## Hexagonal Architecture
 
 This tool is build using hexagonal architecture with following structure
```

### Comparing `stock-hexagonal-app-0.0.0/README.md` & `stock-hexagonal-app-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.0.0/pyproject.toml` & `stock-hexagonal-app-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
+version = "0.1.3"
 name = "stock-hexagonal-app"
 authors = [
     {name = "Jeremiasz Macura", email = "jeremiaszmacura99@gmail.com"},
 ]
 description = "Python tool for analyzing stock data build on hexagonal architecture."
 readme = "README.md"
 requires-python = ">=3.11"
-dynamic = ["version"]
 keywords = ["analyze", "stock", "hexagonal architecture"]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -26,15 +26,16 @@
 docs = [
     "mkdocs==1.5.3",
 ]
 qa = [
     "pre-commit==3.7.0",
 ]
 upload = [
-    "twine==5.0.0"
+    "build==1.2.1",
+    "twine==5.0.0",
 ]
 
 [project.scripts]
 stock-cli-app = "entrypoints.cli_entrypoint:app"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `stock-hexagonal-app-0.0.0/src/entrypoints/cli_entrypoint.py` & `stock-hexagonal-app-0.1.3/src/entrypoints/cli_entrypoint.py`

 * *Files identical despite different names*

### Comparing `stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/PKG-INFO` & `stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-hexagonal-app
-Version: 0.0.0
+Version: 0.1.3
 Summary: Python tool for analyzing stock data build on hexagonal architecture.
 Author-email: Jeremiasz Macura <jeremiaszmacura99@gmail.com>
 License: Copyright 2024 Jeremiasz Macura
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,14 +20,15 @@
 License-File: LICENSE
 Requires-Dist: typer==0.12.1
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Provides-Extra: qa
 Requires-Dist: pre-commit==3.7.0; extra == "qa"
 Provides-Extra: upload
+Requires-Dist: build==1.2.1; extra == "upload"
 Requires-Dist: twine==5.0.0; extra == "upload"
 
 # Python CLI tool to analyze stock data
 
 ## Hexagonal Architecture
 
 This tool is build using hexagonal architecture with following structure
```

### Comparing `stock-hexagonal-app-0.0.0/src/stock_hexagonal_app.egg-info/SOURCES.txt` & `stock-hexagonal-app-0.1.3/src/stock_hexagonal_app.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 README.md
 mkdocs.yml
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 .github/CODEOWNERS
 .github/workflows/qa.yml
+.github/workflows/release.yml
 docs/index.md
 src/__init__.py
 src/adapters/__init__.py
 src/adapters/alpha_vantage_adapter.py
 src/domain/__init__.py
 src/domain/prepare_data.py
 src/domain/statistics.py
```

