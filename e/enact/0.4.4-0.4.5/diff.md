# Comparing `tmp/enact-0.4.4.tar.gz` & `tmp/enact-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enact-0.4.4.tar", last modified: Fri Feb 23 22:38:28 2024, max compression
+gzip compressed data, was "enact-0.4.5.tar", last modified: Mon Apr  8 21:46:07 2024, max compression
```

## Comparing `enact-0.4.4.tar` & `enact-0.4.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.4/LICENSE
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-02-23 22:38:28.312029 enact-0.4.4/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.4/README.md
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-02-23 22:36:31.000000 enact-0.4.4/pyproject.toml
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-02-23 22:38:28.312029 enact-0.4.4/setup.cfg
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/src/
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/src/enact/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3260 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7626 2024-02-11 19:18:39.000000 enact-0.4.4/src/enact/contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4062 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/digests.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/src/enact/fastapi/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-02-23 22:36:31.000000 enact-0.4.4/src/enact/fastapi/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/fastapi/fastapi.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    18263 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/function_wrappers.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/src/enact/gradio/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      813 2024-02-23 22:36:31.000000 enact-0.4.4/src/enact/gradio/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26488 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/gradio/gradio.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7845 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/interfaces.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/invocation_generators.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    32624 2023-12-14 01:55:35.000000 enact-0.4.4/src/enact/invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.4/src/enact/py.typed
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11286 2023-12-14 01:56:00.000000 enact-0.4.4/src/enact/references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/resource_digests.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    15763 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5024 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5760 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/serialization.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-02-11 18:04:33.000000 enact-0.4.4/src/enact/type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1440 2023-12-06 01:14:11.000000 enact-0.4.4/src/enact/utils.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/src/enact.egg-info/
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-02-23 22:38:28.000000 enact-0.4.4/src/enact.egg-info/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1087 2024-02-23 22:38:28.000000 enact-0.4.4/src/enact.egg-info/SOURCES.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-02-23 22:38:28.000000 enact-0.4.4/src/enact.egg-info/dependency_links.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-02-23 22:38:28.000000 enact-0.4.4/src/enact.egg-info/requires.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-02-23 22:38:28.000000 enact-0.4.4/src/enact.egg-info/top_level.txt
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-02-23 22:38:28.312029 enact-0.4.4/tests/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6618 2024-02-11 21:16:37.000000 enact-0.4.4/tests/test_contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_digest.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_function_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_invocation_generator.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26951 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6350 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7559 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5680 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2271 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_serialize.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-02-11 18:04:33.000000 enact-0.4.4/tests/test_type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2538 2023-12-06 01:14:11.000000 enact-0.4.4/tests/test_utils.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.5/LICENSE
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-08 21:46:07.072802 enact-0.4.5/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.5/README.md
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-04-08 21:45:31.000000 enact-0.4.5/pyproject.toml
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-04-08 21:46:07.072802 enact-0.4.5/setup.cfg
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.064803 enact-0.4.5/src/
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.068802 enact-0.4.5/src/enact/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3260 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8742 2024-04-08 21:41:00.000000 enact-0.4.5/src/enact/contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4062 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/digests.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact/fastapi/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-04-02 22:20:36.000000 enact-0.4.5/src/enact/fastapi/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/fastapi/fastapi.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    18263 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/function_wrappers.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact/gradio/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      813 2024-04-02 22:20:36.000000 enact-0.4.5/src/enact/gradio/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26488 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/gradio/gradio.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8972 2024-04-03 21:00:20.000000 enact-0.4.5/src/enact/interfaces.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/invocation_generators.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    32624 2023-12-14 01:55:35.000000 enact-0.4.5/src/enact/invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.5/src/enact/py.typed
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11286 2024-04-03 20:56:13.000000 enact-0.4.5/src/enact/references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resource_digests.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    15763 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5024 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5760 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/serialization.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-02-11 18:04:33.000000 enact-0.4.5/src/enact/type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1440 2023-12-06 01:14:11.000000 enact-0.4.5/src/enact/utils.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/src/enact.egg-info/
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1087 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/requires.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-04-08 21:46:07.000000 enact-0.4.5/src/enact.egg-info/top_level.txt
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-08 21:46:07.072802 enact-0.4.5/tests/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7465 2024-04-08 21:41:00.000000 enact-0.4.5/tests/test_contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_digest.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_function_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_invocation_generator.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26951 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6787 2024-04-03 21:00:20.000000 enact-0.4.5/tests/test_references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7559 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5680 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2271 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_serialize.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-02-11 18:04:33.000000 enact-0.4.5/tests/test_type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2538 2023-12-06 01:14:11.000000 enact-0.4.5/tests/test_utils.py
```

### Comparing `enact-0.4.4/LICENSE` & `enact-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/PKG-INFO` & `enact-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.4
+Version: 0.4.5
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.4/README.md` & `enact-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/pyproject.toml` & `enact-0.4.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "enact"
-version = "0.4.4"
+version = "0.4.5"
 dependencies = [
   "numpy",
   "Pillow",
   "wrapt",
 ]
 description = "A framework for generative software."
 readme = "README.md"
```

### Comparing `enact-0.4.4/src/enact/__init__.py` & `enact-0.4.5/src/enact/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/contexts.py` & `enact-0.4.5/src/enact/contexts.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,39 +29,41 @@
 class ContextTypeError(ContextError):
   """Error raised when the context has an unexpected type"""
 
 
 class NoActiveContext(ContextError):
   """Raised when there is no active context."""
 
+ContextBaseT = TypeVar('ContextBaseT', bound='_ContextBase')
+ContextSuperT = TypeVar('ContextSuperT', bound='_ContextBase')
 ContextT = TypeVar('ContextT', bound='Context')
-ContextSuperT = TypeVar('ContextSuperT', bound='Context')
+AsyncContextT = TypeVar('AsyncContextT', bound='AsyncContext')
 
 
-class Context:
+class _ContextBase:
   """A thread-aware context superclass."""
 
-  def __init__(self: ContextT):
+  def __init__(self: ContextBaseT):
     """Creates a new context."""
-    self._token: Optional[contextvars.Token[Optional[ContextT]]] = None
+    self._token: Optional[contextvars.Token[Optional[ContextBaseT]]] = None
 
   @classmethod
-  def _get_context_var(cls: Type[ContextT]) -> (
-      contextvars.ContextVar[Optional[ContextT]]):
+  def _get_context_var(cls: Type[ContextBaseT]) -> (
+      contextvars.ContextVar[Optional[ContextBaseT]]):
     """Returns the context var for this type."""
     try:
       return cast(
-        contextvars.ContextVar[Optional[ContextT]], _context_vars[cls])
+        contextvars.ContextVar[Optional[ContextBaseT]], _context_vars[cls])
     except KeyError as key_error:
       raise ContextError(
         f'Context {cls} not registered. A context class must be registered '
         f'with the "@register" decorator.') from key_error
 
   @classmethod
-  def permissive_initialization(cls: Type[ContextT]) -> bool:
+  def permissive_initialization(cls: Type[ContextBaseT]) -> bool:
     """Returns whether the class has permissive initialization.
 
     Contexts use contextvars for tracking whether an execution is in-context or
     out-of-context. Contextvars have special handling in threads and async
     executions, e.g., they are thread-local and hence starting a new thread will
     erase the context stack. The Context class can detect when this happens,
     since it will store information in the main thread during registration. This
@@ -78,26 +80,25 @@
     accidentally operating in a fresh context is a problem, e.g., when
     implementing contexts that deal with encryption.
     """
     return True
 
   @classmethod
   @contextlib.contextmanager
-  def top_level(cls: Type[ContextT]):
+  def top_level(cls: Type[ContextBaseT]):
     """Returns a context manager to execute code in a top-level context."""
     context_var = cls._get_context_var()
     token = context_var.set(None)
     try:
       yield
     finally:
       context_var.reset(token)
 
-
   @classmethod
-  def get_current(cls: Type[ContextT]) -> Optional[ContextT]:
+  def get_current(cls: Type[ContextBaseT]) -> Optional[ContextBaseT]:
     """Returns the current context of this type or None."""
     context_var = cls._get_context_var()
     try:
       current_context = context_var.get()
     except LookupError as lookup_error:
       if cls.permissive_initialization():
         context_var.set(None)
@@ -109,21 +110,25 @@
         ) from lookup_error
     if current_context is not None and not isinstance(current_context, cls):
       raise ContextTypeError(
         f'Current context {current_context} is not of type {cls}.')
     return current_context
 
   @classmethod
-  def current(cls: Type[ContextT]) -> ContextT:
+  def current(cls: Type[ContextBaseT]) -> ContextBaseT:
     """Returns the current context of this type or raises an error."""
     context = cls.get_current()
     if context is None:
       raise NoActiveContext(f'No context of type {cls.__qualname__} is active.')
     return context
 
+
+class Context(_ContextBase):
+  """A thread-aware context superclass."""
+
   def __enter__(self: ContextT) -> ContextT:
     """Enters the context."""
     context_var = self._get_context_var()
     try:
       self.get_current()  # Raise an error if the context is not initialized.
     except ContextTypeError:
       pass   #  We don't care here if the context has the wrong type.
@@ -135,45 +140,76 @@
     """Exits the context."""
     context_var = self._get_context_var()
     assert self._token
     context_var.reset(self._token)
     self.exit()
     self._token = None
 
-  def enter(self: ContextT):
+  def enter(self):
     """Overridable on context entry."""
 
-  def exit(self: ContextT):
+  def exit(self):
     """Overridable on context exit."""
 
-def register(cls: Type[ContextT]) -> Type[ContextT]:
+
+class AsyncContext(_ContextBase):
+  """A thread-aware async context superclass."""
+
+  async def __aenter__(self: AsyncContextT) -> AsyncContextT:
+    """Enters the context."""
+    context_var = self._get_context_var()
+    try:
+      self.get_current()  # Raise an error if the context is not initialized.
+    except ContextTypeError:
+      pass   #  We don't care here if the context has the wrong type.
+    await self.aenter()
+    self._token = context_var.set(self)
+    return self
+
+  async def __aexit__(self, exc_type, exc_value, traceback):
+    """Exits the context."""
+    context_var = self._get_context_var()
+    assert self._token
+    context_var.reset(self._token)
+    await self.aexit()
+    self._token = None
+
+  async def aenter(self):
+    """Overridable on context entry."""
+
+  async def aexit(self):
+    """Overridable on context exit."""
+
+
+
+def register(cls: Type[ContextBaseT]) -> Type[ContextBaseT]:
   """Registers a context class."""
   assert cls not in _context_vars, (
     f'Context class already registered: {cls}')
   ctx_var: contextvars.ContextVar[Optional[Context]] = (
     contextvars.ContextVar(cls.__qualname__))
   ctx_var.set(None)
   _context_vars[cls] = ctx_var
   return cls
 
 
 def register_to_superclass(superclass: Type[ContextSuperT]) -> Callable[
-    [Type[ContextT]], Type[ContextT]]:
-  def _register(cls: Type[ContextT]) -> Type[ContextT]:
+    [Type[ContextBaseT]], Type[ContextBaseT]]:
+  def _register(cls: Type[ContextBaseT]) -> Type[ContextBaseT]:
     """Registers a context class."""
     assert cls not in _context_vars, (
       f'Context class already registered: {cls}')
     assert superclass in _context_vars, (
       f'Superclass {superclass} not registered.')
     assert issubclass(cls, superclass), (
       f'Context class {cls} must be a subclass of {superclass}.')
     _context_vars[cls] = _context_vars[superclass]
     # MyPy can't handle intersection types, which is what would be required
     # here. We cast to Type[ContextT] to make it happy.
-    return cast(Type[ContextT], cls)
+    return cast(Type[ContextBaseT], cls)
   return _register
 
 
 R = TypeVar('R')
 
 
 def _with_contexts(
```

### Comparing `enact-0.4.4/src/enact/digests.py` & `enact-0.4.5/src/enact/digests.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/fastapi/__init__.py` & `enact-0.4.5/src/enact/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/fastapi/fastapi.py` & `enact-0.4.5/src/enact/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/function_wrappers.py` & `enact-0.4.5/src/enact/function_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/gradio/__init__.py` & `enact-0.4.5/src/enact/gradio/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/gradio/gradio.py` & `enact-0.4.5/src/enact/gradio/gradio.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/interfaces.py` & `enact-0.4.5/src/enact/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 # limitations under the License.
 
 """Core resource interface."""
 
 import abc
 import functools
 import json
-from typing import Dict, Generic, Iterable, List, Tuple, Type, TypeVar, Union
+from typing import (
+  Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union)
+
+from enact import contexts
 
 
 JsonLeaf = Union[int, float, str, bool, None]
 Json = Union[JsonLeaf, List['Json'], Dict[str, 'Json']]
 
 
 PRIMITIVES = (int, float, str, bytes, bool, type(None))
@@ -48,39 +51,67 @@
   'ResourceDict']
 
 
 C = TypeVar('C', bound='ResourceBase')
 
 
 class FrameworkError(Exception):
-  """Superclass for framework related errors.
+  """Superclass for framework related errors."""
 
-  Framework errors are not caught by the framework during tracked execution, but
-  are instead propagated to the caller.
-  """
 
 class ResourceError(FrameworkError):
   """Superclass for resource related errors."""
 
 
 class ImplementationMissing(FrameworkError):
   """Superclass for errors where an implementaton is missing."""
 
 
 class FieldTypeError(FrameworkError):
   """Superclass for errors related to field types."""
 
 
+@contexts.register
+class _AcyclicContext(contexts.Context):
+  """Helper to safeguard against cyclic data-structures."""
+
+  def __init__(self, obj):
+    """Initializes the context."""
+    super().__init__()
+    self.parent: Optional[_AcyclicContext] = None
+    self.obj = obj
+
+  def enter(self):
+    """Check if the resource is already being committed."""
+    self.parent = _AcyclicContext.get_current()
+    parent = self.parent
+    parents: List[_AcyclicContext] = []
+    while parent is not None:
+      parents.append(parent)
+      if parent.obj is self.obj:
+        raise FieldTypeError(
+          f'Resources may not have cyclic graph structure. '
+          f'Encountered cycle: '
+          f'{" -> ".join(str(p.obj) for p in parents)}')
+      parent = parent.parent
+
+
 class ResourceBase:
   """Base class for resources.
 
   Not an abstract base class in order to avoid meta-class conflict.
 
   Resources have a unique type identifier. Each resource class is associated
-  with a fixed list of named fields.
+  with a fixed list of named fields. These fields must have value semantics,
+  that is, replacing a field by a copy should not change the meaning of the
+  resource. This means, for example, that code using resources should not rely
+  on aliasing assumptions (e.g., two resources sharing the same list instance).
+
+  In particular, this also means that resources may not mutually reference each
+  other.
   """
 
   @classmethod
   def type_descr(cls) -> Dict[str, Json]:
     """Returns a unique descriptor for the type."""
     return {'name': f'{cls.__module__}.{cls.__qualname__}'}
 
@@ -111,33 +142,34 @@
                   field_dict: Dict[str, FieldValue]) -> C:
     """Constructs the resource from a field dictionary."""
     raise NotImplementedError()
 
   @staticmethod
   def _to_dict_value(value: FieldValue) -> ResourceDictValue:
     """Transforms a field value to a resource dict value."""
-    if isinstance(value, ResourceBase):
-      return value.to_resource_dict()
-    if isinstance(value, PRIMITIVES):
-      return value
-    if isinstance(value, type) and issubclass(value, ResourceBase):
-      return value
-    if isinstance(value, List):
-      return [ResourceBase._to_dict_value(x) for x in value]
-    if isinstance(value, Dict):
-      def _assert_str(maybe_str: str) -> str:
-        if type(maybe_str) is not str:  # pylint: disable=unidiomatic-typecheck
-          raise FieldTypeError(
-            f'Expected string key, got {type(maybe_str)}')
-        return maybe_str
-      return {
-        _assert_str(k): ResourceBase._to_dict_value(v)
-        for k, v in value.items()}
-    raise FieldTypeError(
-      f'Encountered unsupported field type {type(value)}: {value}')
+    with _AcyclicContext(value):
+      if isinstance(value, ResourceBase):
+        return value.to_resource_dict()
+      if isinstance(value, PRIMITIVES):
+        return value
+      if isinstance(value, type) and issubclass(value, ResourceBase):
+        return value
+      if isinstance(value, List):
+        return [ResourceBase._to_dict_value(x) for x in value]
+      if isinstance(value, Dict):
+        def _assert_str(maybe_str: str) -> str:
+          if type(maybe_str) is not str:  # pylint: disable=unidiomatic-typecheck
+            raise FieldTypeError(
+              f'Expected string key, got {type(maybe_str)}')
+          return maybe_str
+        return {
+          _assert_str(k): ResourceBase._to_dict_value(v)
+          for k, v in value.items()}
+      raise FieldTypeError(
+        f'Encountered unsupported field type {type(value)}: {value}')
 
   @staticmethod
   def _from_dict_value(value: ResourceDictValue) -> FieldValue:
     """Transforms a resource dict value to a field value."""
     if isinstance(value, PRIMITIVES):
       return value
     if isinstance(value, type) and issubclass(value, ResourceBase):
```

### Comparing `enact-0.4.4/src/enact/invocation_generators.py` & `enact-0.4.5/src/enact/invocation_generators.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/invocations.py` & `enact-0.4.5/src/enact/invocations.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/pretty_print.py` & `enact-0.4.5/src/enact/pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/references.py` & `enact-0.4.5/src/enact/references.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/registration.py` & `enact-0.4.5/src/enact/registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/resource_registry.py` & `enact-0.4.5/src/enact/resource_registry.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/resources.py` & `enact-0.4.5/src/enact/resources.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/serialization.py` & `enact-0.4.5/src/enact/serialization.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/type_wrappers.py` & `enact-0.4.5/src/enact/type_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact/utils.py` & `enact-0.4.5/src/enact/utils.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/src/enact.egg-info/PKG-INFO` & `enact-0.4.5/src/enact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.4
+Version: 0.4.5
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.4/src/enact.egg-info/SOURCES.txt` & `enact-0.4.5/src/enact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_contexts.py` & `enact-0.4.5/tests/test_contexts.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for the context module."""
 
+import asyncio
 import unittest
 import threading
 from typing import Any, Optional
 
 from enact import contexts
 
 
@@ -42,14 +43,34 @@
     else:
       self.depth = 1
 
   def exit(self):
     self.depth = None
 
 
+@contexts.register
+class AsyncSimpleContext(contexts.AsyncContext):
+  """An async context object for testing."""
+
+  def __init__(self):
+    super().__init__()
+    self.depth: Optional[int] = None
+
+  async def aenter(self):
+    cur = AsyncSimpleContext.get_current()
+    if cur:
+      assert cur.depth is not None
+      self.depth = cur.depth + 1
+    else:
+      self.depth = 1
+
+  async def exit(self):
+    self.depth = None
+
+
 class UnregisteredContext(SimpleContext):
   """A context that was not registered."""
 
 
 @contexts.register_to_superclass(SimpleContext)
 class DerivedContextA(SimpleContext):
   """A derived context from SimpleContext."""
@@ -203,7 +224,18 @@
     """Tests that running with the current contexts works."""
     with SimpleContext():
       t = threading.Thread(
         target=contexts.with_current_contexts(self.enter_context))
       t.start()
       t.join()
     self.assertEqual(self.thread_result, 2)
+
+  def test_async_contexts(self):
+    """Test async contexts."""
+    async def _do_test():
+      async with AsyncSimpleContext():
+        self.assertEqual(AsyncSimpleContext.get_current().depth, 1)
+        async with AsyncSimpleContext():
+          self.assertEqual(AsyncSimpleContext.get_current().depth, 2)
+        self.assertEqual(AsyncSimpleContext.get_current().depth, 1)
+
+    asyncio.run(_do_test())
```

### Comparing `enact-0.4.4/tests/test_digest.py` & `enact-0.4.5/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_function_wrappers.py` & `enact-0.4.5/tests/test_function_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_invocation_generator.py` & `enact-0.4.5/tests/test_invocation_generator.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_invocations.py` & `enact-0.4.5/tests/test_invocations.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_pretty_print.py` & `enact-0.4.5/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_references.py` & `enact-0.4.5/tests/test_references.py`

 * *Files 8% similar despite different names*

```diff
@@ -193,7 +193,19 @@
     """Tests the file backend."""
     with tempfile.TemporaryDirectory() as tmpdir:
       store = enact.Store(backend=enact.FileBackend(tmpdir))
       resource = SimpleResource(x=1, y=2.0)
       ref = store.commit(resource)
       self.assertTrue(store.has(ref))
       self.assertEqual(store.checkout(ref), resource)
+
+  def test_commit_cyclic_fails(self):
+    """Tests that commits with cylic resource graphs fail."""
+    with tempfile.TemporaryDirectory() as tmpdir:
+      r1 = SimpleResource(x=1, y=2.0)
+      r2 = SimpleResource(x=1, y=2.0)
+      r1.x = r2  # type: ignore
+      r2.x = r1  # type: ignore
+
+      with enact.Store(backend=enact.FileBackend(tmpdir)):
+        with self.assertRaises(interfaces.FieldTypeError):
+          enact.commit(r1)
```

### Comparing `enact-0.4.4/tests/test_registration.py` & `enact-0.4.5/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_resource_registry.py` & `enact-0.4.5/tests/test_resource_registry.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_resources.py` & `enact-0.4.5/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_serialize.py` & `enact-0.4.5/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_type_wrappers.py` & `enact-0.4.5/tests/test_type_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.4/tests/test_utils.py` & `enact-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

