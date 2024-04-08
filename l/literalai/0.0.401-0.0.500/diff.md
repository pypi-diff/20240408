# Comparing `tmp/literalai-0.0.401.tar.gz` & `tmp/literalai-0.0.500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.401.tar", last modified: Sat Mar 30 15:40:30 2024, max compression
+gzip compressed data, was "literalai-0.0.500.tar", last modified: Mon Apr  8 09:20:56 2024, max compression
```

## Comparing `literalai-0.0.401.tar` & `literalai-0.0.500.tar`

### file list

```diff
@@ -1,39 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.013003 literalai-0.0.401/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-30 15:40:23.000000 literalai-0.0.401/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-30 15:40:30.013003 literalai-0.0.401/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-30 15:40:23.000000 literalai-0.0.401/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.009003 literalai-0.0.401/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63271 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.013003 literalai-0.0.401/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.013003 literalai-0.0.401/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-03-30 15:40:23.000000 literalai-0.0.401/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.013003 literalai-0.0.401/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-30 15:40:29.000000 literalai-0.0.401/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-30 15:40:29.000000 literalai-0.0.401/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:40:29.000000 literalai-0.0.401/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-30 15:40:29.000000 literalai-0.0.401/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-30 15:40:29.000000 literalai-0.0.401/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:40:30.013003 literalai-0.0.401/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-30 15:40:23.000000 literalai-0.0.401/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:30.013003 literalai-0.0.401/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:40:23.000000 literalai-0.0.401/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.017223 literalai-0.0.500/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 09:20:34.000000 literalai-0.0.500/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 09:20:56.017223 literalai-0.0.500/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 09:20:34.000000 literalai-0.0.500/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.013223 literalai-0.0.500/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.017223 literalai-0.0.500/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    36330 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.017223 literalai-0.0.500/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.017223 literalai-0.0.500/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-08 09:20:34.000000 literalai-0.0.500/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.013223 literalai-0.0.500/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 09:20:55.000000 literalai-0.0.500/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 09:20:55.000000 literalai-0.0.500/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:20:55.000000 literalai-0.0.500/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 09:20:55.000000 literalai-0.0.500/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 09:20:55.000000 literalai-0.0.500/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:20:56.017223 literalai-0.0.500/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 09:20:34.000000 literalai-0.0.500/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:56.017223 literalai-0.0.500/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:34.000000 literalai-0.0.500/tests/__init__.py
```

### Comparing `literalai-0.0.401/LICENSE` & `literalai-0.0.500/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/README.md` & `literalai-0.0.500/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 @client.thread
 def main():
     print(my_step("Hello"))
 
 
 main()
-client.wait_until_queue_empty()
+client.flush_and_stop()
 print("Done")
 ```
 
 ## Development
 
 ### Setup
```

### Comparing `literalai-0.0.401/literalai/callback/langchain_callback.py` & `literalai-0.0.500/literalai/callback/langchain_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,15 @@
                         variables=variables,
                         duration=duration,
                         token_throughput_in_s=throughput,
                         tt_first_token=completion_start.get("tt_first_token"),
                         prompt=completion_start["prompt"],
                         completion=completion,
                     )
-                    current_step.output = completion
+                    current_step.output = {"content": completion}
 
                 if current_step:
                     if current_step.metadata is None:
                         current_step.metadata = {}
                     current_step.end()
 
                 return
@@ -465,15 +465,15 @@
 
         def _on_error(self, error: BaseException, *, run_id: "UUID", **kwargs: Any):
             if current_step := self.steps.get(str(run_id), None):
                 if current_step.metadata is None:
                     current_step.metadata = {}
                 current_step.error = str(error)
                 current_step.end()
-                self.client.flush_sync()
+                self.client.flush()
 
         on_llm_error = _on_error
         on_chain_error = _on_error
         on_tool_error = _on_error
         on_retriever_error = _on_error
 
     return LangchainTracer
```

### Comparing `literalai-0.0.401/literalai/client.py` & `literalai-0.0.500/literalai/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
-from literalai.api import API
+from literalai.api import AsyncLiteralAPI, LiteralAPI
 from literalai.callback.langchain_callback import get_langchain_callback
 from literalai.context import active_steps_var, active_thread_var
 from literalai.event_processor import EventProcessor
 from literalai.instrumentation.openai import instrument_openai
 from literalai.message import Message
 from literalai.my_types import Attachment
 from literalai.step import (
@@ -14,45 +14,62 @@
     StepContextManager,
     TrueStepType,
     step_decorator,
 )
 from literalai.thread import ThreadContextManager, thread_decorator
 
 
-class LiteralClient:
+class BaseLiteralClient:
+    api: Union[LiteralAPI, AsyncLiteralAPI]
+
     def __init__(
         self,
         batch_size: int = 1,
+        is_async: bool = False,
         api_key: Optional[str] = None,
         url: Optional[str] = None,
     ):
         if not api_key:
             api_key = os.getenv("LITERAL_API_KEY", None)
             if not api_key:
                 raise Exception("LITERAL_API_KEY not provided")
         if not url:
             url = os.getenv("LITERAL_API_URL", "https://cloud.getliteral.ai")
-        self.api = API(api_key=api_key, url=url)
+        if is_async:
+            self.api = AsyncLiteralAPI(api_key=api_key, url=url)
+        else:
+            self.api = LiteralAPI(api_key=api_key, url=url)
+
         self.event_processor = EventProcessor(
-            api=self.api,
+            api=LiteralAPI(api_key=api_key, url=url),
             batch_size=batch_size,
         )
 
+    def to_sync(self) -> "LiteralClient":
+        if isinstance(self.api, AsyncLiteralAPI):
+            return LiteralClient(
+                batch_size=self.event_processor.batch_size,
+                api_key=self.api.api_key,
+                url=self.api.url,
+            )
+        else:
+            return self  # type: ignore
+
     def instrument_openai(self):
-        instrument_openai(self)
+        instrument_openai(self.to_sync())
 
     def langchain_callback(
         self,
         to_ignore: Optional[List[str]] = None,
         to_keep: Optional[List[str]] = None,
         **kwargs: Any,
     ):
         LangchainTracer = get_langchain_callback()
         return LangchainTracer(
-            self,
+            self.to_sync(),
             to_ignore=to_ignore,
             to_keep=to_keep,
             **kwargs,
         )
 
     def thread(
         self,
@@ -117,27 +134,31 @@
             thread_id=thread_id,
         )
 
     def message(
         self,
         content: str = "",
         id: Optional[str] = None,
+        parent_id: Optional[str] = None,
         type: Optional[MessageStepType] = None,
         name: Optional[str] = None,
         thread_id: Optional[str] = None,
         attachments: List[Attachment] = [],
+        tags: Optional[List[str]] = None,
         metadata: Dict = {},
     ):
         step = Message(
             name=name,
             id=id,
+            parent_id=parent_id,
             thread_id=thread_id,
             type=type,
             content=content,
             attachments=attachments,
+            tags=tags,
             metadata=metadata,
             processor=self.event_processor,
         )
         step.end()
 
         return step
 
@@ -170,18 +191,41 @@
     def get_current_thread(self):
         return active_thread_var.get()
 
     def reset_context(self):
         active_steps_var.set([])
         active_thread_var.set(None)
 
-    def wait_until_queue_empty(self):
-        self.event_processor.flush_and_stop()
-
     def flush_and_stop(self):
         self.event_processor.flush_and_stop()
 
-    def flush_sync(self):
+
+class LiteralClient(BaseLiteralClient):
+    api: LiteralAPI
+
+    def __init__(
+        self,
+        batch_size: int = 1,
+        api_key: Optional[str] = None,
+        url: Optional[str] = None,
+    ):
+        super().__init__(
+            batch_size=batch_size, is_async=False, api_key=api_key, url=url
+        )
+
+    def flush(self):
         self.event_processor.flush()
 
+
+class AsyncLiteralClient(BaseLiteralClient):
+    api: AsyncLiteralAPI
+
+    def __init__(
+        self,
+        batch_size: int = 1,
+        api_key: Optional[str] = None,
+        url: Optional[str] = None,
+    ):
+        super().__init__(batch_size=batch_size, is_async=True, api_key=api_key, url=url)
+
     async def flush(self):
         await self.event_processor.aflush()
```

### Comparing `literalai-0.0.401/literalai/dataset_item.py` & `literalai-0.0.500/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai/event_processor.py` & `literalai-0.0.500/literalai/event_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import queue
 import threading
 import time
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
-    from literalai.api import API
+    from literalai.api import LiteralAPI
     from literalai.step import StepDict
 
 
 # to_thread is a backport of asyncio.to_thread from Python 3.9
 async def to_thread(func, /, *args, **kwargs):
     import contextvars
     import functools
@@ -19,15 +19,15 @@
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     return await loop.run_in_executor(None, func_call)
 
 
 class EventProcessor:
     event_queue: queue.Queue
 
-    def __init__(self, api: "API", batch_size: int = 1):
+    def __init__(self, api: "LiteralAPI", batch_size: int = 1):
         self.batch_size = batch_size
         self.api = api
         self.event_queue = queue.Queue()
         self.processing_thread = threading.Thread(
             target=self._process_events, daemon=True
         )
         self.processing_thread.start()
@@ -36,59 +36,53 @@
     def add_event(self, event: "StepDict"):
         self.event_queue.put(event)
 
     async def a_add_events(self, event: "StepDict"):
         await to_thread(self.event_queue.put, event)
 
     def _process_events(self):
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
         while True:
             batch: List["StepDict"] = []
             try:
                 # Try to fill the batch up to the batch_size
                 while len(batch) < self.batch_size:
                     # Attempt to get events with a timeout
                     event = self.event_queue.get(timeout=0.5)
                     batch.append(event)
             except queue.Empty:
                 # No more events at the moment, proceed with processing what's in the batch
                 pass
 
             # Process the batch if any events are present
             if batch:
-                loop.run_until_complete(self._process_batch(batch))
+                self._process_batch(batch)
 
             # Stop if the stop_event is set and the queue is empty
             if self.stop_event.is_set() and self.event_queue.empty():
                 break
 
-    async def _process_batch(self, batch):
-        res = await self.api.send_steps(
+    def _process_batch(self, batch):
+        res = self.api.send_steps(
             steps=batch,
         )
         # simple one-try retry in case of network failure (no retry on graphql errors)
         if not res:
-            await asyncio.sleep(0.5)
-            await self.api.send_steps(
+            time.sleep(0.5)
+            self.api.send_steps(
                 steps=batch,
             )
             return
 
     def flush_and_stop(self):
         self.stop_event.set()
         self.processing_thread.join()
 
-    # Legacy
-    def wait_until_queue_empty(self):
-        self.flush_and_stop()
-
-    async def flush(self):
+    async def aflush(self):
         while not self.event_queue.empty():
             await asyncio.sleep(0.2)
 
-    def flush_sync(self):
+    def flush(self):
         while not self.event_queue.empty():
             time.sleep(0.2)
 
     def __del__(self):
         self.flush_and_stop()
```

### Comparing `literalai-0.0.401/literalai/filter.py` & `literalai-0.0.500/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai/helper.py` & `literalai-0.0.500/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai/instrumentation/openai.py` & `literalai-0.0.500/literalai/instrumentation/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             if isinstance(generation, ChatGeneration):
                 step.output = generation.message_completion  # type: ignore
             else:
                 step.output = {"content": generation.completion}
             step.generation = generation
             step.end()
         else:
-            client.api.create_generation_sync(generation)
+            client.api.create_generation(generation)
 
     def after_wrapper(metadata: Dict):
         # Needs to be done in a separate function to avoid transforming all returned data into generators
         def after(result, context: AfterContext, *args, **kwargs):
             step = context.get("step")
             generation = context.get("generation")
 
@@ -369,15 +369,15 @@
                 if isinstance(generation, ChatGeneration):
                     step.output = generation.message_completion  # type: ignore
                 else:
                     step.output = {"content": generation.completion}
                 step.generation = generation
                 step.end()
             else:
-                client.api.create_generation_sync(generation)
+                client.api.create_generation(generation)
             return result
 
         return after
 
     async def async_streaming_response(
         generation: Union[ChatGeneration, CompletionGeneration],
         result,
```

### Comparing `literalai-0.0.401/literalai/message.py` & `literalai-0.0.500/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai/my_types.py` & `literalai-0.0.500/literalai/my_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
             token_count=generation_dict.get("tokenCount"),
             input_token_count=generation_dict.get("inputTokenCount"),
             output_token_count=generation_dict.get("outputTokenCount"),
             tt_first_token=generation_dict.get("ttFirstToken"),
             token_throughput_in_s=generation_dict.get("tokenThroughputInSeconds"),
             duration=generation_dict.get("duration"),
             messages=generation_dict.get("messages", []),
-            message_completion=generation_dict.get("message_completion"),
+            message_completion=generation_dict.get("messageCompletion"),
         )
 
 
 class ScoreDict(TypedDict, total=False):
     id: Optional[str]
     name: str
     type: ScoreType
```

### Comparing `literalai-0.0.401/literalai/prompt.py` & `literalai-0.0.500/literalai/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 import chevron
 
 if TYPE_CHECKING:
-    from literalai.api import API
+    from literalai.api import LiteralAPI
 
 from literalai.my_types import GenerationMessage, GenerationType
 
 
 class ProviderSettings(TypedDict, total=False):
     provider: str
     model: str
@@ -59,15 +59,15 @@
     settings: ProviderSettings
     variables: List[PromptVariable]
     variablesDefaultValues: Optional[Dict[str, Any]]
 
 
 @dataclass
 class Prompt:
-    api: "API"
+    api: "LiteralAPI"
     id: str
     created_at: str
     updated_at: str
     type: "GenerationType"
     name: str
     version: int
     version_desc: Optional[str]
@@ -93,31 +93,32 @@
             "provider": self.provider,
             "settings": self.settings,
             "variables": self.variables,
             "variablesDefaultValues": self.variables_default_values,
         }
 
     @classmethod
-    def from_dict(cls, api: "API", prompt_dict: PromptDict) -> "Prompt":
+    def from_dict(cls, api: "LiteralAPI", prompt_dict: PromptDict) -> "Prompt":
         # Create a Prompt instance from a dictionary (PromptDict)
-        provider = prompt_dict.get("settings", {}).pop("provider", "")
+        settings = prompt_dict.get("settings") or {}
+        provider = settings.pop("provider", "")
 
         return cls(
             api=api,
             id=prompt_dict.get("id", ""),
             name=prompt_dict.get("lineage", {}).get("name", ""),
             version=prompt_dict.get("version", 0),
             created_at=prompt_dict.get("createdAt", ""),
             updated_at=prompt_dict.get("updatedAt", ""),
             type=prompt_dict.get("type", GenerationType.CHAT),
             version_desc=prompt_dict.get("versionDesc"),
             template_messages=prompt_dict.get("templateMessages", []),
             tools=prompt_dict.get("tools", None) or None,
             provider=provider,
-            settings=prompt_dict.get("settings", {}),
+            settings=settings,
             variables=prompt_dict.get("variables", []),
             variables_default_values=prompt_dict.get("variablesDefaultValues"),
         )
 
     def format(
         self, variables: Optional[Dict[str, Any]] = None
     ) -> List[LiteralMessageDict]:
```

### Comparing `literalai-0.0.401/literalai/requirements.py` & `literalai-0.0.500/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai/step.py` & `literalai-0.0.500/literalai/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Literal,
     Optional,
     TypedDict,
     Union,
 )
 
 if TYPE_CHECKING:
-    from literalai.client import LiteralClient
+    from literalai.client import BaseLiteralClient
     from literalai.event_processor import EventProcessor
 
 from literalai.context import active_steps_var, active_thread_var
 from literalai.helper import utc_now
 from literalai.my_types import (
     Attachment,
     AttachmentDict,
@@ -195,15 +195,15 @@
 
         return step
 
 
 class StepContextManager:
     def __init__(
         self,
-        client: "LiteralClient",
+        client: "BaseLiteralClient",
         name: str = "",
         type: TrueStepType = "undefined",
         id: Optional[str] = None,
         parent_id: Optional[str] = None,
         thread_id: Optional[str] = None,
     ):
         self.client = client
@@ -251,15 +251,15 @@
         if exc_type:
             self.step.error = str(exc_val)
             self.client.event_processor.flush_sync()
         self.step.end()
 
 
 def step_decorator(
-    client: "LiteralClient",
+    client: "BaseLiteralClient",
     func: Callable,
     type: TrueStepType = "undefined",
     name: str = "",
     id: Optional[str] = None,
     parent_id: Optional[str] = None,
     thread_id: Optional[str] = None,
     ctx_manager: Optional[StepContextManager] = None,
```

### Comparing `literalai-0.0.401/literalai/thread.py` & `literalai-0.0.500/literalai/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, TypedDict
 
 from literalai.context import active_thread_var
 from literalai.my_types import UserDict
 from literalai.step import Step, StepDict
 
 if TYPE_CHECKING:
-    from literalai.client import LiteralClient
+    from literalai.client import BaseLiteralClient
 
 
 class ThreadDict(TypedDict, total=False):
     id: Optional[str]
     name: Optional[str]
     metadata: Optional[Dict]
     tags: Optional[List[str]]
@@ -93,38 +93,39 @@
 
         return thread
 
 
 class ThreadContextManager:
     def __init__(
         self,
-        client: "LiteralClient",
+        client: "BaseLiteralClient",
         thread_id: "Optional[str]" = None,
         name: "Optional[str]" = None,
         **kwargs,
     ):
         self.client = client
         self.thread_id = thread_id
         self.name = name
         self.kwargs = kwargs
 
     def upsert(self):
         thread = active_thread_var.get()
         thread_data = thread.to_dict()
         thread_data_to_upsert = {
-            "thread_id": thread_data["id"],
+            "id": thread_data["id"],
             "name": thread_data["name"],
         }
         if metadata := thread_data.get("metadata"):
             thread_data_to_upsert["metadata"] = metadata
         if tags := thread_data.get("tags"):
             thread_data_to_upsert["tags"] = tags
         if participant_id := thread_data.get("participant_id"):
             thread_data_to_upsert["participant_id"] = participant_id
-        self.client.api.upsert_thread_sync(**thread_data_to_upsert)
+
+        self.client.to_sync().api.upsert_thread(**thread_data_to_upsert)
 
     def __call__(self, func):
         return thread_decorator(
             self.client, func=func, name=self.name, ctx_manager=self
         )
 
     def __enter__(self) -> "Optional[Thread]":
@@ -145,15 +146,15 @@
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if (thread := active_thread_var.get()) and thread.needs_upsert:
             self.upsert()
         active_thread_var.set(None)
 
 
 def thread_decorator(
-    client: "LiteralClient",
+    client: "BaseLiteralClient",
     func: Callable,
     thread_id: Optional[str] = None,
     name: Optional[str] = None,
     ctx_manager: Optional[ThreadContextManager] = None,
     **decorator_kwargs,
 ):
     if not ctx_manager:
```

### Comparing `literalai-0.0.401/literalai/wrappers.py` & `literalai-0.0.500/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.401/literalai.egg-info/SOURCES.txt` & `literalai-0.0.500/literalai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 literalai/__init__.py
-literalai/api.py
 literalai/client.py
 literalai/context.py
 literalai/dataset.py
 literalai/dataset_item.py
 literalai/event_processor.py
 literalai/filter.py
 literalai/helper.py
@@ -20,12 +19,22 @@
 literalai/version.py
 literalai/wrappers.py
 literalai.egg-info/PKG-INFO
 literalai.egg-info/SOURCES.txt
 literalai.egg-info/dependency_links.txt
 literalai.egg-info/requires.txt
 literalai.egg-info/top_level.txt
+literalai/api/__init__.py
+literalai/api/attachment_helpers.py
+literalai/api/dataset_helpers.py
+literalai/api/generation_helpers.py
+literalai/api/gql.py
+literalai/api/prompt_helpers.py
+literalai/api/score_helpers.py
+literalai/api/step_helpers.py
+literalai/api/thread_helpers.py
+literalai/api/user_helpers.py
 literalai/callback/__init__.py
 literalai/callback/langchain_callback.py
 literalai/instrumentation/__init__.py
 literalai/instrumentation/openai.py
 tests/__init__.py
```

