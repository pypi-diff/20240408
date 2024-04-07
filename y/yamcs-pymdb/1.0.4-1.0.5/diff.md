# Comparing `tmp/yamcs-pymdb-1.0.4.tar.gz` & `tmp/yamcs-pymdb-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs-pymdb-1.0.4.tar", last modified: Sun Mar 24 15:08:38 2024, max compression
+gzip compressed data, was "yamcs-pymdb-1.0.5.tar", last modified: Sun Apr  7 22:18:46 2024, max compression
```

## Comparing `yamcs-pymdb-1.0.4.tar` & `yamcs-pymdb-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-24 15:08:38.214822 yamcs-pymdb-1.0.4/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs-pymdb-1.0.4/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs-pymdb-1.0.4/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-03-24 15:08:38.214573 yamcs-pymdb-1.0.4/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs-pymdb-1.0.4/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-03-24 15:08:38.214876 yamcs-pymdb-1.0.4/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-03-24 15:06:27.000000 yamcs-pymdb-1.0.4/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-24 15:08:38.179482 yamcs-pymdb-1.0.4/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-24 15:08:38.179288 yamcs-pymdb-1.0.4/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-24 15:08:38.195652 yamcs-pymdb-1.0.4/src/yamcs/pymdb/
--rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/alarms.py
--rw-r--r--   0 fdi        (503) staff       (20)     2417 2024-03-22 14:56:54.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/algorithms.py
--rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/ancillary.py
--rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/calibrators.py
--rw-r--r--   0 fdi        (503) staff       (20)     6124 2024-02-25 20:53:48.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/ccsds.py
--rw-r--r--   0 fdi        (503) staff       (20)     4780 2024-02-23 15:56:43.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/checks.py
--rw-r--r--   0 fdi        (503) staff       (20)    16996 2024-03-22 09:32:00.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/commands.py
--rw-r--r--   0 fdi        (503) staff       (20)     6613 2024-03-22 17:56:34.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/containers.py
--rw-r--r--   0 fdi        (503) staff       (20)     8015 2024-03-22 18:00:25.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/csp.py
--rw-r--r--   0 fdi        (503) staff       (20)    18311 2024-03-22 15:49:39.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/datatypes.py
--rw-r--r--   0 fdi        (503) staff       (20)     9843 2024-02-02 12:27:55.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/encodings.py
--rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/expressions.py
--rw-r--r--   0 fdi        (503) staff       (20)    16565 2024-03-22 15:49:54.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/parameters.py
--rw-r--r--   0 fdi        (503) staff       (20)     7374 2024-03-22 14:54:26.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/systems.py
--rw-r--r--   0 fdi        (503) staff       (20)     4421 2024-02-08 10:27:50.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/verifiers.py
--rw-r--r--   0 fdi        (503) staff       (20)    75047 2024-03-22 17:54:15.000000 yamcs-pymdb-1.0.4/src/yamcs/pymdb/xtce.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-03-24 15:08:38.214244 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-03-24 15:08:38.000000 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      737 2024-03-24 15:08:38.000000 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-03-24 15:08:38.000000 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-03-24 15:08:38.000000 yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.922074 yamcs-pymdb-1.0.5/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs-pymdb-1.0.5/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs-pymdb-1.0.5/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-07 22:18:46.921820 yamcs-pymdb-1.0.5/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs-pymdb-1.0.5/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-04-07 22:18:46.922130 yamcs-pymdb-1.0.5/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-04-07 22:16:02.000000 yamcs-pymdb-1.0.5/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.892946 yamcs-pymdb-1.0.5/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.892724 yamcs-pymdb-1.0.5/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.904308 yamcs-pymdb-1.0.5/src/yamcs/pymdb/
+-rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/alarms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/algorithms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/ancillary.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/calibrators.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6124 2024-02-25 20:53:48.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/ccsds.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/checks.py
+-rw-r--r--   0 fdi        (503) staff       (20)    17143 2024-03-28 12:30:59.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/commands.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6642 2024-03-28 12:28:20.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/containers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8015 2024-03-28 21:21:31.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/csp.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18231 2024-03-28 12:30:59.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/datatypes.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/encodings.py
+-rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/expressions.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/parameters.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/systems.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/verifiers.py
+-rw-r--r--   0 fdi        (503) staff       (20)    78132 2024-04-05 11:47:37.000000 yamcs-pymdb-1.0.5/src/yamcs/pymdb/xtce.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-04-07 22:18:46.921505 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      737 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-04-07 22:18:46.000000 yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/top_level.txt
```

### Comparing `yamcs-pymdb-1.0.4/LICENSE` & `yamcs-pymdb-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/PKG-INFO` & `yamcs-pymdb-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs-pymdb-1.0.4/README.md` & `yamcs-pymdb-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/setup.py` & `yamcs-pymdb-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="yamcs-pymdb",
-    version="1.0.4",
+    version="1.0.5",
     description="Generate XTCE for use with Yamcs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/yamcs/pymdb",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     license="LGPL",
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/__init__.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/alarms.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/alarms.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/ancillary.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/ancillary.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/calibrators.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/calibrators.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/ccsds.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/ccsds.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/checks.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/checks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from yamcs.pymdb.commands import ArrayArgument
 from yamcs.pymdb.datatypes import FloatDataType
-from yamcs.pymdb.encodings import ByteOrder, FloatDataEncoding, IntegerDataEncoding
+from yamcs.pymdb.encodings import FloatEncoding, IntegerEncoding
 from yamcs.pymdb.parameters import ArrayParameter
 from yamcs.pymdb.systems import System
 from yamcs.pymdb.verifiers import TerminationAction
 
 
 def iter_parameter_data_types(system: System):
     for parameter in system.parameters:
@@ -74,26 +74,26 @@
     encoding.
 
     A common mistake is to have a float of 32 bits, with an encoding of 64 bits.
     """
     ok = True
     for data_type in iter_parameter_data_types(system):
         if isinstance(data_type, FloatDataType) and isinstance(
-            data_type.encoding, FloatDataEncoding
+            data_type.encoding, FloatEncoding
         ):
             if data_type.bits == 32 and data_type.encoding.bits == 64:
                 ok = False
                 print(
                     f"Parameter {data_type}: float bits (32) is "
                     "smaller than encoding (64)"
                 )
 
     for command, argument, data_type in iter_argument_data_types(system):
         if isinstance(data_type, FloatDataType) and isinstance(
-            data_type.encoding, FloatDataEncoding
+            data_type.encoding, FloatEncoding
         ):
             if data_type.bits == 32 and data_type.encoding.bits == 64:
                 ok = False
                 print(
                     f"Command {command}: argument {argument.name} float bits (32) is "
                     "smaller than encoding (64)"
                 )
@@ -107,36 +107,28 @@
     ok = True
     for parameter in system.parameters:
         data_type = parameter
         if isinstance(parameter, ArrayParameter):
             data_type = parameter.data_type
 
         encoding = data_type.encoding
-        if isinstance(encoding, IntegerDataEncoding):
-            if (
-                encoding.byte_order != ByteOrder.LITTLE_ENDIAN
-                and encoding.bits
-                and encoding.bits > 8
-            ):
+        if isinstance(encoding, IntegerEncoding):
+            if not encoding.little_endian and encoding.bits and encoding.bits > 8:
                 ok = False
                 print(f"Parameter {parameter} is not in little endian")
 
     for command in system.commands:
         for argument in command.arguments:
             data_type = argument
             if isinstance(argument, ArrayArgument):
                 data_type = argument.data_type
 
             encoding = data_type.encoding
-            if isinstance(encoding, IntegerDataEncoding):
-                if (
-                    encoding.byte_order != ByteOrder.LITTLE_ENDIAN
-                    and encoding.bits
-                    and encoding.bits > 8
-                ):
+            if isinstance(encoding, IntegerEncoding):
+                if not encoding.little_endian and encoding.bits and encoding.bits > 8:
                     ok = False
                     print(
                         f"Command {command}: argument {argument.name} "
                         "is not in little endian"
                     )
 
     for subsystem in system.subsystems:
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/commands.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     EnumeratedDataType,
     Epoch,
     FloatDataType,
     IntegerDataType,
     Member,
     StringDataType,
 )
-from yamcs.pymdb.encodings import DataEncoding, TimeEncoding
+from yamcs.pymdb.encodings import Encoding, TimeEncoding
 from yamcs.pymdb.expressions import Expression
 from yamcs.pymdb.verifiers import (
     AcceptedVerifier,
     CompleteVerifier,
     ExecutionVerifier,
     FailedVerifier,
     QueuedVerifier,
@@ -81,15 +81,15 @@
         name: str,
         *,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         self.name: str = name
         """Short name of this argument"""
 
         self.default: Any = default
         """Default value"""
 
@@ -141,15 +141,15 @@
         name: str,
         members: Sequence[Member],
         *,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         AggregateDataType.__init__(
             self,
             members=members,
         )
         Argument.__init__(
             self,
@@ -169,15 +169,15 @@
         data_type: DataType,
         length: int,
         *,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         ArrayDataType.__init__(
             self,
             data_type=data_type,
             length=length,
         )
         Argument.__init__(
@@ -199,15 +199,15 @@
         min_length: int | None = None,
         max_length: int | None = None,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BinaryDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Argument.__init__(
@@ -230,15 +230,15 @@
         zero_string_value: str = "False",
         one_string_value: str = "True",
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BooleanDataType.__init__(
             self,
             zero_string_value=zero_string_value,
             one_string_value=one_string_value,
         )
         Argument.__init__(
@@ -260,15 +260,15 @@
         choices: Choices,
         *,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         EnumeratedDataType.__init__(
             self,
             choices=choices,
         )
         Argument.__init__(
             self,
@@ -293,15 +293,15 @@
         maximum: float | None = None,
         maximum_inclusive: bool = True,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         FloatDataType.__init__(
             self,
             bits=bits,
             minimum=minimum,
             minimum_inclusive=minimum_inclusive,
@@ -331,15 +331,15 @@
         minimum: int | None = None,
         maximum: int | None = None,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         IntegerDataType.__init__(
             self,
             signed=signed,
             bits=bits,
             minimum=minimum,
@@ -366,15 +366,15 @@
         min_length: int | None = None,
         max_length: int | None = None,
         default: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         StringDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Argument.__init__(
@@ -445,64 +445,64 @@
         *,
         aliases: Mapping[str, str] | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         abstract: bool = False,
         parent: Command | None = None,
-        restriction_criteria: Expression | None = None,
+        condition: Expression | None = None,
         assignments: Mapping[str, Any] | None = None,
         arguments: Sequence[Argument] | None = None,
         entries: Sequence[CommandEntry] | None = None,
         level: CommandLevel = CommandLevel.NORMAL,
         warning_message: str | None = None,
     ):
-        self.name = name
+        self.name: str = name
         """Short name of this command"""
 
-        self.system = system
+        self.system: System = system
         """System this command belongs to"""
 
-        self.aliases = aliases or {}
+        self.aliases: dict[str, str] = dict(aliases or {})
         """Alternative names, keyed by namespace"""
 
-        self.short_description = short_description
+        self.short_description: str | None = short_description
         """Oneline description"""
 
-        self.long_description = long_description
+        self.long_description: str | None = long_description
         """Multiline description"""
 
-        self.extra = extra or {}
+        self.extra: dict[str, str] = dict(extra or {})
         """Arbitrary information, keyed by name"""
 
-        self.abstract = abstract
-        self.parent = parent
-        self.restriction_criteria = restriction_criteria
-        self.assignments = assignments or {}
+        self.abstract: bool = abstract
+        self.parent: Command | str | None = parent
+        self.condition: Expression | None = condition
+        self.assignments: dict[str, Any] = dict(assignments or {})
         self.arguments: list[Argument] = list(arguments or [])
         self._entries: list[CommandEntry] | None = (
             list(entries) if entries is not None else None
         )
 
         self.transferred_to_range_verifier: TransferredToRangeVerifier | None = None
         self.sent_from_range_verifier: SentFromRangeVerifier | None = None
         self.received_verifier: ReceivedVerifier | None = None
         self.accepted_verifier: AcceptedVerifier | None = None
         self.queued_verifier: QueuedVerifier | None = None
         self.execution_verifiers: list[ExecutionVerifier] = []
         self.complete_verifiers: list[CompleteVerifier] = []
         self.failed_verifier: FailedVerifier | None = None
 
-        self.level = level
+        self.level: CommandLevel = level
         """
         The importance of this telecommand in terms of the nature and
         significance of its on-board effect.
         """
 
-        self.warning_message = warning_message
+        self.warning_message: str | None = warning_message
         """Message explaining the importance of this telecommand"""
 
         if name in system._commands_by_name:
             raise Exception(f"System already contains a command {name}")
         system._commands_by_name[name] = self
 
     @property
@@ -521,15 +521,15 @@
         res.extend(self.execution_verifiers)
         res.extend(self.complete_verifiers)
         if self.failed_verifier:
             res.append(self.failed_verifier)
         return res
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """
         Absolute path of this item covering the full system tree. For example,
         an item ``C`` in a subystem ``B`` of a top-level system ``A`` is
         represented as ``/A/B/C``
         """
         path = "/" + self.name
 
@@ -547,15 +547,15 @@
         :param visit_parents:
             Search upwards in parent commands
         """
         for argument in self.arguments:
             if argument.name == name:
                 return argument
 
-        if visit_parents and self.parent:
+        if visit_parents and self.parent and isinstance(self.parent, Command):
             return self.parent.get_argument(name)
         else:
             return None
 
     @property
     def entries(self) -> list[CommandEntry]:
         """
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/containers.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self,
         system: System,
         name: str,
         entries: Sequence[ParameterEntry | ContainerEntry] | None = None,
         *,
         parent: Container | str | None = None,
         abstract: bool = False,
-        restriction_criteria: Expression | None = None,
+        condition: Expression | None = None,
         aliases: Mapping[str, str] | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         bits: int | None = None,
         rate: float | None = None,
         hint_partition: bool = False,
@@ -126,27 +126,28 @@
         Hint that this container's name should be used for partitioning when
         stored to Yamcs.
         """
 
         self.entries: list[ParameterEntry | ContainerEntry] = list(entries or [])
         self.parent: Container | str | None = parent
         self.abstract: bool = abstract
-        self.restriction_criteria: Expression | None = restriction_criteria
+        self.condition: Expression | None = condition
+        """Restriction criteria for this container."""
 
         if name in system._containers_by_name:
             raise Exception(
                 "System {} already contains a container {}".format(
                     system.qualified_name, name
                 )
             )
 
         system._containers_by_name[name] = self
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """
         Absolute path of this item covering the full system tree. For example,
         an item ``C`` in a subystem ``B`` of a top-level system ``A`` is
         represented as ``/A/B/C``
         """
         path = "/" + self.name
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/csp.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/csp.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/datatypes.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Mapping, Sequence
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum, auto
 from typing import TYPE_CHECKING, Any, Literal, TypeAlias
 
-from yamcs.pymdb.encodings import DataEncoding, TimeEncoding
+from yamcs.pymdb.encodings import Encoding, TimeEncoding
 
 if TYPE_CHECKING:
     from yamcs.pymdb.calibrators import Calibrator
     from yamcs.pymdb.parameters import AbsoluteTimeParameter, IntegerParameter
 
 
 class Epoch(Enum):
@@ -37,29 +37,29 @@
 class DataType:
     def __init__(
         self,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         self.short_description: str | None = short_description
         """Oneline description"""
 
         self.long_description: str | None = long_description
         """Multiline description"""
 
         self.extra: dict[str, str] = dict(extra or {})
         """Arbitrary information, keyed by name"""
 
         self.units: str | None = units
         """Engineering units"""
 
-        self.encoding: DataEncoding | None = encoding
+        self.encoding: Encoding | None = encoding
         """
         How this data is sent or received from some non-native, off-platform
         device. (e.g. a spacecraft)
         """
 
 
 class AbsoluteTimeDataType(DataType):
@@ -87,15 +87,15 @@
     def __init__(
         self,
         members: Sequence[Member],
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -114,15 +114,15 @@
     def __init__(
         self,
         data_type: DataType,
         length: int | DynamicInteger,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             encoding=encoding,
@@ -136,15 +136,15 @@
         self,
         min_length: int | None = None,
         max_length: int | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -163,15 +163,15 @@
         self,
         zero_string_value: str = "False",
         one_string_value: str = "True",
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -186,15 +186,15 @@
     def __init__(
         self,
         choices: Choices,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -224,15 +224,15 @@
         minimum_inclusive: bool = True,
         maximum: float | None = None,
         maximum_inclusive: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
@@ -265,15 +265,15 @@
         bits: int = 32,
         minimum: int | None = None,
         maximum: int | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
@@ -300,15 +300,15 @@
         self,
         min_length: int | None = None,
         max_length: int | None = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -327,15 +327,15 @@
         self,
         name: str,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -382,15 +382,15 @@
         self,
         name: str,
         members: Sequence[Member],
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         AggregateDataType.__init__(
             self,
             members=members,
         )
         Member.__init__(
             self,
@@ -409,15 +409,15 @@
         name: str,
         data_type: DataType,
         length: int,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         ArrayDataType.__init__(
             self,
             data_type=data_type,
             length=length,
         )
         Member.__init__(
@@ -438,15 +438,15 @@
         min_length: int | None = None,
         max_length: int | None = None,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BinaryDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Member.__init__(
@@ -468,15 +468,15 @@
         zero_string_value: str = "False",
         one_string_value: str = "True",
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BooleanDataType.__init__(
             self,
             zero_string_value=zero_string_value,
             one_string_value=one_string_value,
         )
         Member.__init__(
@@ -497,15 +497,15 @@
         name: str,
         choices: Choices,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         EnumeratedDataType.__init__(
             self,
             choices=choices,
         )
         Member.__init__(
             self,
@@ -529,15 +529,15 @@
         maximum: float | None = None,
         maximum_inclusive: bool = True,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         FloatDataType.__init__(
             self,
             bits=bits,
             minimum=minimum,
             minimum_inclusive=minimum_inclusive,
@@ -566,15 +566,15 @@
         minimum: int | None = None,
         maximum: int | None = None,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
     ) -> None:
         IntegerDataType.__init__(
             self,
             signed=signed,
             bits=bits,
             minimum=minimum,
@@ -600,15 +600,15 @@
         min_length: int | None = None,
         max_length: int | None = None,
         initial_value: Any = None,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         StringDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Member.__init__(
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/encodings.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/encodings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,14 @@
-from enum import Enum, auto
-from typing import TypeAlias
-
-from yamcs.pymdb.algorithms import JavaAlgorithm
-
+from __future__ import annotations
 
-class ByteOrder(Enum):
-    """
-    Byte order (endianness)
-    """
-
-    BIG_ENDIAN = auto()
-    """Big Endian (most significant byte first)"""
+from enum import Enum, auto
+from typing import TYPE_CHECKING, TypeAlias
 
-    LITTLE_ENDIAN = auto()
-    """Little Endian (least significant byte first)"""
+if TYPE_CHECKING:
+    from yamcs.pymdb.algorithms import UnnamedAlgorithm
 
 
 class Charset(Enum):
     """String encoding"""
 
     US_ASCII = auto()
     """US-ASCII"""
@@ -46,25 +37,25 @@
     UTF_32LE = auto()
     """UTF-32LE"""
 
     UTF_32BE = auto()
     """UTF-16BE"""
 
 
-class FloatDataEncodingScheme(Enum):
+class FloatEncodingScheme(Enum):
     """Float encoding"""
 
     IEEE754_1985 = auto()
     """IEEE 754-1985"""
 
     MILSTD_1750A = auto()
     """MIL-STD-1750A"""
 
 
-class IntegerDataEncodingScheme(Enum):
+class IntegerEncodingScheme(Enum):
     """Integer encoding"""
 
     UNSIGNED = auto()
     """Unsigned"""
 
     SIGN_MAGNITUDE = auto()
     """Sign-magnitude"""
@@ -72,109 +63,109 @@
     TWOS_COMPLEMENT = auto()
     """Two's complement"""
 
     ONES_COMPLEMENT = auto()
     """Ones' complement"""
 
 
-class DataEncoding:
+class Encoding:
     def __init__(self, bits: int | None = None) -> None:
         self.bits = bits
 
 
-class BinaryDataEncoding(DataEncoding):
+class BinaryEncoding(Encoding):
     def __init__(
         self,
         bits: int | None = None,
         length_bits: int | None = None,
-        encoder: JavaAlgorithm | None = None,
-        decoder: JavaAlgorithm | None = None,
+        encoder: UnnamedAlgorithm | None = None,
+        decoder: UnnamedAlgorithm | None = None,
     ) -> None:
         super().__init__(bits=bits)
 
         self.length_bits: int | None = length_bits
         """
         Length in bits of a leading size tag
         """
 
-        self.encoder: JavaAlgorithm | None = encoder
+        self.encoder: UnnamedAlgorithm | None = encoder
         """
         Custom encoder, when this encoding is used for telecommanding
         """
 
-        self.decoder: JavaAlgorithm | None = decoder
+        self.decoder: UnnamedAlgorithm | None = decoder
         """
         Custom decoder, when this encoding is used for telemetry
         """
 
 
-class IntegerDataEncoding(DataEncoding):
+class IntegerEncoding(Encoding):
     def __init__(
         self,
         bits: int,
-        byte_order: ByteOrder = ByteOrder.BIG_ENDIAN,
-        scheme: IntegerDataEncodingScheme = IntegerDataEncodingScheme.UNSIGNED,
+        little_endian: bool = False,
+        scheme: IntegerEncodingScheme = IntegerEncodingScheme.UNSIGNED,
     ) -> None:
         super().__init__(bits=bits)
-        self.byte_order: ByteOrder = byte_order
-        self.scheme: IntegerDataEncodingScheme = scheme
+        self.little_endian: bool = little_endian
+        self.scheme: IntegerEncodingScheme = scheme
 
 
-class FloatDataEncoding(DataEncoding):
+class FloatEncoding(Encoding):
     def __init__(
         self,
         bits: int,
-        byte_order: ByteOrder = ByteOrder.BIG_ENDIAN,
-        scheme: FloatDataEncodingScheme = FloatDataEncodingScheme.IEEE754_1985,
+        little_endian: bool = False,
+        scheme: FloatEncodingScheme = FloatEncodingScheme.IEEE754_1985,
     ) -> None:
         super().__init__(bits=bits)
-        self.byte_order: ByteOrder = byte_order
-        self.scheme: FloatDataEncodingScheme = scheme
+        self.little_endian: bool = little_endian
+        self.scheme: FloatEncodingScheme = scheme
 
 
-class FloatTimeEncoding(FloatDataEncoding):
+class FloatTimeEncoding(FloatEncoding):
     def __init__(
         self,
         bits: int,
-        byte_order: ByteOrder = ByteOrder.BIG_ENDIAN,
-        scheme: FloatDataEncodingScheme = FloatDataEncodingScheme.IEEE754_1985,
+        little_endian: bool = False,
+        scheme: FloatEncodingScheme = FloatEncodingScheme.IEEE754_1985,
         offset: float = 0,
         scale: float = 1,
     ) -> None:
         super().__init__(
             bits=bits,
-            byte_order=byte_order,
+            little_endian=little_endian,
             scheme=scheme,
         )
         self.offset: float = offset
         self.scale: float = scale
 
 
-class IntegerTimeEncoding(IntegerDataEncoding):
+class IntegerTimeEncoding(IntegerEncoding):
     def __init__(
         self,
         bits: int,
-        byte_order: ByteOrder = ByteOrder.BIG_ENDIAN,
-        scheme: IntegerDataEncodingScheme = IntegerDataEncodingScheme.UNSIGNED,
+        little_endian: bool = False,
+        scheme: IntegerEncodingScheme = IntegerEncodingScheme.UNSIGNED,
         offset: float = 0,
         scale: float = 1,
     ) -> None:
         super().__init__(
             bits=bits,
-            byte_order=byte_order,
+            little_endian=little_endian,
             scheme=scheme,
         )
         self.offset: float = offset
         self.scale: float = scale
 
 
 TimeEncoding: TypeAlias = FloatTimeEncoding | IntegerTimeEncoding
 
 
-class StringDataEncoding(DataEncoding):
+class StringEncoding(Encoding):
     def __init__(
         self,
         bits: int | None = None,
         length_bits: int | None = None,
         max_bits: int | None = 8388608,
         charset: Charset = Charset.US_ASCII,
         termination: bytes = b"\0",
@@ -194,212 +185,126 @@
         Default is 1 MB
         """
 
         self.charset: Charset = charset
         self.termination: bytes = termination
 
 
-uint1_t = IntegerDataEncoding(
-    bits=1,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint1_t = IntegerEncoding(bits=1, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 1-bit integer"""
 
-uint2_t = IntegerDataEncoding(
-    bits=2,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint2_t = IntegerEncoding(bits=2, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 2-bit integer"""
 
-uint3_t = IntegerDataEncoding(
-    bits=3,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint3_t = IntegerEncoding(bits=3, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 3-bit integer"""
 
-uint4_t = IntegerDataEncoding(
-    bits=4,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint4_t = IntegerEncoding(bits=4, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 4-bit integer"""
 
-uint5_t = IntegerDataEncoding(
-    bits=5,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint5_t = IntegerEncoding(bits=5, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 5-bit integer"""
 
-uint6_t = IntegerDataEncoding(
-    bits=6,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint6_t = IntegerEncoding(bits=6, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 6-bit integer"""
 
-uint7_t = IntegerDataEncoding(
-    bits=7,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint7_t = IntegerEncoding(bits=7, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 7-bit integer"""
 
-int8_t = IntegerDataEncoding(
-    bits=8,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.TWOS_COMPLEMENT,
-)
+int8_t = IntegerEncoding(bits=8, scheme=IntegerEncodingScheme.TWOS_COMPLEMENT)
 """Signed 8-bit integer in two's complement notation (big endian)"""
 
-uint8_t = IntegerDataEncoding(
-    bits=8,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint8_t = IntegerEncoding(bits=8, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 8-bit integer (big endian)"""
 
-uint8_t = IntegerDataEncoding(
-    bits=8,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint8_t = IntegerEncoding(bits=8, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 8-bit integer"""
 
 bool_t = uint8_t
 """Same as ``uint8_t``. 0=False, 1=True"""
 
-uint9_t = IntegerDataEncoding(
-    bits=9,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint9_t = IntegerEncoding(bits=9, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 9-bit integer"""
 
-uint10_t = IntegerDataEncoding(
-    bits=10,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint10_t = IntegerEncoding(bits=10, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 10-bit integer"""
 
-uint11_t = IntegerDataEncoding(
-    bits=11,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint11_t = IntegerEncoding(bits=11, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 11-bit integer"""
 
-uint12_t = IntegerDataEncoding(
-    bits=12,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint12_t = IntegerEncoding(bits=12, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 12-bit integer"""
 
-uint13_t = IntegerDataEncoding(
-    bits=13,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint13_t = IntegerEncoding(bits=13, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 13-bit integer"""
 
-uint14_t = IntegerDataEncoding(
-    bits=14,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint14_t = IntegerEncoding(bits=14, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 14-bit integer"""
 
-uint15_t = IntegerDataEncoding(
-    bits=15,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint15_t = IntegerEncoding(bits=15, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 15-bit integer"""
 
-int16_t = IntegerDataEncoding(
-    bits=16,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.TWOS_COMPLEMENT,
-)
+int16_t = IntegerEncoding(bits=16, scheme=IntegerEncodingScheme.TWOS_COMPLEMENT)
 """Signed 16-bit integer in two's complement notation (big endian)"""
 
-int16le_t = IntegerDataEncoding(
+int16le_t = IntegerEncoding(
     bits=16,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=IntegerDataEncodingScheme.TWOS_COMPLEMENT,
+    little_endian=True,
+    scheme=IntegerEncodingScheme.TWOS_COMPLEMENT,
 )
 """Signed 16-bit integer in two's complement notation (little endian)"""
 
-uint16_t = IntegerDataEncoding(
-    bits=16,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint16_t = IntegerEncoding(bits=16, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 16-bit integer (big endian)"""
 
-uint16le_t = IntegerDataEncoding(
+uint16le_t = IntegerEncoding(
     bits=16,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
+    little_endian=True,
+    scheme=IntegerEncodingScheme.UNSIGNED,
 )
 """Unsigned 16-bit integer (little endian)"""
 
-int32_t = IntegerDataEncoding(
-    bits=32,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.TWOS_COMPLEMENT,
-)
+int24_t = IntegerEncoding(bits=24, scheme=IntegerEncodingScheme.TWOS_COMPLEMENT)
+"""Signed 24-bit integer in two's complement notation"""
+
+uint24_t = IntegerEncoding(bits=24, scheme=IntegerEncodingScheme.UNSIGNED)
+"""Unsigned 24-bit integer"""
+
+int32_t = IntegerEncoding(bits=32, scheme=IntegerEncodingScheme.TWOS_COMPLEMENT)
 """Signed 32-bit integer in two's complement notation (big endian)"""
 
-int32le_t = IntegerDataEncoding(
+int32le_t = IntegerEncoding(
     bits=32,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=IntegerDataEncodingScheme.TWOS_COMPLEMENT,
+    little_endian=True,
+    scheme=IntegerEncodingScheme.TWOS_COMPLEMENT,
 )
 """Signed 32-bit integer in two's complement notation (little endian)"""
 
-uint32_t = IntegerDataEncoding(
-    bits=32,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
-)
+uint32_t = IntegerEncoding(bits=32, scheme=IntegerEncodingScheme.UNSIGNED)
 """Unsigned 32-bit integer (big endian)"""
 
-uint32le_t = IntegerDataEncoding(
+uint32le_t = IntegerEncoding(
     bits=32,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=IntegerDataEncodingScheme.UNSIGNED,
+    little_endian=True,
+    scheme=IntegerEncodingScheme.UNSIGNED,
 )
 """Unsigned 32-bit integer (little endian)"""
 
-float32_t = FloatDataEncoding(
-    bits=32,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=FloatDataEncodingScheme.IEEE754_1985,
-)
+float32_t = FloatEncoding(bits=32, scheme=FloatEncodingScheme.IEEE754_1985)
 """32-bit float in IEEE754-1985 encoding (big endian)"""
 
-float32le_t = FloatDataEncoding(
+float32le_t = FloatEncoding(
     bits=32,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=FloatDataEncodingScheme.IEEE754_1985,
+    little_endian=True,
+    scheme=FloatEncodingScheme.IEEE754_1985,
 )
 """32-bit float in IEEE754-1985 encoding (little endian)"""
 
-float64_t = FloatDataEncoding(
-    bits=64,
-    byte_order=ByteOrder.BIG_ENDIAN,
-    scheme=FloatDataEncodingScheme.IEEE754_1985,
-)
+float64_t = FloatEncoding(bits=64, scheme=FloatEncodingScheme.IEEE754_1985)
 """64-bit float in IEEE754-1985 encoding (big endian)"""
 
-float64le_t = FloatDataEncoding(
+float64le_t = FloatEncoding(
     bits=64,
-    byte_order=ByteOrder.LITTLE_ENDIAN,
-    scheme=FloatDataEncodingScheme.IEEE754_1985,
+    little_endian=True,
+    scheme=FloatEncodingScheme.IEEE754_1985,
 )
 """64-bit float in IEEE754-1985 encoding (little endian)"""
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/expressions.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/expressions.py`

 * *Files identical despite different names*

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/parameters.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     EnumeratedDataType,
     Epoch,
     FloatDataType,
     IntegerDataType,
     Member,
     StringDataType,
 )
-from yamcs.pymdb.encodings import DataEncoding, TimeEncoding
+from yamcs.pymdb.encodings import Encoding, TimeEncoding
 
 if TYPE_CHECKING:
     from yamcs.pymdb.calibrators import Calibrator
     from yamcs.pymdb.systems import System
 
 
 class DataSource(Enum):
@@ -86,20 +86,20 @@
         self,
         system: System,
         name: str,
         *,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         DataType.__init__(
             self,
             short_description=short_description,
             long_description=long_description,
             extra=extra,
             units=units,
@@ -121,27 +121,27 @@
         """
 
         self.initial_value: Any = initial_value
         """Initial value"""
 
         self.persistent: bool = persistent
         """
-        If true, the parameter's latest value is restored in case of a
+        If true, the parameter's last value is restored in case of a
         restart of the Yamcs system.
 
         If :attr:`initial_value` is set too, attr:`initial_value` is only
         used once (when there is no other value to persist).
         """
 
         if name in system._parameters_by_name:
             raise Exception(f"System already contains a parameter {name}")
         system._parameters_by_name[name] = self
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """
         Absolute path of this item covering the full system tree. For example,
         an item ``C`` in a subystem ``B`` of a top-level system ``A`` is
         represented as ``/A/B/C``
         """
         path = "/" + self.name
 
@@ -168,15 +168,15 @@
         self,
         system: System,
         name: str,
         reference: Epoch | datetime | AbsoluteTimeParameter,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
         encoding: TimeEncoding | None = None,
     ) -> None:
         AbsoluteTimeDataType.__init__(
@@ -209,19 +209,19 @@
         self,
         system: System,
         name: str,
         members: Sequence[Member],
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         AggregateDataType.__init__(
             self,
             members=members,
         )
         Parameter.__init__(
             self,
@@ -249,19 +249,19 @@
         system: System,
         name: str,
         data_type: DataType,
         length: int | DynamicInteger,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         ArrayDataType.__init__(
             self,
             data_type=data_type,
             length=length,
         )
         Parameter.__init__(
@@ -289,20 +289,20 @@
         system: System,
         name: str,
         min_length: int | None = None,
         max_length: int | None = None,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BinaryDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Parameter.__init__(
@@ -331,20 +331,20 @@
         system: System,
         name: str,
         zero_string_value: str = "False",
         one_string_value: str = "True",
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         BooleanDataType.__init__(
             self,
             zero_string_value=zero_string_value,
             one_string_value=one_string_value,
         )
         Parameter.__init__(
@@ -373,20 +373,20 @@
         system: System,
         name: str,
         choices: Choices,
         alarm: EnumerationAlarm | None = None,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         EnumeratedDataType.__init__(
             self,
             choices=choices,
         )
         Parameter.__init__(
             self,
@@ -420,20 +420,20 @@
         minimum: float | None = None,
         minimum_inclusive: bool = True,
         maximum: float | None = None,
         maximum_inclusive: bool = True,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
         alarm: ThresholdAlarm | None = None,
     ) -> None:
         FloatDataType.__init__(
             self,
             bits=bits,
             minimum=minimum,
@@ -473,20 +473,20 @@
         signed: bool = True,
         bits: int = 32,
         minimum: int | None = None,
         maximum: int | None = None,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
         calibrator: Calibrator | None = None,
         alarm: ThresholdAlarm | None = None,
     ) -> None:
         IntegerDataType.__init__(
             self,
             signed=signed,
             bits=bits,
@@ -523,20 +523,20 @@
         system: System,
         name: str,
         min_length: int | None = None,
         max_length: int | None = None,
         aliases: Mapping[str, str] | None = None,
         data_source: DataSource = DataSource.TELEMETERED,
         initial_value: Any = None,
-        persistent: bool = False,
+        persistent: bool = True,
         short_description: str | None = None,
         long_description: str | None = None,
         extra: Mapping[str, str] | None = None,
         units: str | None = None,
-        encoding: DataEncoding | None = None,
+        encoding: Encoding | None = None,
     ) -> None:
         StringDataType.__init__(
             self,
             min_length=min_length,
             max_length=max_length,
         )
         Parameter.__init__(
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/systems.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/systems.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
+from typing import TYPE_CHECKING
 
 from yamcs.pymdb import xtce
-from yamcs.pymdb.commands import Command
-from yamcs.pymdb.containers import Container
-from yamcs.pymdb.parameters import Parameter
+
+if TYPE_CHECKING:
+    from yamcs.pymdb.algorithms import Algorithm
+    from yamcs.pymdb.commands import Command
+    from yamcs.pymdb.containers import Container
+    from yamcs.pymdb.parameters import Parameter
 
 
 class System:
     """
     The top-level system is the root element for the set of metadata
     necessary to monitor and command a space device, such as a satellite.
 
@@ -40,14 +44,15 @@
 
         self.long_description: str | None = long_description
         """Multiline description"""
 
         self.extra: dict[str, str] = dict(extra or {})
         """Arbitrary information, keyed by name"""
 
+        self._algorithms_by_name: dict[str, Algorithm] = {}
         self._commands_by_name: dict[str, Command] = {}
         self._containers_by_name: dict[str, Container] = {}
         self._parameters_by_name: dict[str, Parameter] = {}
         self._subsystems_by_name: dict[str, Subsystem] = {}
 
     @property
     def root(self) -> System:
@@ -84,14 +89,23 @@
         Parameters directly belonging to this system
         """
         copy = list(self._parameters_by_name.values())
         copy.sort()
         return copy
 
     @property
+    def algorithms(self) -> list[Algorithm]:
+        """
+        Algorithms directly belonging to this system
+        """
+        copy = list(self._algorithms_by_name.values())
+        copy.sort()
+        return copy
+
+    @property
     def subsystems(self) -> list[Subsystem]:
         """
         Subsystems directly belonging to this system
         """
         copy = list(self._subsystems_by_name.values())
         copy.sort()
         return copy
@@ -128,14 +142,26 @@
         """
         try:
             self._containers_by_name.pop(name)
             return True
         except KeyError:
             return False
 
+    def remove_algorithm(self, name: str) -> bool:
+        """
+        Removes an algorithm directly belonging to this system.
+
+        Raises an exception if no such algorithm exists
+        """
+        try:
+            self._algorithms_by_name.pop(name)
+            return True
+        except KeyError:
+            return False
+
     def remove_subsystem(self, name: str) -> bool:
         """
         Removes a subsystem directly belonging to this system.
 
         Raises an exception if no such subsystem exists
         """
         try:
@@ -164,14 +190,22 @@
         """
         Find a container belonging directly to this system.
 
         Raises an exception if no container is found
         """
         return self._containers_by_name[name]
 
+    def find_algorithm(self, name: str) -> Algorithm:
+        """
+        Find an algorithm belonging directly to this system.
+
+        Raises an exception if no algorithm is found
+        """
+        return self._algorithms_by_name[name]
+
     def find_subsystem(self, name: str) -> Subsystem:
         """
         Find a subsystem belonging directly to this system.
 
         Raises an exception if no subsystem is found
         """
         return self._subsystems_by_name[name]
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/verifiers.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/verifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import TYPE_CHECKING, TypeAlias
 
 if TYPE_CHECKING:
-    from yamcs.pymdb.algorithms import JavaAlgorithm
+    from yamcs.pymdb.algorithms import UnnamedAlgorithm
     from yamcs.pymdb.containers import Container
     from yamcs.pymdb.expressions import Expression
     from yamcs.pymdb.parameters import Parameter
 
 
 class TerminationAction(Enum):
     SUCCESS = auto()
     FAIL = auto()
 
 
 class AlgorithmCheck:
-    def __init__(self, algorithm: JavaAlgorithm):
+    def __init__(self, algorithm: UnnamedAlgorithm):
         self.algorithm = algorithm
 
 
 class ContainerCheck:
     def __init__(self, container: Container):
         self.container = container
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs/pymdb/xtce.py` & `yamcs-pymdb-1.0.5/src/yamcs/pymdb/xtce.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,27 @@
 
 import os
 import xml.etree.ElementTree as ET
 from binascii import hexlify
 from collections.abc import Mapping
 from datetime import datetime, timezone
 from enum import Enum
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Sequence, cast
 from xml.dom import minidom
 
 from yamcs.pymdb.alarms import AlarmLevel, ThresholdAlarm
-from yamcs.pymdb.algorithms import JavaAlgorithm
+from yamcs.pymdb.algorithms import (
+    Algorithm,
+    ContainerTrigger,
+    InputParameter,
+    OutputParameter,
+    ParameterTrigger,
+    Trigger,
+    UnnamedAlgorithm,
+)
 from yamcs.pymdb.ancillary import AncillaryData
 from yamcs.pymdb.calibrators import Calibrator, Interpolate, Polynomial
 from yamcs.pymdb.commands import (
     Argument,
     ArgumentEntry,
     BooleanArgument,
     Command,
@@ -44,25 +52,24 @@
     FloatMember,
     IntegerDataType,
     IntegerMember,
     StringDataType,
     StringMember,
 )
 from yamcs.pymdb.encodings import (
-    BinaryDataEncoding,
-    ByteOrder,
+    BinaryEncoding,
     Charset,
-    DataEncoding,
-    FloatDataEncoding,
-    FloatDataEncodingScheme,
+    Encoding,
+    FloatEncoding,
+    FloatEncodingScheme,
     FloatTimeEncoding,
-    IntegerDataEncoding,
-    IntegerDataEncodingScheme,
+    IntegerEncoding,
+    IntegerEncodingScheme,
     IntegerTimeEncoding,
-    StringDataEncoding,
+    StringEncoding,
 )
 from yamcs.pymdb.exceptions import ExportError
 from yamcs.pymdb.expressions import (
     AndExpression,
     EqExpression,
     Expression,
     GteExpression,
@@ -199,16 +206,16 @@
             self.add_aliases(el, command.aliases)
 
         if command.extra:
             self.add_ancillary_data(el, command.extra)
 
         if command.parent:
             base_el = ET.SubElement(el, "BaseMetaCommand")
-            base_el.attrib["metaCommandRef"] = self.make_ref(
-                target=command.parent.qualified_name,
+            base_el.attrib["metaCommandRef"] = self.make_command_ref(
+                target=command.parent,
                 start=command.system,
             )
 
             if command.assignments:
                 assignments_el = ET.SubElement(base_el, "ArgumentAssignmentList")
                 for k, v in command.assignments.items():
                     arg = command.get_argument(k)
@@ -232,16 +239,16 @@
         container_el = ET.SubElement(el, "CommandContainer")
         container_el.attrib["name"] = command.name
 
         self.add_command_entry_list(container_el, command)
 
         if command.parent:
             base_el = ET.SubElement(container_el, "BaseContainer")
-            base_el.attrib["containerRef"] = self.make_ref(
-                target=command.parent.qualified_name,
+            base_el.attrib["containerRef"] = self.make_command_ref(
+                target=command.parent,
                 start=command.system,
             )
 
         sign_el = ET.SubElement(el, "DefaultSignificance")
 
         if command.level == CommandLevel.NORMAL:
             sign_el.attrib["consequenceLevel"] = "normal"
@@ -327,16 +334,16 @@
             extra["yamcs.onTimeout"] = ""
 
         self.add_ancillary_data(el, extra)
 
         check = verifier.check
         if isinstance(check, ContainerCheck):
             ref_el = ET.SubElement(el, "ContainerRef")
-            ref_el.attrib["containerRef"] = self.make_ref(
-                target=check.container.qualified_name,
+            ref_el.attrib["containerRef"] = self.make_container_ref(
+                target=check.container,
                 start=command.system,
             )
         elif isinstance(check, ExpressionCheck):
             expr_el = ET.SubElement(el, "BooleanExpression")
             self.add_expression_condition(expr_el, command.system, check.expression)
         elif isinstance(check, AlgorithmCheck):
             self.add_input_only_algorithm(
@@ -355,16 +362,16 @@
             (
                 CompleteVerifier,
                 FailedVerifier,
             ),
         ):
             if verifier.return_parameter:
                 ret_el = ET.SubElement(el, "ReturnParmRef")
-                ret_el.attrib["parameterRef"] = self.make_ref(
-                    target=verifier.return_parameter.qualified_name,
+                ret_el.attrib["parameterRef"] = self.make_parameter_ref(
+                    target=verifier.return_parameter,
                     start=command.system,
                 )
 
     def add_argument(self, parent: ET.Element, command: Command, argument: Argument):
         el = ET.SubElement(parent, "Argument")
         el.attrib["name"] = argument.name
         el.attrib["argumentTypeRef"] = f"{command.name}__{argument.name}"
@@ -493,14 +500,23 @@
             )
 
     def add_telemetry_metadata(self, parent: ET.Element, system: System):
         el = ET.SubElement(parent, "TelemetryMetaData")
         self.add_parameter_type_set(el, system)
         self.add_parameter_set(el, system)
         self.add_container_set(el, system)
+        self.add_algorithm_set(el, system)
+
+    def add_algorithm_set(self, parent: ET.Element, system: System):
+        if not system.algorithms:
+            return
+
+        el = ET.SubElement(parent, "AlgorithmSet")
+        for algorithm in system.algorithms:
+            self.add_custom_algorithm(el, system, algorithm)
 
     def add_parameter_type_set(self, parent: ET.Element, system: System):
         if not system.parameters:
             return
 
         el = ET.SubElement(parent, "ParameterTypeSet")
         for parameter in system.parameters:
@@ -737,16 +753,17 @@
             unit_el.attrib["form"] = "calibrated"
             unit_el.text = data_type.units
 
         if data_type.encoding:
             self.add_data_encoding(el, system, data_type.encoding)
 
         if data_type.minimum is not None or data_type.maximum is not None:
-            range_el = ET.SubElement(el, "ValidRange")
-            range_el.attrib["validRangeAppliesToCalibrated"] = "true"
+            set_el = ET.SubElement(el, "ValidRangeSet")
+            set_el.attrib["validRangeAppliesToCalibrated"] = "true"
+            range_el = ET.SubElement(set_el, "ValidRange")
             if data_type.minimum is not None:
                 if data_type.minimum_inclusive:
                     range_el.attrib["minInclusive"] = str(data_type.minimum)
                 else:
                     range_el.attrib["minExclusive"] = str(data_type.minimum)
             if data_type.maximum is not None:
                 if data_type.maximum_inclusive:
@@ -923,24 +940,18 @@
         ET.SubElement(start_idx_el, "FixedValue").text = "0"
 
         end_idx_el = ET.SubElement(dim_el, "EndingIndex")
         if isinstance(data_type.length, DynamicInteger):
             dyn_el = ET.SubElement(end_idx_el, "DynamicValue")
             ref_el = ET.SubElement(dyn_el, "ParameterInstanceRef")
             parameter = data_type.length.parameter
-            if isinstance(parameter, Parameter):
-                ref_el.attrib["parameterRef"] = self.make_ref(
-                    parameter.qualified_name,
-                    start=system,
-                )
-            else:
-                ref_el.attrib["parameterRef"] = self.make_ref(
-                    parameter,
-                    start=system,
-                )
+            ref_el.attrib["parameterRef"] = self.make_parameter_ref(
+                parameter,
+                start=system,
+            )
             adj_el = ET.SubElement(dyn_el, "LinearAdjustment")
             adj_el.attrib["intercept"] = "-1"
         else:
             ET.SubElement(end_idx_el, "FixedValue").text = str(data_type.length - 1)
 
         el_type = data_type.data_type
         if isinstance(el_type, AbsoluteTimeDataType):
@@ -1049,16 +1060,16 @@
             if data_type.reference.tzinfo:
                 utctime = data_type.reference.astimezone(tz=timezone.utc)
                 epoch_el.text = utctime.isoformat().replace("+00:00", "Z")
             else:
                 epoch_el.text = data_type.reference.isoformat() + "Z"
         else:
             offset_el = ET.SubElement(ref_el, "OffsetFrom")
-            offset_el.attrib["parameterRef"] = self.make_ref(
-                data_type.reference.qualified_name,
+            offset_el.attrib["parameterRef"] = self.make_parameter_ref(
+                data_type.reference,
                 start=self.system,
             )
 
     def add_binary_parameter_type(
         self,
         parent: ET.Element,
         system: System,
@@ -1339,34 +1350,34 @@
                 else:
                     range_el.attrib["maxInclusive"] = str(alarm.severe_high)
 
     def add_data_encoding(
         self,
         parent: ET.Element,
         system: System,
-        encoding: DataEncoding,
+        encoding: Encoding,
         calibrator: Calibrator | None = None,
     ):
         if isinstance(encoding, FloatTimeEncoding):
             self.add_float_time_encoding(parent, encoding)
         elif isinstance(encoding, IntegerTimeEncoding):
             self.add_integer_time_encoding(parent, encoding)
-        elif isinstance(encoding, BinaryDataEncoding):
+        elif isinstance(encoding, BinaryEncoding):
             self.add_binary_data_encoding(parent, system, encoding)
-        elif isinstance(encoding, IntegerDataEncoding):
+        elif isinstance(encoding, IntegerEncoding):
             self.add_integer_data_encoding(parent, encoding, calibrator)
-        elif isinstance(encoding, FloatDataEncoding):
+        elif isinstance(encoding, FloatEncoding):
             self.add_float_data_encoding(parent, encoding, calibrator)
-        elif isinstance(encoding, StringDataEncoding):
+        elif isinstance(encoding, StringEncoding):
             self.add_string_data_encoding(parent, encoding)
         else:
             raise Exception("Unexpected encoding")
 
     def add_binary_data_encoding(
-        self, parent: ET.Element, system: System, encoding: BinaryDataEncoding
+        self, parent: ET.Element, system: System, encoding: BinaryEncoding
     ):
         el = ET.SubElement(parent, "BinaryDataEncoding")
         size_el = ET.SubElement(el, "SizeInBits")
 
         if encoding.bits is not None:
             fv_el = ET.SubElement(size_el, "FixedValue")
             fv_el.text = str(encoding.bits)
@@ -1412,47 +1423,89 @@
 
         if encoding.encoder:
             self.add_input_only_algorithm(
                 el, system, "ToBinaryTransformAlgorithm", encoding.encoder
             )
 
     def add_input_only_algorithm(
-        self, parent: ET.Element, system: System, tag: str, algorithm: JavaAlgorithm
+        self, parent: ET.Element, system: System, tag: str, algorithm: UnnamedAlgorithm
     ):
         el = ET.SubElement(parent, tag)
-        if isinstance(algorithm, JavaAlgorithm):
-            el.attrib["name"] = algorithm.java.replace(".", "_")
-            if algorithm.extra:
-                self.add_ancillary_data(el, algorithm.extra)
-            text_el = ET.SubElement(el, "AlgorithmText")
-            text_el.attrib["language"] = "Java"
-            text_el.text = algorithm.java
-
-            if algorithm.inputs:
-                inputset_el = ET.SubElement(el, "InputSet")
-                for input in algorithm.inputs:
-                    ref_el = ET.SubElement(inputset_el, "InputParameterInstanceRef")
-                    if isinstance(input.parameter, Parameter):
-                        ref_el.attrib["parameterRef"] = self.make_ref(
-                            input.parameter.qualified_name,
-                            start=system,
-                        )
-                    else:
-                        ref_el.attrib["parameterRef"] = self.make_ref(
-                            input.parameter,
-                            start=system,
-                        )
-                    if input.name:
-                        ref_el.attrib["inputName"] = input.name
+        el.attrib["name"] = "Unnamed"
+        if algorithm.extra:
+            self.add_ancillary_data(el, algorithm.extra)
+        text_el = ET.SubElement(el, "AlgorithmText")
+        text_el.attrib["language"] = algorithm.language
+        text_el.text = algorithm.text
+
+        self.add_inputs(el, system, algorithm.inputs)
+
+    def add_triggers(
+        self, parent: ET.Element, system: System, triggers: Sequence[Trigger]
+    ):
+        if triggers:
+            triggerset_el = ET.SubElement(parent, "TriggerSet")
+            for trigger in triggers:
+                self.add_trigger(triggerset_el, system, trigger)
+
+    def add_trigger(self, parent: ET.Element, system: System, trigger: Trigger):
+        if isinstance(trigger, ParameterTrigger):
+            el = ET.SubElement(parent, "OnParameterUpdateTrigger")
+            el.attrib["parameterRef"] = self.make_parameter_ref(
+                trigger.parameter, system
+            )
+        elif isinstance(trigger, ContainerTrigger):
+            el = ET.SubElement(parent, "OnContainerUpdateTrigger")
+            el.attrib["containerRef"] = self.make_container_ref(
+                trigger.container, system
+            )
         else:
-            raise Exception("Unexpected algorithm type")
+            raise ExportError(f"Unexpected trigger {trigger.__class__}")
+
+    def add_inputs(
+        self,
+        parent: ET.Element,
+        system: System,
+        inputs: Sequence[InputParameter],
+    ):
+        if inputs:
+            inputset_el = ET.SubElement(parent, "InputSet")
+            for input in inputs:
+                self.add_input(inputset_el, system, input)
+
+    def add_input(self, parent: ET.Element, system: System, input: InputParameter):
+        ref_el = ET.SubElement(parent, "InputParameterInstanceRef")
+        ref_el.attrib["parameterRef"] = self.make_parameter_ref(
+            input.parameter,
+            start=system,
+        )
+        if input.name:
+            ref_el.attrib["inputName"] = input.name
 
-    def add_string_data_encoding(
-        self, parent: ET.Element, encoding: StringDataEncoding
+    def add_outputs(
+        self,
+        parent: ET.Element,
+        system: System,
+        outputs: Sequence[OutputParameter],
     ):
+        if outputs:
+            outputset_el = ET.SubElement(parent, "OutputSet")
+            for output in outputs:
+                self.add_output(outputset_el, system, output)
+
+    def add_output(self, parent: ET.Element, system: System, output: OutputParameter):
+        ref_el = ET.SubElement(parent, "OutputParameterRef")
+        ref_el.attrib["parameterRef"] = self.make_parameter_ref(
+            output.parameter,
+            start=system,
+        )
+        if output.name:
+            ref_el.attrib["outputName"] = output.name
+
+    def add_string_data_encoding(self, parent: ET.Element, encoding: StringEncoding):
         el = ET.SubElement(parent, "StringDataEncoding")
 
         if encoding.charset == Charset.US_ASCII:
             el.attrib["encoding"] = "US-ASCII"
         elif encoding.charset == Charset.ISO_8859_1:
             el.attrib["encoding"] = "ISO-8859-1"
         elif encoding.charset == Charset.WINDOWS_1252:
@@ -1475,20 +1528,20 @@
             raise Exception(f"Unexpected charset {encoding.charset}")
 
         if encoding.bits is not None:
             size_el = ET.SubElement(el, "SizeInBits")
             fixed_el = ET.SubElement(size_el, "Fixed")
             fv_el = ET.SubElement(fixed_el, "FixedValue")
             fv_el.text = str(encoding.bits)
-            if encoding.length_bits:
-                lsize_el = ET.SubElement(size_el, "LeadingSize")
-                lsize_el.attrib["sizeInBitsOfSizeTag"] = str(encoding.length_bits)
             if encoding.termination is not None:
                 termination_el = ET.SubElement(size_el, "TerminationChar")
                 termination_el.text = hexlify(encoding.termination).decode("ascii")
+            if encoding.length_bits:
+                lsize_el = ET.SubElement(size_el, "LeadingSize")
+                lsize_el.attrib["sizeInBitsOfSizeTag"] = str(encoding.length_bits)
         else:
             var_el = ET.SubElement(el, "Variable")
             var_el.attrib["maxSizeInBits"] = str(encoding.max_bits)  # Required
 
             # XTCE 1.2 enforces the use of either DynamicValue or DiscreteLookupList.
             # Use a special value recognized by Yamcs to work around this limitation.
             dyn_el = ET.SubElement(var_el, "DynamicValue")
@@ -1518,56 +1571,56 @@
         el.attrib["scale"] = str(encoding.scale)
         el.attrib["units"] = "seconds"
         self.add_integer_data_encoding(el, encoding, calibrator=None)
 
     def add_integer_data_encoding(
         self,
         parent: ET.Element,
-        encoding: IntegerDataEncoding,
+        encoding: IntegerEncoding,
         calibrator: Calibrator | None,
     ):
         el = ET.SubElement(parent, "IntegerDataEncoding")
         el.attrib["sizeInBits"] = str(encoding.bits)
 
-        if encoding.scheme == IntegerDataEncodingScheme.UNSIGNED:
+        if encoding.scheme == IntegerEncodingScheme.UNSIGNED:
             el.attrib["encoding"] = "unsigned"
-        elif encoding.scheme == IntegerDataEncodingScheme.SIGN_MAGNITUDE:
+        elif encoding.scheme == IntegerEncodingScheme.SIGN_MAGNITUDE:
             el.attrib["encoding"] = "signMagnitude"
-        elif encoding.scheme == IntegerDataEncodingScheme.TWOS_COMPLEMENT:
+        elif encoding.scheme == IntegerEncodingScheme.TWOS_COMPLEMENT:
             el.attrib["encoding"] = "twosComplement"
-        elif encoding.scheme == IntegerDataEncodingScheme.ONES_COMPLEMENT:
+        elif encoding.scheme == IntegerEncodingScheme.ONES_COMPLEMENT:
             el.attrib["encoding"] = "onesComplement"
 
         if (encoding.bits is not None) and (encoding.bits > 8):
-            if encoding.byte_order == ByteOrder.BIG_ENDIAN:
-                el.attrib["byteOrder"] = "mostSignificantByteFirst"
-            elif encoding.byte_order == ByteOrder.LITTLE_ENDIAN:
+            if encoding.little_endian:
                 el.attrib["byteOrder"] = "leastSignificantByteFirst"
+            else:
+                el.attrib["byteOrder"] = "mostSignificantByteFirst"
 
         if calibrator:
             self.add_calibrator(el, calibrator)
 
     def add_float_data_encoding(
         self,
         parent: ET.Element,
-        encoding: FloatDataEncoding,
+        encoding: FloatEncoding,
         calibrator: Calibrator | None,
     ):
         el = ET.SubElement(parent, "FloatDataEncoding")
         el.attrib["sizeInBits"] = str(encoding.bits)
 
-        if encoding.scheme == FloatDataEncodingScheme.IEEE754_1985:
+        if encoding.scheme == FloatEncodingScheme.IEEE754_1985:
             el.attrib["encoding"] = "IEEE754_1985"
-        elif encoding.scheme == FloatDataEncodingScheme.MILSTD_1750A:
+        elif encoding.scheme == FloatEncodingScheme.MILSTD_1750A:
             el.attrib["encoding"] = "MILSTD_1750A"
 
-        if encoding.byte_order == ByteOrder.BIG_ENDIAN:
-            el.attrib["byteOrder"] = "mostSignificantByteFirst"
-        elif encoding.byte_order == ByteOrder.LITTLE_ENDIAN:
+        if encoding.little_endian:
             el.attrib["byteOrder"] = "leastSignificantByteFirst"
+        else:
+            el.attrib["byteOrder"] = "mostSignificantByteFirst"
 
         if calibrator:
             self.add_calibrator(el, calibrator)
 
     def add_calibrator(self, parent: ET.Element, calibrator: Calibrator):
         el = ET.SubElement(parent, "DefaultCalibrator")
         if isinstance(calibrator, Polynomial):
@@ -1645,14 +1698,46 @@
         if not system.containers:
             return
 
         el = ET.SubElement(parent, "ContainerSet")
         for container in system.containers:
             self.add_sequence_container(el, container)
 
+    def add_custom_algorithm(
+        self, parent: ET.Element, system: System, algorithm: Algorithm
+    ):
+        el = ET.SubElement(parent, "CustomAlgorithm")
+        el.attrib["name"] = algorithm.name
+
+        if algorithm.short_description:
+            el.attrib["shortDescription"] = algorithm.short_description
+
+        if algorithm.long_description:
+            ET.SubElement(el, "LongDescription").text = algorithm.long_description
+
+        if algorithm.aliases:
+            self.add_aliases(el, algorithm.aliases)
+
+        extra = AncillaryData(algorithm.extra)
+
+        for input in algorithm.inputs:
+            if input.required and input.name:
+                extra.append("Yamcs:AlgorithmMandatoryInput", input.name)
+
+        if len(extra):
+            self.add_ancillary_data(el, extra)
+
+        text_el = ET.SubElement(el, "AlgorithmText")
+        text_el.attrib["language"] = algorithm.language
+        text_el.text = algorithm.text
+
+        self.add_inputs(el, system, algorithm.inputs)
+        self.add_outputs(el, system, algorithm.outputs)
+        self.add_triggers(el, system, algorithm.triggers)
+
     def add_sequence_container(self, parent: ET.Element, container: Container):
         el = ET.SubElement(parent, "SequenceContainer")
         el.attrib["name"] = container.name
         el.attrib["abstract"] = _to_xml_value(container.abstract)
 
         if container.short_description:
             el.attrib["shortDescription"] = container.short_description
@@ -1761,38 +1846,26 @@
         value: Any,
         operator: str,
         calibrated: bool,
     ):
         condition_el = ET.SubElement(parent, "Condition")
 
         pref_el = ET.SubElement(condition_el, "ParameterInstanceRef")
-        data_type: DataType | None
-        if isinstance(ref, Parameter):
-            data_type = ref
-            pref_el.attrib["parameterRef"] = self.make_ref(
-                ref.qualified_name,
-                start=system,
-            )
-        elif isinstance(ref, ParameterMember):
-            data_type = ref.path[-1]
-            parameter_ref = self.make_ref(
-                ref.parameter.qualified_name,
-                start=system,
-            )
-            for member in ref.path:
-                parameter_ref += "/" + member.name
-            pref_el.attrib["parameterRef"] = parameter_ref
-        else:  # str
-            data_type = None
-            pref_el.attrib["parameterRef"] = self.make_ref(ref, start=system)
+        pref_el.attrib["parameterRef"] = self.make_parameter_ref(ref, start=system)
         pref_el.attrib["useCalibratedValue"] = _to_xml_value(calibrated)
 
         ET.SubElement(condition_el, "ComparisonOperator").text = operator
         val_el = ET.SubElement(condition_el, "Value")
 
+        data_type: DataType | None = None
+        if isinstance(ref, Parameter):
+            data_type = ref
+        elif isinstance(ref, ParameterMember):
+            data_type = ref.path[-1]
+
         val_el.text = _to_xml_value(value)
         if isinstance(data_type, BooleanDataType) and isinstance(value, bool):
             if value:
                 val_el.text = data_type.one_string_value
             else:
                 val_el.text = data_type.zero_string_value
         elif isinstance(data_type, EnumeratedDataType) and isinstance(value, int):
@@ -1815,16 +1888,16 @@
     def add_parameter_ref_entry(
         self,
         parent: ET.Element,
         container: Container,
         entry: ParameterEntry,
     ):
         el = ET.SubElement(parent, "ParameterRefEntry")
-        el.attrib["parameterRef"] = self.make_ref(
-            entry.parameter.qualified_name,
+        el.attrib["parameterRef"] = self.make_parameter_ref(
+            entry.parameter,
             start=container.system,
         )
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
@@ -1848,16 +1921,16 @@
     def add_container_ref_entry(
         self,
         parent: ET.Element,
         container: Container,
         entry: ContainerEntry,
     ):
         el = ET.SubElement(parent, "ContainerRefEntry")
-        el.attrib["containerRef"] = self.make_ref(
-            entry.container.qualified_name,
+        el.attrib["containerRef"] = self.make_container_ref(
+            entry.container,
             start=container.system,
         )
         if entry.short_description:
             el.attrib["shortDescription"] = entry.short_description
 
         loc_el = ET.SubElement(el, "LocationInContainerInBits")
 
@@ -1875,47 +1948,73 @@
             self.add_expression_condition(
                 expr_el,
                 system=container.system,
                 expression=entry.condition,
             )
 
     def make_ref(self, target: str, start: System):
-        if os.path.commonprefix([target, start.qualified_name]) == "/":
-            return target  # abs path
+        if target.startswith("/"):
+            if os.path.commonprefix([target, start.qualified_name]) == "/":
+                return target  # abs path
+            else:
+                return os.path.relpath(target, start=start.qualified_name)
         else:
-            return os.path.relpath(target, start=start.qualified_name)
+            return target
+
+    def make_parameter_ref(
+        self, target: Parameter | ParameterMember | str, start: System
+    ):
+        if isinstance(target, Parameter):
+            return self.make_ref(target.qualified_name, start)
+        elif isinstance(target, ParameterMember):
+            parameter_ref = self.make_ref(target.parameter.qualified_name, start)
+            for member in target.path:
+                parameter_ref += "/" + member.name
+            return parameter_ref
+        elif isinstance(target, str):
+            return self.make_ref(target, start)
+        else:
+            raise ExportError("Unexpected parameter reference")
+
+    def make_container_ref(self, target: Container | str, start: System):
+        if isinstance(target, Container):
+            return self.make_ref(target.qualified_name, start)
+        elif isinstance(target, str):
+            return self.make_ref(target, start)
+        else:
+            raise ExportError("Unexpected container reference")
+
+    def make_command_ref(self, target: Command | str, start: System):
+        if isinstance(target, Command):
+            return self.make_ref(target.qualified_name, start)
+        elif isinstance(target, str):
+            return self.make_ref(target, start)
+        else:
+            raise ExportError("Unexpected command reference")
 
     def add_base_container(
         self,
         parent: ET.Element,
         base_container: Container | str,
         container: Container,
     ):
         el = ET.SubElement(parent, "BaseContainer")
 
-        if isinstance(base_container, Container):
-            el.attrib["containerRef"] = self.make_ref(
-                target=base_container.qualified_name,
-                start=container.system,
-            )
-        elif isinstance(base_container, str):
-            el.attrib["containerRef"] = self.make_ref(
-                target=base_container,
-                start=container.system,
-            )
-        else:
-            raise ExportError("Unexpected container parent")
+        el.attrib["containerRef"] = self.make_container_ref(
+            target=base_container,
+            start=container.system,
+        )
 
-        if container.restriction_criteria:
+        if container.condition:
             criteria_el = ET.SubElement(el, "RestrictionCriteria")
             expr_el = ET.SubElement(criteria_el, "BooleanExpression")
             self.add_expression_condition(
                 expr_el,
                 system=container.system,
-                expression=container.restriction_criteria,
+                expression=container.condition,
             )
 
     def add_space_systems(self, parent: ET.Element, system: System):
         for subsystem in system.subsystems:
             self.generate_space_system(subsystem, parent)
 
     def generate_space_system(
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/PKG-INFO` & `yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs-pymdb-1.0.4/src/yamcs_pymdb.egg-info/SOURCES.txt` & `yamcs-pymdb-1.0.5/src/yamcs_pymdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

