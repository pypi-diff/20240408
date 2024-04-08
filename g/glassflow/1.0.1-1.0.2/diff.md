# Comparing `tmp/glassflow-1.0.1.tar.gz` & `tmp/glassflow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassflow-1.0.1.tar", last modified: Thu Apr  4 12:09:16 2024, max compression
+gzip compressed data, was "glassflow-1.0.2.tar", last modified: Mon Apr  8 10:00:36 2024, max compression
```

## Comparing `glassflow-1.0.1.tar` & `glassflow-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 12:09:09.000000 glassflow-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-04 12:09:16.509062 glassflow-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-04 12:09:09.000000 glassflow-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 12:09:09.000000 glassflow-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:09:16.509062 glassflow-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 12:09:09.000000 glassflow-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.501062 glassflow-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/clienterror.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/errors/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.505062 glassflow-1.0.1/src/glassflow/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/consumeevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/consumefailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/models/operations/publishevent.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/src/glassflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-04 12:09:09.000000 glassflow-1.0.1/src/glassflow/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:09:16.509062 glassflow-1.0.1/src/glassflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 12:09:16.000000 glassflow-1.0.1/src/glassflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 10:00:32.000000 glassflow-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-08 10:00:36.538823 glassflow-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-08 10:00:32.000000 glassflow-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 10:00:32.000000 glassflow-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:00:36.538823 glassflow-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 10:00:32.000000 glassflow-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/glassflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/glassflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/clienterror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/consumeevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/consumefailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/publishevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/top_level.txt
```

### Comparing `glassflow-1.0.1/LICENSE.md` & `glassflow-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/PKG-INFO` & `glassflow-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassflow
-Version: 1.0.1
+Version: 1.0.2
 Summary: GlassFlow Python Client SDK
 Home-page: https://learn.glassflow.dev/docs
 Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -51,29 +51,30 @@
 pip install glassflow
 ```
 
 ## Available Operations
 
 * [publish](#publish) - Publish a new event into the pipeline
 * [consume](#consume) - Consume the transformed event from the pipeline
+* [consume failed](#consume-failed) - Consume the events that failed from the pipeline
 
 
 ## publish
 
 Publish a new event into the pipeline
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
 data = {} # your json event
-res = pipeline_client.publish(request_body=data, pipeline_access_token="<str token>")
+res = pipeline_client.publish(request_body=data)
 
 if res.status_code == 200:
     print("Published sucessfully")
 ```
 
 
 ## consume
@@ -82,16 +83,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 ## consume failed
 
@@ -99,16 +100,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume_failed(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume_failed()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glassflow Version: 1.0.1 Summary: GlassFlow Python
+Metadata-Version: 2.1 Name: glassflow Version: 1.0.2 Summary: GlassFlow Python
 Client SDK Home-page: https://learn.glassflow.dev/docs Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: urllib3==1.26.15 Requires-Dist: certifi>=2023.7.22
 Requires-Dist: charset-normalizer>=3.2.0 Requires-Dist: dataclasses-json>=0.6.4
 Requires-Dist: idna>=3.4 Requires-Dist: jsonpath-python>=1.0.6 Requires-Dist:
 marshmallow>=3.19.0 Requires-Dist: mypy-extensions>=1.0.0 Requires-Dist:
@@ -22,28 +22,30 @@
 consume events to your [GlassFlow pipelines](https://learn.glassflow.dev/docs/
    concepts/pipeline-configuration). See how it is easy to setup a new data
  pipeline and do data transformation with GlassFlow: ![GlassFlow data pipeline
  creation](/assets/GlassFlow%20quickstart.gif) ## Installation You can install
    the GlassFlow Python SDK using pip: ```shell pip install glassflow ``` ##
    Available Operations * [publish](#publish) - Publish a new event into the
     pipeline * [consume](#consume) - Consume the transformed event from the
-  pipeline ## publish Publish a new event into the pipeline ### Example Usage
-```python import glassflow client = glassflow.GlassFlowClient() pipeline_client
-   = client.pipeline_client(space_id="", pipeline_id=" your json event res =
-    pipeline_client.publish(request_body=data, pipeline_access_token="") if
+ pipeline * [consume failed](#consume-failed) - Consume the events that failed
+from the pipeline ## publish Publish a new event into the pipeline ### Example
+     Usage ```python import glassflow client = glassflow.GlassFlowClient()
+pipeline_client = client.pipeline_client(space_id="", pipeline_id=" data = {} #
+      your json event res = pipeline_client.publish(request_body=data) if
  res.status_code == 200: print("Published sucessfully") ``` ## consume Consume
   the transformed event from the pipeline ### Example Usage ```python import
        glassflow client = glassflow.GlassFlowClient() pipeline_client =
-client.pipeline_client(space_id="", pipeline_id="") if res.status_code == 200:
- print(res.body.event) ``` ## consume failed If the transformation failed for
- any event, they are available in a failed queue. You can consume those events
-    from the pipeline ### Example Usage ```python import glassflow client =
-     glassflow.GlassFlowClient() pipeline_client = client.pipeline_client
-(space_id="", pipeline_id="") if res.status_code == 200: print(res.body.event)
-         ``` ## Quickstart Follow the quickstart guide [here](https://
+client.pipeline_client(space_id="", pipeline_id=" res = pipeline_client.consume
+ () if res.status_code == 200: print(res.body.event) ``` ## consume failed If
+the transformation failed for any event, they are available in a failed queue.
+  You can consume those events from the pipeline ### Example Usage ```python
+    import glassflow client = glassflow.GlassFlowClient() pipeline_client =
+            client.pipeline_client(space_id="", pipeline_id=" res =
+       pipeline_client.consume_failed() if res.status_code == 200: print
+(res.body.event) ``` ## Quickstart Follow the quickstart guide [here](https://
   learn.glassflow.dev/docs/get-started/quickstart) ## Code Samples [GlassFlow
   Examples](https://github.com/glassflow/glassflow-examples) ## SDK Maturity
  Please note that the GlassFlow Python SDK is currently in beta and is subject
   to potential breaking changes. We recommend keeping an eye on the official
  documentation and updating your code accordingly to ensure compatibility with
 future versions of the SDK. ## User Guides For more detailed information on how
 to use the GlassFlow Python SDK, please refer to the [GlassFlow Documentation](
```

### Comparing `glassflow-1.0.1/README.md` & `glassflow-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,30 @@
 pip install glassflow
 ```
 
 ## Available Operations
 
 * [publish](#publish) - Publish a new event into the pipeline
 * [consume](#consume) - Consume the transformed event from the pipeline
+* [consume failed](#consume-failed) - Consume the events that failed from the pipeline
 
 
 ## publish
 
 Publish a new event into the pipeline
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
 data = {} # your json event
-res = pipeline_client.publish(request_body=data, pipeline_access_token="<str token>")
+res = pipeline_client.publish(request_body=data)
 
 if res.status_code == 200:
     print("Published sucessfully")
 ```
 
 
 ## consume
@@ -55,16 +56,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 ## consume failed
 
@@ -72,16 +73,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume_failed(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume_failed()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -10,28 +10,30 @@
 consume events to your [GlassFlow pipelines](https://learn.glassflow.dev/docs/
    concepts/pipeline-configuration). See how it is easy to setup a new data
  pipeline and do data transformation with GlassFlow: ![GlassFlow data pipeline
  creation](/assets/GlassFlow%20quickstart.gif) ## Installation You can install
    the GlassFlow Python SDK using pip: ```shell pip install glassflow ``` ##
    Available Operations * [publish](#publish) - Publish a new event into the
     pipeline * [consume](#consume) - Consume the transformed event from the
-  pipeline ## publish Publish a new event into the pipeline ### Example Usage
-```python import glassflow client = glassflow.GlassFlowClient() pipeline_client
-   = client.pipeline_client(space_id="", pipeline_id=" your json event res =
-    pipeline_client.publish(request_body=data, pipeline_access_token="") if
+ pipeline * [consume failed](#consume-failed) - Consume the events that failed
+from the pipeline ## publish Publish a new event into the pipeline ### Example
+     Usage ```python import glassflow client = glassflow.GlassFlowClient()
+pipeline_client = client.pipeline_client(space_id="", pipeline_id=" data = {} #
+      your json event res = pipeline_client.publish(request_body=data) if
  res.status_code == 200: print("Published sucessfully") ``` ## consume Consume
   the transformed event from the pipeline ### Example Usage ```python import
        glassflow client = glassflow.GlassFlowClient() pipeline_client =
-client.pipeline_client(space_id="", pipeline_id="") if res.status_code == 200:
- print(res.body.event) ``` ## consume failed If the transformation failed for
- any event, they are available in a failed queue. You can consume those events
-    from the pipeline ### Example Usage ```python import glassflow client =
-     glassflow.GlassFlowClient() pipeline_client = client.pipeline_client
-(space_id="", pipeline_id="") if res.status_code == 200: print(res.body.event)
-         ``` ## Quickstart Follow the quickstart guide [here](https://
+client.pipeline_client(space_id="", pipeline_id=" res = pipeline_client.consume
+ () if res.status_code == 200: print(res.body.event) ``` ## consume failed If
+the transformation failed for any event, they are available in a failed queue.
+  You can consume those events from the pipeline ### Example Usage ```python
+    import glassflow client = glassflow.GlassFlowClient() pipeline_client =
+            client.pipeline_client(space_id="", pipeline_id=" res =
+       pipeline_client.consume_failed() if res.status_code == 200: print
+(res.body.event) ``` ## Quickstart Follow the quickstart guide [here](https://
   learn.glassflow.dev/docs/get-started/quickstart) ## Code Samples [GlassFlow
   Examples](https://github.com/glassflow/glassflow-examples) ## SDK Maturity
  Please note that the GlassFlow Python SDK is currently in beta and is subject
   to potential breaking changes. We recommend keeping an eye on the official
  documentation and updating your code accordingly to ensure compatibility with
 future versions of the SDK. ## User Guides For more detailed information on how
 to use the GlassFlow Python SDK, please refer to the [GlassFlow Documentation](
```

### Comparing `glassflow-1.0.1/setup.py` & `glassflow-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="glassflow",
-    version="1.0.1",
+    version="1.0.2",
     author="glassflow",
     description="GlassFlow Python Client SDK",
     url="https://learn.glassflow.dev/docs",
     project_urls={
         'Source': 'https://github.com/glassflow/glassflow-python-sdk',
     },
     long_description=long_description,
```

### Comparing `glassflow-1.0.1/src/glassflow/client.py` & `glassflow-1.0.2/src/glassflow/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,23 @@
         Args:
             organization_id: Organization ID of the user. If not provided, the default organization will be used
         """
         rclient = requests_http.Session()
         self.glassflow_config = GlassFlowConfig(rclient)
         self.organization_id = organization_id
 
-    def pipeline_client(self, space_id: str,
-                        pipeline_id: str) -> PipelineClient:
+    def pipeline_client(self, space_id: str, pipeline_id: str,
+                        pipeline_access_token: str) -> PipelineClient:
         """Create a new PipelineClient object to interact with a specific pipeline
 
         Args:
             space_id: The space id where the pipeline is located
             pipeline_id: The pipeline id to interact with
+            pipeline_access_token: The access token to access the pipeline
 
         Returns:
             PipelineClient: Client object to publish and consume events from the given pipeline.
         """
         return PipelineClient(glassflow_client=self,
                               space_id=space_id,
-                              pipeline_id=pipeline_id)
+                              pipeline_id=pipeline_id,
+                              pipeline_access_token=pipeline_access_token)
```

### Comparing `glassflow-1.0.1/src/glassflow/config.py` & `glassflow-1.0.2/src/glassflow/config.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/models/errors/clienterror.py` & `glassflow-1.0.2/src/glassflow/models/errors/clienterror.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/models/errors/error.py` & `glassflow-1.0.2/src/glassflow/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/models/operations/consumeevent.py` & `glassflow-1.0.2/src/glassflow/models/operations/consumeevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/models/operations/consumefailed.py` & `glassflow-1.0.2/src/glassflow/models/operations/consumefailed.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/models/operations/publishevent.py` & `glassflow-1.0.2/src/glassflow/models/operations/publishevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow/pipelines.py` & `glassflow-1.0.2/src/glassflow/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,49 +7,50 @@
     """Client object to publish and consume events from the given pipeline.
 
     Attributes:
         glassflow_client: GlassFlowClient object to interact with GlassFlow API
         space_id: The space id where the pipeline is located
         pipeline_id: The pipeline id to interact with
         organization_id: Organization ID of the user. If not provided, the default organization will be used
+        pipeline_access_token: The access token to access the pipeline
     """
 
-    def __init__(self, glassflow_client, space_id: str,
-                 pipeline_id: str) -> None:
+    def __init__(self, glassflow_client, space_id: str, pipeline_id: str,
+                 pipeline_access_token: str) -> None:
         """Create a new PipelineClient object to interact with a specific pipeline
 
         Args:
             glassflow_client: GlassFlowClient object to interact with GlassFlow API
             space_id: The space id where the pipeline is located
             pipeline_id: The pipeline id to interact with
+            pipeline_access_token: The access token to access the pipeline
         """
         self.glassflow_client = glassflow_client
         self.space_id = space_id
         self.pipeline_id = pipeline_id
         self.organization_id = self.glassflow_client.organization_id
+        self.pipeline_access_token = pipeline_access_token
 
-    def publish(self, request_body: dict,
-                pipeline_access_token: str) -> operations.PublishEventResponse:
+    def publish(self, request_body: dict) -> operations.PublishEventResponse:
         """Push a new message into the pipeline
 
         Args:
             request_body: The message to be published into the pipeline
-            pipeline_access_token: The access token to access the pipeline
 
         Returns:
             PublishEventResponse: Response object containing the status code and the raw response
 
         Raises:
             ClientError: If an error occurred while publishing the event
         """
         request = operations.PublishEventRequest(
             organization_id=self.organization_id,
             space_id=self.space_id,
             pipeline_id=self.pipeline_id,
-            x_pipeline_access_token=pipeline_access_token,
+            x_pipeline_access_token=self.pipeline_access_token,
             request_body=request_body,
         )
 
         base_url = self.glassflow_client.glassflow_config.server_url
 
         url = utils.generate_url(
             operations.PublishEventRequest, base_url,
@@ -97,33 +98,29 @@
         elif http_res.status_code == 401 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.ClientError('API error occurred',
                                      http_res.status_code, http_res.text,
                                      http_res)
 
         return res
 
-    def consume(self,
-                pipeline_access_token: str) -> operations.ConsumeEventResponse:
+    def consume(self) -> operations.ConsumeEventResponse:
         """Consume the last message from the pipeline
 
-        Args:
-            pipeline_access_token: The access token to access the pipeline
-
         Returns:
             ConsumeEventResponse: Response object containing the status code and the raw response
 
         Raises:
             ClientError: If an error occurred while consuming the event
 
         """
         request = operations.ConsumeEventRequest(
             space_id=self.space_id,
             pipeline_id=self.pipeline_id,
             organization_id=self.organization_id,
-            x_pipeline_access_token=pipeline_access_token,
+            x_pipeline_access_token=self.pipeline_access_token,
         )
 
         base_url = self.glassflow_client.glassflow_config.server_url
 
         url = utils.generate_url(
             operations.ConsumeEventRequest, base_url,
             '/pipelines/{pipeline_id}/topics/output/events/consume', request)
@@ -170,34 +167,29 @@
         elif http_res.status_code == 401 or http_res.status_code == 404 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.ClientError('API error occurred',
                                      http_res.status_code, http_res.text,
                                      http_res)
 
         return res
 
-    def consume_failed(
-            self,
-            pipeline_access_token: str) -> operations.ConsumeFailedResponse:
+    def consume_failed(self) -> operations.ConsumeFailedResponse:
         """Consume the failed message from the pipeline
 
-        Args:
-            pipeline_access_token: The access token to access the pipeline
-
         Returns:
             ConsumeFailedResponse: Response object containing the status code and the raw response
 
         Raises:
             ClientError: If an error occurred while consuming the event
 
         """
         request = operations.ConsumeFailedRequest(
             space_id=self.space_id,
             pipeline_id=self.pipeline_id,
             organization_id=self.organization_id,
-            x_pipeline_access_token=pipeline_access_token,
+            x_pipeline_access_token=self.pipeline_access_token,
         )
 
         base_url = self.glassflow_client.glassflow_config.server_url
 
         url = utils.generate_url(
             operations.ConsumeFailedRequest, base_url,
             '/pipelines/{pipeline_id}/topics/failed/events/consume', request)
```

### Comparing `glassflow-1.0.1/src/glassflow/utils/utils.py` & `glassflow-1.0.2/src/glassflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.1/src/glassflow.egg-info/PKG-INFO` & `glassflow-1.0.2/src/glassflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassflow
-Version: 1.0.1
+Version: 1.0.2
 Summary: GlassFlow Python Client SDK
 Home-page: https://learn.glassflow.dev/docs
 Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -51,29 +51,30 @@
 pip install glassflow
 ```
 
 ## Available Operations
 
 * [publish](#publish) - Publish a new event into the pipeline
 * [consume](#consume) - Consume the transformed event from the pipeline
+* [consume failed](#consume-failed) - Consume the events that failed from the pipeline
 
 
 ## publish
 
 Publish a new event into the pipeline
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
 data = {} # your json event
-res = pipeline_client.publish(request_body=data, pipeline_access_token="<str token>")
+res = pipeline_client.publish(request_body=data)
 
 if res.status_code == 200:
     print("Published sucessfully")
 ```
 
 
 ## consume
@@ -82,16 +83,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 ## consume failed
 
@@ -99,16 +100,16 @@
 
 ### Example Usage
 
 ```python
 import glassflow
 
 client = glassflow.GlassFlowClient()
-pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value")
-res = pipeline_client.consume_failed(pipeline_access_token="<str value>")
+pipeline_client = client.pipeline_client(space_id="<str value>", pipeline_id="<str value", pipeline_access_token="<str value>")
+res = pipeline_client.consume_failed()
 
 if res.status_code == 200:
     print(res.body.event)
 ```
 
 
 ## Quickstart
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glassflow Version: 1.0.1 Summary: GlassFlow Python
+Metadata-Version: 2.1 Name: glassflow Version: 1.0.2 Summary: GlassFlow Python
 Client SDK Home-page: https://learn.glassflow.dev/docs Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: urllib3==1.26.15 Requires-Dist: certifi>=2023.7.22
 Requires-Dist: charset-normalizer>=3.2.0 Requires-Dist: dataclasses-json>=0.6.4
 Requires-Dist: idna>=3.4 Requires-Dist: jsonpath-python>=1.0.6 Requires-Dist:
 marshmallow>=3.19.0 Requires-Dist: mypy-extensions>=1.0.0 Requires-Dist:
@@ -22,28 +22,30 @@
 consume events to your [GlassFlow pipelines](https://learn.glassflow.dev/docs/
    concepts/pipeline-configuration). See how it is easy to setup a new data
  pipeline and do data transformation with GlassFlow: ![GlassFlow data pipeline
  creation](/assets/GlassFlow%20quickstart.gif) ## Installation You can install
    the GlassFlow Python SDK using pip: ```shell pip install glassflow ``` ##
    Available Operations * [publish](#publish) - Publish a new event into the
     pipeline * [consume](#consume) - Consume the transformed event from the
-  pipeline ## publish Publish a new event into the pipeline ### Example Usage
-```python import glassflow client = glassflow.GlassFlowClient() pipeline_client
-   = client.pipeline_client(space_id="", pipeline_id=" your json event res =
-    pipeline_client.publish(request_body=data, pipeline_access_token="") if
+ pipeline * [consume failed](#consume-failed) - Consume the events that failed
+from the pipeline ## publish Publish a new event into the pipeline ### Example
+     Usage ```python import glassflow client = glassflow.GlassFlowClient()
+pipeline_client = client.pipeline_client(space_id="", pipeline_id=" data = {} #
+      your json event res = pipeline_client.publish(request_body=data) if
  res.status_code == 200: print("Published sucessfully") ``` ## consume Consume
   the transformed event from the pipeline ### Example Usage ```python import
        glassflow client = glassflow.GlassFlowClient() pipeline_client =
-client.pipeline_client(space_id="", pipeline_id="") if res.status_code == 200:
- print(res.body.event) ``` ## consume failed If the transformation failed for
- any event, they are available in a failed queue. You can consume those events
-    from the pipeline ### Example Usage ```python import glassflow client =
-     glassflow.GlassFlowClient() pipeline_client = client.pipeline_client
-(space_id="", pipeline_id="") if res.status_code == 200: print(res.body.event)
-         ``` ## Quickstart Follow the quickstart guide [here](https://
+client.pipeline_client(space_id="", pipeline_id=" res = pipeline_client.consume
+ () if res.status_code == 200: print(res.body.event) ``` ## consume failed If
+the transformation failed for any event, they are available in a failed queue.
+  You can consume those events from the pipeline ### Example Usage ```python
+    import glassflow client = glassflow.GlassFlowClient() pipeline_client =
+            client.pipeline_client(space_id="", pipeline_id=" res =
+       pipeline_client.consume_failed() if res.status_code == 200: print
+(res.body.event) ``` ## Quickstart Follow the quickstart guide [here](https://
   learn.glassflow.dev/docs/get-started/quickstart) ## Code Samples [GlassFlow
   Examples](https://github.com/glassflow/glassflow-examples) ## SDK Maturity
  Please note that the GlassFlow Python SDK is currently in beta and is subject
   to potential breaking changes. We recommend keeping an eye on the official
  documentation and updating your code accordingly to ensure compatibility with
 future versions of the SDK. ## User Guides For more detailed information on how
 to use the GlassFlow Python SDK, please refer to the [GlassFlow Documentation](
```

### Comparing `glassflow-1.0.1/src/glassflow.egg-info/SOURCES.txt` & `glassflow-1.0.2/src/glassflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

