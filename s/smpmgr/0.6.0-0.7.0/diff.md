# Comparing `tmp/smpmgr-0.6.0.tar.gz` & `tmp/smpmgr-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpmgr-0.6.0.tar", max compression
+gzip compressed data, was "smpmgr-0.7.0.tar", max compression
```

## Comparing `smpmgr-0.6.0.tar` & `smpmgr-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11366 2024-04-03 23:41:22.394472 smpmgr-0.6.0/LICENSE
--rw-r--r--   0        0        0     2556 2024-04-03 23:41:22.394472 smpmgr-0.6.0/README.md
--rw-r--r--   0        0        0     1083 2024-04-03 23:41:22.394472 smpmgr-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/__init__.py
--rw-r--r--   0        0        0       92 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/__main__.py
--rw-r--r--   0        0        0     4041 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/common.py
--rw-r--r--   0        0        0     3531 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/image_management.py
--rw-r--r--   0        0        0     3373 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/logging.py
--rw-r--r--   0        0        0     5257 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/main.py
--rw-r--r--   0        0        0     1086 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/os_management.py
--rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/py.typed
--rw-r--r--   0        0        0        0 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/user/__init__.py
--rw-r--r--   0        0        0     2541 2024-04-03 23:41:22.394472 smpmgr-0.6.0/smpmgr/user/intercreate.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 smpmgr-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11366 2024-04-08 17:13:19.688326 smpmgr-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2556 2024-04-08 17:13:19.688326 smpmgr-0.7.0/README.md
+-rw-r--r--   0        0        0     1103 2024-04-08 17:13:19.688326 smpmgr-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/__main__.py
+-rw-r--r--   0        0        0     4041 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/common.py
+-rw-r--r--   0        0        0     3531 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/image_management.py
+-rw-r--r--   0        0        0     3373 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/logging.py
+-rw-r--r--   0        0        0     5300 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/main.py
+-rw-r--r--   0        0        0     1086 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/os_management.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/py.typed
+-rw-r--r--   0        0        0     2212 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/terminal.py
+-rw-r--r--   0        0        0        0 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/user/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-08 17:13:19.688326 smpmgr-0.7.0/smpmgr/user/intercreate.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 smpmgr-0.7.0/PKG-INFO
```

### Comparing `smpmgr-0.6.0/LICENSE` & `smpmgr-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/README.md` & `smpmgr-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/pyproject.toml` & `smpmgr-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
 smpclient = "^1.3.1"
 typer = {extras = ["all"], version = "^0.9.0"}
+readchar = "^4.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 black = "^23.11.0"
 flake8 = "^6.1.0"
```

### Comparing `smpmgr-0.6.0/smpmgr/common.py` & `smpmgr-0.7.0/smpmgr/common.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/smpmgr/image_management.py` & `smpmgr-0.7.0/smpmgr/image_management.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/smpmgr/logging.py` & `smpmgr-0.7.0/smpmgr/logging.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/smpmgr/main.py` & `smpmgr-0.7.0/smpmgr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from smp.os_management import OS_MGMT_RET_RC
 from smpclient.generics import error, success
 from smpclient.mcuboot import IMAGE_TLV, ImageInfo, TLVNotFound
 from smpclient.requests.image_management import ImageStatesWrite
 from smpclient.requests.os_management import ResetWrite
 from typing_extensions import Annotated
 
-from smpmgr import image_management, os_management
+from smpmgr import image_management, os_management, terminal
 from smpmgr.common import (
     Options,
     TransportDefinition,
     connect_with_spinner,
     get_smpclient,
     smp_request,
 )
@@ -34,14 +34,15 @@
     "Copyright (c) 2023-2024 Intercreate, Inc. and Contributors\n",
 )
 
 app: Final = typer.Typer(help="\n".join(HELP_LINES))
 app.add_typer(os_management.app)
 app.add_typer(image_management.app)
 app.add_typer(intercreate.app)
+app.command()(terminal.terminal)
 
 
 @app.callback(invoke_without_command=True)
 def options(
     ctx: typer.Context,
     port: str = typer.Option(
         None, help="The serial port to connect to, e.g. COM1, /dev/ttyACM0, etc."
```

### Comparing `smpmgr-0.6.0/smpmgr/os_management.py` & `smpmgr-0.7.0/smpmgr/os_management.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/smpmgr/user/intercreate.py` & `smpmgr-0.7.0/smpmgr/user/intercreate.py`

 * *Files identical despite different names*

### Comparing `smpmgr-0.6.0/PKG-INFO` & `smpmgr-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: smpmgr
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple Management Protocol (SMP) Manager for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jp@intercreate.io
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: readchar (>=4.0.5,<5.0.0)
 Requires-Dist: smpclient (>=1.3.1,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Simple Management Protocol (SMP) Manager
 
 `smpmgr` is a CLI application for interacting with device firmware over a
```

