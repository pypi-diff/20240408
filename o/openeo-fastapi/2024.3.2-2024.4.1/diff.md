# Comparing `tmp/openeo_fastapi-2024.3.2.tar.gz` & `tmp/openeo_fastapi-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_fastapi-2024.3.2.tar", max compression
+gzip compressed data, was "openeo_fastapi-2024.4.1.tar", max compression
```

## Comparing `openeo_fastapi-2024.3.2.tar` & `openeo_fastapi-2024.4.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    11358 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/LICENSE
--rw-r--r--   0        0        0     2191 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/README.md
--rw-r--r--   0        0        0        0 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/api/__init__.py
--rw-r--r--   0        0        0    18853 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/api/app.py
--rw-r--r--   0        0        0      786 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/api/requests.py
--rw-r--r--   0        0        0    24748 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/api/responses.py
--rw-r--r--   0        0        0    15114 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/api/types.py
--rw-r--r--   0        0        0        0 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/__init__.py
--rw-r--r--   0        0        0     4971 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/auth.py
--rw-r--r--   0        0        0     2579 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/collections.py
--rw-r--r--   0        0        0      451 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/conformance.py
--rw-r--r--   0        0        0     4510 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/core.py
--rw-r--r--   0        0        0      178 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/exceptions.py
--rw-r--r--   0        0        0     3308 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/files.py
--rw-r--r--   0        0        0    15551 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/jobs.py
--rw-r--r--   0        0        0     8044 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/processes.py
--rw-r--r--   0        0        0        0 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/psql/__init__.py
--rw-r--r--   0        0        0     3455 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/psql/engine.py
--rw-r--r--   0        0        0     2002 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/psql/models.py
--rw-r--r--   0        0        0      356 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/psql/settings.py
--rw-r--r--   0        0        0      223 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/register.py
--rw-r--r--   0        0        0     1134 2024-03-28 13:46:48.647762 openeo_fastapi-2024.3.2/openeo_fastapi/client/settings.py
--rw-r--r--   0        0        0     1411 2024-03-28 13:46:48.651762 openeo_fastapi-2024.3.2/pyproject.toml
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 openeo_fastapi-2024.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-08 12:01:39.406196 openeo_fastapi-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     2191 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/api/__init__.py
+-rw-r--r--   0        0        0    19123 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/api/app.py
+-rw-r--r--   0        0        0    21803 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/api/models.py
+-rw-r--r--   0        0        0    18134 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/api/types.py
+-rw-r--r--   0        0        0     1778 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/__init__.py
+-rw-r--r--   0        0        0     7732 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/auth.py
+-rw-r--r--   0        0        0     6469 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/collections.py
+-rw-r--r--   0        0        0     6361 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/core.py
+-rw-r--r--   0        0        0     3408 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/files.py
+-rw-r--r--   0        0        0    13680 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/jobs.py
+-rw-r--r--   0        0        0    11239 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/processes.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/psql/__init__.py
+-rw-r--r--   0        0        0     5077 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/psql/engine.py
+-rw-r--r--   0        0        0     2493 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/psql/models.py
+-rw-r--r--   0        0        0      828 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/psql/settings.py
+-rw-r--r--   0        0        0      737 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/register.py
+-rw-r--r--   0        0        0     2257 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/client/settings.py
+-rw-r--r--   0        0        0     1426 2024-04-08 12:01:39.410196 openeo_fastapi-2024.4.1/openeo_fastapi/templates.py
+-rw-r--r--   0        0        0     1525 2024-04-08 12:01:39.414196 openeo_fastapi-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 openeo_fastapi-2024.4.1/PKG-INFO
```

### Comparing `openeo_fastapi-2024.3.2/LICENSE` & `openeo_fastapi-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.3.2/README.md` & `openeo_fastapi-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.3.2/openeo_fastapi/api/app.py` & `openeo_fastapi-2024.4.1/openeo_fastapi/api/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,526 +1,432 @@
+"""OpenEO Api class for preparing the FastApi object from the client that is provided by the user.
+"""
 import attr
 from fastapi import APIRouter, HTTPException, Response
 from starlette.responses import JSONResponse
 
-from openeo_fastapi.api import responses
+from openeo_fastapi.api import models
 
 HIDDEN_PATHS = ["/openapi.json", "/docs", "/docs/oauth2-redirect", "/redoc"]
 
-
 @attr.define
 class OpenEOApi:
     """Factory for creating FastApi applications conformant to the OpenEO Api specification."""
 
     client: attr.field
     app: attr.field
     router: APIRouter = attr.ib(default=attr.Factory(APIRouter))
     response_class: type[Response] = attr.ib(default=JSONResponse)
 
     def register_well_known(self):
-        """Register well known page (GET /).
-
-
-        Returns:
-            None
+        """Register well known endpoint (GET /.well-known/openeo).
         """
         self.router.add_api_route(
             name=".well-known",
             path="/.well-known/openeo",
-            response_model=responses.WellKnownOpeneoGetResponse,
+            response_model=models.WellKnownOpeneoGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_well_known,
         )
 
     def register_get_capabilities(self):
-        """Register landing page (GET /).
-
-        Returns:
-            None
-        """
+        """Register endpoint for capabilities (GET /)."""
         self.router.add_api_route(
             name="capabilities",
             path=f"/{self.client.settings.OPENEO_VERSION}" + "/",
-            response_model=responses.Capabilities,
+            response_model=models.Capabilities,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_capabilities,
         )
 
     def register_get_conformance(self):
-        """Register conformance page (GET /conformance).
-        Returns:
-            None
-        """
+        """Register endpoint for api conformance (GET /conformance)."""
         self.router.add_api_route(
             name="conformance",
             path=f"/{self.client.settings.OPENEO_VERSION}/conformance",
-            response_model=responses.ConformanceGetResponse,
+            response_model=models.ConformanceGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_conformance,
         )
 
     def register_get_file_formats(self):
-        """Register supported file formats page (GET /file_formats).
-        Returns:
-            None
-        """
+        """Register endpoint for supported file formats (GET /file_formats)."""
         self.router.add_api_route(
             name="file_formats",
             path=f"/{self.client.settings.OPENEO_VERSION}/file_formats",
-            response_model=responses.FileFormatsGetResponse,
+            response_model=models.FileFormatsGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_file_formats,
         )
 
     def register_get_health(self):
-        """Register api health endpoint (GET /health).
-        Returns:
-            None
-        """
+        """Register endpoint for api health (GET /health)."""
         self.router.add_api_route(
             name="health",
             path=f"/{self.client.settings.OPENEO_VERSION}/health",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_health,
         )
 
     def register_get_user_info(self):
-        """Register conformance page (GET /me).
-        Returns:
-            None
-        """
+        """Register endpoint for user info (GET /me)."""
         self.router.add_api_route(
             name="me",
             path=f"/{self.client.settings.OPENEO_VERSION}/me",
-            response_model=responses.MeGetResponse,
+            response_model=models.MeGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.get_user_info,
         )
 
     def register_get_udf_runtimes(self):
-        """Register supported udf runtimes (GET /udf_runtimes).
-        Returns:
-            None
-        """
+        """Register endpoint to list the supported udf runtimes (GET /udf_runtimes)."""
         self.router.add_api_route(
             name="udf_runtimes",
             path=f"/{self.client.settings.OPENEO_VERSION}/udf_runtimes",
-            response_model=responses.UdfRuntimesGetResponse,
+            response_model=models.UdfRuntimesGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
-            endpoint=self.client.udf_runtimes,
+            endpoint=self.client.get_udf_runtimes,
         )
 
     def register_validate_user_process_graph(self):
-        """Register validate user process graph (GET /validation).
-        Returns:
-            None
-        """
+        """Register endpoint for validating a user process graph (GET /validation)."""
         self.router.add_api_route(
             name="validation",
             path=f"/{self.client.settings.OPENEO_VERSION}/validation",
-            response_model=responses.ValidationPostResponse,
+            response_model=models.ValidationPostResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=self.client.processes.validate_user_process_graph,
         )
 
     def register_run_sync_job(self):
-        """Register run synchronous job (GET /result).
-        Returns:
-            None
-        """
+        """Register endpoint for executing synchronous jobs (GET /result)."""
         self.router.add_api_route(
             name="result",
             path=f"/{self.client.settings.OPENEO_VERSION}/result",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=self.client.jobs.process_sync_job,
         )
 
     def register_get_collections(self):
-        """Register collection Endpoint (GET /collections).
-        Returns:
-            None
-        """
+        """Register endpoint for listing available collections (GET /collections)."""
         self.router.add_api_route(
             name="collections",
             path=f"/{self.client.settings.OPENEO_VERSION}/collections",
-            response_model=responses.Collections,
+            response_model=models.Collections,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.collections.get_collections,
         )
 
     def register_get_collection(self):
-        """Register Endpoint for Individual Collection (GET /collections/{collection_id}).
-        Returns:
-            None
-        """
+        """Register endpoint for getting a specific collection (GET /collections/{collection_id})."""
         self.router.add_api_route(
             name="collection",
             path=f"/{self.client.settings.OPENEO_VERSION}"
             + "/collections/{collection_id}",
-            response_model=responses.Collection,
+            response_model=models.Collection,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.collections.get_collection,
         )
 
-    def register_get_processes(self):
-        """Register Endpoint for Processes (GET /processes).
+    def register_get_collection_items(self):
+        """Register endpoint for getting collection items (GET /collections/{collection_id}/items)."""
+        self.router.add_api_route(
+            name="collection_items",
+            path=f"/{self.client.settings.OPENEO_VERSION}/collections"
+            + "/{collection_id}/items",
+            response_model=models.Collections,
+            response_model_exclude_unset=False,
+            response_model_exclude_none=True,
+            methods=["GET"],
+            endpoint=self.client.collections.get_collection_items,
+        )
 
-        Returns:
-            None
-        """
+    def register_get_collection_item(self):
+        """Register endpoint for getting a specific collection item (GET /collections/{collection_id}/items/{item_id})."""
+        self.router.add_api_route(
+            name="collection_item",
+            path=f"/{self.client.settings.OPENEO_VERSION}"
+            + "/collections/{collection_id}/items/{item_id}",
+            response_model=models.Collection,
+            response_model_exclude_unset=False,
+            response_model_exclude_none=True,
+            methods=["GET"],
+            endpoint=self.client.collections.get_collection_item,
+        )
+
+    def register_get_processes(self):
+        """Register endpoint for listing all predefined processes (GET /processes)."""
         self.router.add_api_route(
             name="processes",
             path=f"/{self.client.settings.OPENEO_VERSION}/processes",
-            response_model=responses.ProcessesGetResponse,
+            response_model=models.ProcessesGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.processes.list_processes,
         )
 
     def register_list_user_process_graphs(self):
-        """Register Endpoint for User Processes Graphs (GET /processes_graphs).
-
-        Returns:
-            None
-        """
+        """Register endpoint for listing user defined processes graphs (GET /processes_graphs)."""
         self.router.add_api_route(
             name="list_user_process_graphs",
             path=f"/{self.client.settings.OPENEO_VERSION}/process_graphs",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.processes.list_user_process_graphs,
         )
 
     def register_get_user_process_graph(self):
-        """Register Endpoint for User Processes Graphs (GET /processes_graphs/{process_graph_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for getting a specific user defined processes graphs (GET /processes_graphs/{process_graph_id})."""
         self.router.add_api_route(
             name="get_user_process_graphs",
             path=f"/{self.client.settings.OPENEO_VERSION}/process_graphs"
             + "/{process_graph_id}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.processes.get_user_process_graph,
         )
 
     def register_put_user_process_graph(self):
-        """Register Endpoint for User Processes Graphs (PUT /processes_graphs/{process_graph_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for creatings a user defined processes graph (PUT /processes_graphs/{process_graph_id})."""
         self.router.add_api_route(
             name="put_user_process_graphs",
             path=f"/{self.client.settings.OPENEO_VERSION}/process_graphs"
             + "/{process_graph_id}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["PUT"],
             endpoint=self.client.processes.put_user_process_graph,
         )
 
     def register_delete_user_process_graph(self):
-        """Register Endpoint for User Processes Graphs (DELETE /processes_graphs/{process_graph_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for deleting a user defined processes graph (DELETE /processes_graphs/{process_graph_id})."""
         self.router.add_api_route(
             name="delete_user_process_graphs",
             path=f"/{self.client.settings.OPENEO_VERSION}/process_graphs"
             + "/{process_graph_id}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=self.client.processes.delete_user_process_graph,
         )
 
     def register_get_jobs(self):
-        """Register Endpoint for Jobs (GET /jobs).
-
-        Returns:
-            None
-        """
+        """Register endpoint for listing all jobs (GET /jobs)."""
         self.router.add_api_route(
             name="get_jobs",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs",
-            response_model=responses.JobsGetResponse,
+            response_model=models.JobsGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.jobs.list_jobs,
         )
 
     def register_create_job(self):
-        """Register Endpoint for Jobs (POST /jobs).
-
-        Returns:
-            None
-        """
+        """Register endpoint for creating a new job (POST /jobs)."""
         self.router.add_api_route(
             name="post_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=self.client.jobs.create_job,
         )
 
     def register_update_job(self):
-        """Register Endpoint for Jobs (POST /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register update jobs endpoint (POST /jobs/{job_id})."""
         self.router.add_api_route(
             name="post_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["PATCH"],
             endpoint=self.client.jobs.update_job,
         )
 
     def register_get_job(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for retreiving job metadata (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="get_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}",
-            response_model=responses.BatchJob,
+            response_model=models.BatchJob,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.jobs.get_job,
         )
 
     def register_delete_job(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for deleting the record of a batch job (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="delete_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=self.client.jobs.delete_job,
         )
 
     def register_get_estimate(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for estimating a batch job (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="get_estimate",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}/estimate",
-            response_model=responses.JobsGetEstimateGetResponse,
+            response_model=models.JobsGetEstimateGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.jobs.estimate,
         )
 
     def register_get_logs(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for retrieving job logs (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="get_logs",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}/logs",
-            response_model=responses.JobsGetLogsResponse,
+            response_model=models.JobsGetLogsResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.jobs.logs,
         )
 
     def register_get_results(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for getting the results from a batch job (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="get_results",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}/results",
-            response_model=responses.Collection,
+            response_model=models.Collection,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.jobs.get_results,
         )
 
     def register_start_job(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for starting batch job processing (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="start_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}/results",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=self.client.jobs.start_job,
         )
 
     def register_cancel_job(self):
-        """Register Endpoint for Jobs (GET /jobs/{job_id}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for cancelling job processing (GET /jobs/{job_id})."""
         self.router.add_api_route(
             name="cancel_job",
             path=f"/{self.client.settings.OPENEO_VERSION}/jobs" + "/{job_id}/results",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=self.client.jobs.cancel_job,
         )
 
     def register_list_files(self):
-        """Register Endpoint for Files (GET /files).
-
-        Returns:
-            None
-        """
+        """Register endpoint for listing a user's fils (GET /files)."""
         self.router.add_api_route(
             name="list_files",
             path=f"/{self.client.settings.OPENEO_VERSION}/files",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.files.list_files,
         )
 
     def register_download_file(self):
-        """Register Endpoint for Files (GET /files/{path}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for downloading a specific file (GET /files/{path})."""
         self.router.add_api_route(
             name="download_file",
             path=f"/{self.client.settings.OPENEO_VERSION}/files" + "/{path}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=self.client.files.download_file,
         )
 
     def register_upload_file(self):
-        """Register Endpoint for Files (PUT /files/{path}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for uploading a new file (PUT /files/{path})."""
         self.router.add_api_route(
             name="upload_file",
             path=f"/{self.client.settings.OPENEO_VERSION}/files" + "/{path}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["PUT"],
             endpoint=self.client.files.upload_file,
         )
 
     def register_delete_file(self):
-        """Register Endpoint for Files (DELETE /files/{path}).
-
-        Returns:
-            None
-        """
+        """Register endpoint for deleting a new file (DELETE /files/{path})."""
         self.router.add_api_route(
             name="delete_file",
             path=f"/{self.client.settings.OPENEO_VERSION}/files" + "/{path}",
             response_model=None,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=self.client.files.delete_file,
         )
 
     def register_core(self):
-        """Register core OpenEO endpoints.
-
-            GET /
-            GET /capabilities
-            GET /collections
-            GET /collections/{collection_id}
-            GET /processes
-            GET /well_known
-
-
-        Injects application logic (OpenEOApi.client) into the API layer.
-
-        Returns:
-            None
+        """
+            Add application logic to the API layer.
         """
         self.register_get_conformance()
         self.register_get_health()
         self.register_get_user_info()
         self.register_run_sync_job()
         self.register_get_udf_runtimes()
         self.register_validate_user_process_graph()
         self.register_get_file_formats()
         self.register_get_collections()
         self.register_get_collection()
+        self.register_get_collection_items()
+        self.register_get_collection_item()
         self.register_get_processes()
         self.register_list_user_process_graphs()
         self.register_get_user_process_graph()
         self.register_put_user_process_graph()
         self.register_delete_user_process_graph()
         self.register_get_jobs()
         self.register_create_job()
@@ -535,36 +441,32 @@
         self.register_list_files()
         self.register_download_file()
         self.register_upload_file()
         self.register_delete_file()
         self.register_well_known()
 
     def http_exception_handler(self, request, exception):
-        """Register exception handler to turn python exceptions into expected OpenEO error output."""
+        """
+            Register exception handler to turn python exceptions into expected OpenEO error output.
+        """
+        
         exception_headers = {
             "allow_origin": "*",
             "allow_credentials": "true",
             "allow_methods": "*",
         }
         from fastapi.encoders import jsonable_encoder
-
         return JSONResponse(
             headers=exception_headers,
             status_code=exception.status_code,
             content=jsonable_encoder(exception.detail),
         )
 
     def __attrs_post_init__(self):
-        """Post-init hook.
-
-        Responsible for setting up the application upon instantiation of the class.
-
-        Returns:
-            None
         """
-
+            Post-init hook responsible for setting up the application upon instantiation of the class.
+        """
         # Register core endpoints
         self.register_core()
-
         self.register_get_capabilities()
         self.app.include_router(router=self.router)
         self.app.add_exception_handler(HTTPException, self.http_exception_handler)
```

### Comparing `openeo_fastapi-2024.3.2/openeo_fastapi/api/responses.py` & `openeo_fastapi-2024.4.1/openeo_fastapi/api/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+"""Pydantic Models describing different api request and response bodies."""
 import uuid
-from enum import Enum
-from typing import Any, Dict, List, Optional, TypedDict, Union
 
 from pydantic import AnyUrl, BaseModel, Extra, Field, validator
+from typing import Any, Optional, TypedDict, Union
 
 from openeo_fastapi.api.types import (
     Billing,
+    Dimension,
     Endpoint,
     Error,
+    Extent,
     File,
     FileFormat,
     Link,
     Process,
     RFC3339Datetime,
+    StacProvider,
     Status,
-    Storage1,
-    Type1,
-    Type2,
+    Storage,
     Type5,
+    Version,
     Usage,
 )
 
-
+###########
+# Base
+###########
 class Capabilities(BaseModel):
+    """Response model for GET (/)."""
     api_version: str = Field(
         ...,
         description="Version number of the openEO specification this back-end implements.",
     )
     backend_version: str = Field(
         ...,
         description="Version number of the back-end implementation.\nEvery change on back-end side MUST cause a change of the version number.",
@@ -106,151 +111,83 @@
                 "href": "http://www.cool-cloud-corp.com/api/v1.0/collections",
                 "rel": "data",
                 "type": "application/json",
                 "title": "List of Datasets",
             },
         ],
     )
+    
 
-
-class ConformanceGetResponse(BaseModel):
-    conformsTo: list[AnyUrl]
-
-
-class Version(BaseModel):
-    url: AnyUrl = Field(
-        ...,
-        description="*Absolute* URLs to the service.",
-        example="https://example.com/api/v1.0",
-    )
-    production: Optional[bool] = None
-    api_version: str = Field(
-        ...,
-        description="Version number of the openEO specification this back-end implements.",
-    )
-
-
-class WellKnownOpeneoGetResponse(BaseModel):
-    versions: list[Version]
-
-
-#############
-# Collections
-#############
-class Role(Enum):
-    producer = "producer"
-    licensor = "licensor"
-    processor = "processor"
-    host = "host"
-
-
-class StacProvider(BaseModel):
-    name: str = Field(
-        ...,
-        description="The name of the organization or the individual.",
-        example="Cool EO Cloud Corp",
-    )
-    description: Optional[str] = Field(
+class MeGetResponse(BaseModel):
+    """Response model for GET (/me)."""
+    user_id: uuid.UUID
+    name: Optional[str] = Field(
         None,
-        description=(
-            "Multi-line description to add further provider information such as processing details for "
-            "processors and producers, hosting details for hosts or basic contact information."
-            "CommonMark 0.29 syntax MAY be used for rich text representation."
-        ),
-        example="No further processing applied.",
+        description="The user name, a human-friendly displayable name. Could be the user's real name or a nickname.",
     )
-    roles: Optional[list[Role]] = Field(
+    default_plan: Optional[str] = Field(
         None,
-        description=(
-            "Roles of the provider.\n\nThe provider's role(s) can be one or more of the following "
-            "elements:\n* licensor: The organization that is licensing the dataset under the license"
-            "specified in the collection's license field.\n* producer: The producer of the data is the"
-            "provider that initially captured and processed the source data, e.g. ESA for Sentinel-2 data."
-            "* processor: A processor is any provider who processed data to a derived product.\n* host: The"
-            "host is the actual provider offering the data on their storage. There SHOULD be no more than"
-            "one host, specified as last element of the list."
-        ),
-        example=["producer", "licensor", "host"],
+        description="Name of the plan the user has subscribed to.\n\nOverrides the default plan of the back-end, but back-ends\nMAY also allow overriding this plan for each individual\nprocessing request (e.g. job or service) with the\ncorresponding `plan` property.",
+        example="free",
     )
-    url: Optional[AnyUrl] = Field(
+    storage: Optional[Storage] = Field(
         None,
-        description=(
-            "Homepage on which the provider describes the dataset and publishes contact information."
-        ),
-        example="http://cool-eo-cloud-corp.com",
-    )
-
-
-class StacProviders(BaseModel):
-    __root__: list[StacProvider] = Field(
-        ...,
-        description=(
-            "A list of providers, which MAY include all organizations capturing or processing "
-            "the data or the hosting provider. Providers SHOULD be listed in chronological order"
-            "with the most recent provider being the last element of the list."
-        ),
+        description="Information about the storage space available to the user.",
+        title="User Storage",
     )
-
-
-class Dimension(BaseModel):
-    type: Type2 = Field(..., description="Type of the dimension.")
-    description: Optional[str] = None
-
-
-class Spatial(BaseModel):
-    bbox: Optional[list[list[float]]] = Field(
+    budget: Optional[float] = None
+    links: Optional[list[Link]] = Field(
         None,
-        description=(
-            "One or more bounding boxes that describe the spatial extent\nof the dataset."
-            "The first bounding box describes the overall spatial extent\nof the data. All "
-            "subsequent bounding boxes describe more\nprecise bounding boxes, e.g. to identify "
-            "clusters of data.\nClients only interested in the overall spatial extent will "
-            "only need to access the first item in each array."
-        ),
-        min_items=1,
+        description="Links related to the user profile, e.g. where payments\nare handled or the user profile could be edited.\n\nIt is RECOMMENDED to provide links with the following `rel` (relation) types:\n\n1. `payment`: A page where users can recharge their user account with money or credits.\n\n2. `edit-form`: Points to a page where the user can edit his user profile.\n\nFor additional relation types see also the lists of\n[common relation types in openEO](#section/API-Principles/Web-Linking).",
+        example=[
+            {"href": "https://example.openeo.org/john_doe/payment/", "rel": "payment"},
+            {"href": "https://example.openeo.org/john_doe/edit/", "rel": "edit-form"},
+            {
+                "href": "https://example.openeo.org/john_doe/",
+                "rel": "alternate",
+                "type": "text/html",
+                "title": "User profile",
+            },
+            {
+                "href": "https://example.openeo.org/john_doe.vcf",
+                "rel": "alternate",
+                "type": "text/vcard",
+                "title": "vCard of John Doe",
+            },
+        ],
     )
 
 
-class Temporal(BaseModel):
-    interval: Optional[list[list[Any]]] = Field(
-        None,
-        description=(
-            "One or more time intervals that describe the temporal extent of the dataset."
-            "The first time interval describes the overall temporal extent of the data. "
-            "All subsequent time intervals describe more precise time intervals, e.g. to "
-            "identify clusters of data. Clients only interested in the overall extent will"
-            "only need to access the first item in each array."
-        ),
-        min_items=1,
-    )
+class ConformanceGetResponse(BaseModel):
+    """Response model for GET (/conformance)."""
+    conformsTo: list[AnyUrl]
 
 
-class Extent(BaseModel):
-    spatial: Spatial = Field(
-        ...,
-        description="The *potential* spatial extents of the features in the collection.",
-        title="Collection Spatial Extent",
-    )
-    temporal: Temporal = Field(
-        ...,
-        description="The *potential* temporal extents of the features in the collection.",
-        title="Collection Temporal Extent",
-    )
+class WellKnownOpeneoGetResponse(BaseModel):
+    """Response model for GET (/.well-known/openeo)."""
+    versions: list[Version]
+    
 
+class UdfRuntimesGetResponse(BaseModel):
+    """Response model for GET (/udf_runtimes)."""
+    pass
 
-class CollectionSummaryStats(BaseModel):
-    min: Union[str, float] = Field(alias="minimum")
-    max: Union[str, float] = Field(alias="maximum")
+    class Config:
+        extra = Extra.allow
 
 
+#############
+# Collections
+#############
 class Collection(BaseModel):
+    """Response model for GET (/collection/{collection_id})"""
     stac_version: str
     stac_extensions: Optional[list[Union[AnyUrl, str]]] = None
-    type: Optional[Type1] = Field(
-        None, description="For STAC versions >= 1.0.0-rc.1 this field is required."
+    type: str = Field(
+        description="For STAC versions >= 1.0.0-rc.1 this field is required.", default="Collection"
     )
     id: str
     title: Optional[str] = Field(
         None, description="A short descriptive one-line title for the collection."
     )
     description: str = Field(
         ...,
@@ -279,15 +216,15 @@
             "the\nlinks and MUST refer to the collection that can be used instead.\n\nThis property "
             "REQUIRES to add `version` (STAC < 1.0.0-rc.1) or\n"
             "`https://stac-extensions.github.io/version/v1.0.0/schema.json` (STAC >= 1.0.0-rc.1)\n"
             "to the list of `stac_extensions`."
         ),
     )
     license: str
-    providers: Optional[StacProviders] = None
+    providers: Optional[list[StacProvider]] = None
     extent: Extent = Field(
         ...,
         description=(
             "The extent of the data in the collection. Additional members MAY\nbe added to "
             "represent other extents, for example, thermal or\npressure ranges.\n\nThe first "
             "item in the array always describes the overall extent of\nthe data. All subsequent "
             "items describe more preciseextents,\ne.g. to identify clusters of data.\nClients only "
@@ -324,15 +261,15 @@
             "with the axis set to `x`\n* `y` for the dimension of type `spatial` with the axis set to `y`* "
             "`z` for the dimension of type `spatial` with the axis set to `z`\n* `t` for the dimension of "
             " type `temporal` * `bands` for dimensions of type `bands`\n\nThis property REQUIRES to add "
             "`datacube` to the list of `stac_extensions`."
         ),
         title="STAC Collection Cube Dimensions",
     )
-    summaries: Optional[dict[str, Union[list[Any], CollectionSummaryStats]]] = Field(
+    summaries: Optional[dict[str, Union[list[Any], Any]]] = Field(
         None,
         description=(
             "Collection properties from STAC extensions (e.g. EO,SAR, Satellite or Scientific) or even "
             "custom extensions.Summaries are either a unique set of all available\nvalues *or* "
             "statistics. Statistics by default only specify the range (minimum and maximum values), "
             "but can optionally be accompanied by additional statistical values. The range can specify"
             "the potential range of values, but it is recommended to be as precise as possible. The set "
@@ -358,53 +295,64 @@
 
     class Config:
         extra = Extra.allow
         allow_population_by_field_name = True
 
 
 class Collections(TypedDict, total=False):
+    """Response model for GET (/collections)."""
     collections: list[Collection]
     links: list[dict[str, Any]]
 
 
 ###########
 # Processes
 ###########
 class ProcessesGetResponse(BaseModel):
+    """Response model for GET (/processes)."""
     processes: list[Process]
     links: list[Link]
 
 
 class ProcessGraphWithMetadata(Process):
+    """Reponse model for
+                GET (/process_graphs/{process_graph_id})
+    
+    Request model for
+            PUT (/process_graphs/{process_graph_id})
+            POST (/validation)
+    """
     id: str = Field(default=None, alias="id")
     summary: Optional[Any] = None
     description: Optional[Any] = None
     parameters: Optional[Any] = None
     returns: Optional[Any] = None
     process_graph: Any = None
 
     class Config:
         allow_population_by_field_name = True
 
 
 class ProcessGraphsGetResponse(BaseModel):
+    """Response model for GET (/process_graphs)."""
     processes: list[ProcessGraphWithMetadata] = Field(
         ..., description="Array of user-defined processes"
     )
     links: list[Link]
 
 
 class ValidationPostResponse(BaseModel):
+    """Response model for POST (/validation)."""
     errors: list[Error] = Field(..., description="A list of validation errors.")
 
-
 ###########
 # Jobs
 ###########
 class BatchJob(BaseModel):
+    """Reponse model for GET (/jobs/{job_id})."""
     job_id: uuid.UUID = Field(default=None, alias="id")
     title: Optional[str] = None
     description: Optional[str] = None
     process: Optional[ProcessGraphWithMetadata] = None
     status: Status
     progress: Optional[float] = Field(
         None,
@@ -431,24 +379,27 @@
             raise ValueError(f"Job id can only be of type UUID or str.")
 
     class Config:
         allow_population_by_field_name = True
 
 
 class JobsGetResponse(BaseModel):
+    """Reponse model for GET (/jobs)."""
     jobs: list[BatchJob]
     links: list[Link]
 
 
 class JobsGetLogsResponse(BaseModel):
+    """Reponse model for GET (/jobs/{job_id}/logs)."""
     logs: list[Any]
     links: list[Link]
 
 
 class JobsGetEstimateGetResponse(BaseModel):
+    """Reponse model for GET (/jobs/{job_id}/estimate)."""
     costs: Optional[float] = None
     duration: Optional[str] = Field(
         None,
         description="Estimated duration for the operation. Duration MUST be specified as a ISO 8601 duration.",
         example="P1Y2M10DT2H30M",
     )
     size: Optional[int] = Field(
@@ -464,69 +415,41 @@
     expires: Optional[RFC3339Datetime] = Field(
         None,
         description="Time until which the estimate is valid, formatted as a [RFC 3339](https://www.rfc-editor.org/rfc/RFC3339Datetime.html) date-time.",
         example="2020-11-01T00:00:00Z",
     )
 
 
+class JobsRequest(BaseModel):
+    """Request model for
+            POST (/jobs)
+            PATCH (/jobs/{job_id})
+            POST (/result)
+    """
+    title: str = None
+    description: Optional[str] = None
+    process: Optional[ProcessGraphWithMetadata] = None
+    plan: Optional[str] = None
+    budget: Optional[str] = None
+
+###########
+# Files
+###########
 class FilesGetResponse(BaseModel):
+    """Reponse model for GET (/files)."""
     files: list[File]
     links: list[Link]
 
 
 class FileFormatsGetResponse(BaseModel):
+    """Reponse model for GET (/file_formats)."""
     input: dict[str, FileFormat] = Field(
         ...,
         description="Map of supported input file formats, i.e. file formats a back-end can **read** from. The property keys are the file format names that are used by clients and users, for example in process graphs.",
         title="Input File Formats",
     )
     output: dict[str, FileFormat] = Field(
         ...,
         description="Map of supported output file formats, i.e. file formats a back-end can **write** to. The property keys are the file format names that are used by clients and users, for example in process graphs.",
         title="Output File Formats",
     )
 
-
-class MeGetResponse(BaseModel):
-    user_id: uuid.UUID
-    name: Optional[str] = Field(
-        None,
-        description="The user name, a human-friendly displayable name. Could be the user's real name or a nickname.",
-    )
-    default_plan: Optional[str] = Field(
-        None,
-        description="Name of the plan the user has subscribed to.\n\nOverrides the default plan of the back-end, but back-ends\nMAY also allow overriding this plan for each individual\nprocessing request (e.g. job or service) with the\ncorresponding `plan` property.",
-        example="free",
-    )
-    storage: Optional[Storage1] = Field(
-        None,
-        description="Information about the storage space available to the user.",
-        title="User Storage",
-    )
-    budget: Optional[float] = None
-    links: Optional[list[Link]] = Field(
-        None,
-        description="Links related to the user profile, e.g. where payments\nare handled or the user profile could be edited.\n\nIt is RECOMMENDED to provide links with the following `rel` (relation) types:\n\n1. `payment`: A page where users can recharge their user account with money or credits.\n\n2. `edit-form`: Points to a page where the user can edit his user profile.\n\nFor additional relation types see also the lists of\n[common relation types in openEO](#section/API-Principles/Web-Linking).",
-        example=[
-            {"href": "https://example.openeo.org/john_doe/payment/", "rel": "payment"},
-            {"href": "https://example.openeo.org/john_doe/edit/", "rel": "edit-form"},
-            {
-                "href": "https://example.openeo.org/john_doe/",
-                "rel": "alternate",
-                "type": "text/html",
-                "title": "User profile",
-            },
-            {
-                "href": "https://example.openeo.org/john_doe.vcf",
-                "rel": "alternate",
-                "type": "text/vcard",
-                "title": "vCard of John Doe",
-            },
-        ],
-    )
-
-
-class UdfRuntimesGetResponse(BaseModel):
-    pass
-
-    class Config:
-        extra = Extra.allow
```

### Comparing `openeo_fastapi-2024.3.2/openeo_fastapi/api/types.py` & `openeo_fastapi-2024.4.1/openeo_fastapi/api/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,107 @@
+"""Pydantic Models and Enums describining different attribute types used by the models in openeo_fastapi.api.models."""
 import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 from pydantic import AnyUrl, BaseModel, Extra, Field, validator
 
 
-class JsonSchemaType(Enum):
-    array = "array"
-    boolean = "boolean"
-    integer = "integer"
-    null = "null"
-    number = "number"
-    object = "object"
-    string = "string"
+class STACConformanceClasses(Enum):
+    """Available conformance classes with STAC."""
+    CORE = "https://api.stacspec.org/v1.0.0/core"
+    COLLECTIONS = "https://api.stacspec.org/v1.0.0/collections"
 
 
-class Type1(Enum):
-    Collection = "Collection"
-
-
-class Type2(Enum):
+class DinensionEnum(Enum):
+    """Dimension enum."""
     spatial = "spatial"
     temporal = "temporal"
     bands = "bands"
     other = "other"
 
 
 class Type5(Enum):
+    """Catalog enum."""
     Catalog = "Catalog"
 
 
 class Method(Enum):
+    """HTTP Methods enum."""
     GET = "GET"
     HEAD = "HEAD"
     POST = "POST"
     PATCH = "PATCH"
     PUT = "PUT"
     DELETE = "DELETE"
     OPTIONS = "OPTIONS"
 
 
 class Status(Enum):
+    """Job Status enum."""
     created = "created"
     queued = "queued"
     running = "running"
     canceled = "canceled"
     finished = "finished"
     error = "error"
 
 
 class Level(Enum):
+    """Log level enum."""
     error = "error"
     warning = "warning"
     info = "info"
     debug = "debug"
 
 
 class GisDataType(Enum):
+    """Data type enum."""
     raster = "raster"
     vector = "vector"
     table = "table"
     other = "other"
 
+class Role(Enum):
+    """Role for collection provider."""
+    producer = "producer"
+    licensor = "licensor"
+    processor = "processor"
+    host = "host"
+
 
 class RFC3339Datetime(BaseModel):
-    """Class to consistently represent datetimes as strings compliant to RFC3339Datetime."""
+    """Model to consistently represent datetimes as strings compliant to RFC3339Datetime."""
 
     __root__: str = Field(
         description="", regex=r"[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z"
     )
 
     @validator("__root__", pre=True)
     def ensure_non_fractional_and_timezone(cls, v):
         if isinstance(v, datetime.datetime):
             return v.strftime("%Y-%m-%dT%H:%M:%SZ")
         return v
 
 
-class JsonSchema(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    type: Optional[Union[JsonSchemaType, list[JsonSchemaType]]] = Field(
-        None,
-        description="The allowed basic data type(s) for a value according to [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.1.1).\n\nIf this property is not present, all data types are allowed.",
-    )
-    subtype: Optional[str] = Field(
-        None,
-        description="The allowed sub data type for a value. See the chapter on [subtypes](#section/Processes/Defining-Processes) for more information.",
-    )
-    pattern: Optional[str] = Field(
-        None,
-        description="The regular expression a string value must match against. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.3.3).",
-    )
-    enum: Optional[list] = Field(
-        None,
-        description="An exclusive list of allowed values. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.1.2).",
-    )
-    minimum: Optional[float] = Field(
-        None,
-        description="The minimum value (inclusive) allowed for a numerical value. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.2.4).",
-    )
-    maximum: Optional[float] = Field(
-        None,
-        description="The maximum value (inclusive) allowed for a numerical value. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.2.2).",
-    )
-    minItems: Optional[float] = Field(
-        None,
-        ge=0.0,
-        description="The minimum number of items required in an array. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.4.4).",
-    )
-    maxItems: Optional[float] = Field(
-        None,
-        ge=0.0,
-        description="The maximum number of items required in an array. See [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.4.3).",
-    )
-    items: Optional[Union[list[dict], dict]] = Field(
-        None,
-        description="Specifies schemas for the items in an array according to [JSON Schema draft-07](https://json-schema.org/draft-07/json-schema-validation.html#rfc.section.6.4.1).",
-    )
-    deprecated: Optional[bool] = None
-
-
 class Endpoint(BaseModel):
+    """Model to capture the available endpoint and it's accepted models."""
     path: str = Field(
         ...,
         description="Path to the endpoint, relative to the URL of this endpoint. In general the paths MUST follow the paths specified in the openAPI specification as closely as possible. Therefore, paths MUST be prepended with a leading slash, but MUST NOT contain a trailing slash. Variables in the paths MUST be placed in curly braces and follow the parameter names in the openAPI specification, e.g. `{job_id}`.",
     )
     methods: list[Method] = Field(
         ...,
         description="Supported HTTP verbs in uppercase. It is OPTIONAL to list `OPTIONS` as method (see the [CORS section](#section/Cross-Origin-Resource-Sharing-(CORS))).",
     )
 
 
 class Plan(BaseModel):
+    """Model to capture the the plan the user has subscribe to."""
     name: str = Field(
         ...,
         description="Name of the plan. It MUST be accepted in a *case insensitive* manner throughout the API.",
         example="free",
     )
     description: str = Field(
         ...,
@@ -153,14 +116,15 @@
         None,
         description="URL to a web page with more details about the plan.",
         example="http://cool-cloud-corp.com/plans/free-plan",
     )
 
 
 class Billing(BaseModel):
+    """Model to capture the billing options that are available at the backend."""
     currency: str = Field(
         ...,
         description="The currency the back-end is billing in. The currency MUST be either a valid currency code as defined in ISO-4217 or a proprietary currency, e.g. tiles or back-end specific credits. If set to the default value `null`, budget and costs are not supported by the back-end and users can't be charged.",
         example="USD",
     )
     default_plan: Optional[str] = Field(
         None,
@@ -184,33 +148,36 @@
                 "paid": True,
             },
         ],
     )
 
 
 class File(BaseModel):
+    """Model to capture the stat information of a file stored at the backend."""
     path: str = Field(
         ...,
         description="Path of the file, relative to the root directory of the user's server-side workspace.\nMUST NOT start with a slash `/` and MUST NOT be url-encoded.\n\nThe Windows-style path name component separator `\\` is not supported,\nalways use `/` instead.\n\nNote: The pattern only specifies a minimal subset of invalid characters.\nThe back-ends MAY enforce additional restrictions depending on their OS/environment.",
         example="folder/file.txt",
     )
     size: Optional[int] = Field(None, description="File size in bytes.", example=1024)
     modified: Optional[RFC3339Datetime] = Field(
         None,
         description="Date and time the file has lastly been modified, formatted as a [RFC 3339](https://www.rfc-editor.org/rfc/RFC3339Datetime.html) date-time.",
         example="2018-01-03T10:55:29Z",
     )
 
 
 class UsageMetric(BaseModel):
+    """Model to capture the value and unit of a given metric."""
     value: float
     unit: str
 
 
 class Usage(BaseModel):
+    """Model to capture the usage of a job."""
     class Config:
         extra = Extra.allow
 
     cpu: Optional[UsageMetric] = Field(
         None,
         description="Specifies the CPU usage, usually in a unit such as `cpu-seconds`.",
     )
@@ -233,14 +200,15 @@
     storage: Optional[UsageMetric] = Field(
         None,
         description="Specifies the usage of storage space, usually in a unit such as `b` (bytes), `kb` (kilobytes), `mb` (megabytes) or `gb` (gigabytes).",
     )
 
 
 class Link(BaseModel):
+    """Model to describe the information for a provided URL."""
     rel: str = Field(
         ...,
         description="Relationship between the current document and the linked document. SHOULD be a [registered link relation type](https://www.iana.org/assignments/link-relations/link-relations.xml) whenever feasible.",
         example="related",
     )
     href: Union[AnyUrl, Path] = Field(
         ...,
@@ -254,14 +222,15 @@
     )
     title: Optional[str] = Field(
         None, description="Used as a human-readable label for a link.", example="openEO"
     )
 
 
 class LogEntry(BaseModel):
+    """Model to describe the information for a given log line in job logs."""
     id: str = Field(
         ...,
         description="An unique identifier for the log message, could simply be an incrementing number.",
         example="1",
     )
     code: Optional[str]
     level: Level = Field(
@@ -279,43 +248,45 @@
         description="The date and time the event happened, in UTC. Formatted as a [RFC 3339](https://www.rfc-editor.org/rfc/RFC3339Datetime.html) date-time.",
         title="Date and Time",
     )
     data: Optional[Any] = Field(
         None,
         description="Data of any type. It is the back-ends task to decide how to best\npresent passed data to a user.\n\nFor example, a raster-cube passed to the `debug` SHOULD return the\nmetadata similar to the collection metadata, including `cube:dimensions`.",
     )
-    path: Optional[list[JsonSchema]] = Field(
+    path: Optional[list[str]] = Field(
         None,
         description="Describes where the log entry originates from.\n\nThe first element of the array is the process that has triggered the log entry, the second element is the parent of the process that has triggered the log entry, etc. This pattern is followed until the root of the process graph.",
     )
     usage: Optional[Usage]
     links: Optional[list[Link]]
 
 
 class Process(BaseModel):
+    """Model to describe a process that is exposed by the api."""
     id: Optional[str] = None
     summary: Optional[str] = None
     description: Optional[str] = None
     categories: Optional[list[str]] = None
-    parameters: Optional[Union[JsonSchema, list[JsonSchema]]] = None
-    returns: Optional[Union[JsonSchema, list[JsonSchema]]] = None
+    parameters: Optional[list[dict[str, Union[list[Any], Any]]]] = None
+    returns: Optional[dict[str, Union[list[Any], Any]]] = None
     deprecated: Optional[bool] = None
     experimental: Optional[bool] = None
-    exceptions: Optional[Union[JsonSchema, list[JsonSchema]]] = None
-    examples: Optional[Union[JsonSchema, list[JsonSchema]]] = Field(
+    exceptions: Optional[dict[str, Union[list[Any], Any]]] = None
+    examples: Optional[list[dict[str, Union[list[Any], Any]]]] = Field(
         None, description="Examples, may be used for unit tests."
     )
     links: Optional[list[Link]] = Field(
         None,
         description="Links related to this process, e.g. additional external documentation.\nIt is RECOMMENDED to provide links with the following `rel` (relation) types:\n1. `latest-version`: If a process has been marked as deprecated, a link SHOULD point to the preferred version of the process. The relation types `predecessor-version` (link to older version) and `successor-version` (link to newer version) can also be used to show the relation between versions.\n2. `example`: Links to examples of other processes that use this process.\n3. `cite-as`: For all DOIs associated with the process, the respective DOI links SHOULD be added.\nFor additional relation types see also the lists of [common relation types in openEO](#section/API-Principles/Web-Linking).",
     )
-    process_graph: Optional[JsonSchema] = None
+    process_graph: Optional[dict[str, Union[list[Any], Any]]] = None
 
 
 class Error(BaseModel):
+    """Model to describe the information of a captured exception by the api."""
     id: Optional[str] = Field(
         None,
         description="A back-end MAY add a unique identifier to the error response to be able to log and track errors with further non-disclosable details. A client could communicate this id to a back-end provider to get further information.",
         example="550e8400-e29b-11d4-a716-446655440000",
     )
     code: str
     message: str = Field(
@@ -323,14 +294,15 @@
         description="A message explaining what the client may need to change or what difficulties the server is facing.",
         example="Parameter 'sample' is missing.",
     )
     links: Optional[list[Link]] = None
 
 
 class FileFormat(BaseModel):
+    """Model to describe a file format supported by the processing backend."""
     title: str
     description: Optional[str] = None
     gis_data_types: list[GisDataType] = Field(
         ...,
         description="Specifies the supported GIS spatial data types for this format.\nIt is RECOMMENDED to specify at least one of the data types, which will likely become a requirement in a future API version.",
     )
     deprecated: Optional[bool] = None
@@ -342,18 +314,120 @@
     )
     links: Optional[list[Link]] = Field(
         None,
         description="Links related to this file format, e.g. external documentation.\n\nFor relation types see the lists of\n[common relation types in openEO](#section/API-Principles/Web-Linking).",
     )
 
 
-class Storage1(BaseModel):
+class Storage(BaseModel):
+    """Model to describe the storage resources available to a given user."""
     free: int = Field(
         ...,
         description="Free storage space in bytes, which is still available to the user. Effectively, this is the disk quota minus the used space by the user, e.g. user-uploaded files and job results.",
         example=536870912,
     )
     quota: int = Field(
         ...,
         description="Maximum storage space (disk quota) in bytes available to the user.",
         example=1073741824,
     )
+
+
+class Version(BaseModel):
+    """Model to describe the version of an api that is available."""
+    url: AnyUrl = Field(
+        ...,
+        description="*Absolute* URLs to the service.",
+        example="https://example.com/api/v1.0",
+    )
+    production: Optional[bool] = None
+    api_version: str = Field(
+        ...,
+        description="Version number of the openEO specification this back-end implements.",
+    )
+    
+class StacProvider(BaseModel):
+    """Model to describe the provider of a given stac resource."""
+    name: str = Field(
+        ...,
+        description="The name of the organization or the individual.",
+        example="Cool EO Cloud Corp",
+    )
+    description: Optional[str] = Field(
+        None,
+        description=(
+            "Multi-line description to add further provider information such as processing details for "
+            "processors and producers, hosting details for hosts or basic contact information."
+            "CommonMark 0.29 syntax MAY be used for rich text representation."
+        ),
+        example="No further processing applied.",
+    )
+    roles: Optional[list[Role]] = Field(
+        None,
+        description=(
+            "Roles of the provider.\n\nThe provider's role(s) can be one or more of the following "
+            "elements:\n* licensor: The organization that is licensing the dataset under the license"
+            "specified in the collection's license field.\n* producer: The producer of the data is the"
+            "provider that initially captured and processed the source data, e.g. ESA for Sentinel-2 data."
+            "* processor: A processor is any provider who processed data to a derived product.\n* host: The"
+            "host is the actual provider offering the data on their storage. There SHOULD be no more than"
+            "one host, specified as last element of the list."
+        ),
+        example=["producer", "licensor", "host"],
+    )
+    url: Optional[AnyUrl] = Field(
+        None,
+        description=(
+            "Homepage on which the provider describes the dataset and publishes contact information."
+        ),
+        example="http://cool-eo-cloud-corp.com",
+    )
+
+
+class Dimension(BaseModel):
+    """Model to describe the dimension of some data."""
+    type: DinensionEnum = Field(..., description="Type of the dimension.")
+    description: Optional[str] = None
+
+
+class Spatial(BaseModel):
+    """Model to describe the spatial extent of a collection."""
+    bbox: Optional[list[list[float]]] = Field(
+        None,
+        description=(
+            "One or more bounding boxes that describe the spatial extent\nof the dataset."
+            "The first bounding box describes the overall spatial extent\nof the data. All "
+            "subsequent bounding boxes describe more\nprecise bounding boxes, e.g. to identify "
+            "clusters of data.\nClients only interested in the overall spatial extent will "
+            "only need to access the first item in each array."
+        ),
+        min_items=1,
+    )
+
+
+class Temporal(BaseModel):
+    """Model to describe the temporal range of a collection."""
+    interval: Optional[list[list[Any]]] = Field(
+        None,
+        description=(
+            "One or more time intervals that describe the temporal extent of the dataset."
+            "The first time interval describes the overall temporal extent of the data. "
+            "All subsequent time intervals describe more precise time intervals, e.g. to "
+            "identify clusters of data. Clients only interested in the overall extent will"
+            "only need to access the first item in each array."
+        ),
+        min_items=1,
+    )
+
+
+class Extent(BaseModel):
+    """Model to describe the complete spatiotemporal extent of a collection."""
+    spatial: Spatial = Field(
+        ...,
+        description="The *potential* spatial extents of the features in the collection.",
+        title="Collection Spatial Extent",
+    )
+    temporal: Temporal = Field(
+        ...,
+        description="The *potential* temporal extents of the features in the collection.",
+        title="Collection Temporal Extent",
+    )
```

### Comparing `openeo_fastapi-2024.3.2/openeo_fastapi/client/core.py` & `openeo_fastapi-2024.4.1/openeo_fastapi/client/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,148 @@
+"""Class and model to define the framework and partial application logic for interacting with Jobs.
+
+Classes:
+    - OpenEOCore: Framework for defining the application logic that will passed onto the OpenEO Api.
+"""
 from collections import namedtuple
 from typing import Optional
 from urllib.parse import urlunparse
 
 from attrs import define, field
 from fastapi import Depends, HTTPException, Response
 
-from openeo_fastapi.api import responses, types
-from openeo_fastapi.client import conformance
+from openeo_fastapi.api.models import (
+    Capabilities,
+    ConformanceGetResponse,
+    FileFormatsGetResponse,
+    MeGetResponse,
+    WellKnownOpeneoGetResponse,
+    UdfRuntimesGetResponse
+)
+from openeo_fastapi.api.types import (
+    Error,
+    STACConformanceClasses,
+    Version,
+)
 from openeo_fastapi.client.auth import Authenticator, User
 from openeo_fastapi.client.collections import CollectionRegister
 from openeo_fastapi.client.files import FilesRegister
 from openeo_fastapi.client.jobs import JobsRegister
 from openeo_fastapi.client.processes import ProcessRegister
 from openeo_fastapi.client.settings import AppSettings
 
 
 @define
 class OpenEOCore:
-    """Base client for the OpenEO Api."""
+    """Client for defining the application logic for the OpenEO Api."""
 
     billing: str = field()
     input_formats: list = field()
     output_formats: list = field()
     links: list = field()
 
-    settings = AppSettings()
+    settings: AppSettings = None
 
     _id: str = field(default="OpenEOApi")
 
     collections: Optional[CollectionRegister] = None
     files: Optional[FilesRegister] = None
     jobs: Optional[JobsRegister] = None
     processes: Optional[ProcessRegister] = None
 
     def __attrs_post_init__(self):
+        """Post init hook to set the client registers, if none where provided by the user set to the defaults!
         """
-        Post init hook to set the register objects for the class if none where provided by the user!
-        """
+        self.settings = AppSettings()
+        
         self.collections = self.collections or CollectionRegister(self.settings)
         self.files = self.files or FilesRegister(self.settings, self.links)
         self.jobs = self.jobs or JobsRegister(self.settings, self.links)
         self.processes = self.processes or ProcessRegister(self.links)
 
     def _combine_endpoints(self):
-        """For the various registers that hold endpoint functions, concat those endpoints to register in get_capabilities."""
+        """For the various registers that hold endpoint functions, concat those endpoints to register in get_capabilities.
+        
+        Returns:
+            List: A list of all the endpoints that will be supported by this api deployment.
+        """
         registers = [self.collections, self.files, self.jobs, self.processes]
 
         endpoints = []
         for register in registers:
             if register:
                 endpoints.extend(register.endpoints)
         return endpoints
 
-    def get_well_known(self) -> responses.WellKnownOpeneoGetResponse:
-        """ """
+    def get_capabilities(self) -> Capabilities:
+        """Get the capabilities of the api.
+
+        Returns:
+            Capabilities: The capabilities of the api based off what the user provided.
+        """
+        return Capabilities(
+            id=self._id,
+            title=self.settings.API_TITLE,
+            stac_version=self.settings.STAC_VERSION,
+            api_version=self.settings.OPENEO_VERSION,
+            description=self.settings.API_DESCRIPTION,
+            backend_version=self.settings.OPENEO_VERSION,
+            billing=self.billing,
+            links=self.links,
+            endpoints=self._combine_endpoints(),
+        )
+
+    def get_conformance(self) -> ConformanceGetResponse:
+        """Get the capabilities of the api.
+
+        Returns:
+            ConformanceGetResponse: The conformance classes that this Api wil of the api based off what the user provided.
+        """
+        return ConformanceGetResponse(
+            conformsTo=[
+                STACConformanceClasses.CORE.value,
+                STACConformanceClasses.COLLECTIONS.value
+            ]
+        )
+        
+    def get_file_formats(self) -> FileFormatsGetResponse:
+        """Get the supported file formats for processing input and output.
+
+        Returns:
+            FileFormatsGetResponse: The response defining the input and output formats.
+        """
+        return FileFormatsGetResponse(
+            input={_format.title: _format for _format in self.input_formats},
+            output={_format.title: _format for _format in self.output_formats},
+        )
+
+    def get_health(self):
+        """Basic health endpoint expected to return status code 200.
+
+        Returns:
+            Response: Status code 200.
+        """
+        return Response(status_code=200, content="OK")
 
+    def get_user_info(
+        self, user: User = Depends(Authenticator.validate)
+    ) -> MeGetResponse:
+        """Get the supported file formats for processing input and output.
+
+        Returns:
+            MeGetResponse: The user information for the validated user.
+        """
+        return MeGetResponse(user_id=user.user_id.__str__())
+    
+    def get_well_known(self) -> WellKnownOpeneoGetResponse:
+        """Get the supported file formats for processing input and output.
+
+        Returns:
+            WellKnownOpeneoGetResponse: The api/s which are exposed at this server. 
+        """
         prefix = "https" if self.settings.API_TLS else "http"
 
         Components = namedtuple(
             typename="Components",
             field_names=["scheme", "netloc", "url", "path", "query", "fragment"],
         )
 
@@ -70,60 +154,30 @@
                 query=None,
                 path="",
                 url=f"/openeo/{self.settings.OPENEO_VERSION}/",
                 fragment=None,
             )
         )
 
-        return responses.WellKnownOpeneoGetResponse(
+        return WellKnownOpeneoGetResponse(
             versions=[
-                responses.Version(
+                Version(
                     url=url, production=False, api_version=self.settings.OPENEO_VERSION
                 )
             ]
         )
 
-    def get_capabilities(self) -> responses.Capabilities:
-        """ """
-        return responses.Capabilities(
-            id=self._id,
-            title=self.settings.API_TITLE,
-            stac_version=self.settings.STAC_VERSION,
-            api_version=self.settings.OPENEO_VERSION,
-            description=self.settings.API_DESCRIPTION,
-            backend_version=self.settings.OPENEO_VERSION,
-            billing=self.billing,
-            links=self.links,
-            endpoints=self._combine_endpoints(),
-        )
-
-    def get_conformance(self) -> responses.ConformanceGetResponse:
-        """ """
-        return responses.ConformanceGetResponse(
-            conformsTo=conformance.BASIC_CONFORMANCE_CLASSES
-        )
-
-    def get_file_formats(self) -> responses.FileFormatsGetResponse:
-        """ """
-        return responses.FileFormatsGetResponse(
-            input={_format.title: _format for _format in self.input_formats},
-            output={_format.title: _format for _format in self.output_formats},
-        )
+    def get_udf_runtimes(self) -> UdfRuntimesGetResponse:
+        """Get the supported file formats for processing input and output.
 
-    def get_user_info(
-        self, user: User = Depends(Authenticator.validate)
-    ) -> responses.MeGetResponse:
-        """ """
-        return responses.MeGetResponse(user_id=user.user_id.__str__())
-
-    def get_health(self):
-        """ """
-        return Response(status_code=200, content="OK")
-
-    def udf_runtimes(self) -> responses.UdfRuntimesGetResponse:
-        """ """
+        Raises:
+            HTTPException: Raises an exception with relevant status code and descriptive message of failure.
+        
+        Returns:
+            UdfRuntimesGetResponse: The metadata for the requested BatchJob.
+        """
         raise HTTPException(
             status_code=501,
-            detail=types.Error(
+            detail=Error(
                 code="FeatureUnsupported", message="Feature not supported."
             ),
         )
```

### Comparing `openeo_fastapi-2024.3.2/openeo_fastapi/client/psql/models.py` & `openeo_fastapi-2024.4.1/openeo_fastapi/client/psql/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,69 @@
+"""ORM definitions for defining and storing the associated data in the databse.
+"""
 import datetime
 
-from sqlalchemy import BOOLEAN, VARCHAR, Column, DateTime, String
+from sqlalchemy import BOOLEAN, VARCHAR, Column, DateTime
 from sqlalchemy.dialects.postgresql import ENUM, JSON, UUID
 
 from openeo_fastapi.api.types import Status
 from openeo_fastapi.client.psql.settings import BASE
 
 
 class UserORM(BASE):
     """ORM for the user table."""
 
     __tablename__ = "users"
     __table_args__ = {"extend_existing": True}
 
     user_id = Column(UUID(as_uuid=True), primary_key=True, unique=True)
+    """UUID of the user."""
     oidc_sub = Column(VARCHAR, unique=True)
+    """OIDC substring of the user."""
     created_at = Column(DateTime, default=datetime.datetime.utcnow(), nullable=False)
+    """The datetime the user was created."""
 
 
 class JobORM(BASE):
     """ORM for the job table."""
 
     __tablename__ = "jobs"
 
     job_id = Column(UUID(as_uuid=True), primary_key=True)
-    process_graph_id = Column(VARCHAR, nullable=False)
+    """UUID of the job."""
+    process = Column(JSON, nullable=False)
+    """The process graph for this job."""
     status = Column(ENUM(Status), nullable=False)
+    """The status of the Job."""
     user_id = Column(UUID(as_uuid=True), nullable=False)
+    """The UUID of the user that owns this job."""
     created = Column(DateTime, default=datetime.datetime.utcnow(), nullable=False)
+    """The datetime the job was created."""
     title = Column(VARCHAR)
+    """The title of the job."""
     description = Column(VARCHAR)
-    synchronous = Column(BOOLEAN, default=False, nullable=False)  # if null assume False
-
-
-class ProcessGraphORM(BASE):
-    """ORM for the process graph table."""
-
-    __tablename__ = "process_graph"
-
-    id = Column(VARCHAR, primary_key=True)
-    process_graph = Column(JSON, nullable=False)
-    user_id = Column(
-        UUID(as_uuid=True),
-        nullable=False,
-    )
-    created = Column(DateTime, default=datetime.datetime.utcnow(), nullable=False)
+    """The job description."""
+    synchronous = Column(BOOLEAN, default=False, nullable=False)
+    """If the Job is synchronous."""
 
 
 class UdpORM(BASE):
     """ORM for the UDPS table."""
 
     __tablename__ = "udps"
 
-    id = Column(String, primary_key=True, nullable=False)
+    id = Column(VARCHAR, primary_key=True, nullable=False)
+    """The string name of the UDP. CPK with user_id. Different users can use the same string for id."""
     user_id = Column(UUID(as_uuid=True), primary_key=True, nullable=False)
+    """The UUID of the user that owns this UDP."""
     process_graph = Column(JSON, nullable=False)
+    """The process graph of the UDP."""
     created = Column(DateTime, default=datetime.datetime.utcnow(), nullable=False)
+    """The datetime the UDP was created."""
     parameters = Column("parameters", JSON)
+    """The parameters of the UDP."""
     returns = Column("returns", JSON)
-    summary = Column("summary", String)
-    description = Column("description", String)
+    """The return types of the UDP."""
+    summary = Column("summary", VARCHAR)
+    """A summary of the UPD.""" 
+    description = Column("description", VARCHAR)
+    """A description of what the UDP is intended to do."""
```

### Comparing `openeo_fastapi-2024.3.2/pyproject.toml` & `openeo_fastapi-2024.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "openeo-fastapi"
-version = "2024.3.2"
+version = "2024.4.1"
 description = "FastApi implementation conforming to the OpenEO Api specification."
 authors = ["Sean Hoyal <sean.hoyal@external.eodc.eu>"]
 readme = "README.md"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -34,20 +34,26 @@
 stackstac = ">=0.5.0"
 stac-validator = ">=3.3.2"
 pip = "^23.3.2"
 requests = "^2.31.0"
 SQLAlchemy = "^2.0.27"
 psycopg2-binary = "^2.9.5"
 alembic = "^1.13.1"
+click = "8.1.7"
+poetry = "1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 ipykernel = "^6.15.1"
 pre-commit = "^2.20.0"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.23.0"
 aioresponses = "^0.7.5"
 pytest-postgresql = ">=4.1.1"
+sphinx = "7.2.6"
+
+[tool.poetry.scripts]
+openeo_fastapi = "openeo_fastapi.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openeo_fastapi-2024.3.2/PKG-INFO` & `openeo_fastapi-2024.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: openeo-fastapi
-Version: 2024.3.2
+Version: 2024.4.1
 Summary: FastApi implementation conforming to the OpenEO Api specification.
 Author: Sean Hoyal
 Author-email: sean.hoyal@external.eodc.eu
 Requires-Python: >=3.9,<3.12
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: SQLAlchemy (>=2.0.27,<3.0.0)
 Requires-Dist: aiohttp (>3.9)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: click (==8.1.7)
 Requires-Dist: dask-geopandas (>=0.3.1)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: joblib (>=1.3.2)
 Requires-Dist: odc-stac (>=0.3.8)
 Requires-Dist: openeo-pg-parser-networkx (>=2024.1.1)
 Requires-Dist: openeo-processes-dask (>=2023.11.6)
 Requires-Dist: pip (>=23.3.2,<24.0.0)
 Requires-Dist: planetary_computer (>=1.0.0)
+Requires-Dist: poetry (==1.8.2)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic (<2)
 Requires-Dist: pystac-client (>=0.7.5)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rioxarray (>=0.15.0)
 Requires-Dist: stac-validator (>=3.3.2)
 Requires-Dist: stackstac (>=0.5.0)
```

