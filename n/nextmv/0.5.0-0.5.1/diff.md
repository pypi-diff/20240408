# Comparing `tmp/nextmv-0.5.0.tar.gz` & `tmp/nextmv-0.5.1.tar.gz`

## Comparing `nextmv-0.5.0.tar` & `nextmv-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv-py.code-workspace
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.5.0/requirements.txt
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/python-lint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.5.0/.github/workflows/python-test.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/__about__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/base_model.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/__init__.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/acceptance_test.py
--rw-r--r--   0        0        0    24971 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/application.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/batch_experiment.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/client.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/cloud/input_set.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/check/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/check/schema.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/input.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/location.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/output.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/stop.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.5.0/nextmv/nextroute/schema/vehicle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/test_base_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/cloud/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/cloud/test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/__init__.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/input.json
--rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/output.json
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/output_with_check.json
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/test_input.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.5.0/tests/nextroute/schema/test_output.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.5.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.5.0/LICENSE
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.5.0/README.md
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv-py.code-workspace
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nextmv-0.5.1/requirements.txt
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/python-lint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 nextmv-0.5.1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/__about__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/base_model.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/__init__.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/acceptance_test.py
+-rw-r--r--   0        0        0    25508 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/application.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/batch_experiment.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/client.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/cloud/input_set.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/__init__.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/check/__init__.py
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/check/schema.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/input.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/location.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/output.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/stop.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 nextmv-0.5.1/nextmv/nextroute/schema/vehicle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/test_base_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/cloud/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/cloud/test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/__init__.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/input.json
+-rw-r--r--   0        0        0    25755 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/output.json
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/output_with_check.json
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/test_input.py
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 nextmv-0.5.1/tests/nextroute/schema/test_output.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 nextmv-0.5.1/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nextmv-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nextmv-0.5.1/README.md
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextmv-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 nextmv-0.5.1/PKG-INFO
```

### Comparing `nextmv-0.5.0/.github/workflows/publish.yml` & `nextmv-0.5.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/.github/workflows/python-lint.yml` & `nextmv-0.5.1/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/.github/workflows/python-test.yml` & `nextmv-0.5.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/cloud/__init__.py` & `nextmv-0.5.1/nextmv/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/cloud/acceptance_test.py` & `nextmv-0.5.1/nextmv/cloud/acceptance_test.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/cloud/application.py` & `nextmv-0.5.1/nextmv/cloud/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """This module contains the application class."""
 
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
+import requests
+
 from nextmv.base_model import BaseModel
 from nextmv.cloud.acceptance_test import AcceptanceTest, Metric
 from nextmv.cloud.batch_experiment import BatchExperiment, BatchExperimentMetadata, BatchExperimentRun
 from nextmv.cloud.client import Client, get_size
 from nextmv.cloud.input_set import InputSet
 
 _MAX_RUN_SIZE: int = 5 * 1024 * 1024
@@ -260,15 +262,15 @@
         )
 
         return [InputSet.from_dict(input_set) for input_set in response.json()]
 
     def new_acceptance_test(
         self,
         candidate_instance_id: str,
-        control_instance_id: str,
+        baseline_instance_id: str,
         id: str,
         metrics: List[Union[Metric, Dict[str, Any]]],
         name: str,
         input_set_id: Optional[str] = None,
         description: Optional[str] = None,
     ) -> AcceptanceTest:
         """
@@ -277,15 +279,15 @@
         to provide the input_set_id parameter. In that case, the ID of the
         acceptance test and the batch experiment must be the same. If the batch
         experiment does not exist, you can provide the input_set_id parameter
         and a new batch experiment will be created for you.
 
         Args:
             candidate_instance_id: ID of the candidate instance.
-            control_instance_id: ID of the control instance.
+            baseline_instance_id: ID of the baseline instance.
             id: ID of the acceptance test.
             metrics: List of metrics to use for the acceptance test.
             name: Name of the acceptance test.
             input_set_id: ID of the input set to use for the underlying batch
                 experiment, in case it hasn't been started.
             description: Description of the acceptance test.
 
@@ -295,35 +297,43 @@
         Raises:
             requests.HTTPError: If the response status code is not 2xx.
             ValueError: If the batch experiment ID does not match the
                 acceptance test ID.
         """
 
         if input_set_id is None:
-            batch_experiment = self.batch_experiment(batch_id=id)
-            batch_experiment_id = batch_experiment.id
+            try:
+                batch_experiment = self.batch_experiment(batch_id=id)
+                batch_experiment_id = batch_experiment.id
+            except requests.HTTPError as e:
+                if e.response.status_code != 404:
+                    raise e
+
+                raise ValueError(
+                    f"batch experiment {id} does not exist, input_set_id must be defined to create a new one"
+                ) from e
         else:
             batch_experiment_id = self.new_batch_experiment(
                 name=name,
                 input_set_id=input_set_id,
-                instance_ids=[candidate_instance_id, control_instance_id],
+                instance_ids=[candidate_instance_id, baseline_instance_id],
                 description=description,
                 id=id,
             )
 
         if batch_experiment_id != id:
             raise ValueError(f"batch experiment_id ({batch_experiment_id}) does not match acceptance test id ({id})")
 
         payload_metrics = [{}] * len(metrics)
         for i, metric in enumerate(metrics):
             payload_metrics[i] = metric.to_dict() if isinstance(metric, Metric) else metric
 
         payload = {
             "candidate": {"instance_id": candidate_instance_id},
-            "control": {"instance_id": control_instance_id},
+            "control": {"instance_id": baseline_instance_id},
             "metrics": payload_metrics,
             "experiment_id": batch_experiment_id,
             "name": name,
         }
         if description is not None:
             payload["description"] = description
         if id is not None:
@@ -337,18 +347,18 @@
 
         return AcceptanceTest.from_dict(response.json())
 
     def new_batch_experiment(
         self,
         name: str,
         input_set_id: str,
-        instance_ids: List[str],
+        instance_ids: List[str] = None,
         description: Optional[str] = None,
         id: Optional[str] = None,
-        option_sets: Optional[Dict[str, Any]] = None,
+        option_sets: Optional[Dict[str, Dict[str, str]]] = None,
         runs: Optional[List[Union[BatchExperimentRun, Dict[str, Any]]]] = None,
     ) -> str:
         """
         Create a new batch experiment.
 
         Args:
             name: Name of the batch experiment.
@@ -446,28 +456,29 @@
             payload=payload,
         )
 
         return InputSet.from_dict(response.json())
 
     def new_run(
         self,
-        input: Union[Dict[str, Any], BaseModel] = None,
+        input: Union[Dict[str, Any], BaseModel, str] = None,
         instance_id: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
         upload_id: Optional[str] = None,
         options: Optional[Dict[str, Any]] = None,
         configuration: Optional[Configuration] = None,
     ) -> str:
         """
         Submit an input to start a new run of the application. Returns the
         run_id of the submitted run.
 
         Args:
-            input: Input to use for the run.
+            input: Input to use for the run. This can be JSON (given as dict
+            or BaseModel) or text (given as str).
             instance_id: ID of the instance to use for the run. If not
                 provided, the default_instance_id will be used.
             name: Name of the run.
             description: Description of the run.
             upload_id: ID to use when running a large input.
             options: Options to use for the run.
             configuration: Configuration to use for the run.
@@ -475,23 +486,24 @@
         Returns:
             ID of the submitted run.
 
         Raises:
             requests.HTTPError: If the response status code is not 2xx.
         """
 
+        input_size = 0
         if isinstance(input, BaseModel):
             input = input.to_dict()
+            if input is not None:
+                input_size = get_size(input)
 
-        input_size = 0
-        if input is not None:
-            input_size = get_size(input)
+        upload_url_required = isinstance(input, str) or input_size > _MAX_RUN_SIZE
 
         upload_id_used = upload_id is not None
-        if not upload_id_used and input_size > _MAX_RUN_SIZE:
+        if not upload_id_used and upload_url_required:
             upload_url = self.upload_url()
             self.upload_large_input(input=input, upload_url=upload_url)
             upload_id = upload_url.upload_id
             upload_id_used = True
 
         payload = {}
         if upload_id_used:
@@ -698,15 +710,15 @@
                 f"run {run_id} did not succeed after {polling_options.max_tries} tries",
             )
 
         return self._run_result(run_id=run_id, run_information=run_information)
 
     def upload_large_input(
         self,
-        input: Dict[str, Any],
+        input: Union[Dict[str, Any], str],
         upload_url: UploadURL,
     ) -> None:
         """
         Upload the file located at the given path to the provided upload URL.
 
         Args:
             upload_url: Upload URL to use for uploading the file.
@@ -715,15 +727,15 @@
         Raises:
             requests.HTTPError: If the response status code is not 2xx.
         """
 
         _ = self.client.request(
             method="PUT",
             endpoint=upload_url.upload_url,
-            payload=input,
+            data=input,
             headers={"Content-Type": "application/json"},
         )
 
     def upload_url(self) -> UploadURL:
         """
         Get an upload URL to use for uploading a file.
```

### Comparing `nextmv-0.5.0/nextmv/cloud/batch_experiment.py` & `nextmv-0.5.1/nextmv/cloud/batch_experiment.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     created_at: datetime
     """Creation date of the batch experiment."""
     status: str
     """Status of the batch experiment."""
 
     grouped_distributional_summaries: Optional[List[Dict[str, Any]]] = None
     """Grouped distributional summaries of the batch experiment."""
-    option_sets: Optional[Dict[str, Any]] = None
+    option_sets: Optional[Dict[str, Dict[str, str]]] = None
     """Option sets used for the experiment."""
 
 
 class BatchExperimentRun(BaseModel):
     """A batch experiment run is a single execution of a batch experiment."""
 
     option_set: str
@@ -47,14 +47,20 @@
     """ID of the input used for the experiment."""
 
     instance_id: Optional[str] = None
     """ID of the instance used for the experiment."""
     version_id: Optional[str] = None
     """ID of the version used for the experiment."""
 
+    def __post_init__(self):
+        """Logic to run after the class is initialized."""
+
+        if self.instance_id is None and self.version_id is None:
+            raise ValueError("either instance_id or version_id must be set")
+
 
 class BatchExperimentMetadata(BatchExperimentInformation):
     """Metadata of a batch experiment."""
 
     status: str
     """Status of the batch experiment."""
     created_at: datetime
```

### Comparing `nextmv-0.5.0/nextmv/cloud/client.py` & `nextmv-0.5.1/nextmv/cloud/client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/cloud/input_set.py` & `nextmv-0.5.1/nextmv/cloud/input_set.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/check/__init__.py` & `nextmv-0.5.1/nextmv/nextroute/check/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/check/schema.py` & `nextmv-0.5.1/nextmv/nextroute/check/schema.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/schema/__init__.py` & `nextmv-0.5.1/nextmv/nextroute/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/schema/input.py` & `nextmv-0.5.1/nextmv/nextroute/schema/input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/schema/output.py` & `nextmv-0.5.1/nextmv/nextroute/schema/output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/schema/stop.py` & `nextmv-0.5.1/nextmv/nextroute/schema/stop.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/nextmv/nextroute/schema/vehicle.py` & `nextmv-0.5.1/nextmv/nextroute/schema/vehicle.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/test_base_model.py` & `nextmv-0.5.1/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/cloud/test_client.py` & `nextmv-0.5.1/tests/cloud/test_client.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/nextroute/schema/input.json` & `nextmv-0.5.1/tests/nextroute/schema/input.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/nextroute/schema/output.json` & `nextmv-0.5.1/tests/nextroute/schema/output.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/nextroute/schema/output_with_check.json` & `nextmv-0.5.1/tests/nextroute/schema/output_with_check.json`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/nextroute/schema/test_input.py` & `nextmv-0.5.1/tests/nextroute/schema/test_input.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/tests/nextroute/schema/test_output.py` & `nextmv-0.5.1/tests/nextroute/schema/test_output.py`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/.gitignore` & `nextmv-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/LICENSE` & `nextmv-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/README.md` & `nextmv-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/pyproject.toml` & `nextmv-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nextmv-0.5.0/PKG-INFO` & `nextmv-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextmv
-Version: 0.5.0
+Version: 0.5.1
 Summary: The Python SDK for Nextmv
 Project-URL: Homepage, https://www.nextmv.io
 Project-URL: Documentation, https://www.nextmv.io/docs
 Project-URL: Repository, https://github.com/nextmv-io/nextmv-py
 Author-email: Nextmv <tech@nextmv.io>
 Maintainer-email: Nextmv <tech@nextmv.io>
 License:                                  Apache License
```

