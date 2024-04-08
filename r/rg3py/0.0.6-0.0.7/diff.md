# Comparing `tmp/rg3py-0.0.6-py3-none-win_amd64.whl.zip` & `tmp/rg3py-0.0.7-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7949888 bytes, number of entries: 7
--rw-r--r--  2.0 unx      888 b- defN 24-Apr-07 18:00 rg3py/__init__.py
--rw-r--r--  2.0 unx 20610560 b- defN 24-Apr-07 18:00 rg3py/rg3py.pyd
--rw-r--r--  2.0 unx     8063 b- defN 24-Apr-07 18:00 rg3py/rg3py.pyi
--rw-r--r--  2.0 unx     4821 b- defN 24-Apr-07 18:00 rg3py-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-07 18:00 rg3py-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-07 18:00 rg3py-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 24-Apr-07 18:00 rg3py-0.0.6.dist-info/RECORD
-7 files, 20624946 bytes uncompressed, 7949000 bytes compressed:  61.5%
+Zip file size: 7957277 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      921 b- defN 24-Apr-08 18:35 rg3py/__init__.py
+-rw-r--r--  2.0 unx 20624384 b- defN 24-Apr-08 18:35 rg3py/rg3py.pyd
+-rw-r--r--  2.0 unx     8432 b- defN 24-Apr-08 18:35 rg3py/rg3py.pyi
+-rw-r--r--  2.0 unx     4821 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 24-Apr-08 18:35 rg3py-0.0.7.dist-info/RECORD
+7 files, 20639172 bytes uncompressed, 7956389 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: rg3py/rg3py.pyd
 Comment: 
 
 Filename: rg3py/rg3py.pyi
 Comment: 
 
-Filename: rg3py-0.0.6.dist-info/METADATA
+Filename: rg3py-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: rg3py-0.0.6.dist-info/WHEEL
+Filename: rg3py-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: rg3py-0.0.6.dist-info/top_level.txt
+Filename: rg3py-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: rg3py-0.0.6.dist-info/RECORD
+Filename: rg3py-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rg3py/__init__.py

```diff
@@ -20,8 +20,9 @@
 from .rg3py import ClassParent
 from .rg3py import CppClass
 from .rg3py import CodeAnalyzer
 from .rg3py import AnalyzerContext
 from .rg3py import CppCompilerIssueKind
 from .rg3py import CppCompilerIssue
 from .rg3py import CppTypeReference
-from .rg3py import ClangRuntime
+from .rg3py import ClangRuntime
+from .rg3py import TypeBaseInfo
```

## rg3py/rg3py.pyi

```diff
@@ -166,14 +166,17 @@
 
 
 class TypeStatement:
     @property
     def type_ref(self) -> CppTypeReference: ...
 
     @property
+    def type_info(self) -> TypeBaseInfo: ...
+
+    @property
     def location(self) -> Optional[Location]: ...
 
     @property
     def is_const(self) -> bool: ...
 
     @property
     def is_const_ptr(self) -> bool: ...
@@ -189,14 +192,31 @@
 
     @property
     def is_void(self) -> bool: ...
 
     def get_name(self) -> str: ...
 
 
+class TypeBaseInfo:
+    @property
+    def kind(self) -> CppTypeKind: ...
+
+    @property
+    def namespace(self) -> CppNamespace: ...
+
+    @property
+    def location(self) -> Location: ...
+
+    @property
+    def name(self) -> str: ...
+
+    @property
+    def pretty_name(self) -> str: ...
+
+
 class FunctionArgument:
     @property
     def type_info(self) -> TypeStatement: ...
 
     @property
     def name(self) -> str: ...
```

## Comparing `rg3py-0.0.6.dist-info/METADATA` & `rg3py-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rg3py
-Version: 0.0.6
+Version: 0.0.7
 Summary: RG3 is a C/C++ analyzer framework
 Author: DronCode
 Author-email: alexandrleutin@gmail.com
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

