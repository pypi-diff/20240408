# Comparing `tmp/shipyard_dbt-0.1.0.tar.gz` & `tmp/shipyard_dbt-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_dbt-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_dbt-0.2.0a0.tar", max compression
```

## Comparing `shipyard_dbt-0.1.0.tar` & `shipyard_dbt-0.2.0a0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-26 19:00:30.084274 shipyard_dbt-0.1.0/README.md
--rw-r--r--   0        0        0      549 2024-01-11 15:13:25.668154 shipyard_dbt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-26 19:00:30.085016 shipyard_dbt-0.1.0/shipyard_dbt/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434381 shipyard_dbt-0.1.0/shipyard_dbt/cli/__init__.py
--rw-r--r--   0        0        0      258 2024-02-05 20:53:35.434728 shipyard_dbt-0.1.0/shipyard_dbt/cli/authtest.py
--rw-r--r--   0        0        0     4727 2024-01-11 15:13:25.668281 shipyard_dbt-0.1.0/shipyard_dbt/cli/check_run_status.py
--rw-r--r--   0        0        0     7881 2024-01-11 15:13:25.668393 shipyard_dbt-0.1.0/shipyard_dbt/cli/download_logs_artifacts.py
--rw-r--r--   0        0        0     6649 2024-01-11 15:13:25.668493 shipyard_dbt-0.1.0/shipyard_dbt/cli/execute_job.py
--rw-r--r--   0        0        0     2260 2024-01-11 15:13:25.668574 shipyard_dbt-0.1.0/shipyard_dbt/cli/http_blueprints.py
--rw-r--r--   0        0        0     1204 2023-08-09 00:44:22.122119 shipyard_dbt-0.1.0/shipyard_dbt/dbt.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 shipyard_dbt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 19:00:30.084274 shipyard_dbt-0.2.0a0/README.md
+-rw-r--r--   0        0        0      573 2024-04-08 13:47:30.900177 shipyard_dbt-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-26 19:00:30.085016 shipyard_dbt-0.2.0a0/shipyard_dbt/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434381 shipyard_dbt-0.2.0a0/shipyard_dbt/cli/__init__.py
+-rw-r--r--   0        0        0      273 2024-04-04 19:39:49.110800 shipyard_dbt-0.2.0a0/shipyard_dbt/cli/authtest.py
+-rw-r--r--   0        0        0     3512 2024-04-04 19:39:49.111312 shipyard_dbt-0.2.0a0/shipyard_dbt/cli/download_logs_artifacts.py
+-rw-r--r--   0        0        0     4697 2024-04-04 19:39:49.111722 shipyard_dbt-0.2.0a0/shipyard_dbt/cli/trigger_and_download.py
+-rw-r--r--   0        0        0     2200 2024-04-04 19:39:49.111973 shipyard_dbt-0.2.0a0/shipyard_dbt/cli/trigger_job.py
+-rw-r--r--   0        0        0     7239 2024-04-04 19:39:49.112445 shipyard_dbt-0.2.0a0/shipyard_dbt/dbt.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 shipyard_dbt-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_dbt-0.1.0/PKG-INFO` & `shipyard_dbt-0.2.0a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: shipyard-dbt
-Version: 0.1.0
+Version: 0.2.0a0
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: shipyard-templates (==0.5.0a0)
-Requires-Dist: shipyard-utils (>=0.1.4,<0.2.0)
+Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
+Requires-Dist: shipyard-templates (==0.8.2a0)
 Description-Content-Type: text/markdown
```

