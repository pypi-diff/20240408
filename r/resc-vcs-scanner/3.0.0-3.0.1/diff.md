# Comparing `tmp/resc_vcs_scanner-3.0.0.tar.gz` & `tmp/resc_vcs_scanner-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-3.0.0.tar", last modified: Fri Feb  2 13:50:53 2024, max compression
+gzip compressed data, was "resc_vcs_scanner-3.0.1.tar", last modified: Mon Apr  8 09:39:32 2024, max compression
```

## Comparing `resc_vcs_scanner-3.0.0.tar` & `resc_vcs_scanner-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.517729 resc_vcs_scanner-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-02 13:50:44.000000 resc_vcs_scanner-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-02 13:50:53.517729 resc_vcs_scanner-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-02-02 13:50:44.000000 resc_vcs_scanner-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-02 13:50:53.517729 resc_vcs_scanner-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.509729 resc_vcs_scanner-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.513729 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-02 13:50:53.000000 resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.513729 resc_vcs_scanner-3.0.0/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.513729 resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/output_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.513729 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14972 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/ignore_list_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/secret_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/stdout_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:50:53.513729 resc_vcs_scanner-3.0.0/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-02 13:50:45.000000 resc_vcs_scanner-3.0.0/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 09:39:32.000000 resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.101249 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/ignore_list_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/secret_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:39:32.105249 resc_vcs_scanner-3.0.1/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 09:39:27.000000 resc_vcs_scanner-3.0.1/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.0.0/LICENSE.md` & `resc_vcs_scanner-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/PKG-INFO` & `resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 Metadata-Version: 2.1
-Name: resc_vcs_scanner
-Version: 3.0.0
+Name: resc-vcs-scanner
+Version: 3.0.1
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
-Download-URL: 
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: celery==5.3.1
-Requires-Dist: amqp==5.1.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: typing==3.7.4.3
-Requires-Dist: pydantic==1.8.2
-Requires-Dist: GitPython==3.1.32
-Requires-Dist: resc-backend>=3.0.0
-Requires-Dist: tenacity==8.2.2
-Requires-Dist: prettytable==3.8.0
-Requires-Dist: termcolor==2.3.0
-Requires-Dist: tomlkit==0.12.1
 
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
 [![Gitleaks][gitleaks-shield]][gitleaks-url]
 [![CI][ci-shield]][ci-url]
 [![SonarCloud][sonar-cloud-shield]][sonar-cloud-url]
 
+> [!NOTE]  
+> ## This component is part of Repository Scanner - [resc](https://github.com/abnamro/repository-scanner)
+
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Run locally from source](#run-locally-from-source)
     - [Run locally using docker](#run-locally-using-docker)
@@ -269,7 +262,8 @@
 [pydantic-url]: https://docs.pydantic.dev
 [gitleaks-shield]: https://img.shields.io/badge/Gitleaks-121013?logo=github&logoColor=white
 [gitleaks-url]: https://github.com/zricethezav/gitleaks
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/vcs-scanner-ci.yaml?logo=github
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/vcs-scanner-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-vcs-scanner&metric=alert_status
 [sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
+
```

### Comparing `resc_vcs_scanner-3.0.0/README.md` & `resc_vcs_scanner-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: resc_vcs_scanner
+Version: 3.0.1
+Summary: Repository Scanner - Version Control System - Scanner
+Home-page: https://github.com/ABNAMRO/repository-scanner
+Author: ABN AMRO
+Author-email: resc@nl.abnamro.com
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # Repository Scanner Version Control System Scanner (RESC-VCS-SCANNER)
 [![Python][python-shield]][python-url]
 [![Celery][celery-shield]][celery-url]
 [![Pydantic][pydantic-shield]][pydantic-url]
 [![Gitleaks][gitleaks-shield]][gitleaks-url]
 [![CI][ci-shield]][ci-url]
 [![SonarCloud][sonar-cloud-shield]][sonar-cloud-url]
 
+> [!NOTE]  
+> ## This component is part of Repository Scanner - [resc](https://github.com/abnamro/repository-scanner)
+
 <!-- TABLE OF CONTENTS -->
 ## Table of contents
 1. [About the component](#about-the-component)
 2. [Getting started](#getting-started)
     - [Prerequisites](#prerequisites)
     - [Run locally from source](#run-locally-from-source)
     - [Run locally using docker](#run-locally-using-docker)
@@ -245,8 +261,9 @@
 [pydantic-shield]: https://img.shields.io/badge/Pydantic-e92063.svg?logo=pydantic&style=flat
 [pydantic-url]: https://docs.pydantic.dev
 [gitleaks-shield]: https://img.shields.io/badge/Gitleaks-121013?logo=github&logoColor=white
 [gitleaks-url]: https://github.com/zricethezav/gitleaks
 [ci-shield]: https://img.shields.io/github/actions/workflow/status/abnamro/repository-scanner/vcs-scanner-ci.yaml?logo=github
 [ci-url]: https://github.com/abnamro/repository-scanner/actions/workflows/vcs-scanner-ci.yaml
 [sonar-cloud-shield]: https://sonarcloud.io/api/project_badges/measure?project=abnamro-resc_resc-vcs-scanner&metric=alert_status
-[sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
+[sonar-cloud-url]: https://sonarcloud.io/summary/new_code?id=abnamro-resc_resc-vcs-scanner
+
```

### Comparing `resc_vcs_scanner-3.0.0/setup.cfg` & `resc_vcs_scanner-3.0.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 3.0.0
+version = 3.0.1
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.md
+requirements_files = file: requirements.txt
 
 [options]
 python_requires = >=3.9
-install_requires = 
-	celery==5.3.1
-	amqp==5.1.1
-	requests==2.31.0
-	typing==3.7.4.3
-	pydantic==1.8.2
-	GitPython==3.1.32
-	resc-backend>=3.0.0
-	tenacity==8.2.2
-	prettytable==3.8.0
-	termcolor==2.3.0
-	tomlkit==0.12.1
 include_package_data = False
 zip_safe = False
 package_dir = = src
 packages = find:
 
 [options.packages.find]
 where = src
```

### Comparing `resc_vcs_scanner-3.0.0/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-3.0.1/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 LICENSE.md
-README.md
+requirements.txt
 setup.cfg
 setup.py
 src/resc_vcs_scanner.egg-info/PKG-INFO
 src/resc_vcs_scanner.egg-info/SOURCES.txt
 src/resc_vcs_scanner.egg-info/dependency_links.txt
 src/resc_vcs_scanner.egg-info/entry_points.txt
 src/resc_vcs_scanner.egg-info/not-zip-safe
 src/resc_vcs_scanner.egg-info/requires.txt
 src/resc_vcs_scanner.egg-info/top_level.txt
 src/vcs_scanner/__init__.py
 src/vcs_scanner/common.py
 src/vcs_scanner/constants.py
 src/vcs_scanner/input_parser.py
 src/vcs_scanner/model.py
-src/vcs_scanner/output_module.py
 src/vcs_scanner/resc_worker.py
 src/vcs_scanner/helpers/__init__.py
 src/vcs_scanner/helpers/env_default.py
 src/vcs_scanner/helpers/environment_wrapper.py
 src/vcs_scanner/helpers/finding_action.py
+src/vcs_scanner/helpers/finding_filter.py
+src/vcs_scanner/helpers/ignore_list_provider.py
 src/vcs_scanner/secret_scanners/__init__.py
 src/vcs_scanner/secret_scanners/celery_worker.py
 src/vcs_scanner/secret_scanners/cli.py
 src/vcs_scanner/secret_scanners/configuration.py
 src/vcs_scanner/secret_scanners/git_operation.py
 src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
-src/vcs_scanner/secret_scanners/ignore_list_provider.py
-src/vcs_scanner/secret_scanners/rws_api_writer.py
 src/vcs_scanner/secret_scanners/secret_scanner.py
-src/vcs_scanner/secret_scanners/stdout_writer.py
 src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/common.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/model.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/model.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 from resc_backend.resc_web_service.schema.repository import Repository
 
 # First Party
 from vcs_scanner.common import initialise_logs, load_vcs_instances
 from vcs_scanner.constants import LOG_FILE_PATH
 from vcs_scanner.helpers.environment_wrapper import validate_environment
 from vcs_scanner.model import RepositoryRuntime
+from vcs_scanner.output_modules.rws_api_writer import RESTAPIWriter
 from vcs_scanner.secret_scanners.configuration import (
     GITLEAKS_PATH,
     RABBITMQ_DEFAULT_VHOST,
     RABBITMQ_PASSWORD,
     RABBITMQ_QUEUE,
     RABBITMQ_SERVICE_HOST,
     RABBITMQ_USERNAME,
     REQUIRED_ENV_VARS,
     RESC_API_NO_AUTH_SERVICE_HOST,
     RESC_API_NO_AUTH_SERVICE_PORT,
+    RESC_IGNORE_TAGS,
+    RESC_INCLUDE_TAGS,
     VCS_INSTANCES_FILE_PATH
 )
-from vcs_scanner.secret_scanners.rws_api_writer import RESTAPIWriter
 from vcs_scanner.secret_scanners.secret_scanner import SecretScanner
 
 env_variables = validate_environment(REQUIRED_ENV_VARS)
 app = Celery('secret_scanner_worker',
              broker="amqp://" +
                     f"{env_variables[RABBITMQ_USERNAME]}" + ":" +
                     f"{env_variables[RABBITMQ_PASSWORD]}" + "@" +
@@ -72,20 +74,28 @@
 
         repository = Repository(project_key=repository_runtime.project_key,
                                 repository_id=repository_runtime.repository_id,
                                 repository_name=repository_runtime.repository_name,
                                 repository_url=repository_runtime.repository_url,
                                 vcs_instance=vcs_instance.id_
                                 )
+        # Split the include_tags by comma if supplied
+        include_tags = env_variables[RESC_INCLUDE_TAGS].split(",") if env_variables[RESC_INCLUDE_TAGS] else None
+
+        # Split the ignore_tags by comma if supplied
+        ignore_tags = env_variables[RESC_IGNORE_TAGS].split(",") if env_variables[RESC_IGNORE_TAGS] else None
 
         secret_scanner = SecretScanner(
             gitleaks_binary_path=env_variables[GITLEAKS_PATH],
             gitleaks_rules_path=TEMP_RULE_FILE,
             rule_pack_version=active_rule_pack_version,
-            output_plugin=RESTAPIWriter(rws_url=rws_url),
+            output_plugin=RESTAPIWriter(rws_url=rws_url,
+                                        toml_rule_file_path=TEMP_RULE_FILE,
+                                        include_tags=include_tags,
+                                        ignore_tags=ignore_tags),
             repository=repository,
             username=vcs_instance.username,
             personal_access_token=vcs_instance.token,
             force_base_scan=os.getenv('FORCE_BASE_SCAN', "false").lower() in "true",
             latest_commit=repository_runtime.latest_commit
         )
```

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 # First Party
 from vcs_scanner.common import get_rule_pack_version_from_file, initialise_logs
 from vcs_scanner.constants import CLI_VCS_AZURE, CLI_VCS_BITBUCKET, CLI_VCS_LOCAL_SCAN, LOG_FILE_PATH_CLI
 from vcs_scanner.helpers.env_default import EnvDefault
 from vcs_scanner.model import RepositoryRuntime
-from vcs_scanner.secret_scanners.rws_api_writer import RESTAPIWriter
+from vcs_scanner.output_modules.rws_api_writer import RESTAPIWriter
+from vcs_scanner.output_modules.stdout_writer import STDOUTWriter
 from vcs_scanner.secret_scanners.secret_scanner import SecretScanner
-from vcs_scanner.secret_scanners.stdout_writer import STDOUTWriter
 
 logger_config = initialise_logs(LOG_FILE_PATH_CLI)
 logger = logging.getLogger(__name__)
 
 FAKE_COMMIT = "hash"
 FAKE_URL = "http://fake-host.none"
 
@@ -56,18 +56,24 @@
                                envvar="RESC_EXIT_CODE_WARN",
                                help="Exit code given if CLI encounters findings tagged with Warn, default 2. "
                                     "Can also be set via the RESC_EXIT_CODE_WARN environment variable")
     parser_common.add_argument("-b", "--exit-code-block", required=False, action=EnvDefault, default=1, type=int,
                                envvar="RESC_EXIT_CODE_BLOCK",
                                help="Exit code given if CLI encounters findings tagged with Block, default 1. "
                                     "Can also be set via the RESC_EXIT_CODE_BLOCK environment variable")
-    parser_common.add_argument("--filter-tag", required=False, action=EnvDefault, type=str,
-                               envvar="RESC_FILTER_TAG",
-                               help="Filter for findings based on specified tag. "
-                                    "Can also be set via the RESC_FILTER_TAG environment variable")
+    parser_common.add_argument("--include-tags", required=False, action=EnvDefault, type=str,
+                               envvar="RESC_INCLUDE_TAGS",
+                               help="Filter for outputting findings based on specified tags. "
+                                    "Provided as comma separated list. "
+                                    "Can also be set via the RESC_INCLUDE_TAGS environment variable")
+    parser_common.add_argument("--ignore-tags", required=False, action=EnvDefault, type=str,
+                               envvar="RESC_IGNORE_TAGS",
+                               help="Filter for NOT outputting findings based on specified tags. "
+                                    "Provided as comma separated list. "
+                                    "Can also be set via the RESC_IGNORE_TAGS environment variable")
     parser_common.add_argument("-v", "--verbose", required=False, action="store_true",
                                help="Enable more verbose logging")
 
     repository_common = ArgumentParser(add_help=False)
     repository_common.add_argument("--repo-name", type=str, required=False, action=EnvDefault, envvar="RESC_REPO_NAME",
                                    help="The name of the repository. "
                                         "Can also be set via the RESC_REPO_NAME environment variable")
@@ -151,14 +157,20 @@
     elif args.command == "dir" or \
             (args.command == "repo" and args.repository_location == "local" and not args.repo_name):
         if not os.path.isdir(args.dir.absolute()):
             logger.error(f"The directory {args.dir.absolute()} does not exist")
             valid_arguments = False
         args.repo_name = os.path.split(args.dir.absolute())[1]
 
+    # Split the include_tags by comma if supplied
+    args.include_tags = args.include_tags.split(",") if args.include_tags else None
+
+    # Split the ignore_tags by comma if supplied
+    args.ignore_tags = args.ignore_tags.split(",") if args.ignore_tags else None
+
     if not valid_arguments:
         return False
 
     return args
 
 
 def scan_repository_from_cli():
@@ -202,15 +214,16 @@
         vcs_instance_name="vcs_instance_name",
         latest_commit=FAKE_COMMIT
     )
 
     output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
                                  exit_code_warn=args.exit_code_warn,
                                  exit_code_block=args.exit_code_block,
-                                 filter_tag=args.filter_tag,
+                                 include_tags=args.include_tags,
+                                 ignore_tags=args.ignore_tags,
                                  working_dir=args.dir,
                                  ignore_findings_path=args.ignored_blocker_path)
     with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
         rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
 
@@ -243,22 +256,26 @@
         repository_id=args.repo_name,
         project_key=args.repo_name,
         vcs_instance_name=vcs_name,
         latest_commit=FAKE_COMMIT
     )
 
     if args.rws_url:
-        output_plugin = RESTAPIWriter(rws_url=args.rws_url)
+        output_plugin = RESTAPIWriter(rws_url=args.rws_url,
+                                      toml_rule_file_path=args.gitleaks_rules_path,
+                                      include_tags=args.include_tags,
+                                      ignore_tags=args.ignore_tags)
         rule_pack_version = output_plugin.download_rule_pack()
 
     else:
         output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
                                      exit_code_warn=args.exit_code_warn,
                                      exit_code_block=args.exit_code_block,
-                                     filter_tag=args.filter_tag,
+                                     include_tags=args.include_tags,
+                                     ignore_tags=args.ignore_tags,
                                      working_dir=args.dir,
                                      ignore_findings_path=args.ignored_blocker_path)
         with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
             rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
     if not rule_pack_version:
         rule_pack_version = "0.0.0"
```

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 RABBITMQ_QUEUE = "RABBITMQ_QUEUE"
 
 VCS_INSTANCES_FILE_PATH = "VCS_INSTANCES_FILE_PATH"
 
 RESC_API_NO_AUTH_SERVICE_HOST = "RESC_API_NO_AUTH_SERVICE_HOST"
 RESC_API_NO_AUTH_SERVICE_PORT = "RESC_API_NO_AUTH_SERVICE_PORT"
 
+RESC_INCLUDE_TAGS = "RESC_INCLUDE_TAGS"
+RESC_IGNORE_TAGS = "RESC_IGNORE_TAGS"
 
 REQUIRED_ENV_VARS = [
     EnvironmentVariable(
         GITLEAKS_PATH,
         "The filepath for the gitleaks binary",
         required=True,
     ),
@@ -66,8 +68,20 @@
         required=True,
     ),
     EnvironmentVariable(
         VCS_INSTANCES_FILE_PATH,
         "The absolute path to the json file containing the vcs_instances_definitions",
         required=True,
     ),
+    EnvironmentVariable(
+        RESC_INCLUDE_TAGS,
+        "Filter for outputting findings based on specified tags. Provided as comma seperated list.",
+        required=False,
+        default=None,
+    ),
+    EnvironmentVariable(
+        RESC_IGNORE_TAGS,
+        "Filter for NOT outputting findings based on specified tags. Provided as comma seperated list.",
+        required=False,
+        default=None,
+    )
 ]
```

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/ignore_list_provider.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/helpers/ignore_list_provider.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Third Party
 from resc_backend.resc_web_service.schema.finding import FindingBase
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.scan import Scan
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 # First Party
-from vcs_scanner.output_module import OutputModule
+from vcs_scanner.output_modules.output_module import OutputModule
 from vcs_scanner.resc_worker import RESCWorker
 from vcs_scanner.secret_scanners.git_operation import clone_repository
 from vcs_scanner.secret_scanners.gitleaks_wrapper import GitLeaksWrapper
 
 # This is an arbitrary number to distinguish between no issues, an error and
 # the situation in which leaks are found. Note that this number cannot be bigger than 255 (OS limitation)
 LEAKS_FOUND_EXIT_CODE = 42
```

### Comparing `resc_vcs_scanner-3.0.0/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-3.0.1/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*

