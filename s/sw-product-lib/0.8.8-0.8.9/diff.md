# Comparing `tmp/sw_product_lib-0.8.8.tar.gz` & `tmp/sw_product_lib-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.8.8.tar", max compression
+gzip compressed data, was "sw_product_lib-0.8.9.tar", max compression
```

## Comparing `sw_product_lib-0.8.8.tar` & `sw_product_lib-0.8.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1010 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/apps/admin/__init__.py
--rw-r--r--   0        0        0     4784 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/apps/admin/backend.py
--rw-r--r--   0        0        0     2504 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/apps/admin/status.py
--rw-r--r--   0        0        0        0 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0     2953 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2024-03-11 16:04:25.375162 sw_product_lib-0.8.8/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0     7097 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     2186 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0        0 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/platform/__init__.py
--rw-r--r--   0        0        0      331 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    30814 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/service.py
--rw-r--r--   0        0        0     9932 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/types/backend.py
--rw-r--r--   0        0        0     2416 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/types/batch_job.py
--rw-r--r--   0        0        0    23363 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/types/job.py
--rw-r--r--   0        0        0     8871 2024-03-11 16:04:25.379162 sw_product_lib-0.8.8/sw_product_lib/types/resource.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 sw_product_lib-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1010 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:39.472758 sw_product_lib-0.8.9/sw_product_lib/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/__init__.py
+-rw-r--r--   0        0        0     4784 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/backend.py
+-rw-r--r--   0        0        0     2504 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/apps/admin/status.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0     2953 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0     7097 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     2186 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0        0 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/platform/__init__.py
+-rw-r--r--   0        0        0      331 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    33154 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/service.py
+-rw-r--r--   0        0        0     9932 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/backend.py
+-rw-r--r--   0        0        0     2416 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/batch_job.py
+-rw-r--r--   0        0        0    23981 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/job.py
+-rw-r--r--   0        0        0     8871 2024-03-21 02:43:39.476758 sw_product_lib-0.8.9/sw_product_lib/types/resource.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 sw_product_lib-0.8.9/PKG-INFO
```

### Comparing `sw_product_lib-0.8.8/pyproject.toml` & `sw_product_lib-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.flake8]
 max-line-length = 88
 per-file-ignores = ["__init__.py:F401", "./docs/*:E402"]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.8.8"
+version = "0.8.9"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 gql = "^3.4.1"
```

### Comparing `sw_product_lib-0.8.8/sw_product_lib/apps/admin/backend.py` & `sw_product_lib-0.8.9/sw_product_lib/apps/admin/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/apps/admin/status.py` & `sw_product_lib-0.8.9/sw_product_lib/apps/admin/status.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/client/backend.py` & `sw_product_lib-0.8.9/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/client/billing.py` & `sw_product_lib-0.8.9/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/client/job.py` & `sw_product_lib-0.8.9/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/client/resource.py` & `sw_product_lib-0.8.9/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/service.py` & `sw_product_lib-0.8.9/sw_product_lib/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """product.py."""
 
 import json
 import tempfile
 from dataclasses import dataclass
 from functools import singledispatch
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 from deprecated import deprecated
 from fastapi import Request
 from jose import jwt
 from strangeworks_core.config.config import Config
 from strangeworks_core.errors.error import StrangeworksError
@@ -511,14 +511,73 @@
                 raise StrangeworksError(
                     "unable to upload job file", r.status_code, str(r.content)
                 )
 
     return f
 
 
+def get_jobs(
+    ctx: ServiceContext,
+    resource_slug: str | None = None,
+    parent_job_slug: str | None = None,
+    tags: List[str] | None = None,
+    statuses: List[str] | None = None,
+    cursor: str | None = None,
+    batch_size: int = 50,
+) -> Tuple[List[Job], str, bool]:
+    """Get Jobs (pagination)
+
+    Uses pagination to retrieve list of jobs which match given filters.
+    Example of how to paginate over jobs:
+
+    has_next_page: bool = True
+    cursor: str = None
+    while has_next_page:
+        jobs, cursor, has_next_page = service.get_jobs(ctx, cursor=cursor)
+        ...
+        # do something with jobs
+
+    Avoid reading the complete list of jobs in order to not crash the application due
+    insufficient memory. Read jobs in chunks, use them as needed then release by
+    dereferencing the list so that the garbage collector can claim the unused memory.
+
+    Parameters
+    ----------
+    ctx: ServiceContext
+        contains key-values specific to the current request.
+    resource_slug: str | None = None
+        filters jobs by resource. If ctx is RequestType, ctx.resource_slug can be used.
+        Defaults to None.
+    parent_job_slug: str | None = None
+        filters jobs by their parent slug. Defaults to None.
+    tags: List[str] | None = None
+        filters jobs by their tags. Only jobs which have a tag that matches any in the
+        list will be returned. Defaults to None.
+    statuses: List[str] | None = None
+        filters jobs by their status. Only jobs whose status matches one in the list
+        will be returned. Defaults to None.
+    cursor: str | None = None
+        Used for pagination. The cursor value from prior call must be supplied in order
+        to paginate over the complete result set. The initial value should be None,
+        unless the caller wishes the pagination to begin at a certain cursor. Note that
+        the cursor may become invalid if its associated job entry is deleted.
+    batch_size: int = 50
+        Number of job objects to retrieve with each call. Limited to 50.
+    """
+    return job.get_list(
+        api=ctx.api or _api(),
+        resource_slug=resource_slug,
+        parent_job_slug=parent_job_slug,
+        tags=tags,
+        statuses=statuses,
+        start_cursor=cursor,
+        batch_size=50 if batch_size > 50 else batch_size,
+    )
+
+
 def get_job(ctx: RequestContext, job_slug: str) -> Job:
     """Get the job identified by job_slug.
 
 
     Parameters
     ----------
     ctx: RequestContext
```

### Comparing `sw_product_lib-0.8.8/sw_product_lib/types/backend.py` & `sw_product_lib-0.8.9/sw_product_lib/types/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/types/batch_job.py` & `sw_product_lib-0.8.9/sw_product_lib/types/batch_job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/sw_product_lib/types/job.py` & `sw_product_lib-0.8.9/sw_product_lib/types/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urljoin
 
 import requests
+from deprecated import deprecated
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.platform import auth
 from strangeworks_core.platform.gql import API, Operation
 from strangeworks_core.types.file import File as FileBase
 from strangeworks_core.types.job import Job as JobBase
 from strangeworks_core.types.job import Status as JobStatus
 from strangeworks_core.utils import str_to_datetime
@@ -363,21 +364,37 @@
 get_jobs_request = Operation(
     query="""
         query jobs(
             $external_identifier: String,
             $resource_slug: String,
             $parent_job_slug: String,
             $statuses: [JobStatus!]
+            $tags: [String!]
+            $first: Int,
+            $last: Int,
+            $before: ID,
+            $after: ID,
         ) {
             jobs(
-                externalIdentifier: $external_identifier,
-                resourceSlug: $resource_slug,
-                parentJobSlug: $parent_job_slug,
+                externalIdentifier: $external_identifier
+                resourceSlug: $resource_slug
+                parentJobSlug: $parent_job_slug
                 statuses: $statuses
+                jobTags: $tags
+                pagination: {
+                    before: $before
+                    after: $after
+                    first: $first
+                    last: $last
+                }
             ) {
+                pageInfo {
+                    endCursor
+                    hasNextPage
+                }
                 edges {
                     node {
                         id
                         slug
                         status
                         parentJob {
                             slug
@@ -394,14 +411,45 @@
                 }
             }
         }
 """,
 )
 
 
+def get_list(
+    api: API, start_cursor: str = None, batch_size: int = 50, **kwargs
+) -> Tuple[List[Job], str, bool]:
+    """Return list of jobs."""
+    # has_next_page = True
+    # jobs = []
+    # while has_next_page:
+    platform_result = api.execute(
+        op=get_jobs_request, first=batch_size, after=start_cursor, **kwargs
+    )
+    if "jobs" not in platform_result:
+        raise StrangeworksError(
+            message="Missing field ('jobs') in response to jobs query",
+            status_code=500,
+        )
+    edges = platform_result.get("jobs").get("edges")
+    if edges is None:
+        raise StrangeworksError(
+            message="Missing field ('edges') in response to jobs query",
+            status_code=500,
+        )
+
+    if len(platform_result["jobs"]["edges"]) == 0:
+        return ([], None, False)
+
+    jobs = [Job.from_dict(edge["node"]) for edge in edges if "node" in edge]
+    cursor = platform_result.get("jobs").get("pageInfo").get("endCursor")
+    has_next_page = platform_result.get("jobs").get("pageInfo").get("hasNextPage")
+    return (jobs, cursor, has_next_page)
+
+
 def get_by_external_identifier(
     api: API,
     id: str,
 ) -> Optional[Job]:
     """Retrieve job info
 
     Parameters
@@ -412,44 +460,23 @@
         the external_identifier used to retrieve the job.
 
     Returns
     -------
     Job
         The ``Job`` object identified by id or None.
     """
-    platform_result = api.execute(
-        op=get_jobs_request,
-        external_identifier=id,
-    )
-    if "jobs" not in platform_result:
+    as_list, _, _ = get_list(api=api, external_identifier=id)
+    if len(as_list) > 1:
         raise StrangeworksError(
-            message="Missing field ('jobs') in response to jobs query", status_code=400
+            message=f"More than one job returned for remote id {id}", status_code=500
         )
-    if "edges" not in platform_result["jobs"]:
-        raise StrangeworksError(
-            message="Missing field ('edges') in response to jobs query", status_code=400
-        )
-
-    if len(platform_result["jobs"]["edges"]) == 0:
-        return None
-
-    if len(platform_result["jobs"]["edges"]) > 1:
-        raise StrangeworksError(
-            message="More than one job returned for product identifier", status_code=400
-        )
-
-    if "node" not in platform_result["jobs"]["edges"][0]:
-        raise StrangeworksError(
-            message="Missing field ('node') in response to jobs query", status_code=400
-        )
-
-    val = platform_result["jobs"]["edges"][0]["node"]
-    return Job.from_dict(val)
+    return None if len(as_list) == 0 else as_list[0]
 
 
+@deprecated(reason="This function is deprecated. Use job.get_list instead.")
 def get_by_statuses(
     api: API, statuses: List[JobStatus]
 ) -> Optional[Dict[JobStatus, List[Job]]]:
     """Retrieve jobs filtered by job statuses.
 
     Parameters:
     ----------
@@ -462,30 +489,23 @@
     ----------
     A dictionary where the jobs are grouped by statuses.
     The keys in the dictionary are the statuses.
     Each status has their list of jobs.
 
     Optional[Dict[JobStatus, List[Job]]]
     """
-
-    platform_result = api.execute(op=get_jobs_request, statuses=statuses)
-    if "jobs" not in platform_result:
-        raise StrangeworksError(
-            message="Missing field ('jobs') in response to jobs query", status_code=400
-        )
-    if "edges" not in platform_result["jobs"]:
-        raise StrangeworksError(
-            message="Missing field ('edges') in response to jobs query", status_code=400
+    has_next_page: bool = True
+    cursor: str = None
+    jobs: List[Job] = []
+    while has_next_page:
+        jobs_batch, cursor, has_next_page = get_list(
+            api=api, start_cursor=cursor, statuses=statuses
         )
+        jobs.extend(jobs_batch)
 
-    edges = platform_result["jobs"]["edges"]
-    if len(edges) == 0:
-        return None
-
-    jobs = [Job.from_dict(edge["node"]) for edge in edges if "node" in edge]
     jobs_grouped_by_status = defaultdict(list)
     for job in jobs:
         jobs_grouped_by_status[JobStatus(job.status.strip().upper())].append(job)
     # ensure statuses with no jobs are in the dict
     statuses_with_no_jobs = set(statuses) - set(jobs_grouped_by_status.keys())
     for status in statuses_with_no_jobs:
         jobs_grouped_by_status[status]
```

### Comparing `sw_product_lib-0.8.8/sw_product_lib/types/resource.py` & `sw_product_lib-0.8.9/sw_product_lib/types/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.8.8/PKG-INFO` & `sw_product_lib-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

