# Comparing `tmp/fractal_client-1.4.4.tar.gz` & `tmp/fractal_client-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.4.4.tar", max compression
+gzip compressed data, was "fractal_client-2.0.0a0.tar", max compression
```

## Comparing `fractal_client-1.4.4.tar` & `fractal_client-2.0.0a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1576 2024-04-03 06:59:42.685652 fractal_client-1.4.4/LICENSE
--rw-r--r--   0        0        0     2706 2024-04-03 06:59:42.685652 fractal_client-1.4.4/README.md
--rw-r--r--   0        0        0       22 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/authclient.py
--rw-r--r--   0        0        0     4177 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/client.py
--rw-r--r--   0        0        0    12498 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/__init__.py
--rw-r--r--   0        0        0     7611 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5778 2024-04-03 06:59:42.685652 fractal_client-1.4.4/fractal_client/cmd/_dataset.py
--rw-r--r--   0        0        0     4809 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_job.py
--rw-r--r--   0        0        0     2852 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_project.py
--rw-r--r--   0        0        0     6586 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_task.py
--rw-r--r--   0        0        0     5105 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_user.py
--rw-r--r--   0        0        0     9153 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/cmd/_workflow.py
--rw-r--r--   0        0        0     1126 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/config.py
--rw-r--r--   0        0        0     1609 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/interface.py
--rw-r--r--   0        0        0    25180 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/parser.py
--rw-r--r--   0        0        0     2384 2024-04-03 06:59:42.689652 fractal_client-1.4.4/fractal_client/response.py
--rw-r--r--   0        0        0     2286 2024-04-03 06:59:42.689652 fractal_client-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     3846 1970-01-01 00:00:00.000000 fractal_client-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     2706 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/README.md
+-rw-r--r--   0        0        0       24 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/fractal_client/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-08 14:10:24.253916 fractal_client-2.0.0a0/fractal_client/authclient.py
+-rw-r--r--   0        0        0     4157 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/client.py
+-rw-r--r--   0        0        0    10856 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/__init__.py
+-rw-r--r--   0        0        0     7611 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     2456 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_dataset.py
+-rw-r--r--   0        0        0     4750 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_job.py
+-rw-r--r--   0        0        0     1758 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_project.py
+-rw-r--r--   0        0        0     2474 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_task.py
+-rw-r--r--   0        0        0     4766 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_user.py
+-rw-r--r--   0        0        0     6396 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/cmd/_workflow.py
+-rw-r--r--   0        0        0     1126 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/config.py
+-rw-r--r--   0        0        0      363 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/interface.py
+-rw-r--r--   0        0        0    18989 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/parser.py
+-rw-r--r--   0        0        0     2384 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/fractal_client/response.py
+-rw-r--r--   0        0        0     2248 2024-04-08 14:10:24.257916 fractal_client-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3809 1970-01-01 00:00:00.000000 fractal_client-2.0.0a0/PKG-INFO
```

### Comparing `fractal_client-1.4.4/LICENSE` & `fractal_client-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.4/README.md` & `fractal_client-2.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.4/fractal_client/authclient.py` & `fractal_client-2.0.0a0/fractal_client/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.4/fractal_client/client.py` & `fractal_client-2.0.0a0/fractal_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from httpx import Client
 from httpx import ConnectError
 
 from . import cmd
 from .authclient import AuthClient
 from .authclient import AuthenticationError
 from .config import settings
-from .interface import PrintInterface
+from .interface import Interface
 from .parser import parser_main
 
 
 class MissingCredentialsError(RuntimeError):
     pass
 
 
@@ -108,26 +108,26 @@
             password = kwargs.pop("password") or settings.FRACTAL_PASSWORD
             username, password = _check_credentials(
                 username=username, password=password
             )
             with AuthClient(username=username, password=password) as client:
                 interface = handler(client, **kwargs)
     except AuthenticationError as e:
-        return PrintInterface(retcode=1, data=e.args[0])
+        return Interface(retcode=1, data=e.args[0])
     except ConnectError as e:
-        return PrintInterface(
+        return Interface(
             retcode=1,
             data=(
                 f"ConnectError at {e.request.url}\n"
                 f"Original error: '{e.args[0]}'\n"
                 f"Hint: is {settings.FRACTAL_SERVER} alive?"
             ),
         )
     except Exception as e:
-        return PrintInterface(retcode=1, data=str(e))
+        return Interface(retcode=1, data=str(e))
 
     return interface
 
 
 def main():
     interface = handle()
     interface.show()
```

### Comparing `fractal_client-1.4.4/fractal_client/cmd/__init__.py` & `fractal_client-2.0.0a0/fractal_client/cmd/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from httpx import Client
 
 from ..authclient import AuthClient
 from ..config import settings
-from ..interface import BaseInterface
-from ..interface import PrintInterface
+from ..interface import Interface
 from ._dataset import delete_dataset
-from ._dataset import delete_resource
 from ._dataset import get_dataset
-from ._dataset import get_dataset_history
-from ._dataset import get_dataset_status
 from ._dataset import patch_dataset
 from ._dataset import post_dataset
-from ._dataset import post_resource
 from ._job import get_job
 from ._job import get_job_list
 from ._job import get_job_logs
+from ._job import job_submit
 from ._job import stop_job
 from ._project import delete_project
 from ._project import get_project
 from ._project import get_project_list
 from ._project import patch_project
 from ._project import post_project
 from ._task import delete_task
@@ -36,17 +32,14 @@
 from ._workflow import delete_workflowtask
 from ._workflow import get_workflow
 from ._workflow import get_workflow_list
 from ._workflow import patch_workflow
 from ._workflow import patch_workflowtask
 from ._workflow import post_workflow
 from ._workflow import post_workflowtask
-from ._workflow import workflow_apply
-from ._workflow import workflow_export
-from ._workflow import workflow_import
 from fractal_client import __VERSION__
 
 
 class NoCommandError(ValueError):
     pass
 
 
@@ -55,15 +48,15 @@
 
 
 def project(
     client: AuthClient,
     subcmd: str,
     batch: bool = False,
     **kwargs,
-) -> BaseInterface:
+) -> Interface:
 
     if subcmd == "new":
         parameters = ["name"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = post_project(client, batch=batch, **function_kwargs)
     elif subcmd == "show":
         parameters = ["project_id"]
@@ -71,27 +64,19 @@
         iface = get_project(client, **function_kwargs)
     elif subcmd == "list":
         iface = get_project_list(client)
     elif subcmd == "edit":
         parameters = [
             "project_id",
             "new_name",
-            "make_read_only",
-            "remove_read_only",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = patch_project(client, **function_kwargs)
     elif subcmd == "add-dataset":
-        parameters = [
-            "project_id",
-            "dataset_name",
-            "metadata",
-            "type",
-            "make_read_only",
-        ]
+        parameters = ["project_id", "dataset_name", "zarr_dir", "filters"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = post_dataset(client, batch=batch, **function_kwargs)
     elif subcmd == "delete":
         parameters = ["project_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = delete_project(client, **function_kwargs)
     else:
@@ -101,62 +86,43 @@
 
 
 def dataset(
     client: AuthClient,
     subcmd: str,
     batch: bool = False,
     **kwargs,
-) -> BaseInterface:
+) -> Interface:
     if subcmd == "show":
         parameters = ["project_id", "dataset_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = get_dataset(client, **function_kwargs)
-    elif subcmd == "add-resource":
-        parameters = ["project_id", "dataset_id", "path"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = post_resource(client, batch=batch, **function_kwargs)
-    elif subcmd == "rm-resource":
-        parameters = ["project_id", "dataset_id", "resource_id"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = delete_resource(client, **function_kwargs)
     elif subcmd == "edit":
         parameters = [
             "project_id",
             "dataset_id",
             "new_name",
-            "new_type",
-            "meta_file",
-            "make_read_only",
-            "remove_read_only",
+            "filters",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = patch_dataset(client, **function_kwargs)
     elif subcmd == "delete":
         parameters = ["project_id", "dataset_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = delete_dataset(client, **function_kwargs)
-    elif subcmd == "history":
-        parameters = ["project_id", "dataset_id"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = get_dataset_history(client, **function_kwargs)
-    elif subcmd == "status":
-        parameters = ["project_id", "dataset_id"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = get_dataset_status(client, **function_kwargs)
     else:
         raise NoCommandError(f"Command dataset {subcmd} not found")
     return iface
 
 
 def task(
     client: AuthClient,
     subcmd: str,
     batch: bool = False,
     **kwargs,
-) -> BaseInterface:
+) -> Interface:
 
     if subcmd == "list":
         iface = get_task_list(client)
     elif subcmd == "collect":
         parameters = [
             "package",
             "package_version",
@@ -210,15 +176,15 @@
 
 
 def workflow(
     client: AuthClient,
     subcmd: str,
     batch: bool = False,
     **kwargs,
-) -> BaseInterface:
+) -> Interface:
     if subcmd == "show":
         parameters = ["project_id", "workflow_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = get_workflow(client, **function_kwargs)
     elif subcmd == "new":
         parameters = ["name", "project_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
@@ -239,64 +205,50 @@
         parameters = [
             "project_id",
             "workflow_id",
             "task_id",
             "task_name",
             "task_version",
             "order",
-            "args_file",
-            "meta_file",
+            "args_non_parallel",
+            "args_parallel",
+            "input_filters",
+            "meta_parallel",
+            "meta_non_parallel",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = post_workflowtask(client, batch=batch, **function_kwargs)
     elif subcmd == "edit-task":
         parameters = [
             "project_id",
             "workflow_id",
             "workflow_task_id",
-            "args_file",
-            "meta_file",
+            "input_filters",
+            "args_non_parallel",
+            "args_parallel",
+            "meta_parallel",
+            "meta_non_parallel",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = patch_workflowtask(client, **function_kwargs)
     elif subcmd == "rm-task":
         parameters = ["project_id", "workflow_id", "workflow_task_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = delete_workflowtask(client, **function_kwargs)
-    elif subcmd == "apply":
-        parameters = [
-            "project_id",
-            "workflow_id",
-            "input_dataset_id",
-            "output_dataset_id",
-            "worker_init",
-            "first_task_index",
-            "last_task_index",
-        ]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = workflow_apply(client, batch=batch, **function_kwargs)
-    elif subcmd == "import":
-        parameters = ["project_id", "json_file"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = workflow_import(client, batch=batch, **function_kwargs)
-    elif subcmd == "export":
-        parameters = ["project_id", "workflow_id", "json_file"]
-        function_kwargs = get_kwargs(parameters, kwargs)
-        iface = workflow_export(client, **function_kwargs)
     else:
         raise NoCommandError(f"Command workflow {subcmd} not found")
     return iface
 
 
 def job(
     client: AuthClient,
     subcmd: str,
     batch: bool = False,
     **kwargs,
-) -> BaseInterface:
+) -> Interface:
     if subcmd == "list":
         parameters = ["project_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = get_job_list(client, batch=batch, **function_kwargs)
     elif subcmd == "show":
         parameters = ["project_id", "job_id", "do_not_separate_logs"]
         function_kwargs = get_kwargs(parameters, kwargs)
@@ -305,37 +257,48 @@
         parameters = ["project_id", "job_id", "output_folder"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = get_job_logs(client, **function_kwargs)
     elif subcmd == "stop":
         parameters = ["project_id", "job_id"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = stop_job(client, **function_kwargs)
+    elif subcmd == "submit":
+        parameters = [
+            "project_id",
+            "workflow_id",
+            "dataset_id",
+            "worker_init",
+            "first_task_index",
+            "last_task_index",
+        ]
+        function_kwargs = get_kwargs(parameters, kwargs)
+        iface = job_submit(client, batch=batch, **function_kwargs)
     else:
         raise NoCommandError(f"Command job {subcmd} not found")
     return iface
 
 
-def version(client: Client, **kwargs) -> PrintInterface:
+def version(client: Client, **kwargs) -> Interface:
     res = client.get(f"{settings.FRACTAL_SERVER}/api/alive/")
     data = res.json()
 
-    return PrintInterface(
+    return Interface(
         retcode=0,
         data=(
             f"Fractal client\n\tversion: {__VERSION__}\n"
             "Fractal server:\n"
             f"\turl: {settings.FRACTAL_SERVER}"
             f"\tversion: {data['version']}"
         ),
     )
 
 
 def user(
     client: AuthClient, subcmd: str, batch: bool = False, **kwargs
-) -> BaseInterface:
+) -> Interface:
     if subcmd == "register":
         parameters = [
             "new_email",
             "new_password",
             "cache_dir",
             "slurm_user",
             "username",
```

### Comparing `fractal_client-1.4.4/fractal_client/cmd/_aux_task_caching.py` & `fractal_client-2.0.0a0/fractal_client/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.4/fractal_client/cmd/_dataset.py` & `fractal_client-2.0.0a0/fractal_client/cmd/_job.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,199 +1,162 @@
-import json
+import logging
+import os
+from pathlib import Path
 from typing import Optional
-
-from rich.table import Table
+from zipfile import ZipFile
 
 from ..authclient import AuthClient
 from ..config import settings
-from ..interface import BaseInterface
-from ..interface import PrintInterface
-from ..interface import RichConsoleInterface
-from ..interface import RichJsonInterface
+from ..interface import Interface
 from ..response import check_response
 
 
-def post_dataset(
+def get_job(
     client: AuthClient,
     *,
     project_id: int,
-    dataset_name: str,
-    metadata: Optional[str] = None,
-    type: Optional[str] = None,
+    job_id: int,
     batch: bool = False,
-    make_read_only: bool = False,
-) -> RichJsonInterface:
+) -> Interface:
     """
-    Arguments:
-        project_id: ID of project to add the new dataset to
-        dataset_name: Name of new dataset
-        metadata: Path to file containing dataset metadata in JSON format.
-        type: Dataset type.
-        make_read_only: Make the new dataset read-only.
+    Query the status of a workflow-execution job
     """
-    if metadata is None:
-        meta = {}
-    else:
-        with open(metadata, "r") as f:
-            meta = json.load(f)
 
-    dataset = dict(name=dataset_name, meta=meta, read_only=make_read_only)
-    if type:
-        dataset["type"] = type
-
-    res = client.post(
-        f"{settings.BASE_URL}/project/{project_id}/dataset/",
-        json=dataset,
-    )
-    new_dataset = check_response(res, expected_status_code=201)
+    res = client.get(f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/")
+    job = check_response(res, expected_status_code=200)
     if batch:
-        return PrintInterface(retcode=0, data=new_dataset["id"])
+        return Interface(retcode=0, data=job["status"])
     else:
-        return RichJsonInterface(retcode=0, data=new_dataset)
+        return Interface(retcode=0, data=job)
 
 
-def post_resource(
-    client: AuthClient,
-    *,
-    project_id: int,
-    dataset_id: int,
-    path: str,
-    batch: bool = False,
-) -> BaseInterface:
+def get_job_list(
+    client: AuthClient, *, project_id: int, batch: bool = False
+) -> Interface:
+
+    res = client.get(f"{settings.BASE_URL}/project/{project_id}/job/")
+    jobs = check_response(res, expected_status_code=200)
 
-    res = client.post(
-        (
-            f"{settings.BASE_URL}/project/{project_id}/"
-            f"dataset/{dataset_id}/resource/"
-        ),
-        json=dict(path=path),
-    )
-    new_resource = check_response(res, expected_status_code=201)
     if batch:
-        return PrintInterface(retcode=0, data=new_resource["id"])
+        job_ids = " ".join(str(job["id"]) for job in jobs)
+        return Interface(retcode=0, data=job_ids)
     else:
-        return RichJsonInterface(retcode=0, data=new_resource)
+        return Interface(retcode=0, data=jobs)
 
 
-def delete_resource(
+def get_job_logs(
     client: AuthClient,
     *,
     project_id: int,
-    dataset_id: int,
-    resource_id: int,
-) -> BaseInterface:
-    res = client.delete(
-        (
-            f"{settings.BASE_URL}/project/{project_id}/"
-            f"dataset/{dataset_id}/resource/{resource_id}/"
+    job_id: int,
+    output_folder: str,
+) -> Interface:
+
+    # Check that output_folder does not already exist
+    if Path(output_folder).exists():
+        return Interface(
+            retcode=1, data=f"ERROR: {output_folder=} already exists"
         )
+
+    # Send request to server
+    res = client.get(
+        f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/download/"
     )
-    check_response(res, expected_status_code=204)
-    return PrintInterface(retcode=0, data="")
 
+    # NOTE: We cannot use our default check_response here, because res._content
+    # is binary. Therefore we check the status code by hand
+    if res.status_code != 200:
+        logging.error(f"Server returned {res.status_code}")
+        logging.error(
+            f"Original request: {res._request.method} {res._request.url}"
+        )
+        logging.error(
+            f"Original payload: {res._request._content.decode('utf-8')}"
+        )
+        logging.error("Terminating.\n")
+        exit(1)
 
-def patch_dataset(
-    client: AuthClient,
-    *,
-    project_id: int,
-    dataset_id: int,
-    new_name: Optional[str] = None,
-    new_type: Optional[str] = None,
-    meta_file: Optional[str] = None,
-    make_read_only: bool = False,
-    remove_read_only: bool = False,
-) -> BaseInterface:
-
-    # Prepare payload
-    dataset_update = {}
-    if new_name:
-        dataset_update["name"] = new_name
-    if new_type:
-        dataset_update["type"] = new_type
-    if meta_file:
-        with open(meta_file, "r") as f:
-            meta = json.load(f)
-        dataset_update.update(meta=meta)
-    if make_read_only:
-        dataset_update["read_only"] = True
-    if remove_read_only:
-        dataset_update["read_only"] = False
+    # Check the content-type entry in the response headers
+    content_type = res.headers["content-type"]
+    expected_content_type = "application/x-zip-compressed"
+    if content_type != expected_content_type:
+        logging.error(
+            f"Unexpected {content_type=} in headers of server "
+            f"response, instead of {expected_content_type=}"
+        )
+        logging.error(
+            f"Original request: {res._request.method} {res._request.url}"
+        )
+        logging.error(
+            f"Original payload: {res._request._content.decode('utf-8')}"
+        )
+        logging.error("Terminating.\n")
+        exit(1)
 
-    if not dataset_update:
-        return PrintInterface(retcode=1, data="Nothing to update")
+    # Write response into a temporary zipped file
+    zipped_archive_path = output_folder + "_tmp.zip"
+    with open(zipped_archive_path, "wb") as f:
+        f.write(res.content)
 
-    res = client.patch(
-        (
-            f"{settings.BASE_URL}/project/{project_id}/"
-            f"dataset/{dataset_id}/"
-        ),
-        json=dataset_update,
-    )
-    data = check_response(res, expected_status_code=200)
-    return RichJsonInterface(retcode=0, data=data)
+    # Unzip the log archive
+    unzipped_archived_path = output_folder
+    os.mkdir(unzipped_archived_path)
+    with ZipFile(zipped_archive_path, mode="r") as zipfile:
+        zipfile.extractall(path=unzipped_archived_path)
 
+    # Remove zipped temporary file
+    os.unlink(zipped_archive_path)
 
-def get_dataset(
-    client: AuthClient, *, project_id: int, dataset_id: int
-) -> BaseInterface:
-    res = client.get(
-        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}/"
-    )
-    from rich.console import Group
+    return Interface(retcode=0, data=f"Logs downloaded to {output_folder=}")
 
-    dataset = check_response(res, expected_status_code=200)
 
-    table = Table(title="Dataset")
-    table.add_column("ID", style="cyan", no_wrap=True)
-    table.add_column("Name", justify="right", style="green")
-    table.add_column("Type", style="white")
-    table.add_column("Meta", justify="center")
-    table.add_column("Read only", justify="center")
-
-    table.add_row(
-        str(dataset["id"]),
-        dataset["name"],
-        dataset["type"],
-        json.dumps(dataset["meta"], indent=2),
-        "✅" if dataset["read_only"] else "❌",
-    )
-    table_res = Table(title="Resources")
-    table_res.add_column("Path", justify="center", style="yellow")
-    table_res.add_column("ID", justify="center", style="yellow")
-    table_res.add_column("Dataset ID", justify="center", style="yellow")
-    for r in dataset["resource_list"]:
-        table_res.add_row(r["path"], str(r["id"]), str(r["dataset_id"]))
-    group = Group(table, table_res)
-    return RichConsoleInterface(retcode=0, data=group)
-
-
-def delete_dataset(
-    client: AuthClient, *, project_id: int, dataset_id: int
-) -> PrintInterface:
+def stop_job(client: AuthClient, *, project_id: int, job_id: int) -> Interface:
+    """
+    Stop a workflow-execution job
+    """
 
-    res = client.delete(
-        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}/"
+    res = client.get(
+        f"{settings.BASE_URL}/project/{project_id}/job/{job_id}/stop/"
+    )
+    check_response(res, expected_status_code=202)
+    return Interface(
+        retcode=0, data="Correctly called the job-stopping endpoint"
     )
-    check_response(res, expected_status_code=204)
-    return PrintInterface(retcode=0, data="")
 
 
-def get_dataset_history(
-    client: AuthClient, *, project_id: int, dataset_id: int
-) -> BaseInterface:
-    res = client.get(
-        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}/"
-        "export_history/"
-    )
-    history_workflow = check_response(res, expected_status_code=200)
-    return RichJsonInterface(retcode=0, data=history_workflow)
+def job_submit(
+    client: AuthClient,
+    *,
+    project_id: int,
+    workflow_id: int,
+    dataset_id: int,
+    first_task_index: Optional[int] = None,
+    last_task_index: Optional[int] = None,
+    worker_init: Optional[str] = None,
+    batch: bool = False,
+) -> Interface:
 
+    job_submit = dict()
+    # Prepare JobV2 object, without None attributes
+    if worker_init is not None:
+        job_submit["worker_init"] = worker_init
+    if first_task_index is not None:
+        job_submit["first_task_index"] = first_task_index
+    if last_task_index is not None:
+        job_submit["last_task_index"] = last_task_index
 
-def get_dataset_status(
-    client: AuthClient, *, project_id: int, dataset_id: int
-) -> BaseInterface:
-    res = client.get(
-        f"{settings.BASE_URL}/project/{project_id}/dataset/{dataset_id}/"
-        "status/"
+    # Prepare query parameters
+    query_parameters = f"workflow_id={workflow_id}" f"&dataset_id={dataset_id}"
+
+    res = client.post(
+        (
+            f"{settings.BASE_URL}/project/{project_id}/job/"
+            f"submit/?{query_parameters}"
+        ),
+        json=job_submit,
     )
-    dataset_status = check_response(res, expected_status_code=200)
-    return RichJsonInterface(retcode=0, data=dataset_status)
+    job_read = check_response(res, expected_status_code=202)
+
+    if batch:
+        return Interface(retcode=0, data=job_read["id"])
+    else:
+        return Interface(retcode=0, data=job_read)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fractal_client-1.4.4/fractal_client/cmd/_user.py` & `fractal_client-2.0.0a0/fractal_client/cmd/_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from typing import Optional
-from typing import Union
 
 from ..authclient import AuthClient
 from ..config import settings
-from ..interface import PrintInterface
-from ..interface import RichJsonInterface
+from ..interface import Interface
 from ..response import check_response
 
 
 def user_register(
     client: AuthClient,
     *,
     new_email: str,
     new_password: Optional[str] = None,
     slurm_user: Optional[str] = None,
     cache_dir: Optional[str] = None,
     username: Optional[str] = None,
     superuser: bool = False,
     verified: bool = True,  # TODO: this is not currently exposed in the CLI
     batch: bool = False,
-) -> Union[RichJsonInterface, PrintInterface]:
+) -> Interface:
 
     new_user = dict(
         email=new_email,
         password=new_password,
     )
     if slurm_user:
         new_user["slurm_user"] = slurm_user
@@ -36,15 +34,15 @@
 
     if new_password is None:
         new_password = getpass()
         confirm_new_password = getpass("Confirm password: ")
         if new_password == confirm_new_password:
             new_user["password"] = new_password
         else:
-            return PrintInterface(retcode=1, data="Passwords do not match.")
+            return Interface(retcode=1, data="Passwords do not match.")
 
     res = client.post(
         f"{settings.FRACTAL_SERVER}/auth/register/", json=new_user
     )
     data = check_response(res, expected_status_code=201)
 
     if superuser or verified:
@@ -53,29 +51,29 @@
         res = client.patch(
             f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/",
             json=patch_payload,
         )
         data = check_response(res, expected_status_code=200)
 
     if batch:
-        return PrintInterface(retcode=0, data=data["id"])
+        return Interface(retcode=0, data=data["id"])
     else:
-        return RichJsonInterface(retcode=0, data=data)
+        return Interface(retcode=0, data=data)
 
 
-def user_list(client: AuthClient) -> RichJsonInterface:
+def user_list(client: AuthClient) -> Interface:
     res = client.get(f"{settings.FRACTAL_SERVER}/auth/users/")
     users = check_response(res, expected_status_code=200)
-    return RichJsonInterface(retcode=0, data=users)
+    return Interface(retcode=0, data=users)
 
 
-def user_show(client: AuthClient, *, user_id: str) -> RichJsonInterface:
+def user_show(client: AuthClient, *, user_id: str) -> Interface:
     res = client.get(f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/")
     user = check_response(res, expected_status_code=200)
-    return RichJsonInterface(retcode=0, data=user)
+    return Interface(retcode=0, data=user)
 
 
 def user_edit(
     client: AuthClient,
     *,
     user_id: str,
     new_email: Optional[str] = None,
@@ -83,23 +81,23 @@
     new_slurm_user: Optional[str] = None,
     new_cache_dir: Optional[str] = None,
     new_username: Optional[str] = None,
     make_superuser: bool = False,
     remove_superuser: bool = False,
     make_verified: bool = False,
     remove_verified: bool = False,
-) -> Union[RichJsonInterface, PrintInterface]:
+) -> Interface:
 
     user_update = dict()
     if new_email is not None:
         if (make_verified is False) and (remove_verified is False):
             # Since `fastapi-users` sets `is_verified` to `False` each time the
             # email is updated, we force the user to make explicit whether the
             # account is verified or not.
-            return PrintInterface(
+            return Interface(
                 retcode=1,
                 data=(
                     "Cannot use `--new-email` without `--make-verified` or "
                     "`--remove-verified`"
                 ),
             )
         user_update["email"] = new_email
@@ -116,36 +114,31 @@
     if new_cache_dir is not None:
         user_update["cache_dir"] = new_cache_dir
     if new_slurm_user is not None:
         user_update["slurm_user"] = new_slurm_user
     if new_username is not None:
         user_update["username"] = new_username
 
-    if not user_update:
-        return PrintInterface(retcode=1, data="Nothing to update")
-
     res = client.patch(
         f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/", json=user_update
     )
     new_user = check_response(res, expected_status_code=200)
 
     if new_email is not None:
         # Since `fastapi-users` sets `is_verified` to `False` each time the
         # email is updated, we set `is_verified` as specified by the user.
         res = client.patch(
             f"{settings.FRACTAL_SERVER}/auth/users/{user_id}/",
             json=dict(is_verified=user_update["is_verified"]),
         )
         new_user = check_response(res, expected_status_code=200)
 
-    return RichJsonInterface(retcode=0, data=new_user)
+    return Interface(retcode=0, data=new_user)
 
 
-def user_whoami(
-    client: AuthClient, *, batch: bool
-) -> Union[RichJsonInterface, PrintInterface]:
+def user_whoami(client: AuthClient, *, batch: bool) -> Interface:
     res = client.get(f"{settings.FRACTAL_SERVER}/auth/current-user/")
     user = check_response(res, expected_status_code=200)
     if batch:
-        return PrintInterface(retcode=0, data=user["id"])
+        return Interface(retcode=0, data=user["id"])
     else:
-        return RichJsonInterface(retcode=0, data=user)
+        return Interface(retcode=0, data=user)
```

### Comparing `fractal_client-1.4.4/fractal_client/config.py` & `fractal_client-2.0.0a0/fractal_client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         )
         self.FRACTAL_CACHE_PATH: str = getenv(
             "FRACTAL_CACHE_PATH", str(Path.home() / ".cache/fractal")
         )
 
     @property
     def BASE_URL(self) -> str:
-        return f"{self.FRACTAL_SERVER}/api/v1"
+        return f"{self.FRACTAL_SERVER}/api/v2"
 
 
 settings = Settings()
```

### Comparing `fractal_client-1.4.4/fractal_client/parser.py` & `fractal_client-2.0.0a0/fractal_client/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,33 +96,29 @@
 # project add-dataset
 project_add_dataset_parser = project_subparsers.add_parser(
     "add-dataset",
     description="Add dataset to project.",
     allow_abbrev=False,
 )
 project_add_dataset_parser.add_argument(
-    "project_id", type=int, help="ID of project to add the new dataset to."
-)
-project_add_dataset_parser.add_argument(
-    "dataset_name", help="Name of new dataset."
+    "project_id",
+    type=int,
+    help="ID of project to add the new dataset to.",
 )
 project_add_dataset_parser.add_argument(
-    "--metadata",
-    help="Path to file containing dataset metadata in JSON format.",
+    "dataset_name",
+    help="Name of new dataset.",
 )
 project_add_dataset_parser.add_argument(
-    "--type",
-    help="Dataset type.",
+    "zarr_dir",
+    help="Path to zarr dir.",
 )
 project_add_dataset_parser.add_argument(
-    "--make-read-only",
-    action="store_true",
-    default=False,
-    required=False,
-    help="Make dataset read-only (not required).",
+    "--filters",
+    help="Path to JSON file with filters.",
 )
 
 
 # project edit
 project_edit_parser = project_subparsers.add_parser(
     "edit",
     description="Edit details of a single project.",
@@ -130,101 +126,42 @@
 )
 project_edit_parser.add_argument(
     "project_id", type=int, help="ID of the project to edit."
 )
 project_edit_parser.add_argument(
     "--new-name", help="New project name.", required=False
 )
-project_edit_parser_read_only = (
-    project_edit_parser.add_mutually_exclusive_group()
-)
-project_edit_parser_read_only.add_argument(
-    "--make-read-only",
-    help="Set the read-only flag for this project.",
-    action="store_true",
-    required=False,
-)
-project_edit_parser_read_only.add_argument(
-    "--remove-read-only",
-    help="Remove the read-only flag for this project.",
-    action="store_true",
-    required=False,
-)
 
 
 # DATASET GROUP
 dataset_parser = subparsers_main.add_parser(
     "dataset",
     description="Dataset commands.",
     allow_abbrev=False,
 )
 dataset_subparsers = dataset_parser.add_subparsers(
     title="Valid sub-commands", dest="subcmd", required=True
 )
 
-# dataset add-resource
-dataset_add_resource_parser = dataset_subparsers.add_parser(
-    "add-resource",
-    description="Add resource to existing dataset.",
-    allow_abbrev=False,
-)
-dataset_add_resource_parser.add_argument(
-    "project_id", type=int, help="Project ID."
-)
-dataset_add_resource_parser.add_argument(
-    "dataset_id", type=int, help="Dataset ID."
-)
-dataset_add_resource_parser.add_argument(
-    "path", help="Absolute path to resource."
-)
-
-# dataset rm-resource
-dataset_rm_resource_parser = dataset_subparsers.add_parser(
-    "rm-resource",
-    description="Remove resource to existing dataset.",
-    allow_abbrev=False,
-)
-dataset_rm_resource_parser.add_argument(
-    "project_id", type=int, help="Project ID."
-)
-dataset_rm_resource_parser.add_argument(
-    "dataset_id", type=int, help="Dataset ID."
-)
-dataset_rm_resource_parser.add_argument(
-    "resource_id", type=int, help="Resource ID."
-)
 
 # dataset edit
 dataset_edit_parser = dataset_subparsers.add_parser(
     "edit",
     description="Edit dataset.",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
 dataset_edit_parser.add_argument("project_id", type=int, help="Project ID.")
 dataset_edit_parser.add_argument("dataset_id", type=int, help="Dataset ID.")
 dataset_edit_parser.add_argument("--new-name", help="New name of dataset.")
-dataset_edit_parser.add_argument("--new-type", help="Dataset type.")
 dataset_edit_parser.add_argument(
-    "--meta-file",
+    "--filters",
     help="Path to JSON file with new metadata to replace the current ones.",
 )
-dataset_edit_parser_read = dataset_edit_parser.add_mutually_exclusive_group()
-dataset_edit_parser_read.add_argument(
-    "--make-read-only",
-    help="Set read-only flag of dataset.",
-    action="store_true",
-    required=False,
-)
-dataset_edit_parser_read.add_argument(
-    "--remove-read-only",
-    help="Remove read-only flag of dataset.",
-    action="store_true",
-    required=False,
-)
+
 
 # dataset show
 dataset_show_parser = dataset_subparsers.add_parser(
     "show",
     description="Show dataset.",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
@@ -238,34 +175,14 @@
     description="Delete dataset.",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
 dataset_delete_parser.add_argument("project_id", type=int, help="Project ID.")
 dataset_delete_parser.add_argument("dataset_id", type=int, help="Dataset ID.")
 
-# dataset history
-dataset_history_parser = dataset_subparsers.add_parser(
-    "history",
-    description="Export dataset history as a reproducible worfklow.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-dataset_history_parser.add_argument("project_id", type=int, help="Project ID.")
-dataset_history_parser.add_argument("dataset_id", type=int, help="Dataset ID.")
-
-# dataset status
-dataset_status_parser = dataset_subparsers.add_parser(
-    "status",
-    description="Extract status of WorkflowTasks associated with dataset.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-dataset_status_parser.add_argument("project_id", type=int, help="Project ID.")
-dataset_status_parser.add_argument("dataset_id", type=int, help="Dataset ID.")
-
 # TASK GROUP
 task_parser = subparsers_main.add_parser(
     "task",
     description="Task commands.",
     allow_abbrev=False,
 )
 task_subparsers = task_parser.add_subparsers(
@@ -332,150 +249,14 @@
 )
 task_check_collection_parser.add_argument(
     "--include-logs",
     default=False,
     action="store_true",
     help="Also include task-collection logs.",
 )
-task_check_collection_parser.add_argument(
-    "--do-not-separate-logs",
-    dest="do_not_separate_logs",
-    help=(
-        "Show the task-collection logs in the main output, "
-        "instead of a separate field."
-    ),
-    action="store_true",
-    required=False,
-)
-
-
-# task new
-task_new_parser = task_subparsers.add_parser(
-    "new",
-    description="Create new task.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-task_new_parser.add_argument(
-    "name", help="A human readable name for the task."
-)
-task_new_parser.add_argument(
-    "command", help="The command that executes the task."
-)
-task_new_parser.add_argument("source", help="TBD")
-task_new_parser.add_argument(
-    "--input-type",
-    help="The type of data the task expects as input.",
-    default="Any",
-)
-task_new_parser.add_argument(
-    "--output-type",
-    help="The type of data the task expects as output.",
-    default="Any",
-)
-task_new_parser.add_argument(
-    "--version",
-    help="Task version.",
-)
-task_new_parser.add_argument(
-    "--meta-file",
-    help="Path to JSON file with additional parameters useful for execution.",
-)
-task_new_parser.add_argument(
-    "--args-schema",
-    help="Path to file containing JSON Schema for task arguments.",
-)
-task_new_parser.add_argument(
-    "--args-schema-version",
-    help=(
-        "Label encoding how the task-arguments JSON Schema was generated "
-        "(e.g. `pydantic_v1`)."
-    ),
-)
-
-# task edit
-task_edit_parser = task_subparsers.add_parser(
-    "edit",
-    description="Edit task.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-
-task_edit_id_or_name_group = task_edit_parser.add_mutually_exclusive_group(
-    required=True
-)
-task_edit_id_or_name_group.add_argument(
-    "--id", help="ID of the task to edit.", type=int
-)
-task_edit_id_or_name_group.add_argument(
-    "--name", help="Name of the task to edit."
-)
-
-task_edit_parser.add_argument(
-    "--version",
-    help=(
-        "Version of the task to edit "
-        "(only accepted in combination with `--name`)."
-    ),
-)
-task_edit_parser.add_argument("--new-name", help="New task name.")
-task_edit_parser.add_argument("--new-command", help="New task command.")
-task_edit_parser.add_argument(
-    "--new-input-type",
-    help="New input type.",
-)
-task_edit_parser.add_argument(
-    "--new-output-type",
-    help="New output type.",
-)
-task_edit_parser.add_argument(
-    "--meta-file",
-    help=(
-        "Path to JSON serialised file containing updates to the current "
-        "`meta` dictionary."
-    ),
-)
-task_edit_parser.add_argument(
-    "--new-version",
-    help="New version.",
-)
-task_edit_parser.add_argument(
-    "--new-args-schema",
-    help="Path to file containing the new JSON Schema for task arguments.",
-)
-task_edit_parser.add_argument(
-    "--new-args-schema-version",
-    help=(
-        "New label encoding how the task-arguments JSON Schema was generated."
-    ),
-)
-
-# task delete
-task_delete_parser = task_subparsers.add_parser(
-    "delete",
-    description="Delete task.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-task_delete_id_or_name_group = task_delete_parser.add_mutually_exclusive_group(
-    required=True
-)
-task_delete_id_or_name_group.add_argument(
-    "--id", help="ID of the task to delete.", type=int
-)
-task_delete_id_or_name_group.add_argument(
-    "--name", help="Name of the task to delete."
-)
-task_delete_parser.add_argument(
-    "--version",
-    help=(
-        "Version of the task to delete "
-        "(only accepted in combination with `--name`)."
-    ),
-)
 
 
 # WORKFLOW GROUP
 
 workflow_parser = subparsers_main.add_parser(
     "workflow",
     description="Workflow commands.",
@@ -561,40 +342,47 @@
 )
 workflow_add_task_id_or_name_group.add_argument(
     "--task-id", help="ID of the task to add.", type=int
 )
 workflow_add_task_id_or_name_group.add_argument(
     "--task-name", help="Name of the task to add."
 )
-
 workflow_add_task_parser.add_argument(
     "--task-version",
     help=(
         "Version of task to add "
         "(only accepted in combination with --task-name)."
     ),
 )
 workflow_add_task_parser.add_argument(
     "--order", help="Order of this task within the workflow's task list."
 )
+
 workflow_add_task_parser.add_argument(
-    "--args-file",
-    help=(
-        "Path to json serialised file containing the arguments "
-        "overrides of the task."
-    ),
+    "--args-non-parallel", help="Args for non parallel tasks"
 )
+
 workflow_add_task_parser.add_argument(
-    "--meta-file",
-    help=(
-        "Path to json serialised file containing the meta "
-        "overrides of the task."
-    ),
+    "--args-parallel", help="Args for parallel tasks"
 )
 
+workflow_add_task_parser.add_argument(
+    "--meta-non-parallel", help="Metadata file fornon parallel tasks"
+)
+
+workflow_add_task_parser.add_argument(
+    "--meta-parallel", help="Metadata file for parallel tasks"
+)
+
+workflow_add_task_parser.add_argument(
+    "--input-filters",
+    help="Path to json file with filters.",
+)
+
+
 # workflow edit task
 workflow_edit_task_parser = workflow_subparsers.add_parser(
     "edit-task",
     description="Edit task within specific workflow.",
     allow_abbrev=False,
 )
 workflow_edit_task_parser.add_argument(
@@ -607,28 +395,37 @@
 )
 workflow_edit_task_parser.add_argument(
     "workflow_task_id",
     type=int,
     help="Workflow task ID, the ID of a task inside the list of tasks.",
 )
 workflow_edit_task_parser.add_argument(
-    "--args-file",
+    "--input-filters",
     help=(
         "Path to json serialised file containing the arguments "
         "overrides of the task."
     ),
 )
 workflow_edit_task_parser.add_argument(
-    "--meta-file",
-    help=(
-        "Path to json serialised file containing the meta "
-        "overrides of the task."
-    ),
+    "--args-non-parallel", help="Args for non parallel tasks"
+)
+
+workflow_edit_task_parser.add_argument(
+    "--args-parallel", help="Args for parallel tasks"
+)
+
+workflow_edit_task_parser.add_argument(
+    "--meta-non-parallel", help="Metadata file fornon parallel tasks"
+)
+
+workflow_edit_task_parser.add_argument(
+    "--meta-parallel", help="Metadata file for parallel tasks"
 )
 
+
 # workflow remove task
 workflow_remove_task_parser = workflow_subparsers.add_parser(
     "rm-task",
     description="Remove task from a specific workflow.",
     allow_abbrev=False,
 )
 workflow_remove_task_parser.add_argument(
@@ -641,51 +438,14 @@
 )
 workflow_remove_task_parser.add_argument(
     "workflow_task_id",
     type=int,
     help="Workflow task ID (the ID of a task inside the list of tasks).",
 )
 
-# workflow apply
-workflow_apply_parser = workflow_subparsers.add_parser(
-    "apply",
-    description="Apply workflow to dataset.",
-    argument_default=ap.SUPPRESS,
-    allow_abbrev=False,
-)
-
-workflow_apply_parser.add_argument("project_id", type=int)
-workflow_apply_parser.add_argument("workflow_id", type=int)
-workflow_apply_parser.add_argument("input_dataset_id", type=int)
-workflow_apply_parser.add_argument("output_dataset_id", type=int)
-workflow_apply_parser.add_argument(
-    "--start",
-    dest="first_task_index",
-    type=int,
-    help=(
-        "Positional index of the first task to be executed"
-        " (starting from 0)."
-    ),
-    required=False,
-)
-workflow_apply_parser.add_argument(
-    "--end",
-    dest="last_task_index",
-    type=int,
-    help=(
-        "Positional index of the last task to be executed"
-        " (starting from 0)."
-    ),
-    required=False,
-)
-workflow_apply_parser.add_argument(
-    "-w",
-    "--worker-init",
-    help="Command to be run before starting a worker.",
-)
 
 # workflow import
 workflow_import_parser = workflow_subparsers.add_parser(
     "import",
     description="Import workflow to project from file.",
     allow_abbrev=False,
 )
@@ -750,21 +510,14 @@
     "show",
     description="Query status of workflow-execution job.",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
 )
 job_show_parser.add_argument("project_id", type=int, help="Project ID.")
 job_show_parser.add_argument("job_id", type=int, help="Job ID.")
-job_show_parser.add_argument(
-    "--do-not-separate-logs",
-    dest="do_not_separate_logs",
-    help="Show the job logs in the main output, instead of a separate field.",
-    action="store_true",
-    required=False,
-)
 
 # job download-logs
 job_download_logs_parser = job_subparsers.add_parser(
     "download-logs",
     description="Download full folder of workflow-execution job.",
     allow_abbrev=False,
 )
@@ -785,14 +538,52 @@
     description="Stop workflow-execution job.",
     allow_abbrev=False,
 )
 job_stop_parser.add_argument("project_id", type=int, help="Project ID.")
 job_stop_parser.add_argument("job_id", type=int, help="Job ID.")
 
 
+# job submit
+job_submit_parser = job_subparsers.add_parser(
+    "submit",
+    description="Submit a job.",
+    argument_default=ap.SUPPRESS,
+    allow_abbrev=False,
+)
+
+job_submit_parser.add_argument("project_id", type=int)
+job_submit_parser.add_argument("workflow_id", type=int)
+job_submit_parser.add_argument("dataset_id", type=int)
+job_submit_parser.add_argument(
+    "--start",
+    dest="first_task_index",
+    type=int,
+    help=(
+        "Positional index of the first task to be executed"
+        " (starting from 0)."
+    ),
+    required=False,
+)
+job_submit_parser.add_argument(
+    "--end",
+    dest="last_task_index",
+    type=int,
+    help=(
+        "Positional index of the last task to be executed"
+        " (starting from 0)."
+    ),
+    required=False,
+)
+job_submit_parser.add_argument(
+    "-w",
+    "--worker-init",
+    help="Command to be run before starting a worker.",
+)
+
+
 # VERSION GROUP
 version_parser = subparsers_main.add_parser(
     "version",
     description="Print version and exit.",
     allow_abbrev=False,
 )
```

### Comparing `fractal_client-1.4.4/fractal_client/response.py` & `fractal_client-2.0.0a0/fractal_client/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.4.4/pyproject.toml` & `fractal_client-2.0.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.4.4"
+version = "2.0.0a0"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -21,26 +21,24 @@
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/fractal-analytics-platform/fractal-client/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.21.0"
-rich = "^12.5.1"
 httpx = "^0.23.0"
 PyJWT = "^2.4.0"
 packaging = "^23.1"
 
 [tool.poetry.group.dev.dependencies]
 devtools = "^0.9.0"
 pre-commit = "^2.19.0"
 pytest = "^7.1.2"
 bumpver = "^2022.1118"
 coverage = {extras = ["toml"], version = "^6.5.0"}
-pytest-pretty = "^1.1.0"
 fractal-server = { git = "https://github.com/fractal-analytics-platform/fractal-server.git", branch = "main"}
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
@@ -54,15 +52,15 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.4.4"
+current_version = "2.0.0a0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.4.4/PKG-INFO` & `fractal_client-2.0.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.4.4
+Version: 2.0.0a0
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-client
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
 Project-URL: Changelog, https://github.com/fractal-analytics-platform/fractal-client/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fractal-analytics-platform.github.io/fractal-client
 Project-URL: Repository, https://github.com/fractal-analytics-platform/fractal-client
 Description-Content-Type: text/markdown
 
 # Fractal Client
```

