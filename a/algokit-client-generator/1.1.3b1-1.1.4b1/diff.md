# Comparing `tmp/algokit_client_generator-1.1.3b1-py3-none-any.whl.zip` & `tmp/algokit_client_generator-1.1.4b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18557 bytes, number of entries: 14
+Zip file size: 18542 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3208 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
--rw-r--r--  2.0 unx    37448 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
+-rw-r--r--  2.0 unx    37388 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
 -rw-r--r--  2.0 unx     4507 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.3b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.3b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.3b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.3b1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.1.3b1.dist-info/RECORD
-14 files, 63648 bytes uncompressed, 16341 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.1.4b1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.1.4b1.dist-info/RECORD
+14 files, 63588 bytes uncompressed, 16326 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-1.1.3b1.dist-info/LICENSE
+Filename: algokit_client_generator-1.1.4b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-1.1.3b1.dist-info/METADATA
+Filename: algokit_client_generator-1.1.4b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-1.1.3b1.dist-info/WHEEL
+Filename: algokit_client_generator-1.1.4b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-1.1.3b1.dist-info/entry_points.txt
+Filename: algokit_client_generator-1.1.4b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-1.1.3b1.dist-info/RECORD
+Filename: algokit_client_generator-1.1.4b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/generator.py

```diff
@@ -129,25 +129,24 @@
     yield Part.RestoreLineMode
 
 
 def helpers(context: GenerateContext) -> DocumentParts:
     has_abi_create = any(m.abi for m in context.methods.create)
     has_abi_update = any(m.abi for m in context.methods.update_application)
     has_abi_delete = any(m.abi for m in context.methods.delete_application)
-    if context.methods.has_abi_methods:
-        yield '_TReturn = typing.TypeVar("_TReturn")'
-        yield Part.Gap2
-        yield utils.indented(
-            """
+    yield '_TReturn = typing.TypeVar("_TReturn")'
+    yield Part.Gap2
+    yield utils.indented(
+        """
 class _ArgsBase(ABC, typing.Generic[_TReturn]):
     @staticmethod
     @abstractmethod
     def method() -> str:
         ..."""
-        )
+    )
     yield Part.Gap2
     yield '_TArgs = typing.TypeVar("_TArgs", bound=_ArgsBase[typing.Any])'
     yield Part.Gap2
     yield utils.indented(
         """
 @dataclasses.dataclass(kw_only=True)
 class _TArgsHolder(typing.Generic[_TArgs]):
```

## Comparing `algokit_client_generator-1.1.3b1.dist-info/LICENSE` & `algokit_client_generator-1.1.4b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-1.1.3b1.dist-info/METADATA` & `algokit_client_generator-1.1.4b1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 1.1.3b1
+Version: 1.1.4b1
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

