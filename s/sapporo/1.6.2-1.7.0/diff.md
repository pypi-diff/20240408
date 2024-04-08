# Comparing `tmp/sapporo-1.6.2.tar.gz` & `tmp/sapporo-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapporo-1.6.2.tar", last modified: Mon Mar  4 11:13:18 2024, max compression
+gzip compressed data, was "sapporo-1.7.0.tar", last modified: Mon Apr  8 05:40:48 2024, max compression
```

## Comparing `sapporo-1.6.2.tar` & `sapporo-1.7.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:13:18.941654 sapporo-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-03-04 11:13:07.000000 sapporo-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-04 11:13:07.000000 sapporo-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19798 2024-03-04 11:13:18.941654 sapporo-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-03-04 11:13:07.000000 sapporo-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:13:18.937654 sapporo-1.6.2/sapporo/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/auth_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/auth_config.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/executable_workflows.json
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/executable_workflows.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:13:18.941654 sapporo-1.6.2/sapporo/model/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/model/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/model/sapporo_wes_1_0_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/ro_crate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/service-info.json
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/service-info.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/trs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    34616 2024-03-04 11:13:07.000000 sapporo-1.6.2/sapporo-wes-1-0-1-openapi-spec.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 11:13:18.941654 sapporo-1.6.2/sapporo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19798 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-04 11:13:18.000000 sapporo-1.6.2/sapporo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 11:13:18.941654 sapporo-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-04 11:13:07.000000 sapporo-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.998450 sapporo-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-08 05:40:40.000000 sapporo-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 05:40:40.000000 sapporo-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19474 2024-04-08 05:40:47.998450 sapporo-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-04-08 05:40:40.000000 sapporo-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.994450 sapporo-1.7.0/sapporo/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/auth_config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/executable_workflows.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/executable_workflows.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.994450 sapporo-1.7.0/sapporo/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/sapporo_wes_1_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/model/sapporo_wes_1_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23577 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/ro_crate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/service-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/service-info.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/trs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-08 05:40:40.000000 sapporo-1.7.0/sapporo-wes-1-1-0-openapi-spec.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:40:47.998450 sapporo-1.7.0/sapporo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19474 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 05:40:47.000000 sapporo-1.7.0/sapporo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:40:47.998450 sapporo-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-08 05:40:40.000000 sapporo-1.7.0/setup.py
```

### Comparing `sapporo-1.6.2/LICENSE` & `sapporo-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/PKG-INFO` & `sapporo-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapporo
-Version: 1.6.2
+Version: 1.7.0
 Summary: The sapporo-service is a standard implementation conforming to the Global Alliance for Genomics and Health (GA4GH) Workflow Execution Service (WES) API specification.
 Home-page: https://github.com/sapporo-wes/sapporo-service
 Author: DDBJ(Bioinformatics and DDBJ Center)
 Author-email: tazro.ohta@chiba-u.jp
 License: Apache2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,15 +58,15 @@
 [![Apache License](https://img.shields.io/badge/license-Apache%202.0-orange.svg?style=flat&color=important)](http://www.apache.org/licenses/LICENSE-2.0)
 
 <img src="https://raw.githubusercontent.com/sapporo-wes/sapporo/main/logo/sapporo-service.svg" width="400" style="display: block; margin-left: auto; margin-right: auto; margin-top: 30px; margin-bottom: 30px;" alt="sapporo-service logo">
 
 The sapporo-service is a standard implementation conforming to the [Global Alliance for Genomics and Health](https://www.ga4gh.org) (GA4GH) [Workflow Execution Service](https://github.com/ga4gh/workflow-execution-service-schemas) (WES) API specification.
 
 We have also extended the API specification.
-For more details, please refer to [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml) for more details.
+For more details, please refer to [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml) for more details.
 
 One of the key features of the sapporo-service is its ability to abstract workflow engines, making it easy to adapt various workflow engines to the WES standard.
 Currently, we have verified compatibility with the following workflow engines:
 
 - [cwltool](https://github.com/common-workflow-language/cwltool)
 - [nextflow](https://www.nextflow.io)
 - [Toil (experimental)](https://toil.ucsc-cgl.org)
@@ -132,15 +132,15 @@
   --run-only-registered-workflows
                         Only run registered workflows. Check the registered
                         workflows using `GET /executable-workflows`, and specify
                         the `workflow_name` in the `POST /run` request.
   --service-info        Specify the `service-info.json` file. The
                         `supported_wes_versions` and `system_state_counts` will
                         be overwritten by the application.
-  --executable-workflows 
+  --executable-workflows
                         Specify the `executable-workflows.json` file.
   --run-sh              Specify the `run.sh` file.
   --url-prefix          Specify the prefix of the URL (e.g., --url-prefix /foo
                         will result in /foo/service-info).
   --auth-config         Specify the `auth-config.json` file.
 ```
 
@@ -153,15 +153,14 @@
 
 You can switch between these modes using the `--run-only-registered-workflows` startup argument or by setting the `SAPPORO_ONLY_REGISTERED_WORKFLOWS` environment variable to `True` or `False`.
 Note that startup arguments take precedence over environment variables.
 
 #### Standard WES Mode
 
 In this mode, the sapporo-service conforms to the standard WES API specification.
-However, it's important to note that when using the sapporo-service, there is a deviation from the standard WES API specification: **you are required to specify `workflow_engine_name` in the request parameter of `POST /runs`.** This is due to the sapporo-service's ability to abstract workflow engines, as mentioned above.
 
 #### Execute Only Registered Workflows Mode
 
 In this mode, the sapporo-service only allows workflows registered by the system administrator to be executed.
 
 The key changes in this mode are:
 
@@ -235,21 +234,21 @@
 By default, this file is located in the application directory of the sapporo-service.
 You can override this location using the startup argument `--service-info` or the environment variable `SAPPORO_SERVICE_INFO`.
 
 ### Generate Download Link
 
 The sapporo-service allows you to generate download links for files and directories located under the `run_dir`.
 
-For more details, please refer to the `GetData` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `GetData` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Parse Workflow
 
 The sapporo-service offers a feature to inspect the type, version, and inputs of a workflow document.
 
-For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Generate RO-Crate
 
 Upon completion of workflow execution, the sapporo-service generates an RO-Crate from the `run_dir`, which is saved as `ro-crate-metadata.json` within the same directory. You can download the RO-Crate using the `GET /runs/{run_id}/ro-crate/data/ro-crate-metadata.json` endpoint.
 
 Additionally, you can generate an RO-Crate from the `run_dir` as follows:
```

### Comparing `sapporo-1.6.2/README.md` & `sapporo-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Apache License](https://img.shields.io/badge/license-Apache%202.0-orange.svg?style=flat&color=important)](http://www.apache.org/licenses/LICENSE-2.0)
 
 <img src="https://raw.githubusercontent.com/sapporo-wes/sapporo/main/logo/sapporo-service.svg" width="400" style="display: block; margin-left: auto; margin-right: auto; margin-top: 30px; margin-bottom: 30px;" alt="sapporo-service logo">
 
 The sapporo-service is a standard implementation conforming to the [Global Alliance for Genomics and Health](https://www.ga4gh.org) (GA4GH) [Workflow Execution Service](https://github.com/ga4gh/workflow-execution-service-schemas) (WES) API specification.
 
 We have also extended the API specification.
-For more details, please refer to [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml) for more details.
+For more details, please refer to [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml) for more details.
 
 One of the key features of the sapporo-service is its ability to abstract workflow engines, making it easy to adapt various workflow engines to the WES standard.
 Currently, we have verified compatibility with the following workflow engines:
 
 - [cwltool](https://github.com/common-workflow-language/cwltool)
 - [nextflow](https://www.nextflow.io)
 - [Toil (experimental)](https://toil.ucsc-cgl.org)
@@ -82,15 +82,15 @@
   --run-only-registered-workflows
                         Only run registered workflows. Check the registered
                         workflows using `GET /executable-workflows`, and specify
                         the `workflow_name` in the `POST /run` request.
   --service-info        Specify the `service-info.json` file. The
                         `supported_wes_versions` and `system_state_counts` will
                         be overwritten by the application.
-  --executable-workflows 
+  --executable-workflows
                         Specify the `executable-workflows.json` file.
   --run-sh              Specify the `run.sh` file.
   --url-prefix          Specify the prefix of the URL (e.g., --url-prefix /foo
                         will result in /foo/service-info).
   --auth-config         Specify the `auth-config.json` file.
 ```
 
@@ -103,15 +103,14 @@
 
 You can switch between these modes using the `--run-only-registered-workflows` startup argument or by setting the `SAPPORO_ONLY_REGISTERED_WORKFLOWS` environment variable to `True` or `False`.
 Note that startup arguments take precedence over environment variables.
 
 #### Standard WES Mode
 
 In this mode, the sapporo-service conforms to the standard WES API specification.
-However, it's important to note that when using the sapporo-service, there is a deviation from the standard WES API specification: **you are required to specify `workflow_engine_name` in the request parameter of `POST /runs`.** This is due to the sapporo-service's ability to abstract workflow engines, as mentioned above.
 
 #### Execute Only Registered Workflows Mode
 
 In this mode, the sapporo-service only allows workflows registered by the system administrator to be executed.
 
 The key changes in this mode are:
 
@@ -185,21 +184,21 @@
 By default, this file is located in the application directory of the sapporo-service.
 You can override this location using the startup argument `--service-info` or the environment variable `SAPPORO_SERVICE_INFO`.
 
 ### Generate Download Link
 
 The sapporo-service allows you to generate download links for files and directories located under the `run_dir`.
 
-For more details, please refer to the `GetData` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `GetData` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Parse Workflow
 
 The sapporo-service offers a feature to inspect the type, version, and inputs of a workflow document.
 
-For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Generate RO-Crate
 
 Upon completion of workflow execution, the sapporo-service generates an RO-Crate from the `run_dir`, which is saved as `ro-crate-metadata.json` within the same directory. You can download the RO-Crate using the `GET /runs/{run_id}/ro-crate/data/ro-crate-metadata.json` endpoint.
 
 Additionally, you can generate an RO-Crate from the `run_dir` as follows:
```

### Comparing `sapporo-1.6.2/sapporo/app.py` & `sapporo-1.7.0/sapporo/app.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/auth.py` & `sapporo-1.7.0/sapporo/auth.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/auth_config.schema.json` & `sapporo-1.7.0/sapporo/auth_config.schema.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/config.py` & `sapporo-1.7.0/sapporo/config.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/const.py` & `sapporo-1.7.0/sapporo/const.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/controller.py` & `sapporo-1.7.0/sapporo/controller.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/executable_workflows.json` & `sapporo-1.7.0/sapporo/executable_workflows.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/executable_workflows.schema.json` & `sapporo-1.7.0/sapporo/executable_workflows.schema.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/model/factory.py` & `sapporo-1.7.0/sapporo/model/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def generate_service_info() -> ServiceInfo:
     from sapporo.run import count_system_state
     with current_app.config["SERVICE_INFO"].open(mode="r", encoding="utf-8") as f:
         service_info: ServiceInfo = json.load(f)
 
-    service_info["supported_wes_versions"] = ["sapporo-wes-1.0.1"]
+    service_info["supported_wes_versions"] = ["sapporo-wes-1.1.0"]
     service_info["system_state_counts"] = count_system_state()
     service_info["tags"]["get_runs"] = current_app.config["GET_RUNS"]
     service_info["tags"]["workflow_attachment"] = current_app.config["WORKFLOW_ATTACHMENT"]
     service_info["tags"]["registered_only_mode"] = current_app.config["REGISTERED_ONLY_MODE"]
 
     return service_info
```

### Comparing `sapporo-1.6.2/sapporo/model/sapporo_wes_1_0_1.py` & `sapporo-1.7.0/sapporo/model/sapporo_wes_1_0_1.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/parser.py` & `sapporo-1.7.0/sapporo/parser.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/ro_crate.py` & `sapporo-1.7.0/sapporo/ro_crate.py`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/run.py` & `sapporo-1.7.0/sapporo/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 from urllib import parse
 
 import requests
 from flask import current_app, request
 from werkzeug.utils import _filename_ascii_strip_re  # type: ignore
 
 from sapporo.const import RUN_DIR_STRUCTURE, RUN_DIR_STRUCTURE_KEYS
-from sapporo.model import RunRequest, State
+from sapporo.model import AttachedFile, RunRequest, State
 from sapporo.model.factory import (generate_executable_workflows,
                                    generate_service_info)
-from sapporo.model.sapporo_wes_1_0_1 import AttachedFile
 
 
 def resolve_run_dir_path(run_id: str) -> Path:
     run_base_dir: Path = current_app.config["RUN_DIR"]
 
     return run_base_dir.joinpath(run_id[:2]).joinpath(run_id).resolve()
 
@@ -191,15 +190,15 @@
 def convert_wf_engine_params_str(run_request: RunRequest) -> str:
     wf_engine_params: Optional[str] = run_request["workflow_engine_parameters"]
     params: List[str] = []
     if wf_engine_params is None:
         service_info = generate_service_info()
         default_wf_engine_dict = service_info["default_workflow_engine_parameters"]
         default_wf_engine_params = default_wf_engine_dict.get(
-            run_request["workflow_engine_name"], [])
+            run_request["workflow_engine"], [])
         for default_wf_engine_param in default_wf_engine_params:
             params.append(default_wf_engine_param.get("name", ""))
             params.append(default_wf_engine_param.get("default_value", ""))
     else:
         wf_engine_params_obj = json.loads(wf_engine_params)
         if isinstance(wf_engine_params_obj, list):
             params.extend(map(str, wf_engine_params_obj))
```

### Comparing `sapporo-1.6.2/sapporo/run.sh` & `sapporo-1.7.0/sapporo/run.sh`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 set -e
 
 function run_wf() {
   echo "INITIALIZING" >${state}
   download_workflow_attachment
   echo "RUNNING" >${state}
   date +"%Y-%m-%dT%H:%M:%S" >${start_time}
-  # e.g. when wf_engine_name=cwltool, call function run_cwltool
-  local function_name="run_${wf_engine_name}"
+  # e.g. when wf_engine=cwltool, call function run_cwltool
+  local function_name="run_${wf_engine}"
   if [[ "$(type -t ${function_name})" == "function" ]]; then
     ${function_name}
     generate_outputs_list
   else
     executor_error
   fi
   generate_ro_crate
@@ -123,15 +123,15 @@
   local cmd_txt="docker run --mount type=bind,source=${run_dir},target=/streamflow/project --mount type=bind,source=${outputs_dir},target=/streamflow/results ${container} run /streamflow/project/exe/$(basename ${wf_url_local}) 1>${stdout} 2>${stderr}"
   echo ${cmd_txt} >${cmd}
   eval ${cmd_txt} || executor_error
 }
 
 function cancel() {
   # Pre-cancellation procedures
-  if [[ ${wf_engine_name} == "cwltool" ]]; then
+  if [[ ${wf_engine} == "cwltool" ]]; then
     cancel_cwltool
   fi
   cancel_by_request
 }
 
 function cancel_cwltool() {
   :
@@ -213,15 +213,17 @@
 stdout="${run_dir}/stdout.log"
 stderr="${run_dir}/stderr.log"
 wf_engine_params_file="${run_dir}/workflow_engine_params.txt"
 cmd="${run_dir}/cmd.txt"
 task_logs="${run_dir}/task.log"
 
 # Meta characters are escaped.
-wf_engine_name=$(jq -r ".workflow_engine_name" ${run_request})
+# wf_engine=$(jq -r ".workflow_engine" ${run_request})
+# for compatibility with the sapporo-wes 1.0.1, will be deprecated in the future (TODO)
+wf_engine=$(jq -r ".workflow_engine // .workflow_engine_name" ${run_request})
 wf_url=$(jq -r ".workflow_url" ${run_request})
 wf_engine_params=$(head -n 1 ${wf_engine_params_file})
 
 # Sibling docker command
 D_SOCK="-v /var/run/docker.sock:/var/run/docker.sock"
 D_TMP="-v /tmp:/tmp"
 DOCKER_CMD="docker run --rm ${D_SOCK} -e DOCKER_HOST=unix:///var/run/docker.sock ${D_TMP} -v ${run_dir}:${run_dir} -w=${exe_dir}"
```

### Comparing `sapporo-1.6.2/sapporo/service-info.json` & `sapporo-1.7.0/sapporo/service-info.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'tags'": "{'sapporo-version': '1.7.0'}"}*

```diff
@@ -26,15 +26,15 @@
         "http",
         "https",
         "file",
         "s3"
     ],
     "tags": {
         "news_content": "",
-        "sapporo-version": "1.6.2",
+        "sapporo-version": "1.7.0",
         "wes-name": "sapporo"
     },
     "workflow_engine_versions": {
         "cromwell": "80",
         "cwltool": "3.1.20240112164112",
         "ep3 (experimental)": "v1.7.0",
         "nextflow": "22.04.4",
```

### Comparing `sapporo-1.6.2/sapporo/service-info.schema.json` & `sapporo-1.7.0/sapporo/service-info.schema.json`

 * *Files identical despite different names*

### Comparing `sapporo-1.6.2/sapporo/trs.py` & `sapporo-1.7.0/sapporo/trs.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                         elif file["file_type"] == "SECONDARY_DESCRIPTOR":
                             wf["workflow_attachment"].append({
                                 "file_name": url.split("/")[-1],
                                 "file_url": url
                             })
                     if wf["workflow_url"] != "":
                         wfs.append(wf)
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             pass
     return wfs
 
 
 def get_files_via_api(trs_endpoint: str, id_: str, ver: str, _type: str) -> Any:
     url = trs_endpoint.rstrip("/") + f"/tools/{id_}/versions/{ver}/{_type}/files"
     res = requests.get(url, allow_redirects=True, headers=headers, timeout=10)
```

### Comparing `sapporo-1.6.2/sapporo/validator.py` & `sapporo-1.7.0/sapporo/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,21 @@
 def validate_run_request(run_id: str) -> RunRequest:
     # Fields: do not require validation
     wf_params = request.form.get("workflow_params", None)
     wf_engine_params = request.form.get("workflow_engine_parameters", None)
     tags = request.form.get("tags", None)
 
     # Fields: require validation, but not related to the registered mode
-    wf_engine_name = request.form.get("workflow_engine_name", None)
+    wf_engine = request.form.get("workflow_engine", None)
+    if wf_engine is None:  # for compatibility with the sapporo-wes 1.0.1, will be deprecated in the future (TODO)
+        wf_engine = request.form.get("workflow_engine_name", None)
+    __wf_engine_version = request.form.get("workflow_engine_version", None)  # added in WES 1.1, but not used in current impl.
     wf_attachment_str = request.form.get("workflow_attachment", None)
     wf_attachment_files = request.files.getlist("workflow_attachment")
-    wf_engine_name = validate_wf_engine_name(wf_engine_name)
+    wf_engine = validate_wf_engine(wf_engine)
     wf_attachment = validate_wf_attachment(run_id, wf_attachment_str, wf_attachment_files)
 
     # Fields: require validation, related to the registered mode
     wf_url = request.form.get("workflow_url", None)
     wf_name = request.form.get("workflow_name", None)
     wf_type = request.form.get("workflow_type", None)
     wf_type_version = request.form.get("workflow_type_version", None)
@@ -91,31 +94,32 @@
             abort(400, "`workflow_engine_parameters` is not a valid JSON.")
 
     return {
         "workflow_params": wf_params,
         "workflow_type": wf_type,
         "workflow_type_version": wf_type_version,
         "tags": tags,
-        "workflow_engine_name": wf_engine_name,
+        "workflow_engine": wf_engine,
+        "workflow_engine_version": __wf_engine_version if __wf_engine_version is not None else "",
         "workflow_engine_parameters": wf_engine_params,
         "workflow_url": wf_url,
         "workflow_name": wf_name,
         "workflow_attachment": json.dumps(wf_attachment),
     }
 
 
-def validate_wf_engine_name(wf_engine_name: Optional[str]) -> str:
-    if wf_engine_name is None:
-        abort(400, "Workflow engine name is required.")
+def validate_wf_engine(wf_engine: Optional[str]) -> str:
+    if wf_engine is None:
+        abort(400, "Workflow engine is required.")
     service_info = generate_service_info()
-    wf_engines_names = list(service_info["workflow_engine_versions"].keys())
-    if wf_engine_name not in wf_engines_names:
-        abort(400, f"Workflow engine name `{wf_engine_name}` is not supported.")
+    wf_engines = list(service_info["workflow_engine_versions"].keys())
+    if wf_engine not in wf_engines:
+        abort(400, f"Workflow engine `{wf_engine}` is not supported.")
 
-    return wf_engine_name
+    return wf_engine
 
 
 def validate_registered_only_mode() -> None:
     if current_app.config["REGISTERED_ONLY_MODE"]:
         abort(403, "The sapporo-service is currently running in registered-only mode. The `POST /runs` endpoint is unavailable to specify `workflow_url`.")
 
 
@@ -127,15 +131,15 @@
                 wf_attachment_obj = json.loads(wf_attachment_str)
                 try:
                     for attached_file in wf_attachment_obj:
                         wf_attachment.append({
                             "file_name": str(attached_file["file_name"]),
                             "file_url": str(attached_file["file_url"]),
                         })
-                except Exception:
+                except KeyError:
                     abort(400, "`workflow_attachment` must be a list of `AttachedFile`.")
             except json.JSONDecodeError:
                 abort(400, "`workflow_attachment` is invalid.")
         if len(wf_attachment_files):
             exe_dir = resolve_content_path(run_id, "exe_dir")
             endpoint = sapporo_endpoint()
             base_remote_url = f"{endpoint}/runs/{run_id}/data/"
@@ -180,15 +184,15 @@
             parse_result = parse_workflows({
                 "workflow_content": None,
                 "workflow_location": wf_url,
                 "types_of_parsing": ["workflow_type", "workflow_type_version"],
             })
             wf_type = wf_type or parse_result["workflow_type"]
             wf_type_version = wf_type_version or parse_result["workflow_type_version"]
-        except Exception:
+        except Exception:  # pylint: disable=broad-except
             abort(400, "`workflow_type` and `workflow_type_version` are required.")
 
     return wf_type, wf_type_version  # type: ignore
 
 
 def validate_workflow_type(wf_type: str, wf_type_version: str) -> None:
     service_info = generate_service_info()
@@ -208,20 +212,20 @@
         abort(404, f"Run ID `{run_id}` does not exist. Please provide a valid run ID.")
 
 
 def validate_meta_characters(_type: str, content: str) -> None:
     """\
     This function checks the validity of the string that will be evaluated in the 'eval'
     command within run.sh. The string could be of the type 'workflow_url',
-    'workflow_engine_name', or 'workflow_engine_params'. If any of these strings contain
+    'workflow_engine', or 'workflow_engine_params'. If any of these strings contain
     characters from the list of prohibited characters below, the operation will be aborted.
 
     This function is invoked as shown below in the POST /runs endpoint:
 
     validate_meta_characters("workflow_engine_params", joined_params)
     validate_meta_characters("workflow_url", run_request["workflow_url"])
-    validate_meta_characters("workflow_engine_name", run_request["workflow_engine_name"])
+    validate_meta_characters("workflow_engine", run_request["workflow_engine"])
     """
     prohibited_characters = [";", "!", "?", "(", ")", "[", "]", "{", "}", "*", "\\", "&", r"`", "^", "<", ">", "|", "$"]
     for char in content:
         if char in prohibited_characters:
             abort(400, f"The `{_type}` contains a prohibited character `{char}`. Please remove this character.")
```

### Comparing `sapporo-1.6.2/sapporo-wes-1-0-1-openapi-spec.yml` & `sapporo-1.7.0/sapporo-wes-1-1-0-openapi-spec.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 openapi: 3.0.0
 info:
   title: >-
     GA4GH Workflow Execution Service API specification extended for
     the sapporo-service
-  version: sapporo-wes-1.0.1-oas3
+  version: sapporo-wes-1.1.0-oas3
   description: >-
     The Workflow Execution Service (WES) API provides a standard way for users to submit workflow requests to workflow execution systems and monitor their execution.
     This API lets users run a single workflow on multiple different platforms, clouds, and environments.
 
     Key features of the API:
 
     - can request that a workflow be run
+
     - can pass parameters to that workflow (e.g. input files, cmd-line arguments)
+
     - can get information about running workflows (e.g. status, errors, output file locations)
+
     - can cancel a running workflow
 
   license:
     url: https://github.com/sapporo-wes/sapporo-service/blob/main/LICENSE
     name: Apache-2.0
   contact:
     url: https://github.com/sapporo-wes/sapporo-service/issues
@@ -708,14 +711,15 @@
         - RUNNING
         - PAUSED
         - COMPLETE
         - EXECUTOR_ERROR
         - SYSTEM_ERROR
         - CANCELED
         - CANCELING
+        - PREEMPTED
       default: UNKNOWN
       description: >-
         - UNKNOWN: The state of the task is unknown.
         This provides a safe default for messages where this field is missing.
         For example, a missing field does not accidentally imply that the state is QUEUED.
 
         - QUEUED: The task is queued.
@@ -736,35 +740,44 @@
         Generally, this means that an Executor exited with a non-zero exit code.
 
         - SYSTEM_ERROR: The task was stopped due to a system error, but not from an Executor; for example, an upload failed due to network issues, the workers ran out of disk space, etc.
 
         - CANCELED: The task was canceled by the user.
 
         - CANCELING: The task was canceled by the user and is in the process of stopping.
+
+        - PREEMPTED: The task is stopped (preempted) by the system. The reasons for this would be tied to
+        the specific system running the job. Generally, this means that the system reclaimed the compute
+        capacity for reallocation.
     RunListResponse:
       type: object
       additionalProperties: false
       required:
         - runs
       properties:
         runs:
           type: array
           additionalProperties: false
           items:
-            $ref: "#/components/schemas/RunStatus"
+            anyOf:
+              - $ref: "#/components/schemas/RunStatus"
+              - $ref: "#/components/schemas/RunSummary"
           description: >-
             A list of workflow runs that the service has executed or is executing.
             The list is filtered to only include runs that the caller has permission to see.
         next_page_token:
           type: string
           description: >-
             A token may be supplied as `page_token` in the workflow run list request to get the next page of results.
             An empty string indicates there are no more items to return.
       description: >-
         The service will return a RunListResponse when receiving a successful RunListRequest.
+        DEPRECIATION WARNING: The use of `RunStatus` as the schema for `runs` array items will
+        not be permitted from the next major version of the specification (2.0.0) onwards. We
+        encourage implementers to use `RunSummary` instead.
     RunLog:
       type: object
       additionalProperties: false
       required:
         - run_id
         - request
         - state
@@ -794,15 +807,15 @@
           items:
             $ref: "#/components/schemas/AttachedFile"
           description: The outputs from the workflow run.
     RunRequest:
       type: object
       additionalProperties: false
       required:
-        - workflow_engine_name
+        - workflow_engine
       properties:
         workflow_params:
           type: string
           format: application/json
           nullable: true
           description: >-
             The `workflow_params` JSON object specifies input parameters, such as input files.
@@ -822,18 +835,22 @@
             The `workflow_type_version` is the version of the workflow language submitted and must be one supported by this WES instance.
         tags:
           type: string
           nullable: true
           format: application/json
           description: >-
             A key-value map of arbitrary metadata outside the scope of `workflow_params` but useful to track with this run request
-        workflow_engine_name:
+        workflow_engine:
           type: string
           description: >-
             Specify the name of the workflow engine to run a workflow.
+        workflow_engine_version:
+          type: string
+          description: >-
+            Specify the version of the workflow engine to run a workflow.
         workflow_engine_parameters:
           type: string
           format: application/json
           nullable: true
           description: >-
             Additional parameters can be sent to the workflow engine using this field.
             Default values for these parameters can be obtained using the `GetServiceInfo` endpoint.
@@ -877,24 +894,44 @@
       required:
         - run_id
       properties:
         run_id:
           type: string
           description: workflow run ID
     RunStatus:
-      type: object
+      type: object # returned by server during listing
       required:
         - run_id
         - state
       properties:
         run_id:
           type: string
         state:
           $ref: "#/components/schemas/State"
-      description: Small description of a workflow run, returned by server during listing
+      description: State information of a workflow run
+    RunSummary:
+      title: RunSummary,
+      allOf:
+        - $ref: "#/components/schemas/RunStatus"
+        - type: object
+          properties:
+            start_time:
+              type: string
+              description: When the run started executing, in ISO 8601 format "%Y-%m-%dT%H:%M:%SZ"
+            end_time:
+              type: string
+              description: When the run stopped executing (completed, failed, or cancelled), in ISO 8601 format "%Y-%m-%dT%H:%M:%SZ"
+            tags:
+              type: object
+              description: Arbitrary key/value tags added by the client during run creation
+              additionalProperties:
+                type: string
+          required:
+            - tags
+      description: Small description of a workflow run
     WorkflowTypeVersion:
       type: object
       additionalProperties: false
       required:
         - workflow_type_version
       properties:
         workflow_type_version:
```

### Comparing `sapporo-1.6.2/sapporo.egg-info/PKG-INFO` & `sapporo-1.7.0/sapporo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapporo
-Version: 1.6.2
+Version: 1.7.0
 Summary: The sapporo-service is a standard implementation conforming to the Global Alliance for Genomics and Health (GA4GH) Workflow Execution Service (WES) API specification.
 Home-page: https://github.com/sapporo-wes/sapporo-service
 Author: DDBJ(Bioinformatics and DDBJ Center)
 Author-email: tazro.ohta@chiba-u.jp
 License: Apache2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,15 +58,15 @@
 [![Apache License](https://img.shields.io/badge/license-Apache%202.0-orange.svg?style=flat&color=important)](http://www.apache.org/licenses/LICENSE-2.0)
 
 <img src="https://raw.githubusercontent.com/sapporo-wes/sapporo/main/logo/sapporo-service.svg" width="400" style="display: block; margin-left: auto; margin-right: auto; margin-top: 30px; margin-bottom: 30px;" alt="sapporo-service logo">
 
 The sapporo-service is a standard implementation conforming to the [Global Alliance for Genomics and Health](https://www.ga4gh.org) (GA4GH) [Workflow Execution Service](https://github.com/ga4gh/workflow-execution-service-schemas) (WES) API specification.
 
 We have also extended the API specification.
-For more details, please refer to [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml) for more details.
+For more details, please refer to [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml) for more details.
 
 One of the key features of the sapporo-service is its ability to abstract workflow engines, making it easy to adapt various workflow engines to the WES standard.
 Currently, we have verified compatibility with the following workflow engines:
 
 - [cwltool](https://github.com/common-workflow-language/cwltool)
 - [nextflow](https://www.nextflow.io)
 - [Toil (experimental)](https://toil.ucsc-cgl.org)
@@ -132,15 +132,15 @@
   --run-only-registered-workflows
                         Only run registered workflows. Check the registered
                         workflows using `GET /executable-workflows`, and specify
                         the `workflow_name` in the `POST /run` request.
   --service-info        Specify the `service-info.json` file. The
                         `supported_wes_versions` and `system_state_counts` will
                         be overwritten by the application.
-  --executable-workflows 
+  --executable-workflows
                         Specify the `executable-workflows.json` file.
   --run-sh              Specify the `run.sh` file.
   --url-prefix          Specify the prefix of the URL (e.g., --url-prefix /foo
                         will result in /foo/service-info).
   --auth-config         Specify the `auth-config.json` file.
 ```
 
@@ -153,15 +153,14 @@
 
 You can switch between these modes using the `--run-only-registered-workflows` startup argument or by setting the `SAPPORO_ONLY_REGISTERED_WORKFLOWS` environment variable to `True` or `False`.
 Note that startup arguments take precedence over environment variables.
 
 #### Standard WES Mode
 
 In this mode, the sapporo-service conforms to the standard WES API specification.
-However, it's important to note that when using the sapporo-service, there is a deviation from the standard WES API specification: **you are required to specify `workflow_engine_name` in the request parameter of `POST /runs`.** This is due to the sapporo-service's ability to abstract workflow engines, as mentioned above.
 
 #### Execute Only Registered Workflows Mode
 
 In this mode, the sapporo-service only allows workflows registered by the system administrator to be executed.
 
 The key changes in this mode are:
 
@@ -235,21 +234,21 @@
 By default, this file is located in the application directory of the sapporo-service.
 You can override this location using the startup argument `--service-info` or the environment variable `SAPPORO_SERVICE_INFO`.
 
 ### Generate Download Link
 
 The sapporo-service allows you to generate download links for files and directories located under the `run_dir`.
 
-For more details, please refer to the `GetData` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `GetData` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Parse Workflow
 
 The sapporo-service offers a feature to inspect the type, version, and inputs of a workflow document.
 
-For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-0-1-openapi-spec.yml`](./sapporo-wes-1-0-1-openapi-spec.yml).
+For more details, please refer to the `ParseWorkflow` section in [`./sapporo-wes-1-1-0-openapi-spec.yml`](./sapporo-wes-1-1-0-openapi-spec.yml).
 
 ### Generate RO-Crate
 
 Upon completion of workflow execution, the sapporo-service generates an RO-Crate from the `run_dir`, which is saved as `ro-crate-metadata.json` within the same directory. You can download the RO-Crate using the `GET /runs/{run_id}/ro-crate/data/ro-crate-metadata.json` endpoint.
 
 Additionally, you can generate an RO-Crate from the `run_dir` as follows:
```

### Comparing `sapporo-1.6.2/sapporo.egg-info/SOURCES.txt` & `sapporo-1.7.0/sapporo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-sapporo-wes-1-0-1-openapi-spec.yml
+sapporo-wes-1-1-0-openapi-spec.yml
 setup.py
 sapporo/__init__.py
 sapporo/app.py
 sapporo/auth.py
 sapporo/auth_config.json
 sapporo/auth_config.schema.json
 sapporo/config.py
@@ -25,8 +25,9 @@
 sapporo.egg-info/SOURCES.txt
 sapporo.egg-info/dependency_links.txt
 sapporo.egg-info/entry_points.txt
 sapporo.egg-info/requires.txt
 sapporo.egg-info/top_level.txt
 sapporo/model/__init__.py
 sapporo/model/factory.py
-sapporo/model/sapporo_wes_1_0_1.py
+sapporo/model/sapporo_wes_1_0_1.py
+sapporo/model/sapporo_wes_1_1_0.py
```

### Comparing `sapporo-1.6.2/setup.py` & `sapporo-1.7.0/setup.py`

 * *Files identical despite different names*

