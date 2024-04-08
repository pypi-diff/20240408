# Comparing `tmp/pkl-python-0.1.11.tar.gz` & `tmp/pkl-python-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkl-python-0.1.11.tar", last modified: Thu Apr  4 02:24:17 2024, max compression
+gzip compressed data, was "pkl-python-0.1.12.tar", last modified: Mon Apr  8 01:50:51 2024, max compression
```

## Comparing `pkl-python-0.1.11.tar` & `pkl-python-0.1.12.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.228855 pkl-python-0.1.11/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1069 2024-03-29 10:49:37.000000 pkl-python-0.1.11/LICENSE
--rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5982 2024-04-04 02:24:17.228855 pkl-python-0.1.11/PKG-INFO
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     3841 2024-04-04 02:20:34.000000 pkl-python-0.1.11/README.md
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/pkl/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        7 2024-04-04 01:41:54.000000 pkl-python-0.1.11/pkl/VERSION
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     3925 2024-04-04 02:17:34.000000 pkl-python-0.1.11/pkl/__init__.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)    12506 2024-04-03 09:53:08.000000 pkl-python-0.1.11/pkl/evaluator_manager.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     4841 2024-04-03 09:01:42.000000 pkl-python-0.1.11/pkl/evaluator_options.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     8111 2024-04-03 02:57:01.000000 pkl-python-0.1.11/pkl/msgapi.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     8637 2024-04-04 01:53:48.000000 pkl-python-0.1.11/pkl/parser.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1780 2024-04-03 06:30:38.000000 pkl-python-0.1.11/pkl/reader.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     4147 2024-04-03 11:02:36.000000 pkl-python-0.1.11/pkl/server.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      658 2024-04-03 09:53:07.000000 pkl-python-0.1.11/pkl/utils.py
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/pkl_python.egg-info/
--rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5982 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/PKG-INFO
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      515 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/SOURCES.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        1 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/dependency_links.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)       79 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/requires.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        4 2024-04-04 02:24:17.000000 pkl-python-0.1.11/pkl_python.egg-info/top_level.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1131 2024-04-02 16:55:35.000000 pkl-python-0.1.11/pyproject.toml
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/scripts/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      978 2024-03-29 10:49:37.000000 pkl-python-0.1.11/scripts/download_binary.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      917 2024-03-29 10:49:37.000000 pkl-python-0.1.11/scripts/eval.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)       38 2024-04-04 02:24:17.228855 pkl-python-0.1.11/setup.cfg
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1939 2024-04-03 10:11:23.000000 pkl-python-0.1.11/setup.py
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-04 02:24:17.224855 pkl-python-0.1.11/tests/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      474 2024-04-03 10:48:59.000000 pkl-python-0.1.11/tests/test_evaluator_manager.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      385 2024-04-03 10:33:31.000000 pkl-python-0.1.11/tests/test_load.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      975 2024-04-03 05:39:56.000000 pkl-python-0.1.11/tests/test_parser.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1756 2024-04-04 02:18:03.000000 pkl-python-0.1.11/tests/test_readers.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      102 2024-04-02 21:06:36.000000 pkl-python-0.1.11/tests/test_server.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1069 2024-03-29 10:49:37.000000 pkl-python-0.1.12/LICENSE
+-rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5990 2024-04-08 01:50:51.334348 pkl-python-0.1.12/PKG-INFO
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     3849 2024-04-08 01:46:30.000000 pkl-python-0.1.12/README.md
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.330348 pkl-python-0.1.12/pkl/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        7 2024-04-08 01:49:57.000000 pkl-python-0.1.12/pkl/VERSION
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     3970 2024-04-06 04:01:45.000000 pkl-python-0.1.12/pkl/__init__.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)    12637 2024-04-06 04:02:48.000000 pkl-python-0.1.12/pkl/evaluator_manager.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     4841 2024-04-03 09:01:42.000000 pkl-python-0.1.12/pkl/evaluator_options.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     8111 2024-04-06 04:02:47.000000 pkl-python-0.1.12/pkl/msgapi.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     6260 2024-04-06 04:01:45.000000 pkl-python-0.1.12/pkl/parser.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1780 2024-04-03 06:30:38.000000 pkl-python-0.1.12/pkl/reader.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     4114 2024-04-04 07:59:33.000000 pkl-python-0.1.12/pkl/server.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      658 2024-04-05 18:01:12.000000 pkl-python-0.1.12/pkl/utils.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/pkl_python.egg-info/
+-rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5990 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/PKG-INFO
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      515 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/SOURCES.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        1 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/dependency_links.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)       79 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/requires.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)        4 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/top_level.txt
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1131 2024-04-08 01:46:30.000000 pkl-python-0.1.12/pyproject.toml
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/scripts/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      978 2024-03-29 10:49:37.000000 pkl-python-0.1.12/scripts/download_binary.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      917 2024-03-29 10:49:37.000000 pkl-python-0.1.12/scripts/eval.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)       38 2024-04-08 01:50:51.334348 pkl-python-0.1.12/setup.cfg
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1939 2024-04-05 18:55:54.000000 pkl-python-0.1.12/setup.py
+drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/tests/
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      474 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_evaluator_manager.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      385 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_load.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      975 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_parser.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)     1756 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_readers.py
+-rw-rw----   0 jwyang    (1002) jwyang    (1002)      102 2024-04-02 21:06:36.000000 pkl-python-0.1.12/tests/test_server.py
```

### Comparing `pkl-python-0.1.11/LICENSE` & `pkl-python-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/PKG-INFO` & `pkl-python-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkl-python
-Version: 0.1.11
+Version: 0.1.12
 Summary: Python library for Apple's PKL.
 Author-email: Jungwoo Yang <jwyang0213@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jungwoo Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,15 +58,15 @@
 ### Installation
 
 ``` bash
 pip install pkl-python
 ```
 
 ### Basic Usage
-Here's how you can start using PKLL to load a PKL module:
+Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
 print(config)
 ```
```

### Comparing `pkl-python-0.1.11/README.md` & `pkl-python-0.1.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ### Installation
 
 ``` bash
 pip install pkl-python
 ```
 
 ### Basic Usage
-Here's how you can start using PKLL to load a PKL module:
+Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
 print(config)
 ```
```

### Comparing `pkl-python-0.1.11/pkl/__init__.py` & `pkl-python-0.1.12/pkl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,19 +82,21 @@
         source = ModuleSource.from_uri(module_uri)
     else:
         source = ModuleSource.from_path(module_uri)
 
     if project_dir is PKL_DEFAULT:
         project_dir = _search_project_dir(str(module_uri))
 
-    with EvaluatorManager(parser=parser, debug=debug) as manager:
+    with EvaluatorManager(debug=debug) as manager:
         if (Path(project_dir) / "PklProject").exists():
-            evaluator = manager.new_project_evaluator(project_dir, evaluator_options)
+            evaluator = manager.new_project_evaluator(
+                project_dir, evaluator_options, parser=parser
+            )
         else:
-            evaluator = manager.new_evaluator(evaluator_options)
+            evaluator = manager.new_evaluator(evaluator_options, parser=parser)
         config = evaluator.evaluate_expression(source, expr)
     return config
 
 
 __all__ = [
     "load",
     "Evaluator",
```

### Comparing `pkl-python-0.1.11/pkl/evaluator_manager.py` & `pkl-python-0.1.12/pkl/evaluator_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,24 +41,28 @@
     def __init__(
         self,
         evaluatorId: int,
         prev_requestId: int,
         manager: "EvaluatorManager",
         resource_readers: Optional[List[ResourceReader]] = None,
         module_readers: Optional[List[ModuleReader]] = None,
+        *,
+        parser=None,
     ):
         self.evaluatorId = evaluatorId
         self.pending_requests = {}
         self.closed = False
         self._manager = manager
         self._prev_requestId = prev_requestId
 
         self.resource_readers = resource_readers or []
         self.module_readers = module_readers or []
 
+        self.parser = parser or Parser()
+
     def _get_requestId(self):
         res = self._prev_requestId + 1
         self._prev_requestId = res
         return res
 
     def handle_request(self, msg: IncomingMessage):
         if isinstance(msg, EvaluateResponse):
@@ -75,15 +79,15 @@
             self.handle_log(msg)
         else:
             raise ValueError(f"Unhandled request: {msg}")
 
     def evaluate_expression(self, source: ModuleSource, expr: Optional[str]):
         binary_res = self._evaluate_expression_raw(source, expr)
         decoded = msgpack.unpackb(binary_res, strict_map_key=False)
-        parsed = self._manager._parser.parse(decoded)
+        parsed = self.parser.parse(decoded)
         return parsed
 
     def _evaluate_expression_raw(self, source: ModuleSource, expr: Optional[str]):
         if self.closed:
             raise ValueError("Evaluator is closed")
 
         requestId = self._get_requestId()
@@ -96,15 +100,15 @@
             expr=expr,
         )
 
         self._manager.send(request)
         response: EvaluateResponse = self._manager.receive(requestId)
 
         if response.error is not None:
-            raise PklError(response.error)
+            raise PklError("\n" + response.error)
         return response.result
 
     def evaluate_module(self, source: ModuleSource):
         return self.evaluate_expression(source, None)
 
     def evaluate_output_files(self, source: ModuleSource) -> List[str]:
         return self.evaluate_expression(
@@ -210,24 +214,26 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 class EvaluatorManager:
     def __init__(
-        self, pkl_command: Optional[List[str]] = None, *, parser=None, debug=False
+        self,
+        pkl_command: Optional[List[str]] = None,
+        *,
+        debug=False,
     ):
         self._evaluators: Dict[int, Evaluator] = {}
         self._closed = False
         self._debug = debug
         self._pkl_command = pkl_command
         self._server = PKLServer(pkl_command, debug=debug)
 
         self._prev_id = -100
-        self._parser = parser or Parser()
 
     def send(self, msg: OutgoingMessage):
         obj = msg.to_json()
         encoded = msgpack.packb(obj)
         self._server.send(encoded)
         self._server.receive_err()
 
@@ -254,15 +260,15 @@
             ):
                 return decoded
 
             # self._evaluators[decoded.evaluatorId].pending_requests[requestId] = decoded
             self._evaluators[decoded.evaluatorId].handle_request(decoded)
 
     def new_evaluator(
-        self, options: EvaluatorOptions, project: Optional[Project] = None
+        self, options: EvaluatorOptions, project: Optional[Project] = None, parser=None
     ):
         if self._closed:
             raise ValueError("Server closed")
 
         requestId = self._get_start_requestId()
         opt_dict = asdict(options)
 
@@ -282,22 +288,25 @@
 
         evaluator = Evaluator(
             response.evaluatorId,
             requestId,
             self,
             resource_readers=options.resourceReaders,
             module_readers=options.moduleReaders,
+            parser=parser,
         )
         self._evaluators[response.evaluatorId] = evaluator
         return evaluator
 
-    def new_project_evaluator(self, project_dir: str, options: EvaluatorOptions):
-        project_evaluator = self.new_evaluator(PreconfiguredOptions())
+    def new_project_evaluator(
+        self, project_dir: str, options: EvaluatorOptions, parser=None
+    ):
+        project_evaluator = self.new_evaluator(PreconfiguredOptions(), parser=parser)
         project = load_project_from_evaluator(project_evaluator, project_dir)
-        evaluator = self.new_evaluator(options, project)
+        evaluator = self.new_evaluator(options, project, parser)
         return evaluator
 
     def _get_start_requestId(self):
         res = self._prev_id + 100
         self._prev_id = res
         return res
```

### Comparing `pkl-python-0.1.11/pkl/evaluator_options.py` & `pkl-python-0.1.12/pkl/evaluator_options.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/pkl/msgapi.py` & `pkl-python-0.1.12/pkl/msgapi.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/pkl/parser.py` & `pkl-python-0.1.12/pkl/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import types
-from collections import namedtuple
 from dataclasses import dataclass, make_dataclass
 from datetime import timedelta
 from enum import Enum, auto
-from typing import Any, List, Literal
+from typing import Generic, List, Literal, TypeVar
 
 # create module for lookup
 _lookup_module = types.ModuleType(__name__ + "._lookup")
 sys.modules[_lookup_module.__name__] = _lookup_module
 
 
 class ResultType(Enum):
@@ -40,18 +39,22 @@
 CODE_CLASS = 0xC
 CODE_TYPEALIAS = 0xD
 CODE_PROPERTY = 0x10
 CODE_ENTRY = 0x11
 CODE_ELEMENT = 0x12
 
 
+T1 = TypeVar("T1")
+T2 = TypeVar("T2")
+
+
 @dataclass
-class Pair:
-    first: Any
-    second: Any
+class Pair(Generic[T1, T2]):
+    first: T1
+    second: T2
 
 
 @dataclass
 class Duration:
     value: float
     unit: Literal["ns", "us", "ms", "s", "min", "h", "d"]
     _UNIT_MAP = {
@@ -90,21 +93,16 @@
 class Regex:
     pattern: str
 
 
 class Parser:
     def __init__(
         self,
+        namespace=None,
         force_render=False,
-        *,
-        typed_dynamic_result_type=ResultType.DATACLASS,
-        pair_result_type=ResultType.DATACLASS,
-        datasize_result_type=ResultType.DATACLASS,
-        regex_result_type=ResultType.DATACLASS,
-        intseq_result_type=ResultType.DATACLASS,
     ):
         self.type_handlers = {
             CODE_TYPED_DYNAMIC: self.parse_typed_dynamic,
             CODE_MAP: self.parse_map,
             CODE_MAPPING: self.parse_mapping,
             CODE_LIST: self.parse_list,
             CODE_LISTING: self.parse_listing,
@@ -116,26 +114,17 @@
             CODE_REGEX: self.parse_regex,
             CODE_CLASS: self.parse_class,
             CODE_TYPEALIAS: self.parse_typealias,
             CODE_PROPERTY: self.parse_property,
             CODE_ENTRY: self.parse_entry,
             CODE_ELEMENT: self.parse_element,
         }
-        self._dataclass_cache = {}
-        self._namedtuple_cache = {
-            "__Pair__": namedtuple("Pair", ["first", "second"]),
-            "__DataSize__": namedtuple("DataSize", ["value", "unit"]),
-            "__Regex__": namedtuple("Regex", ["pattern"]),
-        }
-        self._force_render = force_render
-        self._typed_dynamic_result_type = typed_dynamic_result_type
-        self._pair_result_type = pair_result_type
-        self._datasize_result_type = datasize_result_type
-        self._regex_result_type = regex_result_type
-        self._intseq_result_type = intseq_result_type
+        self.namespace = namespace
+        self.dataclass_cache = {}
+        self.force_render = force_render
 
     def parse(self, obj):
         return self.handle_type(obj)
 
     def handle_type(self, obj):
         if isinstance(obj, list):
             type_code = obj[0]
@@ -147,53 +136,50 @@
         elif isinstance(obj, dict):
             return {k: self.handle_type(v) for k, v in obj.items()}
         elif isinstance(obj, (set, tuple)):
             return type(obj)(self.handle_type(v) for v in obj)
         return obj
 
     def get_dataclass_class(self, class_name: str, keys: List[str]):
-        if class_name not in self._dataclass_cache:
+        if class_name not in self.dataclass_cache:
             dynamic_class = make_dataclass(class_name, keys)
             dynamic_class.__module__ = _lookup_module.__name__
             setattr(_lookup_module, class_name, dynamic_class)
-            self._dataclass_cache[class_name] = dynamic_class
-        dynamic_class = self._dataclass_cache[class_name]
+            self.dataclass_cache[class_name] = dynamic_class
+        dynamic_class = self.dataclass_cache[class_name]
         return dynamic_class
 
     def parse_typed_dynamic(self, obj):
         _, full_class_name, module_uri, members = obj
 
         member_types = set(m[0] for m in members)
         property_list = list(map(self.handle_type, members))
 
         if CODE_ELEMENT in member_types:  # has element
-            if len(member_types) > 1 and not self._force_render:
+            if len(member_types) > 1 and not self.force_render:
                 raise ValueError(
                     "Cannot render object with both elements and properties/entries.\n"
                     "\tUse 'force_render=True'"
                 )
             # element types
             members = property_list
             return members
 
         # only properties and entries
         members = {k: v for m in property_list for k, v in m.items()}
-        result_type = self._typed_dynamic_result_type
         class_name = full_class_name.split("#")[-1].split(".")[-1]
-        if result_type == ResultType.DATACLASS:
-            dynamic_class = self.get_dataclass_class(class_name, members.keys())
-            res = dynamic_class(*members.values())
-            return res
-        elif result_type == ResultType.NAMEDTUPLE:
-            res = namedtuple(class_name, members.keys())(*members.values())
-            return res
-        elif result_type == ResultType.DICTIONARY:
-            return {full_class_name: members}
+
+        if self.namespace is not None:
+            if class_name not in self.namespace:
+                raise ValueError(f"'namespace' provided but '{class_name}' not found")
+            clazz = self.namespace[class_name]
         else:
-            raise ValueError(f"invalid result_type: '{result_type}'")
+            clazz = self.get_dataclass_class(class_name, members.keys())
+        res = clazz(*members.values())
+        return res
 
     def parse_map(self, obj):
         members = obj[1]
         return dict(zip(members.keys(), map(self.handle_type, members.values())))
 
     def parse_mapping(self, obj):
         return self.parse_map(obj)
@@ -209,50 +195,24 @@
 
     def parse_duration(self, obj):
         _, value, unit = obj
 
         return Duration(value, unit)
 
     def parse_pair(self, obj):
-        if self._pair_result_type == ResultType.DATACLASS:
-            return Pair(obj[1], obj[2])
-        elif self._pair_result_type == ResultType.NAMEDTUPLE:
-            return self._namedtuple_cache["__Pair__"](obj[1], obj[2])
-        elif self._pair_result_type == ResultType.LIST:
-            return [obj[1], obj[2]]
-        elif self._pair_result_type == ResultType.TUPLE:
-            return (obj[1], obj[2])
-        else:
-            raise ValueError(f"ResultType '{self._pair_result_type}' not supported")
+        return Pair(obj[1], obj[2])
 
     def parse_datasize(self, obj):
-        if self._datasize_result_type == ResultType.DATACLASS:
-            return DataSize(obj[1], obj[2])
-        elif self._datasize_result_type == ResultType.NAMEDTUPLE:
-            return self._namedtuple_cache["__DataSize__"](obj[1], obj[2])
-        elif self._datasize_result_type == ResultType.TUPLE:
-            return (obj[1], obj[2])
-        else:
-            raise ValueError(f"ResultType '{self._datasize_result_type}' not supported")
+        return DataSize(obj[1], obj[2])
 
     def parse_intseq(self, obj):
-        if self._intseq_result_type == ResultType.DATACLASS:
-            return IntSeq(obj[1], obj[2], obj[3])
-        elif self._intseq_result_type == ResultType.RANGE:
-            return range(obj[1], obj[2], obj[3])
-        else:
-            raise ValueError(f"ResultType '{self._intseq_result_type}' not supported")
+        return IntSeq(obj[1], obj[2], obj[3])
 
     def parse_regex(self, obj):
-        if self._datasize_result_type == ResultType.DATACLASS:
-            return Regex(obj[1])
-        elif self._datasize_result_type == ResultType.NAMEDTUPLE:
-            return self._namedtuple_cache["__Regex__"](obj[1])
-        else:
-            raise ValueError(f"ResultType '{self._datasize_result_type}' not supported")
+        return Regex(obj[1])
 
     def parse_class(self, obj):
         return
 
     def parse_typealias(self, obj):
         return
```

### Comparing `pkl-python-0.1.11/pkl/reader.py` & `pkl-python-0.1.12/pkl/reader.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/pkl/server.py` & `pkl-python-0.1.12/pkl/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,19 @@
     def _read(self, stream):
         msg = None
         while msg is None:
             msg = stream.read()
         return msg
 
     def _receive(self, stream):
-        msg = self._read(stream)
         while True:
-            self.unpacker.feed(msg)
             for unpacked in self.unpacker:
                 return unpacked
             msg = self._read(stream)
+            self.unpacker.feed(msg)
 
     def receive(self):
         if self.closed:
             raise ValueError("Server closed")
         return self._receive(self.stdout)
 
     def receive_err(self):
```

### Comparing `pkl-python-0.1.11/pkl/utils.py` & `pkl-python-0.1.12/pkl/utils.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/pkl_python.egg-info/PKG-INFO` & `pkl-python-0.1.12/pkl_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkl-python
-Version: 0.1.11
+Version: 0.1.12
 Summary: Python library for Apple's PKL.
 Author-email: Jungwoo Yang <jwyang0213@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jungwoo Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,15 +58,15 @@
 ### Installation
 
 ``` bash
 pip install pkl-python
 ```
 
 ### Basic Usage
-Here's how you can start using PKLL to load a PKL module:
+Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
 print(config)
 ```
```

### Comparing `pkl-python-0.1.11/pkl_python.egg-info/SOURCES.txt` & `pkl-python-0.1.12/pkl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/pyproject.toml` & `pkl-python-0.1.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/scripts/download_binary.py` & `pkl-python-0.1.12/scripts/download_binary.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/scripts/eval.py` & `pkl-python-0.1.12/scripts/eval.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/setup.py` & `pkl-python-0.1.12/setup.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/tests/test_parser.py` & `pkl-python-0.1.12/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.11/tests/test_readers.py` & `pkl-python-0.1.12/tests/test_readers.py`

 * *Files identical despite different names*

