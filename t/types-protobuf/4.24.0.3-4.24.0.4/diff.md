# Comparing `tmp/types-protobuf-4.24.0.3.tar.gz` & `tmp/types-protobuf-4.24.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-4.24.0.3.tar", last modified: Mon Oct 23 02:16:05 2023, max compression
+gzip compressed data, was "types-protobuf-4.24.0.4.tar", last modified: Sun Oct 29 02:16:23 2023, max compression
```

## Comparing `types-protobuf-4.24.0.3.tar` & `types-protobuf-4.24.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2023-10-23 02:16:02.000000 types-protobuf-4.24.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-23 02:16:02.000000 types-protobuf-4.24.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.600987 types-protobuf-4.24.0.3/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-10-23 02:16:02.000000 types-protobuf-4.24.0.3/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.604987 types-protobuf-4.24.0.3/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    76465 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16112 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2023-10-23 02:15:43.000000 types-protobuf-4.24.0.3/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-10-23 02:16:02.000000 types-protobuf-4.24.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 02:16:05.608987 types-protobuf-4.24.0.3/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-23 02:16:05.000000 types-protobuf-4.24.0.3/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-10-23 02:16:05.000000 types-protobuf-4.24.0.3/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 02:16:05.000000 types-protobuf-4.24.0.3/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-23 02:16:05.000000 types-protobuf-4.24.0.3/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.659463 types-protobuf-4.24.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.651463 types-protobuf-4.24.0.4/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    76466 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16113 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 02:16:23.659463 types-protobuf-4.24.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-4.24.0.3/CHANGELOG.md` & `types-protobuf-4.24.0.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.24.0.4 (2023-10-29)
+
+Enable ruff's isort rules on files generated using mypy-protobuf (#10939)
+
+Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
+
 ## 4.24.0.3 (2023-10-23)
 
 Update mypy-protobuf (#10914)
 
 Co-authored-by: Avasam <samuel.06@hotmail.com>
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
```

### Comparing `types-protobuf-4.24.0.3/PKG-INFO` & `types-protobuf-4.24.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.24.0.3
+Version: 4.24.0.4
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e477c67852834a5bb8c22dec498d580a6421a3ea` and was tested
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
 with mypy 1.6.1, pyright 1.1.332, and
 pytype 2023.10.17.
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/any_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/api_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,21 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
 import collections.abc
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.source_context_pb2
 import google.protobuf.type_pb2
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 
 A plugin executable needs only to be placed somewhere in the path.  The
 plugin should be named "protoc-gen-$NAME", and will then be used when the
 flag "--${NAME}_out" is passed to protoc.
 """
 import builtins
 import collections.abc
+import sys
+import typing
+
 import google.protobuf.descriptor
 import google.protobuf.descriptor_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
-import sys
-import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 The messages in this file describe the definitions found in .proto files.
 A valid .proto file can be translated directly to a FileDescriptorProto
 without any other information (e.g. without reading its imports).
 """
 import builtins
 import collections.abc
+import sys
+import typing
+
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
-import sys
-import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/duration_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/empty_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,20 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
 import collections.abc
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/json_format.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/json_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/message.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/message.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/message_factory.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/service.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/struct_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
 import collections.abc
+import sys
+import typing
+
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
-import sys
-import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/text_format.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/text_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/type_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import builtins
 import collections.abc
+import sys
+import typing
+
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.source_context_pb2
-import sys
-import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/google-stubs/protobuf/wrappers_pb2.pyi` & `types-protobuf-4.24.0.4/google-stubs/protobuf/wrappers_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 These wrappers have no meaningful use within repeated fields as they lack
 the ability to detect presence on individual elements.
 These wrappers have no meaningful use within a map or a oneof since
 individual entries of a map or fields of a oneof can already detect presence.
 """
 import builtins
+import sys
+
 import google.protobuf.descriptor
 import google.protobuf.message
-import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
```

### Comparing `types-protobuf-4.24.0.3/setup.py` & `types-protobuf-4.24.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e477c67852834a5bb8c22dec498d580a6421a3ea` and was tested
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
 with mypy 1.6.1, pyright 1.1.332, and
 pytype 2023.10.17.
 '''.lstrip()
 
 setup(name=name,
-      version="4.24.0.3",
+      version="4.24.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
```

### Comparing `types-protobuf-4.24.0.3/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-4.24.0.4/types_protobuf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.24.0.3
+Version: 4.24.0.4
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e477c67852834a5bb8c22dec498d580a6421a3ea` and was tested
+This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
 with mypy 1.6.1, pyright 1.1.332, and
 pytype 2023.10.17.
```

### Comparing `types-protobuf-4.24.0.3/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-4.24.0.4/types_protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

