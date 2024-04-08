# Comparing `tmp/tvb-gdist-2.2.tar.gz` & `tmp/tvb-gdist-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-gdist-2.2.tar", last modified: Thu Feb 23 14:38:18 2023, max compression
+gzip compressed data, was "tvb-gdist-2.2.1.tar", last modified: Mon Apr  8 08:21:08 2024, max compression
```

## Comparing `tvb-gdist-2.2.tar` & `tvb-gdist-2.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:38:18.068809 tvb-gdist-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-02-23 14:38:05.000000 tvb-gdist-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-23 14:38:05.000000 tvb-gdist-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-02-23 14:38:18.068809 tvb-gdist-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-02-23 14:38:05.000000 tvb-gdist-2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)   433933 2023-02-23 14:38:17.000000 tvb-gdist-2.2/gdist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14326 2023-02-23 14:38:05.000000 tvb-gdist-2.2/gdist.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:38:18.068809 tvb-gdist-2.2/geodesic_library/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/example0.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/example1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (123)    50409 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_exact.h
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_exact_elements.h
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_graph_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_algorithm_subdivision.h
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_constants_and_simple_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_memory.h
--rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_mesh.h
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_mesh_elements.h
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/geodesic_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-02-23 14:38:05.000000 tvb-gdist-2.2/geodesic_library/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-23 14:38:05.000000 tvb-gdist-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-23 14:38:18.068809 tvb-gdist-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-02-23 14:38:05.000000 tvb-gdist-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:38:18.068809 tvb-gdist-2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-02-23 14:38:05.000000 tvb-gdist-2.2/tests/test_gdist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 14:38:18.068809 tvb-gdist-2.2/tvb_gdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-02-23 14:38:17.000000 tvb-gdist-2.2/tvb_gdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-23 14:38:18.000000 tvb-gdist-2.2/tvb_gdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 14:38:17.000000 tvb-gdist-2.2/tvb_gdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 14:38:17.000000 tvb-gdist-2.2/tvb_gdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 14:38:17.000000 tvb-gdist-2.2/tvb_gdist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    37770 2024-04-08 08:21:01.000000 tvb-gdist-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 08:21:01.000000 tvb-gdist-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-08 08:21:01.000000 tvb-gdist-2.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   604267 2024-04-08 08:21:07.000000 tvb-gdist-2.2.1/gdist.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/gdist.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/geodesic_library/
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/example0.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/example1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (127)    50409 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_exact.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_exact_elements.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_graph_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_subdivision.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_constants_and_simple_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17163 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_mesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_mesh_elements.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/geodesic_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/geodesic_library/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-08 08:21:02.000000 tvb-gdist-2.2.1/tests/test_gdist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:21:08.067828 tvb-gdist-2.2.1/tvb_gdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-08 08:21:07.000000 tvb-gdist-2.2.1/tvb_gdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-08 08:21:08.000000 tvb-gdist-2.2.1/tvb_gdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:21:07.000000 tvb-gdist-2.2.1/tvb_gdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-08 08:21:07.000000 tvb-gdist-2.2.1/tvb_gdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 08:21:07.000000 tvb-gdist-2.2.1/tvb_gdist.egg-info/top_level.txt
```

### Comparing `tvb-gdist-2.2/LICENSE` & `tvb-gdist-2.2.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 TheVirtualBrain is a brain-simulation software. See also http://www.thevirtualbrain.org
 
-(c) 2012-2020, Baycrest Centre for Geriatric Care ("Baycrest") and others
+(c) 2012-2024, Baycrest Centre for Geriatric Care ("Baycrest") and others
 
 This program is free software: you can redistribute it and/or modify it under the terms
 of the GNU General Public License as published by the Free Software Foundation, either
 version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

### Comparing `tvb-gdist-2.2/PKG-INFO` & `tvb-gdist-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: tvb-gdist
-Version: 2.2
+Version: 2.2.1
 Summary: Compute geodesic distances
 Home-page: https://github.com/the-virtual-brain/tvb-gdist
 Author: Danil Kirsanov, Gaurav Malhotra and Stuart Knock
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL v3
 Keywords: gdist geodesic distance geo tvb
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: cython
 
 =================
 Geodesic Library 
 =================
 
 
 The **tvb-gdist** module is a Cython interface to a C++ library
```

### Comparing `tvb-gdist-2.2/README.rst` & `tvb-gdist-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/gdist.cpp` & `tvb-gdist-2.2.1/gdist.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NDEBUG",
                 1
             ]
         ],
         "depends": [
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "geodesic_library/geodesic_algorithm_exact.h",
             "geodesic_library/geodesic_constants_and_simple_functions.h",
             "geodesic_library/geodesic_mesh.h",
             "geodesic_library/geodesic_mesh_elements.h",
             "geodesic_library/geodesic_utils.h"
         ],
         "extra_compile_args": [
             "--std=c++1y"
         ],
         "extra_link_args": [
             "--std=c++1y"
         ],
         "include_dirs": [
-            "/tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/core/include",
             "geodesic_library"
         ],
         "language": "c++",
         "name": "gdist",
         "sources": [
             "gdist.pyx"
         ]
@@ -40,28 +40,45 @@
     "module_name": "gdist"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
+#else
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
+#define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define __PYX_EXTRA_ABI_MODULE_NAME ""
+#endif
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -72,31 +89,35 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#define __PYX_LIMITED_VERSION_HEX PY_VERSION_HEX
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -113,141 +134,253 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PYSTON_VERSION)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
   #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(CYTHON_LIMITED_API)
+  #ifdef Py_LIMITED_API
+    #undef __PYX_LIMITED_VERSION_HEX
+    #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
+  #endif
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
   #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
   #undef CYTHON_USE_PYLONG_INTERNALS
   #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
@@ -263,45 +396,70 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
+  #if PY_VERSION_HEX < 0x030700A3
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
   #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
@@ -323,78 +481,136 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
+#ifndef CYTHON_USE_CPP_STD_MOVE
+  #if defined(__cplusplus) && (\
+    __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600))
+    #define CYTHON_USE_CPP_STD_MOVE 1
+  #else
+    #define CYTHON_USE_CPP_STD_MOVE 0
+  #endif
+#endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
+        #else
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -410,158 +626,297 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+#if CYTHON_COMPILING_IN_LIMITED_API
+    static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
+        PyObject *exception_table = NULL;
+        PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
+        PyObject *py_minor_version = NULL;
+        #endif
+        long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
+        #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
+        minor_version = 11;
+        #else
+        if (!(version_info = PySys_GetObject("version_info"))) goto end;
+        if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
+        minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
+        if (minor_version == -1 && PyErr_Occurred()) goto end;
+        #endif
+        if (!(types_module = PyImport_ImportModule("types"))) goto end;
+        if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
+        if (minor_version <= 7) {
+            (void)p;
+            result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else if (minor_version <= 10) {
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else {
+            if (!(exception_table = PyBytes_FromStringAndSize(NULL, 0))) goto end;
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
+        }
+    end:
+        Py_XDECREF(code_type);
+        Py_XDECREF(exception_table);
+        Py_XDECREF(types_module);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
-        return co;
+        return result;
     }
+    #ifndef CO_OPTIMIZED
+    #define CO_OPTIMIZED 0x0001
+    #endif
+    #ifndef CO_NEWLOCALS
+    #define CO_NEWLOCALS 0x0002
+    #endif
+    #ifndef CO_VARARGS
+    #define CO_VARARGS 0x0004
+    #endif
+    #ifndef CO_VARKEYWORDS
+    #define CO_VARKEYWORDS 0x0008
+    #endif
+    #ifndef CO_ASYNC_GENERATOR
+    #define CO_ASYNC_GENERATOR 0x0200
+    #endif
+    #ifndef CO_GENERATOR
+    #define CO_GENERATOR 0x0020
+    #endif
+    #ifndef CO_COROUTINE
+    #define CO_COROUTINE 0x0080
+    #endif
+#elif PY_VERSION_HEX >= 0x030B0000
+  static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+    PyCodeObject *result;
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
+    if (!empty_bytes) return NULL;
+    result =
+      #if PY_VERSION_HEX >= 0x030C0000
+        PyUnstable_Code_NewWithPosOnlyArgs
+      #else
+        PyCode_NewWithPosOnlyArgs
+      #endif
+        (a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, name, fline, lnos, empty_bytes);
+    Py_DECREF(empty_bytes);
+    return result;
+  }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
+#endif
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
+#if __PYX_LIMITED_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
+#else
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -584,46 +939,125 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
+#else
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_READY(op)       (0)
   #else
     #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                                 0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -633,37 +1067,43 @@
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -684,45 +1124,81 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_ITEM(o, i)
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) (PyTuple_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyList_SET_ITEM(o, i, v) (PyList_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_GET_SIZE(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_GET_SIZE(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_GET_SIZE(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_GET_SIZE(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_GET_SIZE(o)
 #else
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_GetItem(o, i)
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) PyTuple_SetItem(o, i, v)
+  #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
+#endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
@@ -732,19 +1208,14 @@
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
   #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
-#endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
   #endif
@@ -777,39 +1248,44 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE__gdist
 #define __PYX_HAVE_API__gdist
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
+
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
+    
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
-
-    /* NumPy API declarations from "numpy/__init__.pxd" */
-    
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include "geodesic_mesh_elements.h"
 #include "geodesic_mesh.h"
@@ -860,17 +1336,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -880,31 +1357,25 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -920,16 +1391,62 @@
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -942,15 +1459,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -972,14 +1489,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1007,31 +1525,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1041,23 +1555,29 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "gdist.pyx",
-  "__init__.pxd",
-  "stringsource",
+  "<stringsource>",
+  "__init__.cython-30.pxd",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* ForceInitThreads.proto */
+#ifndef __PYX_FORCE_INIT_THREADS
+  #define __PYX_FORCE_INIT_THREADS 0
+#endif
+
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -1084,340 +1604,463 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+struct __pyx_defaults;
+typedef struct __pyx_defaults __pyx_defaults;
+struct __pyx_defaults1;
+typedef struct __pyx_defaults1 __pyx_defaults1;
+struct __pyx_defaults2;
+typedef struct __pyx_defaults2 __pyx_defaults2;
+struct __pyx_defaults {
+  double __pyx_arg_max_distance;
+};
+struct __pyx_defaults1 {
+  double __pyx_arg_max_distance;
+};
+struct __pyx_defaults2 {
+  double __pyx_arg_max_distance;
+};
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
 static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
@@ -1433,123 +2076,136 @@
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
-  static size_t __pyx_pyframe_localsplus_offset = 0;
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallNoArg.proto */
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* TupleAndListFromArray.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
+/* IncludeStringH.proto */
+#include <string.h>
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
-#endif
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
+/* fastcall.proto */
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_VARARGS(args, i) PySequence_GetItem(args, i)
+#elif CYTHON_ASSUME_SAFE_MACROS
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#else
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
+#else
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
+#endif
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg) __Pyx_Arg_XDECREF_VARARGS(arg)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
@@ -1598,25 +2254,34 @@
 
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+/* MoveIfSupported.proto */
+#if CYTHON_USE_CPP_STD_MOVE
+  #include <utility>
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
+#else
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
+#endif
 
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
@@ -1648,108 +2313,223 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
+static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
+};
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
+
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
-/* ListCompAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len)) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
-/* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
-};
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
-#endif
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+/* PyMethodNew.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    typesModule = PyImport_ImportModule("types");
+    if (!typesModule) return NULL;
+    methodType = PyObject_GetAttrString(typesModule, "MethodType");
+    Py_DECREF(typesModule);
+    if (!methodType) return NULL;
+    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
+    Py_DECREF(methodType);
+    return result;
+}
+#elif PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject_HEAD
+    PyObject *func;
+#elif PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1813,15 +2593,15 @@
   {
     PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
   }
 }
 #endif
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
@@ -1840,15 +2620,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1878,15 +2658,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1922,116 +2702,124 @@
 /* CIntFromPy.proto */
 static CYTHON_INLINE npy_int32 __Pyx_PyInt_As_npy_int32(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE unsigned int __Pyx_PyInt_As_unsigned_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cpython.buffer' */
-
-/* Module declarations from 'libc.string' */
-
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'libcpp' */
+/* Module declarations from "libcpp" */
 
-/* Module declarations from 'libcpp.vector' */
+/* Module declarations from "libcpp.vector" */
 
-/* Module declarations from 'gdist' */
+/* Module declarations from "gdist" */
 static PyObject *__pyx_f_5gdist_get_mesh(PyArrayObject *, PyArrayObject *, geodesic::Mesh &, bool); /*proto*/
 static std::vector<unsigned int>  __pyx_convert_vector_from_py_unsigned_int(PyObject *); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_unsigned_int(const std::vector<unsigned int>  &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_double(std::vector<double>  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_unsigned_int(std::vector<unsigned int>  const &); /*proto*/
+/* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, __PYX_IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', __PYX_IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "gdist"
 extern int __pyx_module_is_main_gdist;
 int __pyx_module_is_main_gdist = 0;
 
-/* Implementation of 'gdist' */
+/* Implementation of "gdist" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_enumerate;
+static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_N[] = "N";
 static const char __pyx_k_k[] = "k";
+static const char __pyx_k__4[] = "*";
 static const char __pyx_k_kk[] = "kk";
+static const char __pyx_k__12[] = "?";
 static const char __pyx_k_inf[] = "inf";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_rows[] = "rows";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_amesh[] = "amesh";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_faces[] = "faces";
 static const char __pyx_k_gdist[] = "gdist";
 static const char __pyx_k_int32[] = "int32";
@@ -2054,117 +2842,2288 @@
 static const char __pyx_k_algorithm[] = "algorithm";
 static const char __pyx_k_distances[] = "distances";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_gdist_pyx[] = "gdist.pyx";
 static const char __pyx_k_triangles[] = "triangles";
 static const char __pyx_k_csc_matrix[] = "csc_matrix";
 static const char __pyx_k_ImportError[] = "ImportError";
+static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_index_point[] = "index_point";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_max_distance[] = "max_distance";
 static const char __pyx_k_scipy_sparse[] = "scipy.sparse";
 static const char __pyx_k_source_index[] = "source_index";
+static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_compute_gdist[] = "compute_gdist";
 static const char __pyx_k_index_distance[] = "index_distance";
 static const char __pyx_k_is_one_indexed[] = "is_one_indexed";
 static const char __pyx_k_no_of_vertices[] = "no_of_vertices";
 static const char __pyx_k_source_indices[] = "source_indices";
 static const char __pyx_k_target_indices[] = "target_indices";
 static const char __pyx_k_distance_matrix[] = "distance_matrix";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_local_gdist_matrix[] = "local_gdist_matrix";
 static const char __pyx_k_compute_gdist_line_119[] = "compute_gdist (line 119)";
 static const char __pyx_k_propagate_on_max_distance[] = "propagate_on_max_distance";
 static const char __pyx_k_local_gdist_matrix_line_198[] = "local_gdist_matrix (line 198)";
 static const char __pyx_k_This_module_defines_a_Cython_wr[] = "\nThis module defines a Cython wrapper for the geodesic distance C++ library.\nThe algorithm (implemented in C++) extends Mitchell, Mount and Papadimitriou\n(1987) and was written by Danil Kirsanov\n(http://code.google.com/archive/p/geodesic/).\n\nThe interface definitions and wrapper functions are written in Cython syntax\n(http://cython.org/) and provide an API for some of the classes, functions and\nconstants useful for calculating the geodesic distance.\n\nTo compile, and build gdist.so using Cython::\n\n    python setup.py build_ext --inplace\n\n.. moduleauthor:: Gaurav Malhotra <Gaurav@tvb.invalid>\n.. moduleauthor:: Stuart A. Knock <Stuart@tvb.invalid>\n\n";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Function_for_calculating_pairwis[] = "Function for calculating pairwise geodesic distance for a set of points\n    within a distance ``max_distance`` of them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        points (numpy.ndarray[numpy.int32_t, ndim=1]): Indices of the points\n            among which the pairwise distances are to be calculated.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n            is the number of vertices, specifying the pairwise distances among\n            the given points.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> points = numpy.array([2, 5, 10], dtype=numpy.int32)\n        >>> import gdist\n        >>> gdist.distance_matrix_of_selected_points(\n                vertices, triangles, points\n            )\n         <121x121 sparse matrix of type '<class 'numpy.float64'>'\n            with 6 stored elements in Compressed Sparse Column format>\n    ";
 static const char __pyx_k_This_is_the_wrapper_function_for[] = "This is the wrapper function for computing geodesic distance between a\n    set of sources and targets on a mesh surface.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        source_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            source on the mesh.\n        target_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            targets on the mesh.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        numpy.ndarray((len(target_indices), ), dtype=numpy.float64): Specifying\n            the shortest distance to the target vertices from the nearest source\n            vertex on the mesh. If no target_indices are provided, all vertices\n            of the mesh are considered as targets, however, in this case,\n            specifying max_distance will limit the targets to those vertices\n            within max_distance of a source. If no source_indices are provided,\n            it defaults to 0.\n\n    NOTE: This is the function to use when specifying localised stimuli and\n    parameter variations. For efficiently using the whole mesh as sources, such\n    as is required to represent local connectivity within the cortex, see the\n    local_gdist_matrix() function.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> src = numpy.array([1], dtype=numpy.int32)\n        >>> trg = numpy.array([2], dtype=""numpy.int32)\n        >>> import gdist\n        >>> gdist.compute_gdist(vertices, triangles, source_indices=src, target_indices=trg)\n         array([0.2])\n    ";
 static const char __pyx_k_distance_matrix_of_selected_poin[] = "distance_matrix_of_selected_points";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_This_is_the_wrapper_function_for_2[] = "This is the wrapper function for computing geodesic distance from every\n    vertex on the surface to all those within a distance ``max_distance`` of\n    them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n        is the number of vertices, specifying the shortest distance from all\n        vertices to all the vertices within max_distance.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> import gdist\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> gdist.local_gdist_matrix(vertices, triangles, max_distance=1.0)\n         <121x121 sparse matrix of type '<type 'numpy.float64'>'\n             with 6232 stored elements in Compressed Sparse Column format>\n\n    Runtime and guesstimated memory usage as a function of max_distance for the\n    reg_13 cortical surface mesh, ie containing 2**13 vertices per hemisphere.\n    ::\n        [[10, 20, 30, 40,  50,  60,  70,  80,  90, 100], # mm\n         [19, 28, 49, 81, 125, 181, 248, 331, 422, 522], # s\n         [ 3, 13, 30, 56,  89, 129, 177, 232, 292, 358]] # MB]\n\n    where memory is a min-guestimate given by: mem_req = nnz * 8 / 1024 / 1024.\n    ";
 static const char __pyx_k_distance_matrix_of_selected_poin_2[] = "distance_matrix_of_selected_points (line 287)";
-static PyObject *__pyx_kp_u_Function_for_calculating_pairwis;
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_N;
-static PyObject *__pyx_kp_u_This_is_the_wrapper_function_for;
-static PyObject *__pyx_kp_u_This_is_the_wrapper_function_for_2;
-static PyObject *__pyx_n_s_algorithm;
-static PyObject *__pyx_n_s_amesh;
-static PyObject *__pyx_n_s_arange;
-static PyObject *__pyx_n_s_array;
-static PyObject *__pyx_n_s_asarray;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_columns;
-static PyObject *__pyx_n_s_compute_gdist;
-static PyObject *__pyx_kp_u_compute_gdist_line_119;
-static PyObject *__pyx_n_s_csc_matrix;
-static PyObject *__pyx_n_s_data;
-static PyObject *__pyx_n_s_distance;
-static PyObject *__pyx_n_s_distance_matrix;
-static PyObject *__pyx_n_s_distance_matrix_of_selected_poin;
-static PyObject *__pyx_kp_u_distance_matrix_of_selected_poin_2;
-static PyObject *__pyx_n_s_distances;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_enumerate;
-static PyObject *__pyx_n_s_faces;
-static PyObject *__pyx_n_s_flatten;
-static PyObject *__pyx_n_s_gdist;
-static PyObject *__pyx_kp_s_gdist_pyx;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_index_distance;
-static PyObject *__pyx_n_s_index_point;
-static PyObject *__pyx_n_s_inf;
-static PyObject *__pyx_n_s_int32;
-static PyObject *__pyx_n_s_is_one_indexed;
-static PyObject *__pyx_n_s_k;
-static PyObject *__pyx_n_s_kk;
-static PyObject *__pyx_n_s_local_gdist_matrix;
-static PyObject *__pyx_kp_u_local_gdist_matrix_line_198;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_max_distance;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_no_of_vertices;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_point;
-static PyObject *__pyx_n_s_points;
-static PyObject *__pyx_n_s_propagate_on_max_distance;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_s_rows;
-static PyObject *__pyx_n_s_scipy;
-static PyObject *__pyx_n_s_scipy_sparse;
-static PyObject *__pyx_n_s_shape;
-static PyObject *__pyx_n_s_source;
-static PyObject *__pyx_n_s_source_index;
-static PyObject *__pyx_n_s_source_indices;
-static PyObject *__pyx_n_s_sparse;
-static PyObject *__pyx_n_s_target_indices;
-static PyObject *__pyx_n_s_targets;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_triangles;
-static PyObject *__pyx_n_s_vertices;
+/* #### Code section: decls ### */
+static PyObject *__pyx_pf_5gdist_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_5gdist_compute_gdist(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, PyArrayObject *__pyx_v_source_indices, PyArrayObject *__pyx_v_target_indices, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed); /* proto */
+static PyObject *__pyx_pf_5gdist_8__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_5gdist_2local_gdist_matrix(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed); /* proto */
+static PyObject *__pyx_pf_5gdist_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_5gdist_4distance_matrix_of_selected_points(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, PyArrayObject *__pyx_v_points, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed); /* proto */
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_int_1;
-static double __pyx_k_;
-static double __pyx_k__3;
-static double __pyx_k__4;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_tuple__11;
-static PyObject *__pyx_codeobj__8;
-static PyObject *__pyx_codeobj__10;
-static PyObject *__pyx_codeobj__12;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_kp_u_Function_for_calculating_pairwis;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s_MemoryError;
+  PyObject *__pyx_n_s_N;
+  PyObject *__pyx_kp_u_This_is_the_wrapper_function_for;
+  PyObject *__pyx_kp_u_This_is_the_wrapper_function_for_2;
+  PyObject *__pyx_n_s__12;
+  PyObject *__pyx_n_s__4;
+  PyObject *__pyx_n_s_algorithm;
+  PyObject *__pyx_n_s_amesh;
+  PyObject *__pyx_n_s_arange;
+  PyObject *__pyx_n_s_array;
+  PyObject *__pyx_n_s_asarray;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_class_getitem;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_columns;
+  PyObject *__pyx_n_s_compute_gdist;
+  PyObject *__pyx_kp_u_compute_gdist_line_119;
+  PyObject *__pyx_n_s_csc_matrix;
+  PyObject *__pyx_n_s_data;
+  PyObject *__pyx_n_s_distance;
+  PyObject *__pyx_n_s_distance_matrix;
+  PyObject *__pyx_n_s_distance_matrix_of_selected_poin;
+  PyObject *__pyx_kp_u_distance_matrix_of_selected_poin_2;
+  PyObject *__pyx_n_s_distances;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_enumerate;
+  PyObject *__pyx_n_s_faces;
+  PyObject *__pyx_n_s_flatten;
+  PyObject *__pyx_n_s_gdist;
+  PyObject *__pyx_kp_s_gdist_pyx;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_index_distance;
+  PyObject *__pyx_n_s_index_point;
+  PyObject *__pyx_n_s_inf;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_int32;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_n_s_is_one_indexed;
+  PyObject *__pyx_n_s_k;
+  PyObject *__pyx_n_s_kk;
+  PyObject *__pyx_n_s_local_gdist_matrix;
+  PyObject *__pyx_kp_u_local_gdist_matrix_line_198;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_max_distance;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_no_of_vertices;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_point;
+  PyObject *__pyx_n_s_points;
+  PyObject *__pyx_n_s_propagate_on_max_distance;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_rows;
+  PyObject *__pyx_n_s_scipy;
+  PyObject *__pyx_n_s_scipy_sparse;
+  PyObject *__pyx_n_s_shape;
+  PyObject *__pyx_n_s_source;
+  PyObject *__pyx_n_s_source_index;
+  PyObject *__pyx_n_s_source_indices;
+  PyObject *__pyx_n_s_sparse;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_target_indices;
+  PyObject *__pyx_n_s_targets;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_triangles;
+  PyObject *__pyx_n_s_vertices;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_int_1;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__9;
+  PyObject *__pyx_codeobj__11;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Function_for_calculating_pairwis);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_N);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_This_is_the_wrapper_function_for);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_This_is_the_wrapper_function_for_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__4);
+  Py_CLEAR(clear_module_state->__pyx_n_s_algorithm);
+  Py_CLEAR(clear_module_state->__pyx_n_s_amesh);
+  Py_CLEAR(clear_module_state->__pyx_n_s_arange);
+  Py_CLEAR(clear_module_state->__pyx_n_s_array);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asarray);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_columns);
+  Py_CLEAR(clear_module_state->__pyx_n_s_compute_gdist);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_compute_gdist_line_119);
+  Py_CLEAR(clear_module_state->__pyx_n_s_csc_matrix);
+  Py_CLEAR(clear_module_state->__pyx_n_s_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_distance_matrix);
+  Py_CLEAR(clear_module_state->__pyx_n_s_distance_matrix_of_selected_poin);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_distance_matrix_of_selected_poin_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_distances);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_enumerate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_faces);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flatten);
+  Py_CLEAR(clear_module_state->__pyx_n_s_gdist);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_gdist_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_index_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_index_point);
+  Py_CLEAR(clear_module_state->__pyx_n_s_inf);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_one_indexed);
+  Py_CLEAR(clear_module_state->__pyx_n_s_k);
+  Py_CLEAR(clear_module_state->__pyx_n_s_kk);
+  Py_CLEAR(clear_module_state->__pyx_n_s_local_gdist_matrix);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_local_gdist_matrix_line_198);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_max_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_no_of_vertices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_point);
+  Py_CLEAR(clear_module_state->__pyx_n_s_points);
+  Py_CLEAR(clear_module_state->__pyx_n_s_propagate_on_max_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rows);
+  Py_CLEAR(clear_module_state->__pyx_n_s_scipy);
+  Py_CLEAR(clear_module_state->__pyx_n_s_scipy_sparse);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shape);
+  Py_CLEAR(clear_module_state->__pyx_n_s_source);
+  Py_CLEAR(clear_module_state->__pyx_n_s_source_index);
+  Py_CLEAR(clear_module_state->__pyx_n_s_source_indices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sparse);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_target_indices);
+  Py_CLEAR(clear_module_state->__pyx_n_s_targets);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_triangles);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vertices);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Function_for_calculating_pairwis);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_N);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_This_is_the_wrapper_function_for);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_This_is_the_wrapper_function_for_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__4);
+  Py_VISIT(traverse_module_state->__pyx_n_s_algorithm);
+  Py_VISIT(traverse_module_state->__pyx_n_s_amesh);
+  Py_VISIT(traverse_module_state->__pyx_n_s_arange);
+  Py_VISIT(traverse_module_state->__pyx_n_s_array);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asarray);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_columns);
+  Py_VISIT(traverse_module_state->__pyx_n_s_compute_gdist);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_compute_gdist_line_119);
+  Py_VISIT(traverse_module_state->__pyx_n_s_csc_matrix);
+  Py_VISIT(traverse_module_state->__pyx_n_s_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_distance_matrix);
+  Py_VISIT(traverse_module_state->__pyx_n_s_distance_matrix_of_selected_poin);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_distance_matrix_of_selected_poin_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_distances);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_enumerate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_faces);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flatten);
+  Py_VISIT(traverse_module_state->__pyx_n_s_gdist);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_gdist_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_index_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_index_point);
+  Py_VISIT(traverse_module_state->__pyx_n_s_inf);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_one_indexed);
+  Py_VISIT(traverse_module_state->__pyx_n_s_k);
+  Py_VISIT(traverse_module_state->__pyx_n_s_kk);
+  Py_VISIT(traverse_module_state->__pyx_n_s_local_gdist_matrix);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_local_gdist_matrix_line_198);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_max_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_no_of_vertices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_point);
+  Py_VISIT(traverse_module_state->__pyx_n_s_points);
+  Py_VISIT(traverse_module_state->__pyx_n_s_propagate_on_max_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rows);
+  Py_VISIT(traverse_module_state->__pyx_n_s_scipy);
+  Py_VISIT(traverse_module_state->__pyx_n_s_scipy_sparse);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shape);
+  Py_VISIT(traverse_module_state->__pyx_n_s_source);
+  Py_VISIT(traverse_module_state->__pyx_n_s_source_index);
+  Py_VISIT(traverse_module_state->__pyx_n_s_source_indices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sparse);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_target_indices);
+  Py_VISIT(traverse_module_state->__pyx_n_s_targets);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_triangles);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vertices);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_kp_u_Function_for_calculating_pairwis __pyx_mstate_global->__pyx_kp_u_Function_for_calculating_pairwis
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
+#define __pyx_n_s_N __pyx_mstate_global->__pyx_n_s_N
+#define __pyx_kp_u_This_is_the_wrapper_function_for __pyx_mstate_global->__pyx_kp_u_This_is_the_wrapper_function_for
+#define __pyx_kp_u_This_is_the_wrapper_function_for_2 __pyx_mstate_global->__pyx_kp_u_This_is_the_wrapper_function_for_2
+#define __pyx_n_s__12 __pyx_mstate_global->__pyx_n_s__12
+#define __pyx_n_s__4 __pyx_mstate_global->__pyx_n_s__4
+#define __pyx_n_s_algorithm __pyx_mstate_global->__pyx_n_s_algorithm
+#define __pyx_n_s_amesh __pyx_mstate_global->__pyx_n_s_amesh
+#define __pyx_n_s_arange __pyx_mstate_global->__pyx_n_s_arange
+#define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
+#define __pyx_n_s_asarray __pyx_mstate_global->__pyx_n_s_asarray
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_columns __pyx_mstate_global->__pyx_n_s_columns
+#define __pyx_n_s_compute_gdist __pyx_mstate_global->__pyx_n_s_compute_gdist
+#define __pyx_kp_u_compute_gdist_line_119 __pyx_mstate_global->__pyx_kp_u_compute_gdist_line_119
+#define __pyx_n_s_csc_matrix __pyx_mstate_global->__pyx_n_s_csc_matrix
+#define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
+#define __pyx_n_s_distance __pyx_mstate_global->__pyx_n_s_distance
+#define __pyx_n_s_distance_matrix __pyx_mstate_global->__pyx_n_s_distance_matrix
+#define __pyx_n_s_distance_matrix_of_selected_poin __pyx_mstate_global->__pyx_n_s_distance_matrix_of_selected_poin
+#define __pyx_kp_u_distance_matrix_of_selected_poin_2 __pyx_mstate_global->__pyx_kp_u_distance_matrix_of_selected_poin_2
+#define __pyx_n_s_distances __pyx_mstate_global->__pyx_n_s_distances
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_enumerate __pyx_mstate_global->__pyx_n_s_enumerate
+#define __pyx_n_s_faces __pyx_mstate_global->__pyx_n_s_faces
+#define __pyx_n_s_flatten __pyx_mstate_global->__pyx_n_s_flatten
+#define __pyx_n_s_gdist __pyx_mstate_global->__pyx_n_s_gdist
+#define __pyx_kp_s_gdist_pyx __pyx_mstate_global->__pyx_kp_s_gdist_pyx
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_index_distance __pyx_mstate_global->__pyx_n_s_index_distance
+#define __pyx_n_s_index_point __pyx_mstate_global->__pyx_n_s_index_point
+#define __pyx_n_s_inf __pyx_mstate_global->__pyx_n_s_inf
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_int32 __pyx_mstate_global->__pyx_n_s_int32
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_n_s_is_one_indexed __pyx_mstate_global->__pyx_n_s_is_one_indexed
+#define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
+#define __pyx_n_s_kk __pyx_mstate_global->__pyx_n_s_kk
+#define __pyx_n_s_local_gdist_matrix __pyx_mstate_global->__pyx_n_s_local_gdist_matrix
+#define __pyx_kp_u_local_gdist_matrix_line_198 __pyx_mstate_global->__pyx_kp_u_local_gdist_matrix_line_198
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_max_distance __pyx_mstate_global->__pyx_n_s_max_distance
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_no_of_vertices __pyx_mstate_global->__pyx_n_s_no_of_vertices
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
+#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_point __pyx_mstate_global->__pyx_n_s_point
+#define __pyx_n_s_points __pyx_mstate_global->__pyx_n_s_points
+#define __pyx_n_s_propagate_on_max_distance __pyx_mstate_global->__pyx_n_s_propagate_on_max_distance
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_rows __pyx_mstate_global->__pyx_n_s_rows
+#define __pyx_n_s_scipy __pyx_mstate_global->__pyx_n_s_scipy
+#define __pyx_n_s_scipy_sparse __pyx_mstate_global->__pyx_n_s_scipy_sparse
+#define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
+#define __pyx_n_s_source __pyx_mstate_global->__pyx_n_s_source
+#define __pyx_n_s_source_index __pyx_mstate_global->__pyx_n_s_source_index
+#define __pyx_n_s_source_indices __pyx_mstate_global->__pyx_n_s_source_indices
+#define __pyx_n_s_sparse __pyx_mstate_global->__pyx_n_s_sparse
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_target_indices __pyx_mstate_global->__pyx_n_s_target_indices
+#define __pyx_n_s_targets __pyx_mstate_global->__pyx_n_s_targets
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_triangles __pyx_mstate_global->__pyx_n_s_triangles
+#define __pyx_n_s_vertices __pyx_mstate_global->__pyx_n_s_vertices
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
+#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+/* #### Code section: module_code ### */
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_unsigned_int")
+ * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<unsigned int>  __pyx_convert_vector_from_py_unsigned_int(PyObject *__pyx_v_o) {
+  std::vector<unsigned int>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<unsigned int>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  unsigned int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_unsigned_int", 1);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_v_item); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((unsigned int)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_unsigned_int")
+ * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_unsigned_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+static PyObject *__pyx_convert_vector_to_py_double(std::vector<double>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_double", 1);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_convert_vector_to_py_unsigned_int(std::vector<unsigned int>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_unsigned_int", 1);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_unsigned_int")
+ * cdef object __pyx_convert_vector_to_py_unsigned_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_unsigned_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_unsigned_int")
+ * cdef object __pyx_convert_vector_to_py_unsigned_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __Pyx_PyInt_From_unsigned_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_unsigned_int")
+ * cdef object __pyx_convert_vector_to_py_unsigned_int(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_unsigned_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
+ * 
+ *     ctypedef unsigned char      npy_bool
+ */
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):
+ *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ */
+  Py_INCREF(__pyx_v_base);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ */
+  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+  /* function exit code */
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("get_array_base", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
+ *         return None
+ */
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = (__pyx_v_base == NULL);
+  if (__pyx_t_1) {
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ *         return None             # <<<<<<<<<<<<<<
+ *     return <object>base
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+ *     if base is NULL:
+ *         return None
+ *     return <object>base             # <<<<<<<<<<<<<<
+ * 
+ * # Versions of the import_* functions which are more suitable for
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_array", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+ * cdef inline int import_array() except -1:
+ *     try:
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ */
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+ *     try:
+ *         __pyx_import_array()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 987, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_umath", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+ * cdef inline int import_umath() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 993, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+ * cdef inline int import_ufunc() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 999, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
 /* "gdist.pyx":96
  * 
  * 
  * cdef get_mesh(             # <<<<<<<<<<<<<<
  *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
  *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
@@ -2180,22 +5139,23 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_vertices;
   __Pyx_Buffer __pyx_pybuffer_vertices;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject *(*__pyx_t_5)(PyObject *);
-  __pyx_t_5numpy_float64_t __pyx_t_6;
-  __pyx_t_5numpy_int32_t __pyx_t_7;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *(*__pyx_t_6)(PyObject *);
+  __pyx_t_5numpy_float64_t __pyx_t_7;
+  __pyx_t_5numpy_int32_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_mesh", 0);
+  __Pyx_RefNannySetupContext("get_mesh", 1);
   __pyx_pybuffer_vertices.pybuffer.buf = NULL;
   __pyx_pybuffer_vertices.refcount = 0;
   __pyx_pybuffernd_vertices.data = NULL;
   __pyx_pybuffernd_vertices.rcbuffer = &__pyx_pybuffer_vertices;
   __pyx_pybuffer_triangles.pybuffer.buf = NULL;
   __pyx_pybuffer_triangles.refcount = 0;
   __pyx_pybuffernd_triangles.data = NULL;
@@ -2217,71 +5177,91 @@
  *     for coord in vertices.flatten():             # <<<<<<<<<<<<<<
  *         points.push_back(coord)
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_vertices), __pyx_n_s_flatten); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
-    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
-    __pyx_t_5 = NULL;
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 108, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
-    if (likely(!__pyx_t_5)) {
+    if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
-        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 108, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
-      __pyx_t_1 = __pyx_t_5(__pyx_t_2);
+      __pyx_t_1 = __pyx_t_6(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
           else __PYX_ERR(0, 108, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
-    __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+    __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_7 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_coord = __pyx_t_6;
+    __pyx_v_coord = __pyx_t_7;
 
     /* "gdist.pyx":109
  *     cdef numpy.float64_t coord
  *     for coord in vertices.flatten():
  *         points.push_back(coord)             # <<<<<<<<<<<<<<
  * 
  *     # Map numpy array of mesh "triangles" to C++ vector of mesh "faces"
@@ -2309,71 +5289,91 @@
  *     for indx in triangles.flatten():             # <<<<<<<<<<<<<<
  *         faces.push_back(indx)
  * 
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_triangles), __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  }
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-    __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
-    __pyx_t_5 = NULL;
+    __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 113, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
-    if (likely(!__pyx_t_5)) {
+    if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
-        if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
-      __pyx_t_2 = __pyx_t_5(__pyx_t_1);
+      __pyx_t_2 = __pyx_t_6(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
           else __PYX_ERR(0, 113, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
-    __pyx_t_7 = __Pyx_PyInt_As_npy_int32(__pyx_t_2); if (unlikely((__pyx_t_7 == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_npy_int32(__pyx_t_2); if (unlikely((__pyx_t_8 == ((npy_int32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_v_indx = __pyx_t_7;
+    __pyx_v_indx = __pyx_t_8;
 
     /* "gdist.pyx":114
  *     cdef numpy.int32_t indx
  *     for indx in triangles.flatten():
  *         faces.push_back(indx)             # <<<<<<<<<<<<<<
  * 
  *     amesh.initialize_mesh_data(points, faces, is_one_indexed)
@@ -2442,153 +5442,268 @@
  * 
  * 
  * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
  */
 
+static PyObject *__pyx_pf_5gdist_6__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 1);
+  __Pyx_XDECREF(__pyx_r);
+
+  /* "gdist.pyx":122
+ *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
+ *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,             # <<<<<<<<<<<<<<
+ *                   double max_distance=GEODESIC_INF,
+ *                   bool is_one_indexed=False):
+ */
+  __pyx_t_1 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_max_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  /* "gdist.pyx":124
+ *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,
+ *                   double max_distance=GEODESIC_INF,
+ *                   bool is_one_indexed=False):             # <<<<<<<<<<<<<<
+ *     """This is the wrapper function for computing geodesic distance between a
+ *     set of sources and targets on a mesh surface.
+ */
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "gdist.pyx":119
+ * 
+ * 
+ * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
+ *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
+ */
+  __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, Py_None)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None)) __PYX_ERR(0, 119, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("gdist.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* Python wrapper */
-static PyObject *__pyx_pw_5gdist_1compute_gdist(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5gdist_compute_gdist[] = "This is the wrapper function for computing geodesic distance between a\n    set of sources and targets on a mesh surface.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        source_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            source on the mesh.\n        target_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            targets on the mesh.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        numpy.ndarray((len(target_indices), ), dtype=numpy.float64): Specifying\n            the shortest distance to the target vertices from the nearest source\n            vertex on the mesh. If no target_indices are provided, all vertices\n            of the mesh are considered as targets, however, in this case,\n            specifying max_distance will limit the targets to those vertices\n            within max_distance of a source. If no source_indices are provided,\n            it defaults to 0.\n\n    NOTE: This is the function to use when specifying localised stimuli and\n    parameter variations. For efficiently using the whole mesh as sources, such\n    as is required to represent local connectivity within the cortex, see the\n    local_gdist_matrix() function.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> src = numpy.array([1], dtype=numpy.int32)\n        >>> trg = numpy.array([2], dtype=""numpy.int32)\n        >>> import gdist\n        >>> gdist.compute_gdist(vertices, triangles, source_indices=src, target_indices=trg)\n         array([0.2])\n    ";
-static PyMethodDef __pyx_mdef_5gdist_1compute_gdist = {"compute_gdist", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5gdist_1compute_gdist, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5gdist_compute_gdist};
-static PyObject *__pyx_pw_5gdist_1compute_gdist(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5gdist_1compute_gdist(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_5gdist_compute_gdist, "This is the wrapper function for computing geodesic distance between a\n    set of sources and targets on a mesh surface.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        source_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            source on the mesh.\n        target_indices (numpy.ndarray[numpy.int32_t, ndim=1]): Index of the\n            targets on the mesh.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        numpy.ndarray((len(target_indices), ), dtype=numpy.float64): Specifying\n            the shortest distance to the target vertices from the nearest source\n            vertex on the mesh. If no target_indices are provided, all vertices\n            of the mesh are considered as targets, however, in this case,\n            specifying max_distance will limit the targets to those vertices\n            within max_distance of a source. If no source_indices are provided,\n            it defaults to 0.\n\n    NOTE: This is the function to use when specifying localised stimuli and\n    parameter variations. For efficiently using the whole mesh as sources, such\n    as is required to represent local connectivity within the cortex, see the\n    local_gdist_matrix() function.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> src = numpy.array([1], dtype=numpy.int32)\n        >>> trg = numpy.array([2], dtype=""numpy.int32)\n        >>> import gdist\n        >>> gdist.compute_gdist(vertices, triangles, source_indices=src, target_indices=trg)\n         array([0.2])\n    ");
+static PyMethodDef __pyx_mdef_5gdist_1compute_gdist = {"compute_gdist", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5gdist_1compute_gdist, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5gdist_compute_gdist};
+static PyObject *__pyx_pw_5gdist_1compute_gdist(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_vertices = 0;
   PyArrayObject *__pyx_v_triangles = 0;
   PyArrayObject *__pyx_v_source_indices = 0;
   PyArrayObject *__pyx_v_target_indices = 0;
   double __pyx_v_max_distance;
   bool __pyx_v_is_one_indexed;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[6] = {0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("compute_gdist (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_source_indices,&__pyx_n_s_target_indices,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_source_indices,&__pyx_n_s_target_indices,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
+    __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
 
     /* "gdist.pyx":121
  * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,
  *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,             # <<<<<<<<<<<<<<
  *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,
  *                   double max_distance=GEODESIC_INF,
  */
-    values[2] = (PyObject *)((PyArrayObject *)Py_None);
+    values[2] = __Pyx_Arg_NewRef_FASTCALL((PyObject *)((PyArrayObject *)Py_None));
 
     /* "gdist.pyx":122
  *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,             # <<<<<<<<<<<<<<
  *                   double max_distance=GEODESIC_INF,
  *                   bool is_one_indexed=False):
  */
-    values[3] = (PyObject *)((PyArrayObject *)Py_None);
-    if (unlikely(__pyx_kwds)) {
+    values[3] = __Pyx_Arg_NewRef_FASTCALL((PyObject *)((PyArrayObject *)Py_None));
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      switch (__pyx_nargs) {
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_vertices)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vertices)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_triangles)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_triangles)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("compute_gdist", 0, 2, 6, 1); __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_source_indices);
-          if (value) { values[2] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_source_indices);
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_target_indices);
-          if (value) { values[3] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_target_indices);
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_distance);
-          if (value) { values[4] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_distance);
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_is_one_indexed);
-          if (value) { values[5] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_is_one_indexed);
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compute_gdist") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "compute_gdist") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+      switch (__pyx_nargs) {
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_vertices = ((PyArrayObject *)values[0]);
     __pyx_v_triangles = ((PyArrayObject *)values[1]);
     __pyx_v_source_indices = ((PyArrayObject *)values[2]);
     __pyx_v_target_indices = ((PyArrayObject *)values[3]);
     if (values[4]) {
       __pyx_v_max_distance = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_max_distance == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 123, __pyx_L3_error)
     } else {
-      __pyx_v_max_distance = __pyx_k_;
+      __pyx_v_max_distance = __pyx_dynamic_args->__pyx_arg_max_distance;
     }
     if (values[5]) {
       __pyx_v_is_one_indexed = __Pyx_PyObject_IsTrue(values[5]); if (unlikely((__pyx_v_is_one_indexed == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 124, __pyx_L3_error)
     } else {
-
-      /* "gdist.pyx":124
- *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,
- *                   double max_distance=GEODESIC_INF,
- *                   bool is_one_indexed=False):             # <<<<<<<<<<<<<<
- *     """This is the wrapper function for computing geodesic distance between a
- *     set of sources and targets on a mesh surface.
- */
-      __pyx_v_is_one_indexed = ((bool)0);
+      __pyx_v_is_one_indexed = ((bool)((int)0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_gdist", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_gdist", 0, 2, 6, __pyx_nargs); __PYX_ERR(0, 119, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("gdist.compute_gdist", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vertices), __pyx_ptype_5numpy_ndarray, 1, "vertices", 0))) __PYX_ERR(0, 119, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_triangles), __pyx_ptype_5numpy_ndarray, 1, "triangles", 0))) __PYX_ERR(0, 120, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_source_indices), __pyx_ptype_5numpy_ndarray, 1, "source_indices", 0))) __PYX_ERR(0, 121, __pyx_L1_error)
@@ -2604,14 +5719,20 @@
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5gdist_compute_gdist(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, PyArrayObject *__pyx_v_source_indices, PyArrayObject *__pyx_v_target_indices, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed) {
   bool __pyx_v_propagate_on_max_distance;
   std::vector<double>  __pyx_v_points;
@@ -2625,24 +5746,24 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_triangles;
   __Pyx_Buffer __pyx_pybuffer_triangles;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_vertices;
   __Pyx_Buffer __pyx_pybuffer_vertices;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  int __pyx_t_2;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyArrayObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
+  PyArrayObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
+  npy_intp *__pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyArrayObject *__pyx_t_13 = NULL;
   Py_ssize_t __pyx_t_14;
   PyObject *(*__pyx_t_15)(PyObject *);
   double __pyx_t_16;
   unsigned int __pyx_t_17;
   std::vector<unsigned int>  __pyx_t_18;
@@ -2703,64 +5824,63 @@
  *     cdef vector[unsigned] faces
  * 
  *     if source_indices is None:             # <<<<<<<<<<<<<<
  *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0
  *     if target_indices is None:
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_source_indices) == Py_None);
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
+  if (__pyx_t_1) {
 
     /* "gdist.pyx":173
  * 
  *     if source_indices is None:
  *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0             # <<<<<<<<<<<<<<
  *     if target_indices is None:
  *         propagate_on_max_distance = True
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_numpy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_numpy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_arange); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_numpy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__2, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 173, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 173, __pyx_L1_error)
-    __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_source_indices.rcbuffer->pybuffer);
-      __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_source_indices.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_8 < 0)) {
-        PyErr_Fetch(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
+      __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_source_indices.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_7 < 0)) {
+        PyErr_Fetch(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_source_indices.rcbuffer->pybuffer, (PyObject*)__pyx_v_source_indices, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11);
+          Py_XDECREF(__pyx_t_8); Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_9, __pyx_t_10, __pyx_t_11);
+          PyErr_Restore(__pyx_t_8, __pyx_t_9, __pyx_t_10);
         }
-        __pyx_t_9 = __pyx_t_10 = __pyx_t_11 = 0;
+        __pyx_t_8 = __pyx_t_9 = __pyx_t_10 = 0;
       }
       __pyx_pybuffernd_source_indices.diminfo[0].strides = __pyx_pybuffernd_source_indices.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_source_indices.diminfo[0].shape = __pyx_pybuffernd_source_indices.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 173, __pyx_L1_error)
+      if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 173, __pyx_L1_error)
     }
-    __pyx_t_7 = 0;
-    __Pyx_DECREF_SET(__pyx_v_source_indices, ((PyArrayObject *)__pyx_t_6));
     __pyx_t_6 = 0;
+    __Pyx_DECREF_SET(__pyx_v_source_indices, ((PyArrayObject *)__pyx_t_5));
+    __pyx_t_5 = 0;
 
     /* "gdist.pyx":172
  *     cdef vector[unsigned] faces
  * 
  *     if source_indices is None:             # <<<<<<<<<<<<<<
  *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0
  *     if target_indices is None:
@@ -2770,16 +5890,15 @@
   /* "gdist.pyx":174
  *     if source_indices is None:
  *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0
  *     if target_indices is None:             # <<<<<<<<<<<<<<
  *         propagate_on_max_distance = True
  *         target_indices = numpy.arange(vertices.shape[0], dtype=numpy.int32)
  */
-  __pyx_t_2 = (((PyObject *)__pyx_v_target_indices) == Py_None);
-  __pyx_t_1 = (__pyx_t_2 != 0);
+  __pyx_t_1 = (((PyObject *)__pyx_v_target_indices) == Py_None);
   if (__pyx_t_1) {
 
     /* "gdist.pyx":175
  *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0
  *     if target_indices is None:
  *         propagate_on_max_distance = True             # <<<<<<<<<<<<<<
  *         target_indices = numpy.arange(vertices.shape[0], dtype=numpy.int32)
@@ -2790,58 +5909,59 @@
     /* "gdist.pyx":176
  *     if target_indices is None:
  *         propagate_on_max_distance = True
  *         target_indices = numpy.arange(vertices.shape[0], dtype=numpy.int32)             # <<<<<<<<<<<<<<
  * 
  *     for k in vertices.flatten():
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_numpy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_vertices->dimensions[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_numpy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 176, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_11 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_vertices)); if (unlikely(__pyx_t_11 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t((__pyx_t_11[0])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error);
+    __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 176, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 176, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_12);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_target_indices.rcbuffer->pybuffer);
-      __pyx_t_8 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_indices.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
-      if (unlikely(__pyx_t_8 < 0)) {
-        PyErr_Fetch(&__pyx_t_11, &__pyx_t_10, &__pyx_t_9);
+      __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_indices.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      if (unlikely(__pyx_t_7 < 0)) {
+        PyErr_Fetch(&__pyx_t_10, &__pyx_t_9, &__pyx_t_8);
         if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_target_indices.rcbuffer->pybuffer, (PyObject*)__pyx_v_target_indices, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
-          Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_9);
+          Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_8);
           __Pyx_RaiseBufferFallbackError();
         } else {
-          PyErr_Restore(__pyx_t_11, __pyx_t_10, __pyx_t_9);
+          PyErr_Restore(__pyx_t_10, __pyx_t_9, __pyx_t_8);
         }
-        __pyx_t_11 = __pyx_t_10 = __pyx_t_9 = 0;
+        __pyx_t_10 = __pyx_t_9 = __pyx_t_8 = 0;
       }
       __pyx_pybuffernd_target_indices.diminfo[0].strides = __pyx_pybuffernd_target_indices.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_target_indices.diminfo[0].shape = __pyx_pybuffernd_target_indices.rcbuffer->pybuffer.shape[0];
-      if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
+      if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 176, __pyx_L1_error)
     }
     __pyx_t_13 = 0;
     __Pyx_DECREF_SET(__pyx_v_target_indices, ((PyArrayObject *)__pyx_t_12));
     __pyx_t_12 = 0;
 
     /* "gdist.pyx":174
  *     if source_indices is None:
@@ -2855,61 +5975,81 @@
   /* "gdist.pyx":178
  *         target_indices = numpy.arange(vertices.shape[0], dtype=numpy.int32)
  * 
  *     for k in vertices.flatten():             # <<<<<<<<<<<<<<
  *         points.push_back(k)
  *     for k in triangles.flatten():
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_vertices), __pyx_n_s_flatten); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_vertices), __pyx_n_s_flatten); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_7 = 1;
     }
   }
-  __pyx_t_12 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_12 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  }
   if (likely(PyList_CheckExact(__pyx_t_12)) || PyTuple_CheckExact(__pyx_t_12)) {
-    __pyx_t_6 = __pyx_t_12; __Pyx_INCREF(__pyx_t_6); __pyx_t_14 = 0;
+    __pyx_t_5 = __pyx_t_12; __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_14 = 0;
     __pyx_t_15 = NULL;
   } else {
-    __pyx_t_14 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 178, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_15 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_14 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_12); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_15 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 178, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   for (;;) {
     if (likely(!__pyx_t_15)) {
-      if (likely(PyList_CheckExact(__pyx_t_6))) {
-        if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_6)) break;
+      if (likely(PyList_CheckExact(__pyx_t_5))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+          #endif
+          if (__pyx_t_14 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_12 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_14); __Pyx_INCREF(__pyx_t_12); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_12 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_12); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
         #else
-        __pyx_t_12 = PySequence_ITEM(__pyx_t_6, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         #endif
       } else {
-        if (__pyx_t_14 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+          #endif
+          if (__pyx_t_14 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_14); __Pyx_INCREF(__pyx_t_12); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_12 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_12); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
         #else
-        __pyx_t_12 = PySequence_ITEM(__pyx_t_6, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 178, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         #endif
       }
     } else {
-      __pyx_t_12 = __pyx_t_15(__pyx_t_6);
+      __pyx_t_12 = __pyx_t_15(__pyx_t_5);
       if (unlikely(!__pyx_t_12)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
           else __PYX_ERR(0, 178, __pyx_L1_error)
         }
         break;
@@ -2938,82 +6078,102 @@
  *         target_indices = numpy.arange(vertices.shape[0], dtype=numpy.int32)
  * 
  *     for k in vertices.flatten():             # <<<<<<<<<<<<<<
  *         points.push_back(k)
  *     for k in triangles.flatten():
  */
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "gdist.pyx":180
  *     for k in vertices.flatten():
  *         points.push_back(k)
  *     for k in triangles.flatten():             # <<<<<<<<<<<<<<
  *         faces.push_back(k)
  * 
  */
   __pyx_t_12 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_triangles), __pyx_n_s_flatten); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_12);
-    if (likely(__pyx_t_4)) {
+  __pyx_t_3 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_12))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_12);
+    if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
-      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_12, function);
+      __pyx_t_7 = 1;
     }
   }
-  __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
-    __pyx_t_12 = __pyx_t_6; __Pyx_INCREF(__pyx_t_12); __pyx_t_14 = 0;
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
+    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  }
+  if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
+    __pyx_t_12 = __pyx_t_5; __Pyx_INCREF(__pyx_t_12);
+    __pyx_t_14 = 0;
     __pyx_t_15 = NULL;
   } else {
-    __pyx_t_14 = -1; __pyx_t_12 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_14 = -1; __pyx_t_12 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_15 = Py_TYPE(__pyx_t_12)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_12); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 180, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   for (;;) {
     if (likely(!__pyx_t_15)) {
       if (likely(PyList_CheckExact(__pyx_t_12))) {
-        if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_12)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_12);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 180, __pyx_L1_error)
+          #endif
+          if (__pyx_t_14 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_12, __pyx_t_14); __Pyx_INCREF(__pyx_t_6); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_12, __pyx_t_14); __Pyx_INCREF(__pyx_t_5); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 180, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_12, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_14 >= PyTuple_GET_SIZE(__pyx_t_12)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_12);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 180, __pyx_L1_error)
+          #endif
+          if (__pyx_t_14 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_12, __pyx_t_14); __Pyx_INCREF(__pyx_t_6); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_12, __pyx_t_14); __Pyx_INCREF(__pyx_t_5); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 180, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_12, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 180, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_12, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
-      __pyx_t_6 = __pyx_t_15(__pyx_t_12);
-      if (unlikely(!__pyx_t_6)) {
+      __pyx_t_5 = __pyx_t_15(__pyx_t_12);
+      if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
           else __PYX_ERR(0, 180, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GOTREF(__pyx_t_5);
     }
-    __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_6);
-    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_5);
+    __pyx_t_5 = 0;
 
     /* "gdist.pyx":181
  *         points.push_back(k)
  *     for k in triangles.flatten():
  *         faces.push_back(k)             # <<<<<<<<<<<<<<
  * 
  *     distances = compute_gdist_impl(
@@ -3057,68 +6217,75 @@
   /* "gdist.pyx":183
  *         faces.push_back(k)
  * 
  *     distances = compute_gdist_impl(             # <<<<<<<<<<<<<<
  *         points,
  *         faces,
  */
-  __pyx_t_12 = __pyx_convert_vector_to_py_double(compute_gdist_impl(__pyx_v_points, __pyx_v_faces, __pyx_t_18, __pyx_t_19, __pyx_v_max_distance, __pyx_v_is_one_indexed, __pyx_v_propagate_on_max_distance)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_12 = __pyx_convert_vector_to_py_double(compute_gdist_impl(__pyx_v_points, __pyx_v_faces, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_18), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_19), __pyx_v_max_distance, __pyx_v_is_one_indexed, __pyx_v_propagate_on_max_distance)); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __pyx_v_distances = __pyx_t_12;
   __pyx_t_12 = 0;
 
   /* "gdist.pyx":193
  *     )
  *     # TODO: Basically copies, can be improved as memory is contiguous.
  *     distances = numpy.asarray(distances)             # <<<<<<<<<<<<<<
  *     distances[distances == max_distance] = numpy.inf
  *     return distances
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_numpy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_asarray); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_numpy); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_7 = 1;
     }
   }
-  __pyx_t_12 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_v_distances) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_distances);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_distances};
+    __pyx_t_12 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
   __Pyx_DECREF_SET(__pyx_v_distances, __pyx_t_12);
   __pyx_t_12 = 0;
 
   /* "gdist.pyx":194
  *     # TODO: Basically copies, can be improved as memory is contiguous.
  *     distances = numpy.asarray(distances)
  *     distances[distances == max_distance] = numpy.inf             # <<<<<<<<<<<<<<
  *     return distances
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_numpy); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_inf); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_inf); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = PyFloat_FromDouble(__pyx_v_max_distance); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_6 = PyObject_RichCompare(__pyx_v_distances, __pyx_t_12, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_v_distances, __pyx_t_12, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_distances, __pyx_t_6, __pyx_t_4) < 0)) __PYX_ERR(0, 194, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely((PyObject_SetItem(__pyx_v_distances, __pyx_t_5, __pyx_t_3) < 0))) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "gdist.pyx":195
  *     distances = numpy.asarray(distances)
  *     distances[distances == max_distance] = numpy.inf
  *     return distances             # <<<<<<<<<<<<<<
  * 
  * 
@@ -3134,18 +6301,18 @@
  * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_12);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_source_indices.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_target_indices.rcbuffer->pybuffer);
@@ -3174,132 +6341,229 @@
  * 
  * 
  * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                        double max_distance=GEODESIC_INF,
  */
 
+static PyObject *__pyx_pf_5gdist_8__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 1);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_max_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  /* "gdist.pyx":201
+ *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                        double max_distance=GEODESIC_INF,
+ *                        bool is_one_indexed=False):             # <<<<<<<<<<<<<<
+ *     """This is the wrapper function for computing geodesic distance from every
+ *     vertex on the surface to all those within a distance ``max_distance`` of
+ */
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "gdist.pyx":198
+ * 
+ * 
+ * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
+ *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                        double max_distance=GEODESIC_INF,
+ */
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None)) __PYX_ERR(0, 198, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("gdist.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* Python wrapper */
-static PyObject *__pyx_pw_5gdist_3local_gdist_matrix(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5gdist_2local_gdist_matrix[] = "This is the wrapper function for computing geodesic distance from every\n    vertex on the surface to all those within a distance ``max_distance`` of\n    them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n        is the number of vertices, specifying the shortest distance from all\n        vertices to all the vertices within max_distance.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> import gdist\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> gdist.local_gdist_matrix(vertices, triangles, max_distance=1.0)\n         <121x121 sparse matrix of type '<type 'numpy.float64'>'\n             with 6232 stored elements in Compressed Sparse Column format>\n\n    Runtime and guesstimated memory usage as a function of max_distance for the\n    reg_13 cortical surface mesh, ie containing 2**13 vertices per hemisphere.\n    ::\n        [[10, 20, 30, 40,  50,  60,  70,  80,  90, 100], # mm\n         [19, 28, 49, 81, 125, 181, 248, 331, 422, 522], # s\n         [ 3, 13, 30, 56,  89, 129, 177, 232, 292, 358]] # MB]\n\n    where memory is a min-guestimate given by: mem_req = nnz * 8 / 1024 / 1024.\n    ";
-static PyMethodDef __pyx_mdef_5gdist_3local_gdist_matrix = {"local_gdist_matrix", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5gdist_3local_gdist_matrix, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5gdist_2local_gdist_matrix};
-static PyObject *__pyx_pw_5gdist_3local_gdist_matrix(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5gdist_3local_gdist_matrix(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_5gdist_2local_gdist_matrix, "This is the wrapper function for computing geodesic distance from every\n    vertex on the surface to all those within a distance ``max_distance`` of\n    them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n        is the number of vertices, specifying the shortest distance from all\n        vertices to all the vertices within max_distance.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> import gdist\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> gdist.local_gdist_matrix(vertices, triangles, max_distance=1.0)\n         <121x121 sparse matrix of type '<type 'numpy.float64'>'\n             with 6232 stored elements in Compressed Sparse Column format>\n\n    Runtime and guesstimated memory usage as a function of max_distance for the\n    reg_13 cortical surface mesh, ie containing 2**13 vertices per hemisphere.\n    ::\n        [[10, 20, 30, 40,  50,  60,  70,  80,  90, 100], # mm\n         [19, 28, 49, 81, 125, 181, 248, 331, 422, 522], # s\n         [ 3, 13, 30, 56,  89, 129, 177, 232, 292, 358]] # MB]\n\n    where memory is a min-guestimate given by: mem_req = nnz * 8 / 1024 / 1024.\n    ");
+static PyMethodDef __pyx_mdef_5gdist_3local_gdist_matrix = {"local_gdist_matrix", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5gdist_3local_gdist_matrix, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5gdist_2local_gdist_matrix};
+static PyObject *__pyx_pw_5gdist_3local_gdist_matrix(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_vertices = 0;
   PyArrayObject *__pyx_v_triangles = 0;
   double __pyx_v_max_distance;
   bool __pyx_v_is_one_indexed;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("local_gdist_matrix (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
-    PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
+    __pyx_defaults1 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self);
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_vertices)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vertices)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_triangles)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_triangles)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("local_gdist_matrix", 0, 2, 4, 1); __PYX_ERR(0, 198, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_distance);
-          if (value) { values[2] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_distance);
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_is_one_indexed);
-          if (value) { values[3] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_is_one_indexed);
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "local_gdist_matrix") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "local_gdist_matrix") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_vertices = ((PyArrayObject *)values[0]);
     __pyx_v_triangles = ((PyArrayObject *)values[1]);
     if (values[2]) {
       __pyx_v_max_distance = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_max_distance == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 200, __pyx_L3_error)
     } else {
-      __pyx_v_max_distance = __pyx_k__3;
+      __pyx_v_max_distance = __pyx_dynamic_args->__pyx_arg_max_distance;
     }
     if (values[3]) {
       __pyx_v_is_one_indexed = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_is_one_indexed == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     } else {
-
-      /* "gdist.pyx":201
- *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- *                        double max_distance=GEODESIC_INF,
- *                        bool is_one_indexed=False):             # <<<<<<<<<<<<<<
- *     """This is the wrapper function for computing geodesic distance from every
- *     vertex on the surface to all those within a distance ``max_distance`` of
- */
-      __pyx_v_is_one_indexed = ((bool)0);
+      __pyx_v_is_one_indexed = ((bool)((int)0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("local_gdist_matrix", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 198, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("local_gdist_matrix", 0, 2, 4, __pyx_nargs); __PYX_ERR(0, 198, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("gdist.local_gdist_matrix", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vertices), __pyx_ptype_5numpy_ndarray, 1, "vertices", 0))) __PYX_ERR(0, 198, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_triangles), __pyx_ptype_5numpy_ndarray, 1, "triangles", 0))) __PYX_ERR(0, 199, __pyx_L1_error)
   __pyx_r = __pyx_pf_5gdist_2local_gdist_matrix(__pyx_self, __pyx_v_vertices, __pyx_v_triangles, __pyx_v_max_distance, __pyx_v_is_one_indexed);
 
-  /* "gdist.pyx":198
- * 
- * 
- * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
- *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- *                        double max_distance=GEODESIC_INF,
- */
-
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5gdist_2local_gdist_matrix(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed) {
   geodesic::Mesh __pyx_v_amesh;
   geodesic::GeodesicAlgorithmExact *__pyx_v_algorithm;
@@ -3315,32 +6579,33 @@
   __Pyx_LocalBuf_ND __pyx_pybuffernd_triangles;
   __Pyx_Buffer __pyx_pybuffer_triangles;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_vertices;
   __Pyx_Buffer __pyx_pybuffer_vertices;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
+  npy_intp *__pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   Py_ssize_t __pyx_t_7;
-  int __pyx_t_8;
+  Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
+  int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("local_gdist_matrix", 0);
+  __Pyx_RefNannySetupContext("local_gdist_matrix", 1);
   __pyx_pybuffer_vertices.pybuffer.buf = NULL;
   __pyx_pybuffer_vertices.refcount = 0;
   __pyx_pybuffernd_vertices.data = NULL;
   __pyx_pybuffernd_vertices.rcbuffer = &__pyx_pybuffer_vertices;
   __pyx_pybuffer_triangles.pybuffer.buf = NULL;
   __pyx_pybuffer_triangles.refcount = 0;
   __pyx_pybuffernd_triangles.data = NULL;
@@ -3379,15 +6644,16 @@
   /* "gdist.pyx":255
  * 
  *     cdef vector[SurfacePoint] source, targets
  *     cdef Py_ssize_t N = vertices.shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t k
  *     cdef Py_ssize_t kk
  */
-  __pyx_v_N = (__pyx_v_vertices->dimensions[0]);
+  __pyx_t_2 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_vertices)); if (unlikely(__pyx_t_2 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_v_N = (__pyx_t_2[0]);
 
   /* "gdist.pyx":258
  *     cdef Py_ssize_t k
  *     cdef Py_ssize_t kk
  *     cdef numpy.float64_t distance = 0             # <<<<<<<<<<<<<<
  * 
  *     # Add all vertices as targets
@@ -3397,18 +6663,18 @@
   /* "gdist.pyx":261
  * 
  *     # Add all vertices as targets
  *     for k in range(N):             # <<<<<<<<<<<<<<
  *         targets.push_back(SurfacePoint(&amesh.vertices()[k]))
  * 
  */
-  __pyx_t_2 = __pyx_v_N;
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_k = __pyx_t_4;
+  __pyx_t_3 = __pyx_v_N;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_k = __pyx_t_5;
 
     /* "gdist.pyx":262
  *     # Add all vertices as targets
  *     for k in range(N):
  *         targets.push_back(SurfacePoint(&amesh.vertices()[k]))             # <<<<<<<<<<<<<<
  * 
  *     rows = []
@@ -3460,18 +6726,18 @@
   /* "gdist.pyx":267
  *     columns = []
  *     data = []
  *     for k in range(N):             # <<<<<<<<<<<<<<
  *         source.push_back(SurfacePoint(&amesh.vertices()[k]))
  *         algorithm.propagate(source, max_distance, NULL)
  */
-  __pyx_t_2 = __pyx_v_N;
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_k = __pyx_t_4;
+  __pyx_t_3 = __pyx_v_N;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_k = __pyx_t_5;
 
     /* "gdist.pyx":268
  *     data = []
  *     for k in range(N):
  *         source.push_back(SurfacePoint(&amesh.vertices()[k]))             # <<<<<<<<<<<<<<
  *         algorithm.propagate(source, max_distance, NULL)
  *         source.pop_back()
@@ -3504,18 +6770,18 @@
     /* "gdist.pyx":272
  *         source.pop_back()
  * 
  *         for kk in range(N):  # TODO: Reduce to vertices reached during propagate.             # <<<<<<<<<<<<<<
  *             algorithm.best_source(targets[kk], distance)
  * 
  */
-    __pyx_t_5 = __pyx_v_N;
-    __pyx_t_6 = __pyx_t_5;
-    for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
-      __pyx_v_kk = __pyx_t_7;
+    __pyx_t_6 = __pyx_v_N;
+    __pyx_t_7 = __pyx_t_6;
+    for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
+      __pyx_v_kk = __pyx_t_8;
 
       /* "gdist.pyx":273
  * 
  *         for kk in range(N):  # TODO: Reduce to vertices reached during propagate.
  *             algorithm.best_source(targets[kk], distance)             # <<<<<<<<<<<<<<
  * 
  *             if (
@@ -3525,89 +6791,89 @@
       /* "gdist.pyx":276
  * 
  *             if (
  *                 distance is not GEODESIC_INF             # <<<<<<<<<<<<<<
  *                 and distance is not 0
  *                 and distance <= max_distance
  */
-      __pyx_t_9 = ((__pyx_v_distance != geodesic::GEODESIC_INF) != 0);
-      if (__pyx_t_9) {
+      __pyx_t_10 = (__pyx_v_distance != geodesic::GEODESIC_INF);
+      if (__pyx_t_10) {
       } else {
-        __pyx_t_8 = __pyx_t_9;
+        __pyx_t_9 = __pyx_t_10;
         goto __pyx_L10_bool_binop_done;
       }
 
       /* "gdist.pyx":277
  *             if (
  *                 distance is not GEODESIC_INF
  *                 and distance is not 0             # <<<<<<<<<<<<<<
  *                 and distance <= max_distance
  *             ):
  */
-      __pyx_t_9 = ((__pyx_v_distance != 0.0) != 0);
-      if (__pyx_t_9) {
+      __pyx_t_10 = (__pyx_v_distance != 0.0);
+      if (__pyx_t_10) {
       } else {
-        __pyx_t_8 = __pyx_t_9;
+        __pyx_t_9 = __pyx_t_10;
         goto __pyx_L10_bool_binop_done;
       }
 
       /* "gdist.pyx":278
  *                 distance is not GEODESIC_INF
  *                 and distance is not 0
  *                 and distance <= max_distance             # <<<<<<<<<<<<<<
  *             ):
  *                 rows.append(k)
  */
-      __pyx_t_9 = ((__pyx_v_distance <= __pyx_v_max_distance) != 0);
-      __pyx_t_8 = __pyx_t_9;
+      __pyx_t_10 = (__pyx_v_distance <= __pyx_v_max_distance);
+      __pyx_t_9 = __pyx_t_10;
       __pyx_L10_bool_binop_done:;
 
       /* "gdist.pyx":275
  *             algorithm.best_source(targets[kk], distance)
  * 
  *             if (             # <<<<<<<<<<<<<<
  *                 distance is not GEODESIC_INF
  *                 and distance is not 0
  */
-      if (__pyx_t_8) {
+      if (__pyx_t_9) {
 
         /* "gdist.pyx":280
  *                 and distance <= max_distance
  *             ):
  *                 rows.append(k)             # <<<<<<<<<<<<<<
  *                 columns.append(kk)
  *                 data.append(distance)
  */
         __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_rows, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 280, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_rows, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 280, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "gdist.pyx":281
  *             ):
  *                 rows.append(k)
  *                 columns.append(kk)             # <<<<<<<<<<<<<<
  *                 data.append(distance)
  * 
  */
         __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_kk); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_columns, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_columns, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "gdist.pyx":282
  *                 rows.append(k)
  *                 columns.append(kk)
  *                 data.append(distance)             # <<<<<<<<<<<<<<
  * 
  *     return scipy.sparse.csc_matrix((data, (rows, columns)), shape=(N, N))
  */
         __pyx_t_1 = PyFloat_FromDouble(__pyx_v_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_data, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyList_Append(__pyx_v_data, __pyx_t_1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 282, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "gdist.pyx":275
  *             algorithm.best_source(targets[kk], distance)
  * 
  *             if (             # <<<<<<<<<<<<<<
  *                 distance is not GEODESIC_INF
@@ -3623,82 +6889,82 @@
  *     return scipy.sparse.csc_matrix((data, (rows, columns)), shape=(N, N))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_scipy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sparse); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_sparse); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_csc_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_csc_matrix); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
   __Pyx_INCREF(__pyx_v_rows);
   __Pyx_GIVEREF(__pyx_v_rows);
-  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_rows);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_v_rows)) __PYX_ERR(0, 284, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_columns);
   __Pyx_GIVEREF(__pyx_v_columns);
-  PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_columns);
-  __pyx_t_12 = PyTuple_New(2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_12);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_v_columns)) __PYX_ERR(0, 284, __pyx_L1_error);
+  __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
-  PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_v_data);
-  __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_11);
-  __pyx_t_11 = 0;
-  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_v_data)) __PYX_ERR(0, 284, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_12);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_13 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_13);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_13)) __PYX_ERR(0, 284, __pyx_L1_error);
+  __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __pyx_t_14 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
-  __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_15 = PyInt_FromSsize_t(__pyx_v_N); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_13);
+  __pyx_t_16 = PyTuple_New(2); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_14);
-  __pyx_t_13 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_14)) __PYX_ERR(0, 284, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_15);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_15)) __PYX_ERR(0, 284, __pyx_L1_error);
   __pyx_t_14 = 0;
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_shape, __pyx_t_15) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 284, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_15);
+  __pyx_t_15 = 0;
+  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_shape, __pyx_t_16) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+  __pyx_t_16 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_12, __pyx_t_13); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_r = __pyx_t_15;
-  __pyx_t_15 = 0;
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_r = __pyx_t_16;
+  __pyx_t_16 = 0;
   goto __pyx_L0;
 
   /* "gdist.pyx":198
  * 
  * 
  * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                        double max_distance=GEODESIC_INF,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_16);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_triangles.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vertices.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
@@ -3721,144 +6987,245 @@
  * 
  * 
  * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
  *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
  *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  */
 
+static PyObject *__pyx_pf_5gdist_10__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__defaults__", 1);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyFloat_FromDouble(__Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self)->__pyx_arg_max_distance); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  /* "gdist.pyx":292
+ *     numpy.ndarray[numpy.int32_t, ndim=1] points,
+ *     double max_distance=GEODESIC_INF,
+ *     bool is_one_indexed=False             # <<<<<<<<<<<<<<
+ * ):
+ *     """Function for calculating pairwise geodesic distance for a set of points
+ */
+  __pyx_t_2 = __Pyx_PyBool_FromLong(((int)0)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "gdist.pyx":287
+ * 
+ * 
+ * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
+ *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
+ *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ */
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None)) __PYX_ERR(0, 287, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("gdist.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* Python wrapper */
-static PyObject *__pyx_pw_5gdist_5distance_matrix_of_selected_points(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_5gdist_4distance_matrix_of_selected_points[] = "Function for calculating pairwise geodesic distance for a set of points\n    within a distance ``max_distance`` of them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        points (numpy.ndarray[numpy.int32_t, ndim=1]): Indices of the points\n            among which the pairwise distances are to be calculated.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n            is the number of vertices, specifying the pairwise distances among\n            the given points.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> points = numpy.array([2, 5, 10], dtype=numpy.int32)\n        >>> import gdist\n        >>> gdist.distance_matrix_of_selected_points(\n                vertices, triangles, points\n            )\n         <121x121 sparse matrix of type '<class 'numpy.float64'>'\n            with 6 stored elements in Compressed Sparse Column format>\n    ";
-static PyMethodDef __pyx_mdef_5gdist_5distance_matrix_of_selected_points = {"distance_matrix_of_selected_points", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5gdist_5distance_matrix_of_selected_points, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5gdist_4distance_matrix_of_selected_points};
-static PyObject *__pyx_pw_5gdist_5distance_matrix_of_selected_points(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_5gdist_5distance_matrix_of_selected_points(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_5gdist_4distance_matrix_of_selected_points, "Function for calculating pairwise geodesic distance for a set of points\n    within a distance ``max_distance`` of them.\n\n    Args:\n        vertices (numpy.ndarray[numpy.float64_t, ndim=2]): Defines x,y,z\n            coordinates of the mesh's vertices.\n        triangles (numpy.ndarray[numpy.float64_t, ndim=2]): Defines faces of\n            the mesh as index triplets into vertices.\n        points (numpy.ndarray[numpy.int32_t, ndim=1]): Indices of the points\n            among which the pairwise distances are to be calculated.\n        max_distance (double): Propagation algorithm stops after reaching the\n            certain distance from the source.\n        is_one_indexed (bool): defines if the index of the triangles data is\n            one-indexed.\n\n    Returns:\n        scipy.sparse.csc_matrix((N, N), dtype=numpy.float64): where N\n            is the number of vertices, specifying the pairwise distances among\n            the given points.\n\n    Basic usage then looks like::\n        >>> import numpy\n        >>> temp = numpy.loadtxt(\"data/flat_triangular_mesh.txt\", skiprows=1)\n        >>> vertices = temp[0:121].astype(numpy.float64)\n        >>> triangles = temp[121:321].astype(numpy.int32)\n        >>> points = numpy.array([2, 5, 10], dtype=numpy.int32)\n        >>> import gdist\n        >>> gdist.distance_matrix_of_selected_points(\n                vertices, triangles, points\n            )\n         <121x121 sparse matrix of type '<class 'numpy.float64'>'\n            with 6 stored elements in Compressed Sparse Column format>\n    ");
+static PyMethodDef __pyx_mdef_5gdist_5distance_matrix_of_selected_points = {"distance_matrix_of_selected_points", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_5gdist_5distance_matrix_of_selected_points, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_5gdist_4distance_matrix_of_selected_points};
+static PyObject *__pyx_pw_5gdist_5distance_matrix_of_selected_points(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_vertices = 0;
   PyArrayObject *__pyx_v_triangles = 0;
   PyArrayObject *__pyx_v_points = 0;
   double __pyx_v_max_distance;
   bool __pyx_v_is_one_indexed;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("distance_matrix_of_selected_points (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_points,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
-    PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vertices,&__pyx_n_s_triangles,&__pyx_n_s_points,&__pyx_n_s_max_distance,&__pyx_n_s_is_one_indexed,0};
+    __pyx_defaults2 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_self);
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_vertices)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vertices)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_triangles)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_triangles)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distance_matrix_of_selected_points", 0, 3, 5, 1); __PYX_ERR(0, 287, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_points)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_points)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("distance_matrix_of_selected_points", 0, 3, 5, 2); __PYX_ERR(0, 287, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_distance);
-          if (value) { values[3] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_distance);
+          if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_is_one_indexed);
-          if (value) { values[4] = value; kw_args--; }
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_is_one_indexed);
+          if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "distance_matrix_of_selected_points") < 0)) __PYX_ERR(0, 287, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "distance_matrix_of_selected_points") < 0)) __PYX_ERR(0, 287, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_vertices = ((PyArrayObject *)values[0]);
     __pyx_v_triangles = ((PyArrayObject *)values[1]);
     __pyx_v_points = ((PyArrayObject *)values[2]);
     if (values[3]) {
       __pyx_v_max_distance = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_max_distance == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 291, __pyx_L3_error)
     } else {
-      __pyx_v_max_distance = __pyx_k__4;
+      __pyx_v_max_distance = __pyx_dynamic_args->__pyx_arg_max_distance;
     }
     if (values[4]) {
       __pyx_v_is_one_indexed = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_is_one_indexed == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L3_error)
     } else {
-
-      /* "gdist.pyx":292
- *     numpy.ndarray[numpy.int32_t, ndim=1] points,
- *     double max_distance=GEODESIC_INF,
- *     bool is_one_indexed=False             # <<<<<<<<<<<<<<
- * ):
- *     """Function for calculating pairwise geodesic distance for a set of points
- */
-      __pyx_v_is_one_indexed = ((bool)0);
+      __pyx_v_is_one_indexed = ((bool)((int)0));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("distance_matrix_of_selected_points", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 287, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("distance_matrix_of_selected_points", 0, 3, 5, __pyx_nargs); __PYX_ERR(0, 287, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("gdist.distance_matrix_of_selected_points", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vertices), __pyx_ptype_5numpy_ndarray, 1, "vertices", 0))) __PYX_ERR(0, 288, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_triangles), __pyx_ptype_5numpy_ndarray, 1, "triangles", 0))) __PYX_ERR(0, 289, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_points), __pyx_ptype_5numpy_ndarray, 1, "points", 0))) __PYX_ERR(0, 290, __pyx_L1_error)
   __pyx_r = __pyx_pf_5gdist_4distance_matrix_of_selected_points(__pyx_self, __pyx_v_vertices, __pyx_v_triangles, __pyx_v_points, __pyx_v_max_distance, __pyx_v_is_one_indexed);
 
-  /* "gdist.pyx":287
- * 
- * 
- * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
- *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
- *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- */
-
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5gdist_4distance_matrix_of_selected_points(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vertices, PyArrayObject *__pyx_v_triangles, PyArrayObject *__pyx_v_points, double __pyx_v_max_distance, bool __pyx_v_is_one_indexed) {
   std::vector<unsigned int>  __pyx_v_rows;
   std::vector<unsigned int>  __pyx_v_columns;
@@ -3885,23 +7252,23 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
-  PyObject *__pyx_t_11 = NULL;
-  Py_ssize_t __pyx_t_12;
-  PyObject *(*__pyx_t_13)(PyObject *);
-  unsigned int __pyx_t_14;
-  double __pyx_t_15;
+  Py_ssize_t __pyx_t_11;
+  PyObject *(*__pyx_t_12)(PyObject *);
+  unsigned int __pyx_t_13;
+  double __pyx_t_14;
+  npy_intp *__pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("distance_matrix_of_selected_points", 0);
+  __Pyx_RefNannySetupContext("distance_matrix_of_selected_points", 1);
   __pyx_pybuffer_vertices.pybuffer.buf = NULL;
   __pyx_pybuffer_vertices.refcount = 0;
   __pyx_pybuffernd_vertices.data = NULL;
   __pyx_pybuffernd_vertices.rcbuffer = &__pyx_pybuffer_vertices;
   __pyx_pybuffer_triangles.pybuffer.buf = NULL;
   __pyx_pybuffer_triangles.refcount = 0;
   __pyx_pybuffernd_triangles.data = NULL;
@@ -3932,37 +7299,50 @@
  *     for index_point, point in enumerate(points):             # <<<<<<<<<<<<<<
  *         target_indices = points[index_point + 1:]
  * 
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_1 = __pyx_int_0;
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_points))) || PyTuple_CheckExact(((PyObject *)__pyx_v_points))) {
-    __pyx_t_2 = ((PyObject *)__pyx_v_points); __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = ((PyObject *)__pyx_v_points); __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_points)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 331, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 331, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 331, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 331, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 331, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 331, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 331, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 331, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -4014,19 +7394,19 @@
     __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_point);
     __Pyx_GIVEREF(__pyx_v_point);
-    PyList_SET_ITEM(__pyx_t_5, 0, __pyx_v_point);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_v_point)) __PYX_ERR(0, 334, __pyx_L1_error);
     __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_numpy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_int32); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
@@ -4053,15 +7433,15 @@
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v_target_indices);
     __Pyx_GIVEREF(__pyx_v_target_indices);
-    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_target_indices);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_target_indices)) __PYX_ERR(0, 335, __pyx_L1_error);
     __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_numpy); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -4102,225 +7482,201 @@
  *         )
  * 
  */
     __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_is_one_indexed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 343, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_10 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+    #if CYTHON_UNPACK_METHODS
+    if (unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
         __pyx_t_10 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_7)) {
-      PyObject *__pyx_temp[7] = {__pyx_t_6, ((PyObject *)__pyx_v_vertices), ((PyObject *)__pyx_v_triangles), __pyx_v_source_index, __pyx_v_target_indices, __pyx_t_9, __pyx_t_5};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
     #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
-      PyObject *__pyx_temp[7] = {__pyx_t_6, ((PyObject *)__pyx_v_vertices), ((PyObject *)__pyx_v_triangles), __pyx_v_source_index, __pyx_v_target_indices, __pyx_t_9, __pyx_t_5};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_10, 6+__pyx_t_10); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 337, __pyx_L1_error)
+    {
+      PyObject *__pyx_callargs[7] = {__pyx_t_6, ((PyObject *)__pyx_v_vertices), ((PyObject *)__pyx_v_triangles), __pyx_v_source_index, __pyx_v_target_indices, __pyx_t_9, __pyx_t_5};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 6+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_11 = PyTuple_New(6+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 337, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
-      if (__pyx_t_6) {
-        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_6); __pyx_t_6 = NULL;
-      }
-      __Pyx_INCREF(((PyObject *)__pyx_v_vertices));
-      __Pyx_GIVEREF(((PyObject *)__pyx_v_vertices));
-      PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, ((PyObject *)__pyx_v_vertices));
-      __Pyx_INCREF(((PyObject *)__pyx_v_triangles));
-      __Pyx_GIVEREF(((PyObject *)__pyx_v_triangles));
-      PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, ((PyObject *)__pyx_v_triangles));
-      __Pyx_INCREF(__pyx_v_source_index);
-      __Pyx_GIVEREF(__pyx_v_source_index);
-      PyTuple_SET_ITEM(__pyx_t_11, 2+__pyx_t_10, __pyx_v_source_index);
-      __Pyx_INCREF(__pyx_v_target_indices);
-      __Pyx_GIVEREF(__pyx_v_target_indices);
-      PyTuple_SET_ITEM(__pyx_t_11, 3+__pyx_t_10, __pyx_v_target_indices);
-      __Pyx_GIVEREF(__pyx_t_9);
-      PyTuple_SET_ITEM(__pyx_t_11, 4+__pyx_t_10, __pyx_t_9);
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_11, 5+__pyx_t_10, __pyx_t_5);
-      __pyx_t_9 = 0;
-      __pyx_t_5 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 337, __pyx_L1_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 337, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v_distances, __pyx_t_8);
     __pyx_t_8 = 0;
 
     /* "gdist.pyx":346
  *         )
  * 
  *         for index_distance, distance in enumerate(distances):             # <<<<<<<<<<<<<<
  *             rows.push_back(point)
  *             columns.push_back(target_indices[index_distance])
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_8 = __pyx_int_0;
     if (likely(PyList_CheckExact(__pyx_v_distances)) || PyTuple_CheckExact(__pyx_v_distances)) {
-      __pyx_t_7 = __pyx_v_distances; __Pyx_INCREF(__pyx_t_7); __pyx_t_12 = 0;
-      __pyx_t_13 = NULL;
+      __pyx_t_7 = __pyx_v_distances; __Pyx_INCREF(__pyx_t_7);
+      __pyx_t_11 = 0;
+      __pyx_t_12 = NULL;
     } else {
-      __pyx_t_12 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_distances); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
+      __pyx_t_11 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_distances); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_13 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 346, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 346, __pyx_L1_error)
     }
     for (;;) {
-      if (likely(!__pyx_t_13)) {
+      if (likely(!__pyx_t_12)) {
         if (likely(PyList_CheckExact(__pyx_t_7))) {
-          if (__pyx_t_12 >= PyList_GET_SIZE(__pyx_t_7)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_7);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 346, __pyx_L1_error)
+            #endif
+            if (__pyx_t_11 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_11 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_12); __Pyx_INCREF(__pyx_t_11); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L1_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 346, __pyx_L1_error)
           #else
-          __pyx_t_11 = PySequence_ITEM(__pyx_t_7, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 346, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
-          if (__pyx_t_12 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_7);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 346, __pyx_L1_error)
+            #endif
+            if (__pyx_t_11 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_11 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_12); __Pyx_INCREF(__pyx_t_11); __pyx_t_12++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L1_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 346, __pyx_L1_error)
           #else
-          __pyx_t_11 = PySequence_ITEM(__pyx_t_7, __pyx_t_12); __pyx_t_12++; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 346, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_11);
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_7, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
-        __pyx_t_11 = __pyx_t_13(__pyx_t_7);
-        if (unlikely(!__pyx_t_11)) {
+        __pyx_t_5 = __pyx_t_12(__pyx_t_7);
+        if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
             else __PYX_ERR(0, 346, __pyx_L1_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_GOTREF(__pyx_t_5);
       }
-      __Pyx_XDECREF_SET(__pyx_v_distance, __pyx_t_11);
-      __pyx_t_11 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_distance, __pyx_t_5);
+      __pyx_t_5 = 0;
       __Pyx_INCREF(__pyx_t_8);
       __Pyx_XDECREF_SET(__pyx_v_index_distance, __pyx_t_8);
-      __pyx_t_11 = __Pyx_PyInt_AddObjC(__pyx_t_8, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 346, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
+      __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_t_8, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 346, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_8);
-      __pyx_t_8 = __pyx_t_11;
-      __pyx_t_11 = 0;
+      __pyx_t_8 = __pyx_t_5;
+      __pyx_t_5 = 0;
 
       /* "gdist.pyx":347
  * 
  *         for index_distance, distance in enumerate(distances):
  *             rows.push_back(point)             # <<<<<<<<<<<<<<
  *             columns.push_back(target_indices[index_distance])
  *             distance_matrix.push_back(distance)
  */
-      __pyx_t_14 = __Pyx_PyInt_As_unsigned_int(__pyx_v_point); if (unlikely((__pyx_t_14 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyInt_As_unsigned_int(__pyx_v_point); if (unlikely((__pyx_t_13 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 347, __pyx_L1_error)
       try {
-        __pyx_v_rows.push_back(__pyx_t_14);
+        __pyx_v_rows.push_back(__pyx_t_13);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 347, __pyx_L1_error)
       }
 
       /* "gdist.pyx":348
  *         for index_distance, distance in enumerate(distances):
  *             rows.push_back(point)
  *             columns.push_back(target_indices[index_distance])             # <<<<<<<<<<<<<<
  *             distance_matrix.push_back(distance)
  *             # symmetric
  */
-      __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_target_indices, __pyx_v_index_distance); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 348, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_14 = __Pyx_PyInt_As_unsigned_int(__pyx_t_11); if (unlikely((__pyx_t_14 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_target_indices, __pyx_v_index_distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 348, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_13 = __Pyx_PyInt_As_unsigned_int(__pyx_t_5); if (unlikely((__pyx_t_13 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 348, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       try {
-        __pyx_v_columns.push_back(__pyx_t_14);
+        __pyx_v_columns.push_back(__pyx_t_13);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 348, __pyx_L1_error)
       }
 
       /* "gdist.pyx":349
  *             rows.push_back(point)
  *             columns.push_back(target_indices[index_distance])
  *             distance_matrix.push_back(distance)             # <<<<<<<<<<<<<<
  *             # symmetric
  *             rows.push_back(target_indices[index_distance])
  */
-      __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_distance); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
+      __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_v_distance); if (unlikely((__pyx_t_14 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 349, __pyx_L1_error)
       try {
-        __pyx_v_distance_matrix.push_back(__pyx_t_15);
+        __pyx_v_distance_matrix.push_back(__pyx_t_14);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 349, __pyx_L1_error)
       }
 
       /* "gdist.pyx":351
  *             distance_matrix.push_back(distance)
  *             # symmetric
  *             rows.push_back(target_indices[index_distance])             # <<<<<<<<<<<<<<
  *             columns.push_back(point)
  *             distance_matrix.push_back(distance)
  */
-      __pyx_t_11 = __Pyx_PyObject_GetItem(__pyx_v_target_indices, __pyx_v_index_distance); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 351, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_14 = __Pyx_PyInt_As_unsigned_int(__pyx_t_11); if (unlikely((__pyx_t_14 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_target_indices, __pyx_v_index_distance); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_13 = __Pyx_PyInt_As_unsigned_int(__pyx_t_5); if (unlikely((__pyx_t_13 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       try {
-        __pyx_v_rows.push_back(__pyx_t_14);
+        __pyx_v_rows.push_back(__pyx_t_13);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 351, __pyx_L1_error)
       }
 
       /* "gdist.pyx":352
  *             # symmetric
  *             rows.push_back(target_indices[index_distance])
  *             columns.push_back(point)             # <<<<<<<<<<<<<<
  *             distance_matrix.push_back(distance)
  * 
  */
-      __pyx_t_14 = __Pyx_PyInt_As_unsigned_int(__pyx_v_point); if (unlikely((__pyx_t_14 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyInt_As_unsigned_int(__pyx_v_point); if (unlikely((__pyx_t_13 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 352, __pyx_L1_error)
       try {
-        __pyx_v_columns.push_back(__pyx_t_14);
+        __pyx_v_columns.push_back(__pyx_t_13);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 352, __pyx_L1_error)
       }
 
       /* "gdist.pyx":353
  *             rows.push_back(target_indices[index_distance])
  *             columns.push_back(point)
  *             distance_matrix.push_back(distance)             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t no_of_vertices = vertices.shape[0]
  */
-      __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_distance); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L1_error)
+      __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_v_distance); if (unlikely((__pyx_t_14 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 353, __pyx_L1_error)
       try {
-        __pyx_v_distance_matrix.push_back(__pyx_t_15);
+        __pyx_v_distance_matrix.push_back(__pyx_t_14);
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 353, __pyx_L1_error)
       }
 
       /* "gdist.pyx":346
  *         )
@@ -4347,15 +7703,16 @@
   /* "gdist.pyx":355
  *             distance_matrix.push_back(distance)
  * 
  *     cdef Py_ssize_t no_of_vertices = vertices.shape[0]             # <<<<<<<<<<<<<<
  *     return scipy.sparse.csc_matrix(
  *         (distance_matrix, (rows, columns)),
  */
-  __pyx_v_no_of_vertices = (__pyx_v_vertices->dimensions[0]);
+  __pyx_t_15 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_vertices)); if (unlikely(__pyx_t_15 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_v_no_of_vertices = (__pyx_t_15[0]);
 
   /* "gdist.pyx":356
  * 
  *     cdef Py_ssize_t no_of_vertices = vertices.shape[0]
  *     return scipy.sparse.csc_matrix(             # <<<<<<<<<<<<<<
  *         (distance_matrix, (rows, columns)),
  *         shape=(no_of_vertices, no_of_vertices)
@@ -4379,81 +7736,81 @@
  */
   __pyx_t_2 = __pyx_convert_vector_to_py_double(__pyx_v_distance_matrix); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = __pyx_convert_vector_to_py_unsigned_int(__pyx_v_rows); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = __pyx_convert_vector_to_py_unsigned_int(__pyx_v_columns); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 357, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_8);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_8)) __PYX_ERR(0, 357, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_7);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7)) __PYX_ERR(0, 357, __pyx_L1_error);
   __pyx_t_8 = 0;
   __pyx_t_7 = 0;
   __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_11);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_5)) __PYX_ERR(0, 357, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_11 = 0;
+  __pyx_t_5 = 0;
 
   /* "gdist.pyx":356
  * 
  *     cdef Py_ssize_t no_of_vertices = vertices.shape[0]
  *     return scipy.sparse.csc_matrix(             # <<<<<<<<<<<<<<
  *         (distance_matrix, (rows, columns)),
  *         shape=(no_of_vertices, no_of_vertices)
  */
-  __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 356, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error);
   __pyx_t_7 = 0;
 
   /* "gdist.pyx":358
  *     return scipy.sparse.csc_matrix(
  *         (distance_matrix, (rows, columns)),
  *         shape=(no_of_vertices, no_of_vertices)             # <<<<<<<<<<<<<<
  *     )
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_no_of_vertices); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_no_of_vertices); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 358, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8)) __PYX_ERR(0, 358, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_5) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_shape, __pyx_t_9) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
   /* "gdist.pyx":356
  * 
  *     cdef Py_ssize_t no_of_vertices = vertices.shape[0]
  *     return scipy.sparse.csc_matrix(             # <<<<<<<<<<<<<<
  *         (distance_matrix, (rows, columns)),
  *         shape=(no_of_vertices, no_of_vertices)
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_11, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_9;
+  __pyx_t_9 = 0;
   goto __pyx_L0;
 
   /* "gdist.pyx":287
  * 
  * 
  * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
  *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
@@ -4465,15 +7822,14 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_11);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_points.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_triangles.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vertices.rcbuffer->pybuffer);
@@ -4494,1480 +7850,241 @@
   __Pyx_XDECREF(__pyx_v_index_distance);
   __Pyx_XDECREF(__pyx_v_distance);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":735
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":736
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":735
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":738
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":739
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":738
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":741
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":742
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":741
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":744
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":745
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":744
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":747
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":748
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":747
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":750
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":751
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":752
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
- *     else:
- *         return ()
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":751
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":754
- *         return <tuple>d.subarray.shape
- *     else:
- *         return ()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
-    goto __pyx_L0;
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":750
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":929
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":930
- * 
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
- *     PyArray_SetBaseObject(arr, base)
- * 
- */
-  Py_INCREF(__pyx_v_base);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":931
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object get_array_base(ndarray arr):
- */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":929
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":933
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
-  PyObject *__pyx_v_base;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":934
- * 
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
- *     if base is NULL:
- *         return None
- */
-  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":935
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":936
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- *         return None             # <<<<<<<<<<<<<<
- *     return <object>base
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-    goto __pyx_L0;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":935
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":937
- *     if base is NULL:
- *         return None
- *     return <object>base             # <<<<<<<<<<<<<<
- * 
- * # Versions of the import_* functions which are more suitable for
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_base));
-  __pyx_r = ((PyObject *)__pyx_v_base);
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":933
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":942
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":943
- * cdef inline int import_array() except -1:
- *     try:
- *         __pyx_import_array()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
- */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":942
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":944
- *     try:
- *         __pyx_import_array()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":945
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_umath() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 945, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":942
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":941
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":947
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":948
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":949
- * cdef inline int import_umath() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":948
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":950
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":951
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_ufunc() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 951, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":948
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":947
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":953
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":954
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":955
- * cdef inline int import_ufunc() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":954
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":956
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":957
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef extern from *:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 957, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":954
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":953
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":979
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":967
- * 
- * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.timedelta64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":994
- *     bool
- *     """
- *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":982
- * 
- * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
- *     """
- *     Cython equivalent of `isinstance(obj, np.datetime64)`
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
-  npy_datetime __pyx_r;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1004
- *     also needed.  That can be found using `get_datetime64_unit`.
- *     """
- *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":997
- * 
- * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy datetime64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
-  npy_timedelta __pyx_r;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1011
- *     returns the int64 value underlying scalar numpy timedelta64 object
- *     """
- *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1007
- * 
- * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the int64 value underlying scalar numpy timedelta64 object
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
-  NPY_DATETIMEUNIT __pyx_r;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1018
- *     returns the unit part of the dtype for a numpy datetime64 object.
- *     """
- *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
- */
-  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
-  goto __pyx_L0;
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":1014
- * 
- * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  return __pyx_r;
-}
-
-/* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_unsigned_int")
- * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-static std::vector<unsigned int>  __pyx_convert_vector_from_py_unsigned_int(PyObject *__pyx_v_o) {
-  std::vector<unsigned int>  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<unsigned int>  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  unsigned int __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_unsigned_int", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(2, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(2, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __Pyx_PyInt_As_unsigned_int(__pyx_v_item); if (unlikely((__pyx_t_5 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(2, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((unsigned int)__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_unsigned_int")
- * cdef vector[X] __pyx_convert_vector_from_py_unsigned_int(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_unsigned_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_double", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = PyFloat_FromDouble((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_convert_vector_to_py_unsigned_int(const std::vector<unsigned int>  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_unsigned_int", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_unsigned_int")
- * cdef object __pyx_convert_vector_to_py_unsigned_int(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __Pyx_PyInt_From_unsigned_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_unsigned_int")
- * cdef object __pyx_convert_vector_to_py_unsigned_int(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_unsigned_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_gdist(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_gdist},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "gdist",
-    __pyx_k_This_module_defines_a_Cython_wr, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_Function_for_calculating_pairwis, __pyx_k_Function_for_calculating_pairwis, sizeof(__pyx_k_Function_for_calculating_pairwis), 0, 1, 0, 0},
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_N, __pyx_k_N, sizeof(__pyx_k_N), 0, 0, 1, 1},
-  {&__pyx_kp_u_This_is_the_wrapper_function_for, __pyx_k_This_is_the_wrapper_function_for, sizeof(__pyx_k_This_is_the_wrapper_function_for), 0, 1, 0, 0},
-  {&__pyx_kp_u_This_is_the_wrapper_function_for_2, __pyx_k_This_is_the_wrapper_function_for_2, sizeof(__pyx_k_This_is_the_wrapper_function_for_2), 0, 1, 0, 0},
-  {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
-  {&__pyx_n_s_amesh, __pyx_k_amesh, sizeof(__pyx_k_amesh), 0, 0, 1, 1},
-  {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
-  {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-  {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
-  {&__pyx_n_s_compute_gdist, __pyx_k_compute_gdist, sizeof(__pyx_k_compute_gdist), 0, 0, 1, 1},
-  {&__pyx_kp_u_compute_gdist_line_119, __pyx_k_compute_gdist_line_119, sizeof(__pyx_k_compute_gdist_line_119), 0, 1, 0, 0},
-  {&__pyx_n_s_csc_matrix, __pyx_k_csc_matrix, sizeof(__pyx_k_csc_matrix), 0, 0, 1, 1},
-  {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {&__pyx_n_s_distance, __pyx_k_distance, sizeof(__pyx_k_distance), 0, 0, 1, 1},
-  {&__pyx_n_s_distance_matrix, __pyx_k_distance_matrix, sizeof(__pyx_k_distance_matrix), 0, 0, 1, 1},
-  {&__pyx_n_s_distance_matrix_of_selected_poin, __pyx_k_distance_matrix_of_selected_poin, sizeof(__pyx_k_distance_matrix_of_selected_poin), 0, 0, 1, 1},
-  {&__pyx_kp_u_distance_matrix_of_selected_poin_2, __pyx_k_distance_matrix_of_selected_poin_2, sizeof(__pyx_k_distance_matrix_of_selected_poin_2), 0, 1, 0, 0},
-  {&__pyx_n_s_distances, __pyx_k_distances, sizeof(__pyx_k_distances), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
-  {&__pyx_n_s_faces, __pyx_k_faces, sizeof(__pyx_k_faces), 0, 0, 1, 1},
-  {&__pyx_n_s_flatten, __pyx_k_flatten, sizeof(__pyx_k_flatten), 0, 0, 1, 1},
-  {&__pyx_n_s_gdist, __pyx_k_gdist, sizeof(__pyx_k_gdist), 0, 0, 1, 1},
-  {&__pyx_kp_s_gdist_pyx, __pyx_k_gdist_pyx, sizeof(__pyx_k_gdist_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_index_distance, __pyx_k_index_distance, sizeof(__pyx_k_index_distance), 0, 0, 1, 1},
-  {&__pyx_n_s_index_point, __pyx_k_index_point, sizeof(__pyx_k_index_point), 0, 0, 1, 1},
-  {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
-  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
-  {&__pyx_n_s_is_one_indexed, __pyx_k_is_one_indexed, sizeof(__pyx_k_is_one_indexed), 0, 0, 1, 1},
-  {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
-  {&__pyx_n_s_kk, __pyx_k_kk, sizeof(__pyx_k_kk), 0, 0, 1, 1},
-  {&__pyx_n_s_local_gdist_matrix, __pyx_k_local_gdist_matrix, sizeof(__pyx_k_local_gdist_matrix), 0, 0, 1, 1},
-  {&__pyx_kp_u_local_gdist_matrix_line_198, __pyx_k_local_gdist_matrix_line_198, sizeof(__pyx_k_local_gdist_matrix_line_198), 0, 1, 0, 0},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_max_distance, __pyx_k_max_distance, sizeof(__pyx_k_max_distance), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_no_of_vertices, __pyx_k_no_of_vertices, sizeof(__pyx_k_no_of_vertices), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-  {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
-  {&__pyx_n_s_point, __pyx_k_point, sizeof(__pyx_k_point), 0, 0, 1, 1},
-  {&__pyx_n_s_points, __pyx_k_points, sizeof(__pyx_k_points), 0, 0, 1, 1},
-  {&__pyx_n_s_propagate_on_max_distance, __pyx_k_propagate_on_max_distance, sizeof(__pyx_k_propagate_on_max_distance), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_s_rows, __pyx_k_rows, sizeof(__pyx_k_rows), 0, 0, 1, 1},
-  {&__pyx_n_s_scipy, __pyx_k_scipy, sizeof(__pyx_k_scipy), 0, 0, 1, 1},
-  {&__pyx_n_s_scipy_sparse, __pyx_k_scipy_sparse, sizeof(__pyx_k_scipy_sparse), 0, 0, 1, 1},
-  {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
-  {&__pyx_n_s_source, __pyx_k_source, sizeof(__pyx_k_source), 0, 0, 1, 1},
-  {&__pyx_n_s_source_index, __pyx_k_source_index, sizeof(__pyx_k_source_index), 0, 0, 1, 1},
-  {&__pyx_n_s_source_indices, __pyx_k_source_indices, sizeof(__pyx_k_source_indices), 0, 0, 1, 1},
-  {&__pyx_n_s_sparse, __pyx_k_sparse, sizeof(__pyx_k_sparse), 0, 0, 1, 1},
-  {&__pyx_n_s_target_indices, __pyx_k_target_indices, sizeof(__pyx_k_target_indices), 0, 0, 1, 1},
-  {&__pyx_n_s_targets, __pyx_k_targets, sizeof(__pyx_k_targets), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_triangles, __pyx_k_triangles, sizeof(__pyx_k_triangles), 0, 0, 1, 1},
-  {&__pyx_n_s_vertices, __pyx_k_vertices, sizeof(__pyx_k_vertices), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_u_Function_for_calculating_pairwis, __pyx_k_Function_for_calculating_pairwis, sizeof(__pyx_k_Function_for_calculating_pairwis), 0, 1, 0, 0},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_n_s_N, __pyx_k_N, sizeof(__pyx_k_N), 0, 0, 1, 1},
+    {&__pyx_kp_u_This_is_the_wrapper_function_for, __pyx_k_This_is_the_wrapper_function_for, sizeof(__pyx_k_This_is_the_wrapper_function_for), 0, 1, 0, 0},
+    {&__pyx_kp_u_This_is_the_wrapper_function_for_2, __pyx_k_This_is_the_wrapper_function_for_2, sizeof(__pyx_k_This_is_the_wrapper_function_for_2), 0, 1, 0, 0},
+    {&__pyx_n_s__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 1, 1},
+    {&__pyx_n_s__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 1, 1},
+    {&__pyx_n_s_algorithm, __pyx_k_algorithm, sizeof(__pyx_k_algorithm), 0, 0, 1, 1},
+    {&__pyx_n_s_amesh, __pyx_k_amesh, sizeof(__pyx_k_amesh), 0, 0, 1, 1},
+    {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
+    {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
+    {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_columns, __pyx_k_columns, sizeof(__pyx_k_columns), 0, 0, 1, 1},
+    {&__pyx_n_s_compute_gdist, __pyx_k_compute_gdist, sizeof(__pyx_k_compute_gdist), 0, 0, 1, 1},
+    {&__pyx_kp_u_compute_gdist_line_119, __pyx_k_compute_gdist_line_119, sizeof(__pyx_k_compute_gdist_line_119), 0, 1, 0, 0},
+    {&__pyx_n_s_csc_matrix, __pyx_k_csc_matrix, sizeof(__pyx_k_csc_matrix), 0, 0, 1, 1},
+    {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+    {&__pyx_n_s_distance, __pyx_k_distance, sizeof(__pyx_k_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_distance_matrix, __pyx_k_distance_matrix, sizeof(__pyx_k_distance_matrix), 0, 0, 1, 1},
+    {&__pyx_n_s_distance_matrix_of_selected_poin, __pyx_k_distance_matrix_of_selected_poin, sizeof(__pyx_k_distance_matrix_of_selected_poin), 0, 0, 1, 1},
+    {&__pyx_kp_u_distance_matrix_of_selected_poin_2, __pyx_k_distance_matrix_of_selected_poin_2, sizeof(__pyx_k_distance_matrix_of_selected_poin_2), 0, 1, 0, 0},
+    {&__pyx_n_s_distances, __pyx_k_distances, sizeof(__pyx_k_distances), 0, 0, 1, 1},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
+    {&__pyx_n_s_faces, __pyx_k_faces, sizeof(__pyx_k_faces), 0, 0, 1, 1},
+    {&__pyx_n_s_flatten, __pyx_k_flatten, sizeof(__pyx_k_flatten), 0, 0, 1, 1},
+    {&__pyx_n_s_gdist, __pyx_k_gdist, sizeof(__pyx_k_gdist), 0, 0, 1, 1},
+    {&__pyx_kp_s_gdist_pyx, __pyx_k_gdist_pyx, sizeof(__pyx_k_gdist_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_index_distance, __pyx_k_index_distance, sizeof(__pyx_k_index_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_index_point, __pyx_k_index_point, sizeof(__pyx_k_index_point), 0, 0, 1, 1},
+    {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_n_s_is_one_indexed, __pyx_k_is_one_indexed, sizeof(__pyx_k_is_one_indexed), 0, 0, 1, 1},
+    {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
+    {&__pyx_n_s_kk, __pyx_k_kk, sizeof(__pyx_k_kk), 0, 0, 1, 1},
+    {&__pyx_n_s_local_gdist_matrix, __pyx_k_local_gdist_matrix, sizeof(__pyx_k_local_gdist_matrix), 0, 0, 1, 1},
+    {&__pyx_kp_u_local_gdist_matrix_line_198, __pyx_k_local_gdist_matrix_line_198, sizeof(__pyx_k_local_gdist_matrix_line_198), 0, 1, 0, 0},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_max_distance, __pyx_k_max_distance, sizeof(__pyx_k_max_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_no_of_vertices, __pyx_k_no_of_vertices, sizeof(__pyx_k_no_of_vertices), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_n_s_point, __pyx_k_point, sizeof(__pyx_k_point), 0, 0, 1, 1},
+    {&__pyx_n_s_points, __pyx_k_points, sizeof(__pyx_k_points), 0, 0, 1, 1},
+    {&__pyx_n_s_propagate_on_max_distance, __pyx_k_propagate_on_max_distance, sizeof(__pyx_k_propagate_on_max_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_rows, __pyx_k_rows, sizeof(__pyx_k_rows), 0, 0, 1, 1},
+    {&__pyx_n_s_scipy, __pyx_k_scipy, sizeof(__pyx_k_scipy), 0, 0, 1, 1},
+    {&__pyx_n_s_scipy_sparse, __pyx_k_scipy_sparse, sizeof(__pyx_k_scipy_sparse), 0, 0, 1, 1},
+    {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
+    {&__pyx_n_s_source, __pyx_k_source, sizeof(__pyx_k_source), 0, 0, 1, 1},
+    {&__pyx_n_s_source_index, __pyx_k_source_index, sizeof(__pyx_k_source_index), 0, 0, 1, 1},
+    {&__pyx_n_s_source_indices, __pyx_k_source_indices, sizeof(__pyx_k_source_indices), 0, 0, 1, 1},
+    {&__pyx_n_s_sparse, __pyx_k_sparse, sizeof(__pyx_k_sparse), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_target_indices, __pyx_k_target_indices, sizeof(__pyx_k_target_indices), 0, 0, 1, 1},
+    {&__pyx_n_s_targets, __pyx_k_targets, sizeof(__pyx_k_targets), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_triangles, __pyx_k_triangles, sizeof(__pyx_k_triangles), 0, 0, 1, 1},
+    {&__pyx_n_s_vertices, __pyx_k_vertices, sizeof(__pyx_k_vertices), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 261, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 331, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "gdist.pyx":173
- * 
- *     if source_indices is None:
- *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0             # <<<<<<<<<<<<<<
- *     if target_indices is None:
- *         propagate_on_max_distance = True
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_int_1); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 173, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 945, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-1u_x3p6c/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-um2de17m/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 951, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "gdist.pyx":173
+ * 
+ *     if source_indices is None:
+ *         source_indices = numpy.arange(1, dtype=numpy.int32)  # default to 0             # <<<<<<<<<<<<<<
+ *     if target_indices is None:
+ *         propagate_on_max_distance = True
+ */
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_1); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "gdist.pyx":55
+ * 
+ * # For csc_matrix returned by local_gdist_matrix()
+ * import scipy.sparse             # <<<<<<<<<<<<<<
+ * 
+ * # Pre-cdef'd containers from the C++ standard library
+ */
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_scipy, __pyx_n_s_sparse); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "gdist.pyx":119
  * 
  * 
  * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
  */
-  __pyx_tuple__7 = PyTuple_Pack(11, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_source_indices, __pyx_n_s_target_indices, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_propagate_on_max_distance, __pyx_n_s_points, __pyx_n_s_faces, __pyx_n_s_k, __pyx_n_s_distances); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(6, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_compute_gdist, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(11, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_source_indices, __pyx_n_s_target_indices, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_propagate_on_max_distance, __pyx_n_s_points, __pyx_n_s_faces, __pyx_n_s_k, __pyx_n_s_distances); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_compute_gdist, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   /* "gdist.pyx":198
  * 
  * 
  * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
  *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                        double max_distance=GEODESIC_INF,
  */
-  __pyx_tuple__9 = PyTuple_Pack(15, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_amesh, __pyx_n_s_algorithm, __pyx_n_s_source, __pyx_n_s_targets, __pyx_n_s_N, __pyx_n_s_k, __pyx_n_s_kk, __pyx_n_s_distance, __pyx_n_s_rows, __pyx_n_s_columns, __pyx_n_s_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_local_gdist_matrix, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(15, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_amesh, __pyx_n_s_algorithm, __pyx_n_s_source, __pyx_n_s_targets, __pyx_n_s_N, __pyx_n_s_k, __pyx_n_s_kk, __pyx_n_s_distance, __pyx_n_s_rows, __pyx_n_s_columns, __pyx_n_s_data); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_local_gdist_matrix, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 198, __pyx_L1_error)
 
   /* "gdist.pyx":287
  * 
  * 
  * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
  *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
  *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  */
-  __pyx_tuple__11 = PyTuple_Pack(16, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_points, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_rows, __pyx_n_s_columns, __pyx_n_s_distance_matrix, __pyx_n_s_index_point, __pyx_n_s_point, __pyx_n_s_target_indices, __pyx_n_s_source_index, __pyx_n_s_distances, __pyx_n_s_index_distance, __pyx_n_s_distance, __pyx_n_s_no_of_vertices); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(5, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_distance_matrix_of_selected_poin, 287, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(16, __pyx_n_s_vertices, __pyx_n_s_triangles, __pyx_n_s_points, __pyx_n_s_max_distance, __pyx_n_s_is_one_indexed, __pyx_n_s_rows, __pyx_n_s_columns, __pyx_n_s_distance_matrix, __pyx_n_s_index_point, __pyx_n_s_point, __pyx_n_s_target_indices, __pyx_n_s_source_index, __pyx_n_s_distances, __pyx_n_s_index_distance, __pyx_n_s_distance, __pyx_n_s_no_of_vertices); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_gdist_pyx, __pyx_n_s_distance_matrix_of_selected_poin, 287, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#ifndef NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -6011,55 +8128,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6078,14 +8181,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_gdist(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_gdist},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "gdist",
+      __pyx_k_This_module_defines_a_Cython_wr, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -6128,42 +8280,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -6171,251 +8337,290 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_gdist(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'gdist' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("gdist", __pyx_methods, __pyx_k_This_module_defines_a_Cython_wr, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "gdist" pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_gdist(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("gdist", __pyx_methods, __pyx_k_This_module_defines_a_Cython_wr, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_gdist) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "gdist")) {
-      if (unlikely(PyDict_SetItemString(modules, "gdist", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "gdist", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "gdist.pyx":51
  * 
  * # For compatible datatypes
  * import numpy             # <<<<<<<<<<<<<<
  * cimport numpy
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_numpy, __pyx_t_1) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_numpy, __pyx_t_2) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "gdist.pyx":55
  * 
  * # For csc_matrix returned by local_gdist_matrix()
  * import scipy.sparse             # <<<<<<<<<<<<<<
  * 
  * # Pre-cdef'd containers from the C++ standard library
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_scipy_sparse, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_scipy, __pyx_t_1) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_scipy_sparse, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_scipy, __pyx_t_2) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "gdist.pyx":119
+ * 
+ * 
+ * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
+ *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5gdist_1compute_gdist, 0, __pyx_n_s_compute_gdist, NULL, __pyx_n_s_gdist, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 0)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   /* "gdist.pyx":123
  *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
  *                   numpy.ndarray[numpy.int32_t, ndim=1] target_indices=None,
  *                   double max_distance=GEODESIC_INF,             # <<<<<<<<<<<<<<
  *                   bool is_one_indexed=False):
  *     """This is the wrapper function for computing geodesic distance between a
  */
-  __pyx_k_ = geodesic::GEODESIC_INF;
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_max_distance = geodesic::GEODESIC_INF;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_5gdist_6__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_gdist, __pyx_t_2) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gdist.pyx":119
+  /* "gdist.pyx":198
  * 
  * 
- * def compute_gdist(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
- *                   numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- *                   numpy.ndarray[numpy.int32_t, ndim=1] source_indices=None,
+ * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
+ *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
+ *                        double max_distance=GEODESIC_INF,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5gdist_1compute_gdist, NULL, __pyx_n_s_gdist); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_gdist, __pyx_t_1) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5gdist_3local_gdist_matrix, 0, __pyx_n_s_local_gdist_matrix, NULL, __pyx_n_s_gdist, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults1), 0)) __PYX_ERR(0, 198, __pyx_L1_error)
 
   /* "gdist.pyx":200
  * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,
  *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *                        double max_distance=GEODESIC_INF,             # <<<<<<<<<<<<<<
  *                        bool is_one_indexed=False):
  *     """This is the wrapper function for computing geodesic distance from every
  */
-  __pyx_k__3 = geodesic::GEODESIC_INF;
+  __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_2)->__pyx_arg_max_distance = geodesic::GEODESIC_INF;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_5gdist_8__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_local_gdist_matrix, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "gdist.pyx":198
+  /* "gdist.pyx":287
  * 
  * 
- * def local_gdist_matrix(numpy.ndarray[numpy.float64_t, ndim=2] vertices,             # <<<<<<<<<<<<<<
- *                        numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- *                        double max_distance=GEODESIC_INF,
+ * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
+ *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
+ *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5gdist_3local_gdist_matrix, NULL, __pyx_n_s_gdist); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_local_gdist_matrix, __pyx_t_1) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_5gdist_5distance_matrix_of_selected_points, 0, __pyx_n_s_distance_matrix_of_selected_poin, NULL, __pyx_n_s_gdist, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 0)) __PYX_ERR(0, 287, __pyx_L1_error)
 
   /* "gdist.pyx":291
  *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
  *     numpy.ndarray[numpy.int32_t, ndim=1] points,
  *     double max_distance=GEODESIC_INF,             # <<<<<<<<<<<<<<
  *     bool is_one_indexed=False
  * ):
  */
-  __pyx_k__4 = geodesic::GEODESIC_INF;
-
-  /* "gdist.pyx":287
- * 
- * 
- * def distance_matrix_of_selected_points(             # <<<<<<<<<<<<<<
- *     numpy.ndarray[numpy.float64_t, ndim=2] vertices,
- *     numpy.ndarray[numpy.int32_t, ndim=2] triangles,
- */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_5gdist_5distance_matrix_of_selected_points, NULL, __pyx_n_s_gdist); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distance_matrix_of_selected_poin, __pyx_t_1) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_max_distance = geodesic::GEODESIC_INF;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_5gdist_10__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_distance_matrix_of_selected_poin, __pyx_t_2) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "gdist.pyx":1
  * # -*- coding: utf-8 -*-             # <<<<<<<<<<<<<<
  * #
  * #
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_compute_gdist_line_119, __pyx_kp_u_This_is_the_wrapper_function_for) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_local_gdist_matrix_line_198, __pyx_kp_u_This_is_the_wrapper_function_for_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_distance_matrix_of_selected_poin_2, __pyx_kp_u_Function_for_calculating_pairwis) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_unsigned_int")
- * cdef object __pyx_convert_vector_to_py_unsigned_int(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_compute_gdist_line_119, __pyx_kp_u_This_is_the_wrapper_function_for) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_local_gdist_matrix_line_198, __pyx_kp_u_This_is_the_wrapper_function_for_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_distance_matrix_of_selected_poin_2, __pyx_kp_u_Function_for_calculating_pairwis) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init gdist", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init gdist");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -6427,42 +8632,536 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+#endif
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+#endif
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
     uint32_t u32;
     uint8_t u8[4];
   } S;
@@ -6542,15 +9241,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -6592,15 +9291,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -6624,15 +9324,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -6789,56 +9490,62 @@
       }
     }
   } while (ctx->enc_count);
   ctx->enc_type = 0;
   ctx->is_complex = 0;
   return 0;
 }
-static PyObject *
+static int
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
     int i = 0, number, ndim;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
-        return NULL;
+        return -1;
     }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return -1;
     ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
+        if (number == -1) return -1;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i]) {
+            PyErr_Format(PyExc_ValueError,
                         "Expected a dimension of size %zu, got %d",
                         ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
+            return -1;
+        }
+        if (*ts != ',' && *ts != ')') {
+            PyErr_Format(PyExc_ValueError,
                                 "Expected a comma in format string, got '%c'", *ts);
+            return -1;
+        }
         if (*ts == ',') ts++;
         i++;
     }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+    if (i != ndim) {
+        PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
                             ctx->head->field->type->ndim, i);
+        return -1;
+    }
     if (!*ts) {
         PyErr_SetString(PyExc_ValueError,
                         "Unexpected end of format string, expected ')'");
-        return NULL;
+        return -1;
     }
     ctx->is_valid_array = 1;
     ctx->new_count = 1;
     *tsp = ++ts;
-    return Py_None;
+    return 0;
 }
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
   int got_Z = 0;
   while (1) {
     switch(*ts) {
       case 0:
         if (ctx->enc_type != 0 && ctx->head == NULL) {
@@ -6956,15 +9663,15 @@
         break;
       case ':':
         ++ts;
         while(*ts != ':') ++ts;
         ++ts;
         break;
       case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        if (__pyx_buffmt_parse_array(ctx, &ts) < 0) return NULL;
         break;
       default:
         {
           int number = __Pyx_BufFmt_ExpectNumber(&ts);
           if (number == -1) return NULL;
           ctx->new_count = (size_t)number;
         }
@@ -7016,15 +9723,15 @@
   return 0;
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
 /* PyFunctionFastCall */
-  #if CYTHON_FAST_PYCALL
+  #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -7045,15 +9752,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -7061,17 +9767,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    #if PY_MAJOR_VERSION < 3
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -7132,164 +9844,342 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
-
-/* PyObjectCall */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
 
 /* PyObjectCallMethO */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallNoArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
-    }
-#endif
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
-#else
-    if (likely(PyCFunction_Check(func)))
+/* PyObjectFastCall */
+  #if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result = 0;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
+    Py_DECREF(argstuple);
+    return result;
+}
 #endif
-    {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
             return __Pyx_PyObject_CallMethO(func, NULL);
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
+    }
+#endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
+    }
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
-#endif
 
-/* PyCFunctionFastCall */
-  #if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+/* TupleAndListFromArray */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
     }
 }
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
 #endif
 
-/* PyObjectCallOneArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+/* BytesEquals */
+  static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+
+/* UnicodeEquals */
+  static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
     }
 #endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
 #endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
         }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
 #endif
+}
 
-/* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+/* fastcall */
+  #if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;
+            return kwvalues[i];
+        }
+    }
+    return NULL;
 }
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
   static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -7326,38 +10216,83 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
   static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        Py_XDECREF(key); key = NULL;
+        Py_XDECREF(value); value = NULL;
+        if (kwds_is_tuple) {
+            Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(kwds);
+#else
+            size = PyTuple_Size(kwds);
+            if (size < 0) goto bad;
+#endif
+            if (pos >= size) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            key = __Pyx_PySequence_ITEM(kwds, pos);
+            if (!key) goto bad;
+#elif CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kwds, pos);
+#else
+            key = PyTuple_GetItem(kwds, pos);
+            if (!key) goto bad;
+#endif
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(key);
+#endif
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(value);
+            Py_DECREF(key);
+#endif
+            key = NULL;
+            value = NULL;
             continue;
         }
+#if !CYTHON_AVOID_BORROWED_REFS
+        Py_INCREF(key);
+#endif
+        Py_INCREF(value);
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -7370,22 +10305,26 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -7404,53 +10343,64 @@
             goto invalid_keyword_type;
         if (kwds2) {
             if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
         } else {
             goto invalid_keyword;
         }
     }
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return 0;
 arg_passed_twice:
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return -1;
 }
 
 /* ArgTypeTest */
   static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* PyDictVersioning */
   #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
@@ -7481,22 +10431,30 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -7509,155 +10467,137 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* ExtTypeTest */
   static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
-/* PyObjectCall2Args */
-  static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
 /* PyIntBinop */
   #if !CYTHON_COMPILING_IN_PYPY
-static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, int inplace, int zerodivision_check) {
-    (void)inplace;
-    (void)zerodivision_check;
+static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
+    CYTHON_MAYBE_UNUSED_VAR(intval);
+    CYTHON_MAYBE_UNUSED_VAR(inplace);
+    CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
         long a = PyInt_AS_LONG(op1);
-            x = (long)((unsigned long)a + b);
+        
+            x = (long)((unsigned long)a + (unsigned long)b);
             if (likely((x^a) >= 0 || (x^b) >= 0))
                 return PyInt_FromLong(x);
             return PyLong_Type.tp_as_number->nb_add(op1, op2);
     }
     #endif
     #if CYTHON_USE_PYLONG_INTERNALS
     if (likely(PyLong_CheckExact(op1))) {
         const long b = intval;
         long a, x;
 #ifdef HAVE_LONG_LONG
         const PY_LONG_LONG llb = intval;
         PY_LONG_LONG lla, llx;
 #endif
-        const digit* digits = ((PyLongObject*)op1)->ob_digit;
-        const Py_ssize_t size = Py_SIZE(op1);
-        if (likely(__Pyx_sst_abs(size) <= 1)) {
-            a = likely(size) ? digits[0] : 0;
-            if (size == -1) a = -a;
+        if (unlikely(__Pyx_PyLong_IsZero(op1))) {
+            return __Pyx_NewRef(op2);
+        }
+        if (likely(__Pyx_PyLong_IsCompact(op1))) {
+            a = __Pyx_PyLong_CompactValue(op1);
         } else {
+            const digit* digits = __Pyx_PyLong_Digits(op1);
+            const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(op1);
             switch (size) {
                 case -2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 2:
                     if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
                         a = (long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 3:
                     if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
                         a = (long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case -4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = -(PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 case 4:
                     if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
                         a = (long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         break;
-#ifdef HAVE_LONG_LONG
+                    #ifdef HAVE_LONG_LONG
                     } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
                         lla = (PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         goto long_long;
-#endif
+                    #endif
                     }
                     CYTHON_FALLTHROUGH;
                 default: return PyLong_Type.tp_as_number->nb_add(op1, op2);
             }
         }
                 x = a + b;
             return PyLong_FromLong(x);
@@ -7668,29 +10608,34 @@
 #endif
         
         
     }
     #endif
     if (PyFloat_CheckExact(op1)) {
         const long b = intval;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        double a = __pyx_PyFloat_AsDouble(op1);
+#else
         double a = PyFloat_AS_DOUBLE(op1);
+#endif
             double result;
+            
             PyFPE_START_PROTECT("add", return NULL)
             result = ((double)a) + (double)b;
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
 /* GetItemInt */
   static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (!j) return NULL;
+    if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -7743,428 +10688,168 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return m->sq_item(o, i);
+            return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* PyObjectCallOneArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
-    PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
-    if (unlikely(!(m && m->sq_item))) {
-        PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
-        return NULL;
-    }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
         return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
     }
     if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
         PyErr_Clear();
-        PyErr_Format(PyExc_IndexError, "cannot fit '%.200s' into an index-sized integer", Py_TYPE(index)->tp_name);
+        PyErr_Format(PyExc_IndexError,
+            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
+        __Pyx_DECREF_TypeName(index_type_name);
     }
     return NULL;
 }
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key) {
-    PyMappingMethods *m = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(m && m->mp_subscript)) {
-        return m->mp_subscript(obj, key);
-    }
-    return __Pyx_PyObject_GetIndex(obj, key);
-}
-#endif
-
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
+static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
+    __Pyx_TypeName obj_type_name;
+    if (likely(PyType_Check(obj))) {
+        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
+        if (!meth) {
+            PyErr_Clear();
+        } else {
+            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
+            Py_DECREF(meth);
+            return result;
         }
     }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return NULL;
 }
-#else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
-            }
-        }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
-    }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyMappingMethods *mm = tp->tp_as_mapping;
+    PySequenceMethods *sm = tp->tp_as_sequence;
+    if (likely(mm && mm->mp_subscript)) {
+        return mm->mp_subscript(obj, key);
     }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
-        }
-#endif
+    if (likely(sm && sm->sq_item)) {
+        return __Pyx_PyObject_GetIndex(obj, key);
     }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
+    return __Pyx_PyObject_GetItem_Slow(obj, key);
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8172,99 +10857,1471 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__4;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
+        if (unlikely(!op->func_doc)) return NULL;
+#else
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+#endif
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_name = PyObject_GetAttrString(op->func, "__name__");
+#elif PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+#if CYTHON_ASSUME_SAFE_MACROS
+        PyList_SET_ITEM(fromlist, 0, marker);
+#else
+        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
+            Py_DECREF(marker);
+            Py_DECREF(fromlist);
+            return NULL;
+        }
+#endif
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *
+__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_GetAttrString(op->func, "__module__");
+}
+static int
+__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_SetAttrString(op->func, "__module__", value);
+}
+#endif
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+#if CYTHON_COMPILING_IN_LIMITED_API
+    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
+#endif
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#endif
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+#endif
+    if (unlikely(op == NULL))
+        return NULL;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
+    if (unlikely(!op->func)) return NULL;
+#endif
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+#endif
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    Py_XINCREF(module);
+    cf->m_module = module;
+#endif
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_CLEAR(m->func);
+#else
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+#endif
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(m->func);
+#else
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+#endif
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+#endif
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
+    PyObject *py_name = NULL;
+    PyCFunction meth;
+    int flags;
+    meth = PyCFunction_GetFunction(f);
+    if (unlikely(!meth)) return NULL;
+    flags = PyCFunction_GetFlags(f);
+    if (unlikely(flags < 0)) return NULL;
+#else
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    int flags = f->m_ml->ml_flags;
+#endif
+    Py_ssize_t size;
+    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+#endif
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+#endif
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+#if CYTHON_COMPILING_IN_LIMITED_API
+    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+    if (!py_name) return NULL;
+    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
+                 py_name);
+    Py_DECREF(py_name);
+#else
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+#endif
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *self, *result;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
+    if (unlikely(!self) && PyErr_Occurred()) return NULL;
+#else
+    self = ((PyCFunctionObject*)func)->m_self;
+#endif
+    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
+    return result;
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+#if CYTHON_ASSUME_SAFE_MACROS
+        argc = PyTuple_GET_SIZE(args);
+#else
+        argc = PyTuple_Size(args);
+        if (unlikely(!argc) < 0) return NULL;
+#endif
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
@@ -8278,15 +12335,16 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -8356,25 +12414,109 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyCode_Replace_For_AddTraceback(PyObject *code, PyObject *scratch_dict,
+                                                       PyObject *firstlineno, PyObject *name) {
+    PyObject *replace = NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_firstlineno", firstlineno))) return NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_name", name))) return NULL;
+    replace = PyObject_GetAttrString(code, "replace");
+    if (likely(replace)) {
+        PyObject *result;
+        result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
+        Py_DECREF(replace);
+        return result;
+    }
+    PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
+    {
+        PyObject *compiled = NULL, *result = NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
+        compiled = Py_CompileString(
+            "out = type(code)(\n"
+            "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
+            "  code.co_flags, code.co_code, code.co_consts, code.co_names,\n"
+            "  code.co_varnames, code.co_filename, co_name, co_firstlineno,\n"
+            "  code.co_lnotab)\n", "<dummy>", Py_file_input);
+        if (!compiled) return NULL;
+        result = PyEval_EvalCode(compiled, scratch_dict, scratch_dict);
+        Py_DECREF(compiled);
+        if (!result) PyErr_Print();
+        Py_DECREF(result);
+        result = PyDict_GetItemString(scratch_dict, "out");
+        if (result) Py_INCREF(result);
+        return result;
+    }
+    #else
+    return NULL;
+    #endif
+}
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
+    PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
+    PyObject *exc_type, *exc_value, *exc_traceback;
+    int success = 0;
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    PyErr_Fetch(&exc_type, &exc_value, &exc_traceback);
+    code_object = Py_CompileString("_getframe()", filename, Py_eval_input);
+    if (unlikely(!code_object)) goto bad;
+    py_py_line = PyLong_FromLong(py_line);
+    if (unlikely(!py_py_line)) goto bad;
+    py_funcname = PyUnicode_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    dict = PyDict_New();
+    if (unlikely(!dict)) goto bad;
+    {
+        PyObject *old_code_object = code_object;
+        code_object = __Pyx_PyCode_Replace_For_AddTraceback(code_object, dict, py_py_line, py_funcname);
+        Py_DECREF(old_code_object);
+    }
+    if (unlikely(!code_object)) goto bad;
+    getframe = PySys_GetObject("_getframe");
+    if (unlikely(!getframe)) goto bad;
+    if (unlikely(PyDict_SetItemString(dict, "_getframe", getframe))) goto bad;
+    frame = PyEval_EvalCode(code_object, dict, dict);
+    if (unlikely(!frame) || frame == Py_None) goto bad;
+    success = 1;
+  bad:
+    PyErr_Restore(exc_type, exc_value, exc_traceback);
+    Py_XDECREF(code_object);
+    Py_XDECREF(py_py_line);
+    Py_XDECREF(py_funcname);
+    Py_XDECREF(dict);
+    Py_XDECREF(replace);
+    if (success) {
+        PyTraceBack_Here(
+            (struct _frame*)frame);
+    }
+    Py_XDECREF(frame);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -8401,14 +12543,15 @@
     #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
@@ -8416,15 +12559,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -8463,19 +12606,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -8507,15 +12656,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -8527,15 +12676,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -8661,15 +12810,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -8681,15 +12830,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -8827,177 +12976,254 @@
     const npy_int32 neg_one = (npy_int32) -1, const_zero = (npy_int32) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(npy_int32) < sizeof(long)) {
+        if ((sizeof(npy_int32) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(npy_int32, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (npy_int32) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (npy_int32) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(npy_int32, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(npy_int32) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 2 * PyLong_SHIFT) {
-                            return (npy_int32) (((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(npy_int32, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(npy_int32) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) >= 2 * PyLong_SHIFT)) {
+                                return (npy_int32) (((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(npy_int32) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 3 * PyLong_SHIFT) {
-                            return (npy_int32) (((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(npy_int32) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) >= 3 * PyLong_SHIFT)) {
+                                return (npy_int32) (((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(npy_int32) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT) {
-                            return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(npy_int32) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) >= 4 * PyLong_SHIFT)) {
+                                return (npy_int32) (((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (npy_int32) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(npy_int32) <= sizeof(unsigned long)) {
+            if ((sizeof(npy_int32) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(npy_int32, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(npy_int32) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(npy_int32) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(npy_int32, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (npy_int32) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(npy_int32, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(npy_int32,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(npy_int32) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(npy_int32, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(npy_int32) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT)) {
+                                return (npy_int32) (((npy_int32)-1)*(((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(npy_int32) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(npy_int32) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT)) {
+                                return (npy_int32) ((((((npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(npy_int32) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT)) {
+                                return (npy_int32) (((npy_int32)-1)*(((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(npy_int32) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(npy_int32) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT)) {
+                                return (npy_int32) ((((((((npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT) {
-                            return (npy_int32) (((npy_int32)-1)*(((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(npy_int32) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT)) {
+                                return (npy_int32) (((npy_int32)-1)*(((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(npy_int32) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT) {
-                            return (npy_int32) ((((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(npy_int32) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(npy_int32, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(npy_int32) - 1 > 4 * PyLong_SHIFT)) {
+                                return (npy_int32) ((((((((((npy_int32)digits[3]) << PyLong_SHIFT) | (npy_int32)digits[2]) << PyLong_SHIFT) | (npy_int32)digits[1]) << PyLong_SHIFT) | (npy_int32)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(npy_int32) <= sizeof(long)) {
+            if ((sizeof(npy_int32) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(npy_int32, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(npy_int32) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(npy_int32) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(npy_int32, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             npy_int32 val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (npy_int32) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (npy_int32) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (npy_int32) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (npy_int32) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (npy_int32) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(npy_int32) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((npy_int32) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(npy_int32) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((npy_int32) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((npy_int32) 1) << (sizeof(npy_int32) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (npy_int32) -1;
         }
     } else {
         npy_int32 val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (npy_int32) -1;
         val = __Pyx_PyInt_As_npy_int32(tmp);
@@ -9023,177 +13249,254 @@
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(unsigned int) < sizeof(long)) {
+        if ((sizeof(unsigned int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(unsigned int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (unsigned int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(unsigned int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) >= 2 * PyLong_SHIFT) {
-                            return (unsigned int) (((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(unsigned int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 2 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) >= 3 * PyLong_SHIFT) {
-                            return (unsigned int) (((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(unsigned int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 3 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
-                            return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(unsigned int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT)) {
+                                return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (unsigned int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(unsigned int) <= sizeof(unsigned long)) {
+            if ((sizeof(unsigned int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (unsigned int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(unsigned int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(unsigned int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(unsigned int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned int) (((unsigned int)-1)*(((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(unsigned int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(unsigned int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(unsigned int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT) {
-                            return (unsigned int) ((((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(unsigned int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned int) (((unsigned int)-1)*(((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(unsigned int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(unsigned int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT) {
-                            return (unsigned int) ((((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(unsigned int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((((unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned int) (((unsigned int)-1)*(((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(unsigned int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned int) (((unsigned int)-1)*(((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(unsigned int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT) {
-                            return (unsigned int) ((((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(unsigned int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(unsigned int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(unsigned int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (unsigned int) ((((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(unsigned int) <= sizeof(long)) {
+            if ((sizeof(unsigned int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(unsigned int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(unsigned int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(unsigned int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             unsigned int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (unsigned int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (unsigned int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (unsigned int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (unsigned int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (unsigned int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(unsigned int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((unsigned int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(unsigned int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((unsigned int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((unsigned int) 1) << (sizeof(unsigned int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (unsigned int) -1;
         }
     } else {
         unsigned int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (unsigned int) -1;
         val = __Pyx_PyInt_As_unsigned_int(tmp);
@@ -9207,52 +13510,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to unsigned int");
     return (unsigned int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const Py_intptr_t neg_one = (Py_intptr_t) -1, const_zero = (Py_intptr_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(Py_intptr_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(Py_intptr_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -9277,215 +13542,61 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
                                      little, !is_unsigned);
-    }
-}
-
-/* CIntFromPy */
-  static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(size_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (size_t) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
 #else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (size_t) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(size_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(size_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(unsigned int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
         }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            size_t val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
 #endif
-            return (size_t) -1;
-        }
-    } else {
-        size_t val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (size_t) -1;
-        val = __Pyx_PyInt_As_size_t(tmp);
-        Py_DECREF(tmp);
-        return val;
     }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to size_t");
-    return (size_t) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to size_t");
-    return (size_t) -1;
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__12);
+    }
+    return name;
+}
+#endif
+
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -9511,16 +13622,42 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -9529,177 +13666,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -9725,177 +13939,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9912,15 +14203,15 @@
     return (int) -1;
 }
 
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -9933,14 +14224,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -9957,19 +14264,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -10009,86 +14316,121 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
@@ -10135,15 +14477,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -10164,30 +14506,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -10245,21 +14591,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -10319,8 +14663,16 @@
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `tvb-gdist-2.2/gdist.pyx` & `tvb-gdist-2.2.1/gdist.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #
 # TheVirtualBrain-Framework Package. This package holds all Data Management, and
 # Web-UI helpful to run brain-simulations. To use it, you also need do download
 # TheVirtualBrain-Scientific Package (for simulators). See content of the
 # documentation-folder for more details. See also http://www.thevirtualbrain.org
 #
-# (c) 2012-2020, Baycrest Centre for Geriatric Care ("Baycrest") and others
+# (c) 2012-2024, Baycrest Centre for Geriatric Care ("Baycrest") and others
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.  See the GNU General Public License for more details.
```

### Comparing `tvb-gdist-2.2/geodesic_library/example0.cpp` & `tvb-gdist-2.2.1/geodesic_library/example0.cpp`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/example1.cpp` & `tvb-gdist-2.2.1/geodesic_library/example1.cpp`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_base.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_base.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_dijkstra.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_dijkstra.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_exact.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_exact.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_exact_elements.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_exact_elements.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_graph_base.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_graph_base.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_algorithm_subdivision.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_algorithm_subdivision.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_constants_and_simple_functions.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_constants_and_simple_functions.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_memory.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_memory.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_mesh.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_mesh.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_mesh_elements.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_mesh_elements.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/geodesic_utils.h` & `tvb-gdist-2.2.1/geodesic_library/geodesic_utils.h`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/geodesic_library/readme.txt` & `tvb-gdist-2.2.1/geodesic_library/readme.txt`

 * *Files identical despite different names*

### Comparing `tvb-gdist-2.2/setup.py` & `tvb-gdist-2.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #
 # TheVirtualBrain-Framework Package. This package holds all Data Management, and
 # Web-UI helpful to run brain-simulations. To use it, you also need do download
 # TheVirtualBrain-Scientific Package (for simulators). See content of the
 # documentation-folder for more details. See also http://www.thevirtualbrain.org
 #
-# (c) 2012-2020, Baycrest Centre for Geriatric Care ("Baycrest") and others
+# (c) 2012-2024, Baycrest Centre for Geriatric Care ("Baycrest") and others
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.  See the GNU General Public License for more details.
@@ -99,15 +99,15 @@
             self.include_dirs = [self.include_dirs]
         self.include_dirs.append(numpy.get_include())
         super().finalize_options()
 
 
 setuptools.setup(
     name="tvb-" + GEODESIC_NAME,
-    version="2.2",
+    version="2.2.1",
     ext_modules=GEODESIC_MODULE,
     include_dirs=INCLUDE_DIRS,
     cmdclass={"build_ext": new_build_ext},
     install_requires=INSTALL_REQUIREMENTS,
     description="Compute geodesic distances",
     long_description=DESCRIPTION,
     long_description_content_type='text/x-rst',
```

### Comparing `tvb-gdist-2.2/tests/test_gdist.py` & `tvb-gdist-2.2.1/tests/test_gdist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # TheVirtualBrain-Framework Package. This package holds all Data Management, and
 # Web-UI helpful to run brain-simulations. To use it, you also need do download
 # TheVirtualBrain-Scientific Package (for simulators). See content of the
 # documentation-folder for more details. See also http://www.thevirtualbrain.org
 #
-# (c) 2012-2020, Baycrest Centre for Geriatric Care ("Baycrest") and others
+# (c) 2012-2024, Baycrest Centre for Geriatric Care ("Baycrest") and others
 #
 # This program is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 # This program is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE.  See the GNU General Public License for more details.
```

### Comparing `tvb-gdist-2.2/tvb_gdist.egg-info/PKG-INFO` & `tvb-gdist-2.2.1/tvb_gdist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: tvb-gdist
-Version: 2.2
+Version: 2.2.1
 Summary: Compute geodesic distances
 Home-page: https://github.com/the-virtual-brain/tvb-gdist
 Author: Danil Kirsanov, Gaurav Malhotra and Stuart Knock
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL v3
 Keywords: gdist geodesic distance geo tvb
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: cython
 
 =================
 Geodesic Library 
 =================
 
 
 The **tvb-gdist** module is a Cython interface to a C++ library
```

### Comparing `tvb-gdist-2.2/tvb_gdist.egg-info/SOURCES.txt` & `tvb-gdist-2.2.1/tvb_gdist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

