# Comparing `tmp/aios_sdk-0.1.7.tar.gz` & `tmp/aios_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aios_sdk-0.1.7.tar", max compression
+gzip compressed data, was "aios_sdk-0.1.8.tar", max compression
```

## Comparing `aios_sdk-0.1.7.tar` & `aios_sdk-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,35 @@
--rw-r--r--   0        0        0        0 2024-04-05 20:00:00.579828 aios_sdk-0.1.7/README.md
--rw-r--r--   0        0        0      661 2024-04-06 00:44:33.732229 aios_sdk-0.1.7/aios_sdk/__init__.py
--rw-r--r--   0        0        0       39 2024-04-06 01:02:49.549769 aios_sdk-0.1.7/aios_sdk/cli.py
--rw-r--r--   0        0        0      115 2024-04-06 00:26:38.875127 aios_sdk-0.1.7/aios_sdk/models.py
--rw-r--r--   0        0        0     2655 2024-04-05 20:16:53.216910 aios_sdk-0.1.7/aios_sdk/rpc/__pycache__/app_state_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     6034 2024-04-05 20:27:18.949387 aios_sdk-0.1.7/aios_sdk/rpc/__pycache__/app_state_pb2_grpc.cpython-312.pyc
--rw-r--r--   0        0        0     3142 2024-04-05 21:05:43.521758 aios_sdk-0.1.7/aios_sdk/rpc/__pycache__/models_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     8333 2024-04-05 21:05:43.521460 aios_sdk-0.1.7/aios_sdk/rpc/__pycache__/models_pb2_grpc.cpython-312.pyc
--rw-r--r--   0        0        0     2945 2024-04-05 20:05:44.570072 aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2.py
--rw-r--r--   0        0        0     4770 2024-04-05 20:05:44.570256 aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2.pyi
--rw-r--r--   0        0        0     5673 2024-04-05 20:26:55.649399 aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2_grpc.py
--rw-r--r--   0        0        0     2457 2024-04-05 20:05:44.570420 aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2024-04-05 20:05:44.570468 aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2.py
--rw-r--r--   0        0        0     1034 2024-04-05 20:05:44.570515 aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2.pyi
--rw-r--r--   0        0        0     2405 2024-04-05 20:26:55.649634 aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2_grpc.py
--rw-r--r--   0        0        0     1238 2024-04-05 20:05:44.570610 aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2_grpc.pyi
--rw-r--r--   0        0        0     2902 2024-04-05 20:05:44.570671 aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2.py
--rw-r--r--   0        0        0     4952 2024-04-05 20:05:44.570788 aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2.pyi
--rw-r--r--   0        0        0     4020 2024-04-05 20:26:55.649871 aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2_grpc.py
--rw-r--r--   0        0        0     1842 2024-04-05 20:05:44.570881 aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2_grpc.pyi
--rw-r--r--   0        0        0     1298 2024-04-05 20:05:44.570924 aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2.py
--rw-r--r--   0        0        0      632 2024-04-05 20:05:44.570968 aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2.pyi
--rw-r--r--   0        0        0     2331 2024-04-05 20:26:55.649991 aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2_grpc.py
--rw-r--r--   0        0        0     1178 2024-04-05 20:05:44.571060 aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2_grpc.pyi
--rw-r--r--   0        0        0     3604 2024-04-05 20:05:44.571111 aios_sdk-0.1.7/aios_sdk/rpc/models_pb2.py
--rw-r--r--   0        0        0     6093 2024-04-05 20:05:44.571217 aios_sdk-0.1.7/aios_sdk/rpc/models_pb2.pyi
--rw-r--r--   0        0        0     8333 2024-04-05 20:26:55.649158 aios_sdk-0.1.7/aios_sdk/rpc/models_pb2_grpc.py
--rw-r--r--   0        0        0     3179 2024-04-05 20:05:44.571330 aios_sdk-0.1.7/aios_sdk/rpc/models_pb2_grpc.pyi
--rw-r--r--   0        0        0     1833 2024-04-05 20:05:44.571375 aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2.py
--rw-r--r--   0        0        0     2498 2024-04-05 20:05:44.571431 aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2.pyi
--rw-r--r--   0        0        0     2525 2024-04-05 20:26:55.649752 aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2_grpc.py
--rw-r--r--   0        0        0     1340 2024-04-05 20:05:44.571528 aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2_grpc.pyi
--rw-r--r--   0        0        0     3459 2024-04-05 20:05:44.571579 aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2.py
--rw-r--r--   0        0        0     5489 2024-04-05 20:05:44.571696 aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2.pyi
--rw-r--r--   0        0        0     5581 2024-04-05 20:26:55.650104 aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2_grpc.py
--rw-r--r--   0        0        0     2369 2024-04-05 20:05:44.571868 aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2_grpc.pyi
--rw-r--r--   0        0        0      533 2024-04-06 01:03:47.885397 aios_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 aios_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1575 2024-04-08 17:35:05.050215 aios_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0     1389 2024-04-08 17:16:11.666395 aios_sdk-0.1.8/aios_sdk/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-08 16:54:15.111610 aios_sdk-0.1.8/aios_sdk/cli.py
+-rw-r--r--   0        0        0      490 2024-04-08 16:54:15.149136 aios_sdk-0.1.8/aios_sdk/inference.py
+-rw-r--r--   0        0        0      399 2024-04-08 17:09:25.255495 aios_sdk-0.1.8/aios_sdk/models.py
+-rw-r--r--   0        0        0     2945 2024-04-08 16:54:15.111805 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.py
+-rw-r--r--   0        0        0     4770 2024-04-08 16:54:15.112012 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.pyi
+-rw-r--r--   0        0        0     5673 2024-04-08 16:54:15.112215 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.py
+-rw-r--r--   0        0        0     2457 2024-04-08 16:54:15.112300 aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2024-04-08 16:54:15.112379 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.py
+-rw-r--r--   0        0        0     1034 2024-04-08 16:54:15.112462 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.pyi
+-rw-r--r--   0        0        0     2405 2024-04-08 16:54:15.112553 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.py
+-rw-r--r--   0        0        0     1238 2024-04-08 16:54:15.112659 aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2902 2024-04-08 16:54:15.112754 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.py
+-rw-r--r--   0        0        0     4952 2024-04-08 16:54:15.112973 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.pyi
+-rw-r--r--   0        0        0     4020 2024-04-08 16:54:15.113073 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.py
+-rw-r--r--   0        0        0     1842 2024-04-08 16:54:15.113168 aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1298 2024-04-08 16:54:15.113273 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.py
+-rw-r--r--   0        0        0      632 2024-04-08 16:54:15.113361 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.pyi
+-rw-r--r--   0        0        0     2331 2024-04-08 16:54:15.113436 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.py
+-rw-r--r--   0        0        0     1178 2024-04-08 16:54:15.113517 aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3604 2024-04-08 16:54:15.113607 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.py
+-rw-r--r--   0        0        0     6093 2024-04-08 16:54:15.113815 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.pyi
+-rw-r--r--   0        0        0     8333 2024-04-08 16:54:15.113915 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.py
+-rw-r--r--   0        0        0     3179 2024-04-08 16:54:15.114003 aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1833 2024-04-08 16:54:15.114081 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.py
+-rw-r--r--   0        0        0     2498 2024-04-08 16:54:15.114172 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.pyi
+-rw-r--r--   0        0        0     2525 2024-04-08 16:54:15.114265 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.py
+-rw-r--r--   0        0        0     1340 2024-04-08 16:54:15.114356 aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3459 2024-04-08 16:54:15.114449 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.py
+-rw-r--r--   0        0        0     5489 2024-04-08 16:54:15.114650 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.pyi
+-rw-r--r--   0        0        0     5581 2024-04-08 16:54:15.114842 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.py
+-rw-r--r--   0        0        0     2369 2024-04-08 16:54:15.114917 aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.pyi
+-rw-r--r--   0        0        0      533 2024-04-08 17:22:50.520354 aios_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 aios_sdk-0.1.8/PKG-INFO
```

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/app_state_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/app_state_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/helloworld_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/helloworld_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/inference_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/inference_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/kill_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/kill_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/models_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/models_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/models_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/models_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/models_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/system_info_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/system_info_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2.py` & `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2_grpc.py` & `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/aios_sdk/rpc/websocket_pb2_grpc.pyi` & `aios_sdk-0.1.8/aios_sdk/rpc/websocket_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `aios_sdk-0.1.7/pyproject.toml` & `aios_sdk-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aios-sdk"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Ginkoe <ginkoe@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 grpcio = "^1.62.1"
@@ -20,8 +20,8 @@
 
 [tool.poetry-grpc-plugin]
 proto_path = "../aios-rpc/proto"
 python_out = "./rpc"
 venv_proto_paths = ["google/type"]
 
 [tool.poetry.scripts]
-aios-cli = "aios_sdk.cli:cli"
+aios-sdk = "aios_sdk.cli:cli"
```

