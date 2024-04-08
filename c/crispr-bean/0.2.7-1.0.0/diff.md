# Comparing `tmp/crispr-bean-0.2.7.tar.gz` & `tmp/crispr-bean-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr-bean-0.2.7.tar", last modified: Wed Sep 27 21:29:00 2023, max compression
+gzip compressed data, was "crispr-bean-1.0.0.tar", last modified: Mon Apr  8 20:48:35 2024, max compression
```

## Comparing `crispr-bean-0.2.7.tar` & `crispr-bean-1.0.0.tar`

### file list

```diff
@@ -1,374 +1,77 @@
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:29:00.228498 crispr-bean-0.2.7/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.413452 crispr-bean-0.2.7/.eggs/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.416332 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.453755 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.691772 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3511 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/Code.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2979 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/FlowControl.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2486 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9166 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/Parsing.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2071 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/Scanning.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1814 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Compiler/Visitor.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.699280 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.231441 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     8306 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6358 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/array.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1358 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4870 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/buffer.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1443 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/bytearray.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    10066 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/bytes.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1390 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/cellobject.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      236 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/ceval.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1524 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/cobject.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5084 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/codecs.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1824 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5731 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/contextvars.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1696 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/conversion.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    15433 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/datetime.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      728 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/descr.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7939 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/dict.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13830 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/exc.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2889 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/fileobject.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1650 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/float.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2671 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/function.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1052 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/genobject.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      775 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/getargs.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      985 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/instance.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4131 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/int.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1319 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/iterator.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1036 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/iterobject.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4096 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/list.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7047 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/long.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      480 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/longintrepr.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2692 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/mapping.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2897 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/marshal.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5912 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/mem.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2504 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/memoryview.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2196 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/method.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    10128 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/module.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    11922 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/number.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    20003 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/object.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2916 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5700 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2000 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      222 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/pyport.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3779 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/pystate.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1946 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/pythread.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2556 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/ref.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6006 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/sequence.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5383 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/set.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3111 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/slice.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9942 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/string.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1356 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/time.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3219 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/tuple.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2067 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/type.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    29044 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/unicode.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      847 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/version.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1984 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/cpython/weakref.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.365548 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       13 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1224 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/complex.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2049 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/errno.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      966 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/float.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      621 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/limits.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1140 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/locale.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6581 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/math.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      297 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/setjmp.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1179 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/signal.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      164 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/stddef.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3449 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/stdint.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2476 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/stdio.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2444 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/stdlib.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2038 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/string.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1354 2023-07-20 02:14:49.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libc/time.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.716240 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       94 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    23704 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      425 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/any.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1705 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/atomic.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      749 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/bit.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      501 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/cast.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    19935 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/cmath.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3012 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/complex.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6641 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/deque.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      515 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/execution.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2429 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      601 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/functional.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1512 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/iterator.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1821 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/limits.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4438 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/list.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    10481 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/map.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3662 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/memory.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      395 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/numbers.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6571 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/numeric.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      981 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/optional.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       27 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/pair.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      649 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/queue.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6203 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/random.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9176 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/set.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      301 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/stack.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13115 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/string.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      524 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      304 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/typeinfo.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7945 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5810 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1040 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/utility.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6839 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/libcpp/vector.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.735805 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/numpy/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    36457 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/numpy/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5807 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/numpy/math.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1712 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/openmp.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.954251 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       13 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      356 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/dlfcn.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1697 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/fcntl.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       99 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/ioctl.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3475 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/mman.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1338 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/resource.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      619 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/select.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1876 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/signal.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2695 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/stat.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1055 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/stdio.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      935 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/stdlib.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      374 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/strings.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1981 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/time.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1162 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/types.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      822 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/uio.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     8061 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/unistd.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1246 2023-07-20 02:14:48.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Includes/posix/wait.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:57.995891 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      581 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/Actions.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      776 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/DFA.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      732 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/Machines.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1552 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/Scanners.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      590 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Plex/Transitions.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.003570 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Runtime/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6611 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Runtime/refnanny.pyx
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.066215 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4419 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/CConvert.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5511 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/CpdefEnums.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7053 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/CppConvert.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    49582 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/MemoryView.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      152 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/TestCyUtilityLoader.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1795 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/TestCythonScope.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2179 2023-07-20 02:14:47.000000 crispr-bean-0.2.7/.eggs/Cython-3.0.0-py3.8-linux-x86_64.egg/Cython/Utility/UFuncs.pyx
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)        6 2022-01-16 15:09:36.000000 crispr-bean-0.2.7/.gitignore
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       42 2022-08-03 16:07:29.000000 crispr-bean-0.2.7/MANIFEST.in
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    21891 2023-09-27 21:29:00.232101 crispr-bean-0.2.7/PKG-INFO
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    19582 2023-09-27 21:07:45.000000 crispr-bean-0.2.7/README.md
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.073680 crispr-bean-0.2.7/bean/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      450 2023-03-07 17:43:29.000000 crispr-bean-0.2.7/bean/__init__.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.110801 crispr-bean-0.2.7/bean/annotate/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-08-03 16:07:29.000000 crispr-bean-0.2.7/bean/annotate/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7070 2023-03-07 20:34:46.000000 crispr-bean-0.2.7/bean/annotate/_supporting_fn.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    22817 2023-06-19 19:39:53.000000 crispr-bean-0.2.7/bean/annotate/filter_alleles.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7260 2022-08-03 16:07:29.000000 crispr-bean-0.2.7/bean/annotate/ldlr_exons.fa
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    16239 2023-08-21 15:00:42.000000 crispr-bean-0.2.7/bean/annotate/translate_allele.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.143867 crispr-bean-0.2.7/bean/framework/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    11314 2023-08-21 15:00:42.000000 crispr-bean-0.2.7/bean/framework/AminoAcidEdit.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9703 2023-08-21 15:00:43.000000 crispr-bean-0.2.7/bean/framework/Edit.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    38002 2023-09-27 20:09:59.000000 crispr-bean-0.2.7/bean/framework/ReporterScreen.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-08-03 16:07:29.000000 crispr-bean-0.2.7/bean/framework/__init__.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.152057 crispr-bean-0.2.7/bean/framework/__pycache__/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      337 2023-03-07 18:41:42.000000 crispr-bean-0.2.7/bean/framework/__pycache__/ReporterScreen_.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     1742 2022-11-18 04:23:05.000000 crispr-bean-0.2.7/bean/framework/allele_counts.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.271656 crispr-bean-0.2.7/bean/mapping/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)  1367338 2023-09-27 19:47:05.000000 crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.c
--rwxr-xr-x   0 jr1025   (5074632) pinello  (10066)   269256 2023-09-27 19:47:22.000000 crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x   0 jr1025   (5074632) pinello  (10066)   253704 2023-04-18 04:23:44.000000 crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.cpython-39-x86_64-linux-gnu.so
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    14076 2022-08-03 20:23:39.000000 crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    33090 2023-08-27 21:12:54.000000 crispr-bean-0.2.7/bean/mapping/GuideEditCounter.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       46 2022-08-03 20:22:57.000000 crispr-bean-0.2.7/bean/mapping/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9628 2023-08-21 15:00:43.000000 crispr-bean-0.2.7/bean/mapping/_supporting_fn.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     9050 2023-08-27 19:01:14.000000 crispr-bean-0.2.7/bean/mapping/utils.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.427150 crispr-bean-0.2.7/bean/model/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2023-03-08 03:09:43.000000 crispr-bean-0.2.7/bean/model/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    33234 2023-08-29 04:11:39.000000 crispr-bean-0.2.7/bean/model/model.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.467553 crispr-bean-0.2.7/bean/model/post_training/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-12-15 18:23:54.000000 crispr-bean-0.2.7/bean/model/post_training/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1861 2023-08-04 20:42:16.000000 crispr-bean-0.2.7/bean/model/post_training/compare.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3139 2023-08-01 15:16:56.000000 crispr-bean-0.2.7/bean/model/post_training/post_training.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3819 2022-12-14 04:57:35.000000 crispr-bean-0.2.7/bean/model/post_training/utils.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6901 2023-08-29 03:57:24.000000 crispr-bean-0.2.7/bean/model/readwrite.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    17876 2023-08-22 05:15:29.000000 crispr-bean-0.2.7/bean/model/utils.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.491937 crispr-bean-0.2.7/bean/plotting/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2023-03-06 18:53:21.000000 crispr-bean-0.2.7/bean/plotting/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1798 2023-03-09 18:54:16.000000 crispr-bean-0.2.7/bean/plotting/allele_stats.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    15976 2023-08-21 15:00:43.000000 crispr-bean-0.2.7/bean/plotting/editing_patterns.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.534372 crispr-bean-0.2.7/bean/preprocessing/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2023-08-21 15:00:43.000000 crispr-bean-0.2.7/bean/preprocessing/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    45800 2023-08-22 03:58:28.000000 crispr-bean-0.2.7/bean/preprocessing/data_class.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4269 2023-08-29 03:54:14.000000 crispr-bean-0.2.7/bean/preprocessing/get_alpha0.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5357 2023-08-22 04:51:10.000000 crispr-bean-0.2.7/bean/preprocessing/get_pi_alpha0.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7833 2023-08-29 03:58:37.000000 crispr-bean-0.2.7/bean/preprocessing/utils.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.566250 crispr-bean-0.2.7/bean/qc/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       51 2023-03-05 16:09:08.000000 crispr-bean-0.2.7/bean/qc/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1504 2023-09-27 20:47:02.000000 crispr-bean-0.2.7/bean/qc/guide_qc.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1899 2023-09-20 21:09:15.000000 crispr-bean-0.2.7/bean/qc/sample_qc.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6667 2023-09-27 20:03:26.000000 crispr-bean-0.2.7/bean/qc/utils.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.592518 crispr-bean-0.2.7/bean/utils/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)        0 2022-09-08 19:34:16.000000 crispr-bean-0.2.7/bean/utils/__init__.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      221 2022-09-27 03:49:26.000000 crispr-bean-0.2.7/bean/utils/arithmetric.py
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)        0 2022-10-07 21:19:13.000000 crispr-bean-0.2.7/bean/utils/plot.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.486616 crispr-bean-0.2.7/beret_test/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.489892 crispr-bean-0.2.7/beret_test/lib/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.497124 crispr-bean-0.2.7/beret_test/lib/python3.8/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.542487 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.620698 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    36216 2022-07-11 20:28:37.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    34584 2022-07-11 20:28:37.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/__init__.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.507216 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/core/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.509919 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/core/tests/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.512616 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/core/tests/examples/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.632588 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/core/tests/examples/cython/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      615 2022-07-11 20:28:48.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/core/tests/examples/cython/checks.pyx
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.695980 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      431 2022-07-11 20:28:50.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/__init__.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1669 2022-07-11 20:28:50.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_bounded_integers.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4745 2022-07-11 20:28:49.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_common.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.524939 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_examples/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:58.714493 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_examples/cython/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2290 2022-07-11 20:28:50.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_examples/cython/extending.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3870 2022-07-11 20:28:50.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/_examples/cython/extending_distributions.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1007 2022-07-11 20:28:50.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/bit_generator.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6033 2022-07-11 20:28:49.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/numpy/random/c_distributions.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.537196 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.046065 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      278 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/algos.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    49104 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/algos.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      233 2022-07-11 20:41:51.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/arrays.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5848 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/arrays.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      736 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/dtypes.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    50578 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/groupby.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4731 2022-07-11 20:41:51.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/hashing.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3213 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/hashtable.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4586 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/hashtable.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    25989 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/index.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      753 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/indexing.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    24000 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/internals.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    16608 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/interval.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    31899 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/join.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3800 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/khash.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      139 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/lib.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    89097 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/lib.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      408 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/missing.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13911 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/missing.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7749 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/ops.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2570 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/ops_dispatch.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    68845 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/parsers.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1633 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/properties.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1090 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/reduction.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3391 2022-07-11 20:41:53.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/reshape.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    21115 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/sparse.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5790 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/testing.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    25374 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslib.pyx
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.421879 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       85 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/base.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      293 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/base.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      698 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/ccalendar.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     7062 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/ccalendar.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      941 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/conversion.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    24709 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/conversion.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2540 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/dtypes.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     8866 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/dtypes.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    20468 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/fields.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      339 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/nattype.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    36931 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/nattype.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2398 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/np_datetime.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6085 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/np_datetime.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      237 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/offsets.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)   127830 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/offsets.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       94 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/parsing.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    36726 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/parsing.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      187 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/period.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    79256 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/period.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    29116 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/strptime.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      591 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timedeltas.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    48263 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timedeltas.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1059 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timestamps.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    67833 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timestamps.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      451 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timezones.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13006 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/timezones.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      351 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/tzconversion.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    18840 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/tzconversion.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     5225 2022-07-11 20:41:55.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/util.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    12300 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/tslibs/vectorized.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      346 2022-07-11 20:41:54.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/util.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.444429 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/window/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    59190 2022-07-11 20:41:56.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/window/aggregations.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4282 2022-07-11 20:41:56.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/window/indexers.pyx
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4490 2022-07-11 20:41:52.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/_libs/writers.pyx
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.540030 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/io/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.453059 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/io/sas/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    15358 2022-07-11 20:42:21.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/pandas/io/sas/sas.pyx
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.477481 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.495290 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/linalg/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    14403 2022-07-11 20:29:38.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/linalg/cython_blas.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)   192579 2022-07-11 20:29:37.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/linalg/cython_lapack.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       48 2022-07-11 20:29:34.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/linalg.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.510974 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.552947 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:56.556056 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.627996 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3798 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HConst.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2178 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/Highs.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      446 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsIO.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      636 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsInfo.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1217 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsLp.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      315 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsLpUtils.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      366 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsModelUtils.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     3186 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsOptions.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      287 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsRuntimeOptions.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      348 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/HighsStatus.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     4671 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/SimplexConst.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      358 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/_highs/cython/src/highs_c_api.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.686650 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/cython_optimize/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1194 2022-07-11 20:29:43.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/cython_optimize/_zeros.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1085 2022-07-11 20:29:42.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/cython_optimize/c_zeros.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      428 2022-07-11 20:29:42.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize/cython_optimize.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       39 2022-07-11 20:29:34.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/optimize.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.702392 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/special/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13898 2022-07-11 20:29:56.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/special/cython_special.pxd
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       37 2022-07-11 20:29:34.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/special.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.709348 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/stats/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1046 2022-07-11 20:29:59.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/stats/_biasedurn.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.718211 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/stats/_unuran/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    43357 2022-07-11 20:30:00.000000 crispr-bean-0.2.7/beret_test/lib/python3.8/site-packages/scipy/stats/_unuran/unuran.pxd
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.764822 crispr-bean-0.2.7/bin/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     2833 2023-05-01 03:17:22.000000 crispr-bean-0.2.7/bin/bean-count
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     8053 2023-08-21 15:00:43.000000 crispr-bean-0.2.7/bin/bean-count-samples
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    13007 2023-09-22 21:08:05.000000 crispr-bean-0.2.7/bin/bean-filter
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1468 2023-09-27 20:00:17.000000 crispr-bean-0.2.7/bin/bean-qc
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     8813 2023-08-29 03:54:36.000000 crispr-bean-0.2.7/bin/bean-run
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.820044 crispr-bean-0.2.7/crispr_bean.egg-info/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    21891 2023-09-27 21:28:46.000000 crispr-bean-0.2.7/crispr_bean.egg-info/PKG-INFO
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    19501 2023-09-27 21:28:56.000000 crispr-bean-0.2.7/crispr_bean.egg-info/SOURCES.txt
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)        1 2023-09-27 21:28:46.000000 crispr-bean-0.2.7/crispr_bean.egg-info/dependency_links.txt
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)      264 2023-09-27 21:28:46.000000 crispr-bean-0.2.7/crispr_bean.egg-info/requires.txt
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)        5 2023-09-27 21:28:46.000000 crispr-bean-0.2.7/crispr_bean.egg-info/top_level.txt
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:28:59.913207 crispr-bean-0.2.7/docs/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    77435 2023-03-08 22:06:20.000000 crispr-bean-0.2.7/docs/ReporterScreen_api.ipynb
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    49125 2023-03-08 22:06:20.000000 crispr-bean-0.2.7/docs/ReporterScreen_api.rst
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)   350457 2023-03-08 22:06:20.000000 crispr-bean-0.2.7/docs/editing_pattern_analysis.ipynb
--rw-r-----   0 jr1025   (5074632) pinello  (10066)     8601 2023-03-08 22:06:28.000000 crispr-bean-0.2.7/docs/sample_quality_report.ipynb
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:29:00.079400 crispr-bean-0.2.7/imgs/
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    41318 2023-03-02 04:27:44.000000 crispr-bean-0.2.7/imgs/anbe.svg
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     6805 2023-03-07 20:11:49.000000 crispr-bean-0.2.7/imgs/bean_title.svg
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)   591269 2023-03-02 04:27:44.000000 crispr-bean-0.2.7/imgs/output_20_2.png
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)     5136 2023-03-02 04:27:44.000000 crispr-bean-0.2.7/imgs/output_34_1.png
--rw-rw----   0 jr1025   (5074632) pinello  (10066)    86441 2023-03-07 01:04:04.000000 crispr-bean-0.2.7/imgs/reporter_construct.svg
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)   120442 2023-03-02 04:27:44.000000 crispr-bean-0.2.7/imgs/reporter_screen.svg
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)   370867 2023-03-02 04:27:44.000000 crispr-bean-0.2.7/imgs/screendata.svg
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      126 2023-08-28 03:20:57.000000 crispr-bean-0.2.7/pyproject.toml
--rw-rw----   0 jr1025   (5074632) pinello  (10066)       38 2023-09-27 21:29:00.235448 crispr-bean-0.2.7/setup.cfg
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1843 2023-09-27 21:28:34.000000 crispr-bean-0.2.7/setup.py
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:29:00.130722 crispr-bean-0.2.7/tests/
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:29:00.141644 crispr-bean-0.2.7/tests/CRISPRessoCount_on_test/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      241 2022-08-03 16:07:30.000000 crispr-bean-0.2.7/tests/CRISPRessoCount_on_test/CRISPRessoCount_RUNNING_LOG.txt
-drwxr-xr-x   0 jr1025   (5074632) pinello  (10066)        0 2023-09-27 21:29:00.183985 crispr-bean-0.2.7/tests/data/
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1174 2023-08-21 16:05:22.000000 crispr-bean-0.2.7/tests/data/sample_list.csv
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    11034 2023-06-28 19:48:41.000000 crispr-bean-0.2.7/tests/data/test_R1.fastq
--rw-r--r--   0 jr1025   (5074632) pinello  (10066)    11034 2023-06-28 19:48:41.000000 crispr-bean-0.2.7/tests/data/test_R2.fastq
--rwxrwx---   0 jr1025   (5074632) pinello  (10066)   446855 2023-08-21 15:00:44.000000 crispr-bean-0.2.7/tests/data/test_guide_info.csv
--rw-rw----   0 jr1025   (5074632) pinello  (10066)      229 2023-08-22 01:46:00.000000 crispr-bean-0.2.7/tests/test_Edit.py
--rw-rw----   0 jr1025   (5074632) pinello  (10066)     1284 2023-08-22 01:44:49.000000 crispr-bean-0.2.7/tests/test_count.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.245616 crispr-bean-1.0.0/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)       42 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/MANIFEST.in
+-rw-r--r--   0 jykr      (1000) jykr      (1000)     6566 2024-04-08 20:48:35.244165 crispr-bean-1.0.0/PKG-INFO
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     5510 2024-04-01 18:01:27.000000 crispr-bean-1.0.0/README.md
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:34.995738 crispr-bean-1.0.0/bean/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)      450 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/__init__.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.021340 crispr-bean-1.0.0/bean/annotate/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/annotate/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     7293 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/annotate/_supporting_fn.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    23119 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/annotate/filter_alleles.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    25394 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/annotate/translate_allele.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    15513 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/annotate/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.051722 crispr-bean-1.0.0/bean/cli/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/cli/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     2534 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/cli/count.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     7619 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/cli/count_samples.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1130 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/cli/create_screen.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     2468 2024-04-01 13:51:53.000000 crispr-bean-1.0.0/bean/cli/execute.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     9950 2024-04-02 22:05:32.000000 crispr-bean-1.0.0/bean/cli/filter.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1318 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/cli/profile.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     2158 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/cli/qc.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     7780 2024-04-02 22:47:43.000000 crispr-bean-1.0.0/bean/cli/run.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.077854 crispr-bean-1.0.0/bean/framework/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    11436 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/AminoAcidEdit.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    10294 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/Edit.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    39734 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/ReporterScreen.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1742 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/allele_counts.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1354 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/parser.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)      413 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/framework/read_from_csvs.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.115568 crispr-bean-1.0.0/bean/mapping/
+-rw-r--r--   0 jykr      (1000) jykr      (1000)  1370587 2024-04-01 20:13:16.000000 crispr-bean-1.0.0/bean/mapping/CRISPResso2Align.c
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    14076 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/mapping/CRISPResso2Align.pyx
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    35400 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/mapping/GuideEditCounter.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)       46 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/mapping/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     9618 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/mapping/_supporting_fn.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    11598 2024-04-04 15:06:17.000000 crispr-bean-1.0.0/bean/mapping/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.143904 crispr-bean-1.0.0/bean/model/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    34749 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/model.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     8276 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/parser.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     9206 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/readwrite.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    10694 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/run.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    25417 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/survival_model.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     6129 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/model/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.154327 crispr-bean-1.0.0/bean/plotting/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/plotting/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     2489 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/plotting/allele_stats.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    15589 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/plotting/editing_patterns.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1887 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/plotting/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.176793 crispr-bean-1.0.0/bean/preprocessing/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/preprocessing/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    58324 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/preprocessing/data_class.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     4526 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/preprocessing/get_alpha0.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     5357 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/preprocessing/get_pi_alpha0.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)    10006 2024-04-02 21:52:43.000000 crispr-bean-1.0.0/bean/preprocessing/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.189796 crispr-bean-1.0.0/bean/qc/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)       51 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/qc/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     3054 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/qc/guide_qc.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     5367 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/qc/parser.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     2188 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/qc/sample_qc.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     3490 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/qc/utils.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.209564 crispr-bean-1.0.0/bean/utils/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/utils/__init__.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)      221 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/utils/arithmetric.py
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bean/utils/plot.py
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.218951 crispr-bean-1.0.0/bin/
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)      100 2024-04-01 13:51:54.000000 crispr-bean-1.0.0/bin/bean
+drwxr-xr-x   0 jykr      (1000) jykr      (1000)        0 2024-04-08 20:48:35.241316 crispr-bean-1.0.0/crispr_bean.egg-info/
+-rw-r--r--   0 jykr      (1000) jykr      (1000)     6566 2024-04-08 20:48:33.000000 crispr-bean-1.0.0/crispr_bean.egg-info/PKG-INFO
+-rw-r--r--   0 jykr      (1000) jykr      (1000)     1548 2024-04-08 20:48:34.000000 crispr-bean-1.0.0/crispr_bean.egg-info/SOURCES.txt
+-rw-r--r--   0 jykr      (1000) jykr      (1000)        1 2024-04-08 20:48:33.000000 crispr-bean-1.0.0/crispr_bean.egg-info/dependency_links.txt
+-rw-r--r--   0 jykr      (1000) jykr      (1000)      282 2024-04-08 20:48:33.000000 crispr-bean-1.0.0/crispr_bean.egg-info/requires.txt
+-rw-r--r--   0 jykr      (1000) jykr      (1000)        5 2024-04-08 20:48:33.000000 crispr-bean-1.0.0/crispr_bean.egg-info/top_level.txt
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)      126 2024-04-01 13:51:55.000000 crispr-bean-1.0.0/pyproject.toml
+-rw-r--r--   0 jykr      (1000) jykr      (1000)       38 2024-04-08 20:48:35.246822 crispr-bean-1.0.0/setup.cfg
+-rwxr-xr-x   0 jykr      (1000) jykr      (1000)     1956 2024-04-01 13:51:55.000000 crispr-bean-1.0.0/setup.py
```

### Comparing `crispr-bean-0.2.7/bean/annotate/_supporting_fn.py` & `crispr-bean-1.0.0/bean/annotate/_supporting_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import List, Tuple
+from typing import List, Tuple, Union
 from tqdm.auto import tqdm
 from ..framework.Edit import Edit, Allele
 from ..framework.AminoAcidEdit import CodingNoncodingAllele
 import pandas as pd
 from ..annotate.translate_allele import CDS, RefBaseMismatchException
 
 
@@ -39,44 +39,48 @@
         print("No threshold specified")  # TODO: warn
     return (allele_filtered, filtered_edits)
 
 
 def filter_allele_by_base(
     allele: Allele,
     allowed_base_changes: List[Tuple] = None,
-    allowed_ref_base: str = None,
-    allowed_alt_base: str = None,
+    allowed_ref_base: Union[List, str] = None,
+    allowed_alt_base: Union[List, str] = None,
 ):
     """
     Filter alleles based on position and return the filtered allele and
     number of filtered edits.
     """
     filtered_edits = 0
+    if isinstance(allowed_ref_base, str):
+        allowed_ref_base = [allowed_ref_base]
+    if isinstance(allowed_alt_base, str):
+        allowed_alt_base = [allowed_alt_base]
     if (
         not (allowed_ref_base is None and allowed_alt_base is None)
         + (allowed_base_changes is None)
         == 1
     ):
         print("No filters specified or misspecified filters.")
     elif not allowed_base_changes is None:
         for edit in allele.edits.copy():
             if not (edit.ref_base, edit.alt_base) in allowed_base_changes:
                 filtered_edits += 1
                 allele.edits.remove(edit)
     elif not allowed_ref_base is None:
         for edit in allele.edits.copy():
-            if edit.ref_base != allowed_ref_base:
+            if edit.ref_base not in allowed_ref_base:
                 filtered_edits += 1
                 allele.edits.remove(edit)
-            elif not allowed_alt_base is None and edit.alt_base != allowed_alt_base:
+            elif not allowed_alt_base is None and edit.alt_base not in allowed_alt_base:
                 filtered_edits += 1
                 allele.edits.remove(edit)
     else:
         for edit in allele.edits.copy():
-            if edit.alt_base != allowed_alt_base:
+            if edit.alt_base not in allowed_alt_base:
                 filtered_edits += 1
                 allele.edits.remove(edit)
     return (allele, filtered_edits)
 
 
 def get_aa_alleles(allele_str, include_synonymous=True):
     ldlr_cds = CDS()
@@ -141,15 +145,14 @@
     is_cn_allele = isinstance(
         raw_allele_counts.reset_index()[allele_col][0], CodingNoncodingAllele
     )
     for guide, guide_raw_counts in tqdm(
         raw_allele_counts.groupby("guide"),
         desc="Mapping alleles to closest filtered alleles",
     ):
-
         guide_filtered_allele_counts = filtered_allele_counts.loc[
             filtered_allele_counts.guide == guide, :
         ].set_index(allele_col)
         guide_filtered_alleles = guide_filtered_allele_counts.index.tolist()
         if len(guide_filtered_alleles) == 0:
             pass
         else:
```

### Comparing `crispr-bean-0.2.7/bean/annotate/filter_alleles.py` & `crispr-bean-1.0.0/bean/annotate/filter_alleles.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from scipy.stats import fisher_exact
 from tqdm.auto import tqdm
 import pandas as pd
 from scipy.special import softmax
 from ..framework.Edit import Allele
 from ..framework.AminoAcidEdit import CodingNoncodingAllele
 from ._supporting_fn import map_alleles_to_filtered
+from .utils import fast_concat
 
 
 def sum_column_groups(mat, column_index_list):
     cols = [
         mat[:, np.array(colidx)].sum(axis=1, keepdims=True)
         for colidx in column_index_list
     ]
@@ -431,15 +432,17 @@
         filtered_guide = aa_prop_filtered.index.get_level_values("guide").unique()
         append_rows = []
         for guide in tqdm(aa_prop.index.get_level_values("guide").unique().tolist()):
             if guide not in filtered_guide:
                 guide_df = aa_prop.loc[
                     aa_prop.index.get_level_values("guide") == guide,
                 ]
-                max_frequency_idx = np.argmax(guide_df.mean(axis=1))
+                max_frequency_idx = np.nanargmax(
+                    guide_df.mean(axis=1, numeric_only=True).fillna(0)
+                )
                 append_rows.append(guide_df.iloc[[max_frequency_idx], :])
         aa_prop_filtered = pd.concat([aa_prop_filtered] + append_rows, axis=0)
 
     alleles = alleles.set_index(["guide", allele_col])
     aa_filtered = alleles.loc[alleles.index.isin(aa_prop_filtered.index), :]
     alleles = alleles.reset_index()
     aa_filtered = aa_filtered.reset_index()
@@ -488,14 +491,15 @@
         ].set_index(allele_col)
         guide_filtered_alleles = guide_filtered_allele_counts.index.tolist()
         if len(guide_filtered_alleles) != 0:
             # prioritize allele with most mean counts
             merge_priority = guide_filtered_allele_counts.mean(
                 axis=1, numeric_only=True
             )
+            merge_priority = merge_priority.fillna(0)
             if is_cn_allele:
                 guide_raw_counts["allele_mapped"] = guide_raw_counts[allele_col].map(
                     lambda allele: allele.map_to_closest(
                         guide_filtered_alleles,
                         aa_jaccard_threshold=aa_jaccard_threshold,
                         nt_jaccard_threshold=nt_jaccard_threshold,
                         merge_priority=merge_priority,
@@ -510,18 +514,18 @@
                     )
                 )
             guide_raw_counts = (
                 guide_raw_counts.drop(allele_col, axis=1)
                 .rename(columns={"allele_mapped": allele_col})
                 .groupby(["guide", allele_col])
                 .sum()
-            )
+            ).reset_index()
 
             mapped_allele_counts.append(guide_raw_counts)
-    res = pd.concat(mapped_allele_counts).reset_index()
+    res = fast_concat(mapped_allele_counts).reset_index(drop=True)
     res = res.loc[res[allele_col].map(bool), :]
     return res
 
 
 def _distribute_alleles_to_filtered(
     raw_allele_counts: pd.DataFrame,
     filtered_allele_counts: pd.DataFrame,
@@ -572,12 +576,14 @@
             if not (dist_values.sum(axis=0) <= guide_raw_counts.values[i, :]).all():
                 pass  # rounding process can inflate total number of allele counts
             res += dist_values
         added_counts = pd.DataFrame(
             res,
             index=guide_filtered_counts.index,
             columns=guide_filtered_counts.columns,
-        )
+        ).reset_index()
         mapped_allele_counts.append(added_counts)
-    res = pd.concat(mapped_allele_counts).reset_index()
+    # @TODO: these lines are taking very long?
+    print("Contatenating allele counts...")
+    res = fast_concat(mapped_allele_counts).reset_index(drop=True)
     res = res.loc[res[allele_col].map(bool), :]
     return res
```

### Comparing `crispr-bean-0.2.7/bean/framework/AminoAcidEdit.py` & `crispr-bean-1.0.0/bean/framework/AminoAcidEdit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Iterable
+from typing import Iterable, Optional
 from enum import IntEnum
 import warnings
 import numpy as np
 import re
 from ..framework.Edit import Allele, Edit
 from ..utils.arithmetric import jaccard
 
@@ -117,15 +117,16 @@
         if self.gene > other.gene:
             return True
         if self.gene < other.gene:
             return False
 
 
 class AminoAcidAllele(Allele):
-    def __init__(self, edits: Iterable[AminoAcidEdit] = None):
+    def __init__(self, edits: Iterable[AminoAcidEdit] = None, gene=None):
+        self.gene = None
         self.edits = set() if edits is None else set(edits)
 
     @classmethod
     def match_str(cls, allele_str):
         if isinstance(allele_str, AminoAcidAllele):
             return True
         # try:
@@ -239,14 +240,17 @@
         aa_jaccards, nt_jaccards = zip(
             *list(map(lambda o: self.get_jaccard(o), allele_list))
         )
         aa_jaccards = np.array(aa_jaccards)
         nt_jaccards = np.array(nt_jaccards)
         return (aa_jaccards, nt_jaccards)
 
+    def has_coding(self):
+        return len(self.aa_allele.edits) > 0
+
     def map_to_closest(
         self,
         allele_list,
         aa_jaccard_threshold=0.5,
         nt_jaccard_threshold=0.5,
         merge_priority: np.ndarray = None,
     ):
```

### Comparing `crispr-bean-0.2.7/bean/framework/Edit.py` & `crispr-bean-1.0.0/bean/framework/Edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ):
         assert strand in [+1, -1]
         self.chrom = chrom
         self.rel_pos = rel_pos
         self.ref_base = ref_base  # TODO make it ref / alt instead of ref_base and alt_base for AAEdit comp. or make abstract class
         self.alt_base = alt_base
         self.uid = unique_identifier
-        if type(strand) == int:
+        if isinstance(strand, int):
             strand_to_symbol = {1: "+", -1: "-"}
             self.strand = strand_to_symbol[strand]
         else:
             assert strand in {"+", "-"}
             self.strand = strand
         self.pos = self.rel_pos if offset is None else offset + self.rel_pos * strand
 
@@ -64,15 +64,15 @@
             unique_identifier=uid,
         )
 
     @classmethod
     def match_str(cls, edit_str):
         if isinstance(edit_str, Edit):
             return True
-        pattern = r"((chr)?\d+:)?-?\d+:-?\d+:[+-]:[A-Z*-]>[A-Z*-]"
+        pattern = r"(((chr)?\w+|nan):)?-?\d+:-?\d+:[+-]:[A-Z*-]>[A-Z*-]"
         pattern2 = r"[\w*]!-?\d+:-?\d+:[+-]:[A-Z*-]>[A-Z*-]"
         return re.fullmatch(pattern, edit_str) or re.fullmatch(pattern2, edit_str)
 
     def get_abs_edit(self):
         """
         Returns edit representation in sense strand
         """
@@ -88,14 +88,18 @@
 
     def set_uid(self, uid):
         if "!" in uid:
             raise ValueError("Cannot use special character `!` in uid.")
         self.uid = uid
         return self
 
+    def set_chrom(self, chrom):
+        self.chrom = chrom
+        return self
+
     def get_abs_base_change(self):
         if self.strand == "-":
             ref_base = type(self).reverse_map[self.ref_base]
             alt_base = type(self).reverse_map[self.alt_base]
         else:
             ref_base = self.ref_base
             alt_base = self.alt_base
@@ -131,45 +135,55 @@
 
 class Allele:
     # pos, ref, alt
     def __init__(self, edits: Iterable[Edit] = None):
         self.edits = set() if edits is None else set(edits)
         if edits and len(edits) > 0:
             self.chrom = next(iter(edits)).chrom
+        else:
+            self.chrom = None
 
     @classmethod
     def from_str(cls, allele_str):  # pos:strand:start>end
         if type(allele_str) is Allele:
             return allele_str
         edits = set()
         try:
             for edit_str in allele_str.split(","):
                 edit = Edit.from_str(edit_str)
                 edits.add(edit)
-        except ValueError:
+        except ValueError as e:
             if allele_str.strip() == "":
                 return cls(None)
+            else:
+                raise e
         return cls(edits)
 
     @classmethod
     def match_str(cls, allele_str):
         if isinstance(allele_str, Allele):
             return True
         if allele_str == "":
             return True
         return all(map(Edit.match_str, allele_str.split(",")))
 
     def get_range(self):
         """Returns genomic range of the edits in the allele"""
+        if len(self.edits) == 0:
+            return None
         return (
             self.chrom,
             min(edit.pos for edit in self.edits),
             max(edit.pos for edit in self.edits),
         )
 
+    def set_uid(self, uid):
+        self.edits = {edit.set_uid(uid) for edit in self.edits}
+        return self
+
     def get_uid(self):
         uid = None
         if (
             len(self) > 0
             and all(e.uid is not None for e in self.edits)
             and len(np.unique([e.uid for e in self.edits if e.uid is not None]))
         ):
@@ -208,19 +222,24 @@
                 ):
                     return True
             else:
                 return True
         return False
 
     def get_jaccard(self, other):
+        if self.chrom != other.chrom:
+            return 0
         return jaccard(set(map(str, self.edits)), set(map(str, other.edits)))
 
     def get_jaccards(self, allele_list: Iterable[Allele]):
         return np.array(list(map(lambda o: self.get_jaccard(o), allele_list)))
 
+    def set_chrom(self, chrom: str):
+        self.edits = {edit.set_chrom(chrom) for edit in self.edits}
+
     def map_to_closest(
         self, allele_list, jaccard_threshold=0.5, merge_priority: np.ndarray = None
     ):
         """
         Arguments
         merge_priority -- Priority on which allele to merge if the jaccard index is the same.
         """
@@ -231,15 +250,17 @@
             nt_max_idx = np.where(nt_jaccards == np.nanmax(nt_jaccards))[0]
             if len(nt_max_idx) > 0:
                 if len(nt_max_idx) > 1 and merge_priority is not None:
                     if len(merge_priority) != len(allele_list):
                         raise ValueError(
                             f"merge_priority length {len(merge_priority)} is not the same as allele_list length {len(allele_list)}"
                         )
-                    nt_max_idx = nt_max_idx[np.argmax(merge_priority[nt_max_idx])]
+                    nt_max_idx = nt_max_idx[
+                        np.nanargmax(merge_priority.iloc[nt_max_idx])
+                    ]
                 else:
                     nt_max_idx = nt_max_idx[0]
                 if nt_jaccards[nt_max_idx] > jaccard_threshold:
                     return allele_list[nt_max_idx.item()]
         return Allele()
 
     def __bool__(self):
```

### Comparing `crispr-bean-0.2.7/bean/framework/ReporterScreen.py` & `crispr-bean-1.0.0/bean/framework/ReporterScreen.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
         (super().__init__)(X=X, *args, **kwargs)
         if X_edit is not None:
             self.layers["edits"] = X_edit
         if X_bcmatch is not None:
             self.layers["X_bcmatch"] = X_bcmatch
         for k, df in self.uns.items():
             if not isinstance(df, pd.DataFrame):
+                if k == "sample_covariates" and not isinstance(df, list):
+                    self.uns[k] = df.tolist()
                 continue
             if "guide" in df.columns and len(df) > 0:
                 if (
                     "allele" in df.columns
                     and (not isinstance(df["allele"].iloc[0], Allele))
                     and any(df["allele"].map(Allele.match_str))
                 ):
@@ -319,16 +321,35 @@
             vidx = slice(vidx, vidx + 1, 1)
         guides_include = self.guides.iloc[oidx].index.tolist()
         condit_include = self.samples.iloc[vidx].index.tolist()
         adata = super().__getitem__(index)
         new_uns = deepcopy(self.uns)
         for k, df in adata.uns.items():
             if k.startswith("repguide_mask"):
-                new_uns[k] = df.loc[guides_include, adata.var.rep.unique()]
+                if "sample_covariates" in adata.uns:
+                    adata.var["_rc"] = adata.var[
+                        ["replicate"] + list(adata.uns["sample_covariates"])
+                    ].values.tolist()
+                    adata.var["_rc"] = adata.var["_rc"].map(
+                        lambda slist: ".".join(slist)
+                    )
+                    new_uns[k] = df.loc[guides_include, adata.var._rc.unique()]
+                    # adata.var.pop("_rc")
+                else:
+                    try:
+                        new_uns[k] = df.loc[
+                            guides_include, adata.var["replicate"].unique()
+                        ]
+                    except KeyError as e:
+                        raise ValueError(
+                            f"Replicate column should be `replicate`. Modify your ReporterScreen.samples. Current columns: {adata.var.columns.tolist()}"
+                        ) from e
             if not isinstance(df, pd.DataFrame):
+                if k == "sample_covariates":
+                    new_uns[k] = df
                 continue
             if "guide" in df.columns:
                 if "allele" in df.columns:
                     key_col = ["guide", "allele"]
                 elif "edit" in df.columns:
                     key_col = ["guide", "edit"]
                 elif "aa_allele" in df.columns:
@@ -458,15 +479,15 @@
         editable_base_start=3,
         editable_base_end=8,
         bcmatch_thres=1,
         prior_weight: float = None,
         return_result=False,
         count_layer="X_bcmatch",
         edit_layer="edits",
-        unsorted_condition_label="bulk",
+        unsorted_condition_label=None,
     ):
         """
         prior_weight:
         Considering the edit rate to have prior of beta distribution with mean 0.5,
         prior weight to use when calculating posterior edit rate.
         unsorted_condition_label: Editing rate is calculated only for the samples that have this string in the sample index.
         """
@@ -479,17 +500,22 @@
         num_targetable_sites = 1.0
         if normalize_by_editable_base:
             if edited_base not in ["A", "C", "T", "G"]:
                 raise ValueError("Specify the correct edited_base")
             num_targetable_sites = self.guides.sequence.map(
                 lambda s: s[editable_base_start:editable_base_end].count(edited_base)
             )
-        bulk_idx = np.where(
-            self.samples.index.astype(str).map(lambda s: unsorted_condition_label in s)
-        )[0]
+        if unsorted_condition_label is not None:
+            bulk_idx = np.where(
+                self.samples.index.astype(str).map(
+                    lambda s: unsorted_condition_label in s
+                )
+            )[0]
+        else:
+            bulk_idx = np.arange(0, len(self.samples)).astype(int)
 
         if prior_weight is None:
             prior_weight = 1
         n_edits = self.layers[edit_layer].copy()[:, bulk_idx].sum(axis=1)
         n_counts = self.layers[count_layer].copy()[:, bulk_idx].sum(axis=1)
         edit_rate = (n_edits + prior_weight / 2) / (
             (n_counts * num_targetable_sites) + prior_weight / 2
@@ -630,15 +656,15 @@
                 *allele_count_df.allele.map(
                     lambda a: filter_allele_by_pos(
                         a, rel_pos_start, rel_pos_end, filter_rel_pos
                     )
                 )
             )
         else:
-            if not "guide_len" in self.guides.columns.tolist():
+            if "guide_len" not in self.guides.columns.tolist():
                 self.guides["guide_len"] = self.guides.sequence.map(len)
             guide_start_pos = (
                 32 - 6 - self.guides.loc[allele_count_df.guide, "guide_len"].values
             )
             filtered_allele, filtered_edits = zip(
                 *[
                     filter_allele_by_pos(
@@ -679,16 +705,16 @@
                     allele_count_df,
                     jaccard_threshold=jaccard_threshold,
                 )
         return allele_count_df
 
     def filter_allele_counts_by_base(
         self,
-        ref_base="A",
-        alt_base="G",
+        ref_base: Union[List, str] = "A",
+        alt_base: Union[List, str] = "G",
         allele_uns_key="allele_counts",
         map_to_filtered=True,
         jaccard_threshold: float = 0.5,
     ):
         """
         Filter alleles based on base change.
 
@@ -846,17 +872,22 @@
         adata = self.copy()
         for k, v in adata.uns.items():
             if isinstance(v, pd.DataFrame) and len(v) > 0:
                 if "edit" in v.columns and isinstance(
                     adata.uns[k]["edit"].iloc[0], Edit
                 ):
                     adata.uns[k].edit = adata.uns[k].edit.map(str)
-                for c in [colname for colname in v.columns if "allele" in colname]:
-                    if isinstance(v[c].iloc[0], (Allele, CodingNoncodingAllele)):
-                        adata.uns[k].loc[:, c] = adata.uns[k][c].map(str)
+                try:
+                    for c in [
+                        colname for colname in v.columns if "allele" in str(colname)
+                    ]:
+                        if isinstance(v[c].iloc[0], (Allele, CodingNoncodingAllele)):
+                            adata.uns[k].loc[:, c] = adata.uns[k][c].map(str)
+                except TypeError as e:
+                    raise TypeError(f"error with {e}: {k, v} cannot be written")
         super(ReporterScreen, adata).write(out_path)
 
 
 def _convert_obj_column_to_str(df, obj_column):
     if obj_column not in df.columns:
         return df
     df = df.rename(columns={obj_column: "obj_col"})
@@ -883,48 +914,51 @@
         raise ValueError(f"axis must be 0 or 1. Provided of invalid axis {axis}.")
     keys = set(screens[0].uns.keys())
     for screen in screens:
         keys.intersection(screen.uns.keys())
 
     if axis == 0:
         for k in keys:
-            if k in ["target_base_change", "tiling"]:
+            if k in ["target_base_change", "tiling", "sample_covariates"]:
                 adata.uns[k] = screens[0].uns[k]
                 continue
             elif "edit" not in k and "allele" not in k:
                 continue
             adata.uns[k] = pd.concat([screen.uns[k] for screen in screens])
 
     if axis == 1:
         # If combining multiple samples, edit/allele tables should be merged.
         for k in keys:
-            if k in ["target_base_change", "tiling"]:
+            if k in ["target_base_change", "tiling", "sample_covariates"]:
                 adata.uns[k] = screens[0].uns[k]
                 continue
             elif "edit" not in k and "allele" not in k:
                 continue
             screen_uns_dfs = [screen.uns[k] for screen in screens]
 
             if max(len(screen_uns_df) for screen_uns_df in screen_uns_dfs) == 0:
                 continue
-            merge_on = screen[0].uns[k].columns[:2].tolist()
+            if "guide_reporter_allele" in k:
+                merge_on = screen[0].uns[k].columns[:3].tolist()
+            else:
+                merge_on = screen[0].uns[k].columns[:2].tolist()
             try:
                 edit_cls = type(screens[0].uns[k][merge_on[1]][0])
             except IndexError:
                 print(merge_on)
                 print(screen[0].uns[k])
                 exit(1)
             screen_uns_dfs = [
                 _convert_obj_column_to_str(df, merge_on[1]) for df in screen_uns_dfs
             ]
 
             for i, screen in enumerate(screens):
                 if screen.uns[k][merge_on].duplicated().any():
                     raise ValueError(
-                        f"{i}-th ReporterScreen .uns['{k}'] has duplicated row. Aborting."
+                        f"{i}-th ReporterScreen .uns['{k}'] has duplicated row. Aborting.: {screen.uns[k][merge_on].loc[screen.uns[k][merge_on].duplicated()]}"
                     )
                 if i == 0:
                     adata.uns[k] = screen.uns[k]
                 else:
                     adata.uns[k] = pd.merge(
                         adata.uns[k], screen.uns[k], on=merge_on, how="outer"
                     )
```

### Comparing `crispr-bean-0.2.7/bean/framework/allele_counts.py` & `crispr-bean-1.0.0/bean/framework/allele_counts.py`

 * *Files identical despite different names*

### Comparing `crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.c` & `crispr-bean-1.0.0/bean/mapping/CRISPResso2Align.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "bean.mapping.CRISPResso2Align",
         "sources": [
@@ -28,23 +28,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
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
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
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
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
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
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -577,25 +607,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
-        PyObject *version_info; // borrowed
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -608,15 +641,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -641,15 +673,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -727,16 +759,21 @@
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
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -752,14 +789,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
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
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -778,14 +840,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
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
@@ -853,27 +917,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
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
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -909,15 +973,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1053,14 +1117,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1131,15 +1204,15 @@
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
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1216,17 +1289,18 @@
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
@@ -1246,32 +1320,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1313,15 +1370,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1334,14 +1391,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1384,14 +1442,15 @@
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
@@ -1431,15 +1490,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1561,14 +1620,15 @@
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
 #elif CYTHON_ATOMICS && defined(_MSC_VER)
     #include <intrin.h>
     #undef __pyx_atomic_int_type
     #define __pyx_atomic_int_type long
+    #undef __pyx_nonatomic_int_type
     #define __pyx_nonatomic_int_type long
     #pragma intrinsic (_InterlockedExchangeAdd)
     #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
     #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
@@ -1600,195 +1660,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1848,42 +1908,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2181,29 +2241,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2518,17 +2583,14 @@
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* ssize_strlen.proto */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2546,15 +2608,19 @@
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
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
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
@@ -2586,15 +2652,19 @@
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
 
 /* PyObjectLookupSpecial.proto */
 #if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
 #define __Pyx_PyObject_LookupSpecialNoError(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 0)
 #define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
 static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
 #else
@@ -2753,30 +2823,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -2861,25 +2931,29 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -3148,15 +3222,16 @@
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
@@ -4821,16 +4896,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 131, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shape,&__pyx_n_s_itemsize,&__pyx_n_s_format,&__pyx_n_s_mode,&__pyx_n_s_allocate_buffer,0};
     values[3] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)__pyx_n_s_c));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -4923,18 +4997,19 @@
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, __pyx_nargs); __PYX_ERR(1, 131, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -5209,21 +5284,28 @@
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError, f"Invalid shape in axis {idx}: {dim}."
  */
   __pyx_t_7 = 0;
-  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4); __pyx_t_1 = 0;
+  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = 0;
   for (;;) {
-    if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
+      #endif
+      if (__pyx_t_1 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_7;
     __pyx_t_7 = (__pyx_t_7 + 1);
@@ -5858,18 +5940,16 @@
   __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":211
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data and self.data is not NULL:
@@ -5973,15 +6053,14 @@
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":219
  *         PyObject_Free(self._shape)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def memview(self):
@@ -6006,15 +6085,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":221
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
@@ -6059,15 +6138,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_memview", 0);
+  __Pyx_RefNannySetupContext("get_memview", 1);
 
   /* "View.MemoryView":225
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
@@ -6146,16 +6225,14 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":229
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
@@ -6169,15 +6246,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":231
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
@@ -6204,15 +6280,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getattr__", 0);
+  __Pyx_RefNannySetupContext("__getattr__", 1);
 
   /* "View.MemoryView":232
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
@@ -6274,15 +6350,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":235
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
@@ -6343,15 +6419,15 @@
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setitem__", 0);
+  __Pyx_RefNannySetupContext("__setitem__", 1);
 
   /* "View.MemoryView":238
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6402,53 +6478,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.array.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_array___reduce_cython__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array___reduce_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -6504,16 +6569,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -6540,18 +6604,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -6574,15 +6639,15 @@
 
 static PyObject *__pyx_pf___pyx_array_2__setstate_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -6612,23 +6677,21 @@
  * 
  */
 
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_v_i;
   PyObject **__pyx_v_p;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_allocate_buffer", 0);
 
   /* "View.MemoryView":254
  *     cdef PyObject **p
  * 
  *     self.free_data = True             # <<<<<<<<<<<<<<
  *     self.data = <char *>malloc(self.len)
  *     if not self.data:
@@ -6758,15 +6821,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._allocate_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":268
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):             # <<<<<<<<<<<<<<
@@ -6782,15 +6844,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("array_cwrapper", 0);
+  __Pyx_RefNannySetupContext("array_cwrapper", 1);
 
   /* "View.MemoryView":270
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):
  *     cdef array result
  *     cdef str mode = "fortran" if c_mode[0] == b'f' else "c"  # this often comes from a constant C string.             # <<<<<<<<<<<<<<
  * 
  *     if buf is NULL:
@@ -6959,16 +7021,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 304, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -6994,18 +7055,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 304, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -7025,15 +7087,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "View.MemoryView":305
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
@@ -7080,15 +7142,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":307
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
@@ -7134,39 +7196,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.Enum.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_MemviewEnum___reduce_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7179,15 +7230,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.name,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -7416,16 +7467,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 16, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -7452,18 +7502,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -7487,15 +7538,15 @@
 static PyObject *__pyx_pf___pyx_MemviewEnum_2__setstate_cython__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0x82a3537, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -7545,16 +7596,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 349, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_flags,&__pyx_n_s_dtype_is_object,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -7612,18 +7662,19 @@
     __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     if (values[2]) {
       __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, __pyx_nargs); __PYX_ERR(1, 349, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -7651,15 +7702,15 @@
   int __pyx_t_2;
   int __pyx_t_3;
   Py_intptr_t __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "View.MemoryView":350
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
@@ -7986,22 +8037,20 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_2__dealloc__(struct __pyx_memoryview_obj *__pyx_v_self) {
   int __pyx_v_i;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyThread_type_lock __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":377
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
@@ -8191,15 +8240,14 @@
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":397
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
@@ -8218,15 +8266,15 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_item_pointer", 0);
+  __Pyx_RefNannySetupContext("get_item_pointer", 1);
 
   /* "View.MemoryView":399
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
@@ -8238,37 +8286,50 @@
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
-    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 401, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -8369,15 +8430,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":408
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
@@ -8980,15 +9041,15 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assignment", 1);
 
   /* "View.MemoryView":448
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  *         cdef __Pyx_memviewslice msrc = get_slice_from_memview(src, &src_slice)[0]             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mdst = get_slice_from_memview(dst, &dst_slice)[0]
  * 
@@ -9073,15 +9134,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 1);
 
   /* "View.MemoryView":455
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
@@ -9346,15 +9407,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_indexed", 0);
+  __Pyx_RefNannySetupContext("setitem_indexed", 1);
 
   /* "View.MemoryView":486
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
@@ -9417,15 +9478,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":492
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
@@ -9667,15 +9728,15 @@
   char *__pyx_t_9;
   char *__pyx_t_10;
   char *__pyx_t_11;
   char *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":508
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
@@ -10220,15 +10281,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
@@ -10306,15 +10367,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self._get_base()             # <<<<<<<<<<<<<<
  * 
  *     cdef _get_base(self):
@@ -10352,15 +10413,15 @@
  *         return self.obj
  * 
  */
 
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":565
  * 
  *     cdef _get_base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10416,15 +10477,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":569
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10502,15 +10563,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":573
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError, "Buffer view does not expose strides"
@@ -10617,15 +10678,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":581
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
@@ -10730,15 +10791,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":588
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10795,15 +10856,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":592
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10862,15 +10923,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":596
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10941,15 +11002,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":600
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
@@ -11071,17 +11132,15 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":611
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
@@ -11124,15 +11183,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":616
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
@@ -11160,15 +11218,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":617
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
@@ -11263,15 +11321,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__str__", 0);
+  __Pyx_RefNannySetupContext("__str__", 1);
 
   /* "View.MemoryView":621
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -11340,39 +11398,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_c_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 624, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_c_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_c_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_c_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11382,15 +11429,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_c_contig", 0);
+  __Pyx_RefNannySetupContext("is_c_contig", 1);
 
   /* "View.MemoryView":627
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
@@ -11454,39 +11501,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_f_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 630, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_f_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_f_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_f_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11496,15 +11532,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_f_contig", 0);
+  __Pyx_RefNannySetupContext("is_f_contig", 1);
 
   /* "View.MemoryView":633
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
@@ -11568,39 +11604,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 636, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11610,15 +11635,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy", 0);
+  __Pyx_RefNannySetupContext("copy", 1);
 
   /* "View.MemoryView":638
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
@@ -11700,39 +11725,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy_fortran (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 648, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy_fortran", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy_fortran", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy_fortran", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11743,15 +11757,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy_fortran", 0);
+  __Pyx_RefNannySetupContext("copy_fortran", 1);
 
   /* "View.MemoryView":650
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
@@ -11831,53 +11845,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryview___reduce_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -11933,16 +11936,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -11969,18 +11971,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -12003,15 +12006,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -12047,15 +12050,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
+  __Pyx_RefNannySetupContext("memoryview_cwrapper", 1);
 
   /* "View.MemoryView":663
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
@@ -12130,17 +12133,15 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("memoryview_check", 0);
 
   /* "View.MemoryView":669
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o) noexcept:
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
@@ -12155,15 +12156,14 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":671
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
@@ -12187,15 +12187,15 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_unellipsify", 0);
+  __Pyx_RefNannySetupContext("_unellipsify", 1);
 
   /* "View.MemoryView":677
  *     """
  *     cdef Py_ssize_t idx
  *     tup = <tuple>index if isinstance(index, tuple) else (index,)             # <<<<<<<<<<<<<<
  * 
  *     result = [slice(None)] * ndim
@@ -12269,21 +12269,28 @@
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   if (unlikely(__pyx_v_tup == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(1, 683, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_4 = 0;
   for (;;) {
-    if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
+      #endif
+      if (__pyx_t_4 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "View.MemoryView":684
  *     idx = 0
@@ -12544,23 +12551,21 @@
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
 static int assert_direct_dimensions(Py_ssize_t *__pyx_v_suboffsets, int __pyx_v_ndim) {
   Py_ssize_t __pyx_v_suboffset;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
   /* "View.MemoryView":701
  * 
  * cdef int assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim) except -1:
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError, "Indirect dimensions not supported"
@@ -12619,15 +12624,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView.assert_direct_dimensions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":711
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
@@ -12665,15 +12669,15 @@
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memview_slice", 0);
+  __Pyx_RefNannySetupContext("memview_slice", 1);
 
   /* "View.MemoryView":712
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
@@ -12815,37 +12819,50 @@
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             cindex = index
  */
   __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
-    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
+    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
     __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 747, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       } else {
-        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       }
     } else {
       __pyx_t_8 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_8)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -13216,25 +13233,23 @@
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
 static int __pyx_memoryview_slice_memviewslice(__Pyx_memviewslice *__pyx_v_dst, Py_ssize_t __pyx_v_shape, Py_ssize_t __pyx_v_stride, Py_ssize_t __pyx_v_suboffset, int __pyx_v_dim, int __pyx_v_new_ndim, int *__pyx_v_suboffset_dim, Py_ssize_t __pyx_v_start, Py_ssize_t __pyx_v_stop, Py_ssize_t __pyx_v_step, int __pyx_v_have_start, int __pyx_v_have_stop, int __pyx_v_have_step, int __pyx_v_is_slice) {
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("slice_memviewslice", 1);
 
   /* "View.MemoryView":813
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
@@ -13981,15 +13996,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.slice_memviewslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":896
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
@@ -14009,15 +14023,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_UCS4 __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pybuffer_index", 0);
+  __Pyx_RefNannySetupContext("pybuffer_index", 1);
 
   /* "View.MemoryView":898
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
@@ -14336,15 +14350,14 @@
 static int __pyx_memslice_transpose(__Pyx_memviewslice *__pyx_v_memslice) {
   int __pyx_v_ndim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
@@ -14352,15 +14365,14 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("transpose_memslice", 1);
 
   /* "View.MemoryView":930
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) except -1 nogil:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
@@ -14495,15 +14507,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.transpose_memslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":963
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -14521,16 +14532,14 @@
   __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":964
  * 
  *     def __dealloc__(self):
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
@@ -14542,15 +14551,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":966
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
@@ -14561,15 +14569,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":967
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
@@ -14648,15 +14656,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":973
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
@@ -14725,15 +14733,15 @@
  *         return self.from_object
  * 
  */
 
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":979
  * 
  *     cdef _get_base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  * 
@@ -14779,53 +14787,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryviewslice___reduce_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -14881,16 +14878,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -14917,18 +14913,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -14951,15 +14948,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -15003,15 +15000,15 @@
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
+  __Pyx_RefNannySetupContext("memoryview_fromslice", 1);
 
   /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -15380,15 +15377,15 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
+  __Pyx_RefNannySetupContext("get_slice_from_memview", 1);
 
   /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
@@ -15477,22 +15474,20 @@
  */
 
 static void __pyx_memoryview_slice_copy(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_dst) {
   int __pyx_v_dim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   Py_ssize_t *__pyx_v_suboffsets;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
-  __Pyx_RefNannySetupContext("slice_copy", 0);
 
   /* "View.MemoryView":1067
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
@@ -15589,15 +15584,14 @@
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
@@ -15608,15 +15602,15 @@
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy", 1);
 
   /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
@@ -15672,15 +15666,15 @@
   int __pyx_t_1;
   PyObject *(*__pyx_t_2)(char *);
   int (*__pyx_t_3)(char *, PyObject *);
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 1);
 
   /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
@@ -16481,28 +16475,26 @@
 
 static void *__pyx_memoryview_copy_data_to_temp(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_tmpslice, char __pyx_v_order, int __pyx_v_ndim) {
   int __pyx_v_i;
   void *__pyx_v_result;
   size_t __pyx_v_itemsize;
   size_t __pyx_v_size;
   void *__pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("copy_data_to_temp", 1);
 
   /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
@@ -16722,15 +16714,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.copy_data_to_temp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1247
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
@@ -16942,22 +16933,20 @@
  * cdef int _err_no_memory() except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise MemoryError
  * 
  */
 
 static int __pyx_memoryview_err_no_memory(void) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_err_no_memory", 0);
 
   /* "View.MemoryView":1261
  * @cname('__pyx_memoryview_err_no_memory')
  * cdef int _err_no_memory() except -1 with gil:
  *     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  * 
@@ -16972,15 +16961,14 @@
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._err_no_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
 /* "View.MemoryView":1265
@@ -16997,29 +16985,27 @@
   int __pyx_v_i;
   char __pyx_v_order;
   int __pyx_v_broadcasting;
   int __pyx_v_direct_copy;
   __Pyx_memviewslice __pyx_v_tmp;
   int __pyx_v_ndim;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("memoryview_copy_contents", 1);
 
   /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
@@ -17556,15 +17542,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.memoryview_copy_contents", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
@@ -17730,19 +17715,17 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
-  __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
   /* "View.MemoryView":1368
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
@@ -17754,15 +17737,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "View.MemoryView":1371
  * 
@@ -17771,20 +17753,18 @@
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   CYTHON_UNUSED Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_stride;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
   /* "View.MemoryView":1374
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(shape[0]):
@@ -17890,15 +17870,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1391
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
@@ -18112,16 +18091,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -18176,18 +18154,19 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -18217,15 +18196,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 1);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x82a3537, 0x6ae9995, 0xb068931):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
@@ -18399,15 +18378,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 1);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  *     __pyx_result.name = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -18515,292 +18494,292 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18811,46 +18790,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18861,46 +18840,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18911,46 +18890,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18961,46 +18940,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19011,212 +18990,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
+  __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19230,17 +19206,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
+  __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19248,68 +19224,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 984, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19317,15 +19293,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19340,15 +19316,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19362,17 +19338,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
+  __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19380,68 +19356,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 990, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19449,15 +19425,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19472,15 +19448,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19494,17 +19470,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19512,68 +19488,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 996, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19581,15 +19557,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19604,176 +19580,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19789,20 +19759,18 @@
  *     cdef char* c_string = <char *> malloc((length + 1) * sizeof(char))
  *     if not c_string:
  */
 
 static char *__pyx_f_4bean_7mapping_16CRISPResso2Align_get_c_string_with_length(size_t __pyx_v_length) {
   char *__pyx_v_c_string;
   char *__pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_c_string_with_length", 0);
 
   /* "bean/mapping/CRISPResso2Align.pyx":29
  * 
  * cdef char* get_c_string_with_length(size_t length):
  *     cdef char* c_string = <char *> malloc((length + 1) * sizeof(char))             # <<<<<<<<<<<<<<
  *     if not c_string:
  *         raise MemoryError()
@@ -19856,15 +19824,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("bean.mapping.CRISPResso2Align.get_c_string_with_length", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "bean/mapping/CRISPResso2Align.pyx":35
  * 
  * 
  * def read_matrix(path):             # <<<<<<<<<<<<<<
@@ -19901,16 +19868,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_matrix (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 35, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_path,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -19937,18 +19903,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_path = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("read_matrix", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 35, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -20004,15 +19971,15 @@
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *(*__pyx_t_19)(PyObject *);
   int __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("read_matrix", 0);
+  __Pyx_RefNannySetupContext("read_matrix", 1);
   __pyx_pybuffer_a.pybuffer.buf = NULL;
   __pyx_pybuffer_a.refcount = 0;
   __pyx_pybuffernd_a.data = NULL;
   __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
 
   /* "bean/mapping/CRISPResso2Align.pyx":42
  *     """
@@ -20048,15 +20015,15 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+      PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_t_4 = __pyx_t_3;
@@ -20115,15 +20082,15 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
                 __pyx_t_6 = 1;
               }
             }
             #endif
             {
-              PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+              PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
               __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
               __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
               if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L7_error)
               __Pyx_GOTREF(__pyx_t_1);
               __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             }
             __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strip); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 48, __pyx_L7_error)
@@ -20140,15 +20107,15 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
                 __pyx_t_6 = 1;
               }
             }
             #endif
             {
-              PyObject *__pyx_callargs[1] = {__pyx_t_1, };
+              PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
               __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
               __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
               if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L7_error)
               __Pyx_GOTREF(__pyx_t_4);
               __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             }
             __Pyx_XDECREF_SET(__pyx_v_line, __pyx_t_4);
@@ -20200,38 +20167,51 @@
                 __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
                 __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
                 if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L18_error)
                 __Pyx_GOTREF(__pyx_t_3);
                 __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
               }
               if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
-                __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_11 = 0;
+                __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1);
+                __pyx_t_11 = 0;
                 __pyx_t_12 = NULL;
               } else {
                 __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L18_error)
                 __Pyx_GOTREF(__pyx_t_1);
                 __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 50, __pyx_L18_error)
               }
               __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
               for (;;) {
                 if (likely(!__pyx_t_12)) {
                   if (likely(PyList_CheckExact(__pyx_t_1))) {
-                    if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_1)) break;
+                    {
+                      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+                      #if !CYTHON_ASSUME_SAFE_MACROS
+                      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L18_error)
+                      #endif
+                      if (__pyx_t_11 >= __pyx_temp) break;
+                    }
                     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                     __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L18_error)
                     #else
-                    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L18_error)
+                    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L18_error)
                     __Pyx_GOTREF(__pyx_t_3);
                     #endif
                   } else {
-                    if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+                    {
+                      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+                      #if !CYTHON_ASSUME_SAFE_MACROS
+                      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 50, __pyx_L18_error)
+                      #endif
+                      if (__pyx_t_11 >= __pyx_temp) break;
+                    }
                     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                     __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_3); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 50, __pyx_L18_error)
                     #else
-                    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L18_error)
+                    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 50, __pyx_L18_error)
                     __Pyx_GOTREF(__pyx_t_3);
                     #endif
                   }
                 } else {
                   __pyx_t_3 = __pyx_t_12(__pyx_t_1);
                   if (unlikely(!__pyx_t_3)) {
                     PyObject* exc_type = PyErr_Occurred();
@@ -20363,15 +20343,15 @@
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_5, function);
               __pyx_t_6 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[1] = {__pyx_t_3, };
+            PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
             __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
             if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __Pyx_XDECREF_SET(__pyx_v_line, __pyx_t_1);
@@ -20425,38 +20405,51 @@
                 __Pyx_GOTREF(__pyx_t_5);
                 __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
               }
               __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_t_5, 1, 0, NULL, NULL, &__pyx_slice__14, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L28_error)
               __Pyx_GOTREF(__pyx_t_4);
               __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
               if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
-                __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_11 = 0;
+                __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5);
+                __pyx_t_11 = 0;
                 __pyx_t_12 = NULL;
               } else {
                 __pyx_t_11 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 57, __pyx_L28_error)
                 __Pyx_GOTREF(__pyx_t_5);
                 __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 57, __pyx_L28_error)
               }
               __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
               for (;;) {
                 if (likely(!__pyx_t_12)) {
                   if (likely(PyList_CheckExact(__pyx_t_5))) {
-                    if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_5)) break;
+                    {
+                      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
+                      #if !CYTHON_ASSUME_SAFE_MACROS
+                      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 57, __pyx_L28_error)
+                      #endif
+                      if (__pyx_t_11 >= __pyx_temp) break;
+                    }
                     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                     __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_11); __Pyx_INCREF(__pyx_t_4); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 57, __pyx_L28_error)
                     #else
-                    __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L28_error)
+                    __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L28_error)
                     __Pyx_GOTREF(__pyx_t_4);
                     #endif
                   } else {
-                    if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+                    {
+                      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
+                      #if !CYTHON_ASSUME_SAFE_MACROS
+                      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 57, __pyx_L28_error)
+                      #endif
+                      if (__pyx_t_11 >= __pyx_temp) break;
+                    }
                     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                     __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_11); __Pyx_INCREF(__pyx_t_4); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 57, __pyx_L28_error)
                     #else
-                    __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L28_error)
+                    __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L28_error)
                     __Pyx_GOTREF(__pyx_t_4);
                     #endif
                   }
                 } else {
                   __pyx_t_4 = __pyx_t_12(__pyx_t_5);
                   if (unlikely(!__pyx_t_4)) {
                     PyObject* exc_type = PyErr_Occurred();
@@ -20504,38 +20497,51 @@
             __Pyx_INCREF(__pyx_v_line_vals);
             __Pyx_GIVEREF(__pyx_v_line_vals);
             if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_line_vals)) __PYX_ERR(0, 58, __pyx_L7_error);
             __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_zip, __pyx_t_1, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             if (likely(PyList_CheckExact(__pyx_t_5)) || PyTuple_CheckExact(__pyx_t_5)) {
-              __pyx_t_1 = __pyx_t_5; __Pyx_INCREF(__pyx_t_1); __pyx_t_11 = 0;
+              __pyx_t_1 = __pyx_t_5; __Pyx_INCREF(__pyx_t_1);
+              __pyx_t_11 = 0;
               __pyx_t_12 = NULL;
             } else {
               __pyx_t_11 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L7_error)
               __Pyx_GOTREF(__pyx_t_1);
               __pyx_t_12 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 58, __pyx_L7_error)
             }
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             for (;;) {
               if (likely(!__pyx_t_12)) {
                 if (likely(PyList_CheckExact(__pyx_t_1))) {
-                  if (__pyx_t_11 >= PyList_GET_SIZE(__pyx_t_1)) break;
+                  {
+                    Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+                    #if !CYTHON_ASSUME_SAFE_MACROS
+                    if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 58, __pyx_L7_error)
+                    #endif
+                    if (__pyx_t_11 >= __pyx_temp) break;
+                  }
                   #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                   __pyx_t_5 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 58, __pyx_L7_error)
                   #else
-                  __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L7_error)
+                  __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L7_error)
                   __Pyx_GOTREF(__pyx_t_5);
                   #endif
                 } else {
-                  if (__pyx_t_11 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+                  {
+                    Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+                    #if !CYTHON_ASSUME_SAFE_MACROS
+                    if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 58, __pyx_L7_error)
+                    #endif
+                    if (__pyx_t_11 >= __pyx_temp) break;
+                  }
                   #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                   __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_11); __Pyx_INCREF(__pyx_t_5); __pyx_t_11++; if (unlikely((0 < 0))) __PYX_ERR(0, 58, __pyx_L7_error)
                   #else
-                  __pyx_t_5 = PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L7_error)
+                  __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_11); __pyx_t_11++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L7_error)
                   __Pyx_GOTREF(__pyx_t_5);
                   #endif
                 }
               } else {
                 __pyx_t_5 = __pyx_t_12(__pyx_t_1);
                 if (unlikely(!__pyx_t_5)) {
                   PyObject* exc_type = PyErr_Occurred();
@@ -20661,15 +20667,15 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_3, function);
                 __pyx_t_6 = 1;
               }
             }
             #endif
             {
-              PyObject *__pyx_callargs[1] = {__pyx_t_5, };
+              PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
               __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
               __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
               if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L7_error)
               __Pyx_GOTREF(__pyx_t_1);
               __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
             }
             __Pyx_DECREF_SET(__pyx_v_line, __pyx_t_1);
@@ -20855,16 +20861,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("global_align_base_editor (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 65, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pystr_seqj,&__pyx_n_s_pystr_seqi,&__pyx_n_s_ref_base,&__pyx_n_s_alt_base,&__pyx_n_s_matrix,&__pyx_n_s_gap_incentive,&__pyx_n_s_gap_open,&__pyx_n_s_gap_extend,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -20995,18 +21000,19 @@
     }
     if (values[7]) {
       __pyx_v_gap_extend = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_gap_extend == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L3_error)
     } else {
       __pyx_v_gap_extend = ((int)((int)-1));
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("global_align_base_editor", 0, 6, 8, __pyx_nargs); __PYX_ERR(0, 65, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -21111,15 +21117,15 @@
   PyObject *__pyx_t_30 = NULL;
   char const *__pyx_t_31;
   long __pyx_t_32;
   double __pyx_t_33;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("global_align_base_editor", 0);
+  __Pyx_RefNannySetupContext("global_align_base_editor", 1);
   __pyx_pybuffer_matrix.pybuffer.buf = NULL;
   __pyx_pybuffer_matrix.refcount = 0;
   __pyx_pybuffernd_matrix.data = NULL;
   __pyx_pybuffernd_matrix.rcbuffer = &__pyx_pybuffer_matrix;
   __pyx_pybuffer_gap_incentive.pybuffer.buf = NULL;
   __pyx_pybuffer_gap_incentive.refcount = 0;
   __pyx_pybuffernd_gap_incentive.data = NULL;
@@ -25727,26 +25733,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../../tmp/pip-build-env-zjqb65zd/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/pip-build-env-wqrzmyjr/overlay/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 992, __pyx_L1_error)
@@ -26189,41 +26195,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 812, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 814, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 816, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 818, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 820, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 822, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 824, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 826, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 828, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 830, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 868, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 812, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 814, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 816, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 818, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 820, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 822, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 824, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 828, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 830, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 868, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -26435,42 +26441,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("CRISPResso2Align", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to CRISPResso2Align pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "CRISPResso2Align" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_CRISPResso2Align(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -27291,14 +27295,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -27348,33 +27354,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -27582,21 +27595,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
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
@@ -27681,15 +27712,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -27700,15 +27731,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -27732,15 +27763,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -28019,17 +28050,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
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
@@ -28098,16 +28135,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -28116,30 +28158,36 @@
 #endif
 
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
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
@@ -28147,36 +28195,25 @@
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -28192,33 +28229,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
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
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
@@ -28513,15 +28556,15 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if PY_VERSION_HEX >= 0x030D0000
+            #if PY_VERSION_HEX >= 0x030d0000
             if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
             #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
@@ -28642,15 +28685,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
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
 
 /* PyObjectCallOneArg */
@@ -28677,15 +28720,17 @@
     }
     return NULL;
 }
 static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
     __Pyx_TypeName obj_type_name;
     if (likely(PyType_Check(obj))) {
         PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (meth) {
+        if (!meth) {
+            PyErr_Clear();
+        } else {
             PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
             Py_DECREF(meth);
             return result;
         }
     }
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
@@ -28786,36 +28831,43 @@
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
 /* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
+#endif
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r;
-#if CYTHON_USE_TYPE_SLOTS
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
     if (likely(PyString_Check(n))) {
         r = __Pyx_PyObject_GetAttrStrNoError(o, n);
         if (unlikely(!r) && likely(!PyErr_Occurred())) {
             r = __Pyx_NewRef(d);
         }
         return r;
     }
-#endif
+  #endif
     r = PyObject_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -28845,15 +28897,15 @@
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
@@ -29171,15 +29223,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -29334,24 +29386,14 @@
     } else if (PyErr_Occurred()) {
         PyErr_Clear();
     }
 #endif
     return __Pyx__ImportDottedModule(name, parts_tuple);
 }
 
-/* ssize_strlen */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
-    size_t len = strlen(s);
-    if (unlikely(len > PY_SSIZE_T_MAX)) {
-        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
-        return -1;
-    }
-    return (Py_ssize_t) len;
-}
-
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
@@ -29527,19 +29569,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_ass_item(o, i, v);
         }
     }
 #else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
+    if (is_list || !PyMapping_Check(o))
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
@@ -29596,14 +29634,15 @@
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
@@ -29612,14 +29651,15 @@
         PyErr_Clear();
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
+#endif
 
 /* PyObjectLookupSpecial */
 #if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error) {
     PyObject *res;
     PyTypeObject *tp = Py_TYPE(obj);
 #if PY_MAJOR_VERSION < 3
@@ -30513,17 +30553,18 @@
     __Pyx_DECREF_TypeName(obj_type_name);
 bad:
     return NULL;
 }
 
 /* IterFinish */
   static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -30537,17 +30578,18 @@
         return -1;
     }
     return __Pyx_IterFinish();
 }
 
 /* UnpackUnboundCMethod */
   static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
     PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
     if (unlikely(!selfless_args)) return NULL;
-    PyObject *result = PyObject_Call(method, selfless_args, kwargs);
+    result = PyObject_Call(method, selfless_args, kwargs);
     Py_DECREF(selfless_args);
     return result;
 }
 static PyMethodDef __Pyx_UnboundCMethod_Def = {
      "CythonUnboundCMethod",
      __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
      METH_VARARGS | METH_KEYWORDS,
@@ -30559,25 +30601,23 @@
     if (unlikely(!method))
         return -1;
     target->method = method;
 #if CYTHON_COMPILING_IN_CPYTHON
     #if PY_MAJOR_VERSION >= 3
     if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
     #else
-    if (likely(!PyCFunction_Check(method)))
+    if (likely(!__Pyx_CyOrPyCFunction_Check(method)))
     #endif
     {
         PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
         target->func = descr->d_method->ml_meth;
         target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
     } else
 #endif
-#if defined(CYTHON_COMPILING_IN_PYPY)
-#elif PY_VERSION_HEX >= 0x03090000
-    if (PyCFunction_CheckExact(method))
+#if CYTHON_COMPILING_IN_PYPY
 #else
     if (PyCFunction_Check(method))
 #endif
     {
         PyObject *self;
         int self_found;
 #if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
@@ -30810,16 +30850,16 @@
 #endif
     return 0;
 }
 #endif
 
 /* PyObjectCallNoArg */
   static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
   static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
@@ -30976,46 +31016,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -31301,18 +31341,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -31358,23 +31398,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -31382,18 +31422,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* FetchSharedCythonModule */
   static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
   static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -31546,15 +31583,29 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
-  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
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
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
@@ -32355,15 +32406,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -32694,16 +32745,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -32715,14 +32766,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -32812,15 +32865,15 @@
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
@@ -33894,15 +33947,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -34030,38 +34083,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
@@ -34092,38 +34147,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
@@ -34291,15 +34348,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -34427,38 +34484,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(char),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(char));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
@@ -34626,15 +34685,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -34899,15 +34958,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -35019,49 +35078,58 @@
         name = __Pyx_NewRef(__pyx_n_s__35);
     }
     return name;
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
-                      "compile time version %s of module '%.100s' "
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
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -35099,16 +35167,32 @@
             return -1;
         #endif
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
```

### Comparing `crispr-bean-0.2.7/bean/mapping/CRISPResso2Align.pyx` & `crispr-bean-1.0.0/bean/mapping/CRISPResso2Align.pyx`

 * *Files identical despite different names*

### Comparing `crispr-bean-0.2.7/bean/mapping/GuideEditCounter.py` & `crispr-bean-1.0.0/bean/mapping/GuideEditCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from tqdm import tqdm
 
 from ._supporting_fn import (
     _base_edit_to_from,
     _check_readname_match,
     _get_edited_allele_crispresso,
     _get_fastq_handle,
-    _multiindex_dict_to_df,
     _read_count_match,
     _read_is_good_quality,
     _write_alignment_matrix,
     _write_paired_end_reads,
     revcomp,
 )
 
@@ -44,14 +43,15 @@
 
 
 class NoReadsAfterQualityFiltering(Exception):
     """Raised when no reads are remaining after quality filtering."""
 
 
 strand_str_to_int = {"neg": -1, "pos": 1, "-": -1, "+": 1}
+base_revcomp = {"A": "T", "T": "A", "G": "C", "C": "G"}
 
 
 def _get_stranded_guide_offset(strand: int, start_pos: int, guide_len: int) -> int:
     if strand == -1:
         offset = start_pos + 32 - 6 - 1
     elif strand == 1:
         offset = start_pos - (32 - 6 - guide_len)
@@ -119,16 +119,17 @@
             self.screen.uns["allele_counts"] = {}
         self.count_guide_reporter_alleles = kwargs["count_guide_reporter_alleles"]
         if self.count_guide_reporter_alleles:
             self.guide_to_guide_reporter_allele = {}
         self.align_score_threshold = 80
         self.target_pos_col = kwargs["target_pos_col"]
 
-        self.guide_start_seq = kwargs["guide_start_seq"]
-        self.guide_end_seq = kwargs["guide_end_seq"]
+        self.guide_start_seq = kwargs["guide_start_seq"].upper()
+        self.guide_end_seq = kwargs["guide_end_seq"].upper()
+        self.barcode_start_seq = kwargs["barcode_start_seq"].upper()
         if not self.guide_start_seq == "":
             info(
                 f"{self.name}: Using guide_start_seq={self.guide_start_seq} for {self.output_dir}"
             )
         assert (
             self.guide_start_seq == "" or self.guide_end_seq == ""
         ), "Doesn't support both start & end seq matching"
@@ -187,25 +188,25 @@
             os.path.basename(self.R1_filename).replace(".fastq", "").replace(".gz", "")
             + "_filtered.fastq.gz"
         )
         self.filtered_R2_filename = self._jp(
             os.path.basename(self.R2_filename).replace(".fastq", "").replace(".gz", "")
             + "_filtered.fastq.gz"
         )
-        if path.exists(self.filtered_R1_filename) and path.exists(
-            self.filtered_R2_filename
-        ):
-            warn("Using preexisting filtered file")
-        else:
-            self._check_names_filter_fastq()
+        self._check_names_filter_fastq()
+        # if (
+        #     path.exists(self.filtered_R1_filename)
+        #     and path.exists(self.filtered_R2_filename)
+        #     and self.reuse_filtered_reads
+        # ):
+        #     warn("Using preexisting filtered file")
+        # else:
+        #     self._check_names_filter_fastq()
 
     def get_counts(self):
-        # infile_R1 = _get_fastq_handle(self.R1_filename)
-        # infile_R2 = _get_fastq_handle(self.R2_filename)
-
         self.nomatch_R1_filename = self.R1_filename.replace(".fastq", "_nomatch.fastq")
         self.nomatch_R2_filename = self.R2_filename.replace(".fastq", "_nomatch.fastq")
         self.semimatch_R1_filename = self.R1_filename.replace(
             ".fastq", "_semimatch.fastq"
         )
         self.semimatch_R2_filename = self.R2_filename.replace(
             ".fastq", "_semimatch.fastq"
@@ -330,58 +331,65 @@
         )
 
         if "guide" in self.screen.uns["guide_edit_counts"].columns:
             self.screen.uns["guide_edit_counts"].guide = self.screen.guides.index[
                 self.screen.uns["guide_edit_counts"].guide
             ]
 
-    def _get_guide_counts_bcmatch(self):
-        NotImplemented
-
     def _count_guide_edits(
         self, matched_guide_idx, R1_record: SeqIO.SeqRecord, single_base_qual_cutoff=30
     ):
         if self.guides_has_strands:
-            strand = self.screen.guides.strand[matched_guide_idx]
+            strand = self.screen.guides.strand.iloc[matched_guide_idx]
             guide_strand = strand_str_to_int.get(strand, 1)
         else:
             guide_strand = 1
-        ref_guide_seq = self.screen.guides.sequence[matched_guide_idx]
+        ref_guide_seq = self.screen.guides.sequence.iloc[matched_guide_idx]
+        if "chrom" in self.screen.guides.columns.tolist():
+            chrom = self.screen.guides.chrom.iloc[matched_guide_idx]
+        else:
+            if self.screen.tiling:
+                raise ValueError(
+                    "'chrom' column denoting gRNA chromosome location column not present in the input. Please check the input file."
+                )
+            else:
+                chrom = None
         read_guide_seq, read_guide_qual = self.get_guide_seq_qual(
             R1_record, len(ref_guide_seq)
         )
         guide_edit_allele, score = _get_edited_allele_crispresso(
             ref_seq=ref_guide_seq,
             query_seq=read_guide_seq,
             ref_base=self.base_edited_from,
             alt_base=self.base_edited_to,
             aln_mat_path=self.output_dir + "/.aln_mat.txt",
             offset=0,
             strand=guide_strand,
+            chrom=chrom,
             start_pos=0,
             end_pos=len(ref_guide_seq),
             positionwise_quality=np.array(read_guide_qual),
             quality_thres=single_base_qual_cutoff,
             objectify_allele=self.objectify_allele,
         )
 
         if not self.count_reporter_edits:
             self._update_counted_guide_allele(matched_guide_idx, guide_edit_allele)
         return (guide_edit_allele, score)
 
     def _get_strand_offset_from_guide_index(self, guide_idx: int) -> Tuple[int, int]:
         """Returns guide starnd and offset for a given guide index."""
         if self.guides_has_strands:
-            strand = self.screen.guides.strand[guide_idx]
+            strand = self.screen.guides.strand.iloc[guide_idx]
             if strand in strand_str_to_int:
                 guide_strand = strand_str_to_int[strand]
                 offset = _get_stranded_guide_offset(
                     strand=guide_strand,
-                    start_pos=self.screen.guides.start_pos[guide_idx],
-                    guide_len=self.screen.guides.guide_len[guide_idx],
+                    start_pos=self.screen.guides.start_pos.iloc[guide_idx],
+                    guide_len=self.screen.guides.guide_len.iloc[guide_idx],
                 )
             else:
                 guide_strand = 1
                 offset = 0
 
         else:
             guide_strand = 1
@@ -430,43 +438,50 @@
             self.guide_to_guide_reporter_allele[guide_idx] = {(allele, guide_allele): 1}
 
     def _count_reporter_edits(
         self,
         matched_guide_idx: int,
         R1_seq: str,
         R2_record: SeqIO.SeqRecord,
+        R2_start: int = 0,
         single_base_qual_cutoff: str = 30,
         guide_allele: Allele = None,
     ):
         """
         Count edits in a single read to save as allele.
 
         Args
         --
         matched_guide_idx: index of guides in self.screen.guides to get information from
         R1_seq: Read1 sequence
         R2_record: Read2 sequence record with quality
         single_base_qual_cutoff: Ignore this base if the Phread quality score is less than this threshold
         guide_allele: Allele from baseedit in gRNA spacer sequence when paired with guide allele.
         """
-        ref_reporter_seq = self.screen.guides.reporter[matched_guide_idx]
-        read_reporter_seq, read_reporter_qual = self.get_reporter_seq_qual(R2_record)
+        ref_reporter_seq = self.screen.guides.reporter.iloc[matched_guide_idx]
+        read_reporter_seq, read_reporter_qual = self.get_reporter_seq_qual(
+            R2_record, R2_start
+        )
 
         guide_strand, offset = self._get_strand_offset_from_guide_index(
             matched_guide_idx
         )
-
+        if "chrom" in self.screen.guides.columns.tolist():
+            chrom = self.screen.guides.chrom.iloc[matched_guide_idx]
+        else:
+            chrom = None
         allele, score = _get_edited_allele_crispresso(
             ref_seq=ref_reporter_seq,
             query_seq=read_reporter_seq,
             ref_base=self.base_edited_from,
             alt_base=self.base_edited_to,
             aln_mat_path=self.output_dir + "/.aln_mat.txt",
             offset=offset,
             strand=guide_strand,
+            chrom=chrom,
             positionwise_quality=np.array(read_reporter_qual),
             quality_thres=single_base_qual_cutoff,
             objectify_allele=self.objectify_allele,
         )
 
         if score < self.align_score_threshold:
             self.semimatch += 1
@@ -478,18 +493,20 @@
 
         if self.count_guide_reporter_alleles and (guide_allele is not None):
             self._update_counted_allele_and_guideAllele(
                 matched_guide_idx, allele, guide_allele
             )
 
     def _get_guide_counts_bcmatch_semimatch(
-        self, bcmatch_layer="X_bcmatch", semimatch_layer="X"
+        self, bcmatch_layer="X_bcmatch", semimatch_layer="X_semimatch"
     ):
         self.screen.layers[semimatch_layer] = np.zeros_like((self.screen.X))
-        R1_iter, R2_iter = self._get_fastq_iterators()
+        R1_iter, R2_iter = self._get_fastq_iterators(
+            self.filtered_R1_filename, self.filtered_R2_filename
+        )
         if self.keep_intermediate:
             outfile_R1_nomatch, outfile_R2_nomatch = self._get_fastq_handle("nomatch")
             outfile_R1_semimatch, outfile_R2_semimatch = self._get_fastq_handle(
                 "semimatch"
             )
             outfile_R1_dup_wo_bc, outfile_R2_dup_wo_bc = self._get_fastq_handle(
                 "duplicate_wo_barcode"
@@ -500,18 +517,19 @@
             total=self.n_reads_after_filtering,
             postfix=f"n_read={self.bcmatch}",
         ) as tqdm_reads:
             for i, (r1, r2) in tqdm_reads:
                 R1_seq = str(r1.seq)
                 R2_seq = str(r2.seq)
 
-                bc_match, semimatch = self._match_read_to_sgRNA_bcmatch_semimatch(
-                    R1_seq, R2_seq
-                )
-
+                (
+                    bc_match,
+                    semimatch,
+                    R2_start,
+                ) = self._match_read_to_sgRNA_bcmatch_semimatch(R1_seq, R2_seq)
                 if len(bc_match) == 0:
                     if len(semimatch) == 0:  # no guide match
                         if self.keep_intermediate:
                             _write_paired_end_reads(
                                 r1, r2, outfile_R1_nomatch, outfile_R2_nomatch
                             )
                         self.nomatch += 1
@@ -541,18 +559,27 @@
                     self.bcmatch += 1
                     if self.count_guide_edits or self.count_guide_reporter_alleles:
                         guide_allele, _ = self._count_guide_edits(matched_guide_idx, r1)
                     if self.count_reporter_edits:
                         # TODO: what if reporter seq doesn't match barcode & guide?
                         if self.count_guide_reporter_alleles:
                             self._count_reporter_edits(
-                                matched_guide_idx, R1_seq, r2, guide_allele=guide_allele
+                                matched_guide_idx,
+                                R1_seq,
+                                r2,
+                                R2_start=R2_start,
+                                guide_allele=guide_allele,
                             )
                         else:
-                            self._count_reporter_edits(matched_guide_idx, R1_seq, r2)
+                            self._count_reporter_edits(
+                                matched_guide_idx,
+                                R1_seq,
+                                r2,
+                                R2_start=R2_start,
+                            )
                 tqdm_reads.postfix = f"n_read={self.bcmatch}"
                 tqdm_reads.update()
 
         self.screen.X = (
             self.screen.layers[semimatch_layer] + self.screen.layers[bcmatch_layer]
         )
 
@@ -629,27 +656,44 @@
 
     def get_reporter_seq(self, R1_seq, R2_seq):
         """This can be edited by user based on the read construct."""
         return revcomp(
             R2_seq[self.guide_bc_len : (self.guide_bc_len + self.reporter_length)]
         )
 
-    def get_reporter_seq_qual(self, R2_record: SeqIO.SeqRecord):
+    def get_reporter_seq_qual(self, R2_record: SeqIO.SeqRecord, R2_start=0):
         seq = R2_record[
-            self.guide_bc_len : (self.guide_bc_len + self.reporter_length)
+            (R2_start + self.guide_bc_len) : (
+                R2_start + self.guide_bc_len + self.reporter_length
+            )
         ].reverse_complement()
         return (str(seq.seq), seq.letter_annotations["phred_quality"])
 
     def get_barcode(self, R1_seq, R2_seq):
-        """This can be edited by user based on the read construct."""
-        return revcomp(R2_seq[: self.guide_bc_len])
+        if self.barcode_start_seq != "":
+            barcode_start_idx = R2_seq.replace(
+                base_revcomp[self.base_edited_from], base_revcomp[self.base_edited_to]
+            ).find(
+                revcomp(self.barcode_start_seq).replace(
+                    base_revcomp[self.base_edited_from],
+                    base_revcomp[self.base_edited_to],
+                )
+            )
+            if barcode_start_idx == -1:
+                return -1, ""
+            barcode_start_idx += len(self.barcode_start_seq)
+        else:
+            barcode_start_idx = 0
+        return barcode_start_idx, revcomp(
+            R2_seq[barcode_start_idx : (barcode_start_idx + self.guide_bc_len)]
+        )
 
     def _match_read_to_sgRNA_bcmatch_semimatch(self, R1_seq: str, R2_seq: str):
         # This should be adjusted for each experimental recipes.
-        guide_barcode = self.get_barcode(R1_seq, R2_seq)
+        bc_start_idx, guide_barcode = self.get_barcode(R1_seq, R2_seq)
         bc_match_idx = np.array([])
         semimatch_idx = np.array([])
         for guide_length in self.guide_lengths:
             seq = self.get_guide_seq(R1_seq, R2_seq, guide_length)
             if seq is None:
                 continue
 
@@ -663,15 +707,15 @@
             )[0]
 
             bc_match_idx = np.append(
                 bc_match_idx, np.intersect1d(_seq_match, _bc_match)
             )
             semimatch_idx = np.append(semimatch_idx, _seq_match)
 
-        return (bc_match_idx.astype(int), semimatch_idx.astype(int))
+        return bc_match_idx.astype(int), semimatch_idx.astype(int), bc_start_idx
 
     def _get_guide_position_seq_of_read(self, seq):
         guide_start_idx = self._get_guide_start_idx(seq)
         if guide_start_idx == -1:
             return None
 
         return [
@@ -700,88 +744,95 @@
         R1_filename = self.R1_filename.replace(".fastq", f"_{out_type}.fastq")
         R2_filename = self.R2_filename.replace(".fastq", f"_{out_type}.fastq")
         R1_handle = _get_fastq_handle(R1_filename, "w")
         R2_handle = _get_fastq_handle(R2_filename, "w")
 
         return (R1_handle, R2_handle)
 
-    def _get_fastq_iterators(self):
-        R1_handle = _get_fastq_handle(self.R1_filename)
-        R2_handle = _get_fastq_handle(self.R2_filename)
+    def _get_fastq_iterators(self, R1_filename=None, R2_filename=None):
+        if R1_filename is None:
+            R1_filename = self.R1_filename
+        if R2_filename is None:
+            R2_filename = self.R2_filename
+        R1_handle = _get_fastq_handle(R1_filename)
+        R2_handle = _get_fastq_handle(R2_filename)
 
         R1_iterator = FastqPhredIterator(R1_handle)
         R2_iterator = FastqPhredIterator(R2_handle)
 
         return (R1_iterator, R2_iterator)
 
-    def _get_seq_records(self):
+    def _get_seq_handles(self):
         R1_handle = _get_fastq_handle(self.R1_filename)
         R2_handle = _get_fastq_handle(self.R2_filename)
-        R1 = list(SeqIO.parse(R1_handle, "fastq"))
-        R2 = list(SeqIO.parse(R2_handle, "fastq"))
-        R1_handle.close()
-        R2_handle.close()
-        return (R1, R2)
+        return (R1_handle, R2_handle)
 
     def _check_names_filter_fastq(self, filter_by_qual=False):
         if self.min_average_read_quality > 0 or self.min_single_bp_quality > 0:
             info(
                 f"Filtering reads with average bp quality < {self.min_average_read_quality} and single bp quality < {self.min_single_bp_quality} ..."
             )
 
         if self.qend_R1 > 0 or self.qend_R2 > 0:
             info(
                 f"In the filtering, bases up to position {self.qend_R1} of R1 and {self.qend_R2} of R2 are considered."
             )
 
-        R1, R2 = self._get_seq_records()
+        R1_iter, R2_iter = self._get_fastq_iterators()
+        (self.n_reads_after_filtering) = self._check_readname_match_and_filter_quality(
+            R1_iter, R2_iter, filter_by_qual
+        )
 
-        _check_readname_match(R1, R2)
-        if filter_by_qual:
-            self.n_reads_after_filtering = self._filter_read_quality(R1, R2)
-            if self.n_reads_after_filtering == 0:
-                raise NoReadsAfterQualityFiltering(
-                    "No reads in input or no reads survived the average or single bp quality filtering."
-                )
-            else:
-                info(
-                    "Number of reads in input:%d\tNumber of reads after filtering:%d\n"
-                    % (self.n_total_reads, self.n_reads_after_filtering)
-                )
+        if self.n_reads_after_filtering == 0:
+            raise NoReadsAfterQualityFiltering(
+                "No reads in input or no reads survived the average or single bp quality filtering."
+            )
         else:
-            self.n_reads_after_filtering = self.n_total_reads
-
-    def _filter_read_quality(self, R1=None, R2=None) -> int:
-        R1_filtered = gzip.open(self.filtered_R1_filename, "w+")
-        R2_filtered = gzip.open(self.filtered_R2_filename, "w+")
+            info(
+                "Number of reads in input:%d\tNumber of reads after filtering:%d\n"
+                % (self.n_total_reads, self.n_reads_after_filtering)
+            )
 
-        if R1 is None or R2 is None:
-            R1, R2 = self._get_seq_records()
+    def _check_readname_match_and_filter_quality(
+        self, R1_iter, R2_iter, filter_by_qual=False
+    ) -> Tuple[int, int]:
+        R1_filtered = gzip.open(self.filtered_R1_filename, "wt+")
+        R2_filtered = gzip.open(self.filtered_R2_filename, "wt+")
 
         n_reads_after_filtering = 0
-        for i, R1_record in enumerate(R1):
-            R2_record = R2[i]
-
-            R1_quality_pass = _read_is_good_quality(
-                R1_record,
-                self.min_average_read_quality,
-                self.min_single_bp_quality,
-                self.qend_R1,
-            )
-            R2_quality_pass = _read_is_good_quality(
-                R2_record,
-                self.min_average_read_quality,
-                self.min_single_bp_quality,
-                self.qend_R2,
-            )
-
+        for R1_record, R2_record in tqdm(
+            zip(R1_iter, R2_iter), total=self.n_total_reads
+        ):
+            if R1_record.name != R2_record.name:
+                raise InputFileError(
+                    "R1 and R2 read discordance in read {} and {}".format(
+                        R1_record.name, R2_record.name
+                    )
+                )
+            if filter_by_qual:
+                R1_quality_pass = _read_is_good_quality(
+                    R1_record,
+                    self.min_average_read_quality,
+                    self.min_single_bp_quality,
+                    self.qend_R1,
+                )
+                R2_quality_pass = _read_is_good_quality(
+                    R2_record,
+                    self.min_average_read_quality,
+                    self.min_single_bp_quality,
+                    self.qend_R2,
+                )
+            else:
+                R1_quality_pass = True
+                R2_quality_pass = True
             if R1_quality_pass and R2_quality_pass:
                 n_reads_after_filtering += 1
-                R1_filtered.write(R1.format("fastq"))
-                R2_filtered.write(R2.format("fastq"))
+                R1_filtered.write(R1_record.format("fastq"))
+                R2_filtered.write(R2_record.format("fastq"))
+
         return n_reads_after_filtering
 
     def _write_start_log(self):
         try:
             os.makedirs(self.output_dir)
             info(f"Creating Folder {self.output_dir}")
         except OSError:
```

### Comparing `crispr-bean-0.2.7/bean/mapping/_supporting_fn.py` & `crispr-bean-1.0.0/bean/mapping/_supporting_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from turtle import position
 from typing import List, Union
 import subprocess as sb
 import numpy as np
 import pandas as pd
 import gzip
 from Bio import SeqIO
 from Bio.Seq import Seq
-from Bio.SeqIO.QualityIO import FastqGeneralIterator
 from .CRISPResso2Align import read_matrix, global_align_base_editor
 from ..framework.Edit import Allele, Edit
 
 
 class InputFileError(Exception):
     pass
 
@@ -85,15 +83,14 @@
                         R1_record.name, R2_record.name
                     )
                 )
 
 
 def _get_guide_to_reporter_df(sgRNA_filename: str) -> pd.DataFrame:
     """Returns a gRNA name to reporter sequence mapping."""
-    guide_to_reporter = {}
 
     with open(sgRNA_filename) as infile:
         sgRNA_df = pd.read_csv(infile)
         if not ("name" in sgRNA_df.columns and "Reporter" in sgRNA_df.columns):
             raise InputFileError(
                 "Input gRNA file doesn't have the column 'gRNA' or 'gRNA_barcode'."
             )
@@ -173,14 +170,15 @@
 def _get_allele_from_alignment(
     ref_aligned: str,
     query_aligned: str,
     offset: int,
     strand: int,
     start_pos: int,
     end_pos: int,
+    chrom: str = None,
     positionwise_quality: np.ndarray = None,
     quality_thres: float = -1,
 ):
     assert len(ref_aligned) == len(query_aligned)
     allele = Allele()
     ref_gaps = 0
     alt_gaps = 0
@@ -206,14 +204,15 @@
             ref_gaps += 1
         elif alt_base == "-":
             alt_gaps += 1
         ref_pos = i - ref_gaps
         if alt_base_is_good_quality and ref_pos >= start_pos and ref_pos < end_pos:
             allele.add(
                 Edit(
+                    chrom=chrom,
                     rel_pos=ref_pos,
                     ref_base=ref_base,
                     alt_base=alt_base,
                     offset=offset,
                     strand=strand,
                 )
             )
@@ -224,14 +223,15 @@
     ref_seq: str,
     query_seq: str,
     ref_base: str,
     alt_base: str,
     aln_mat_path: str,
     offset: int,
     strand: int = 1,
+    chrom: str = None,
     start_pos: int = 0,
     end_pos: int = 100,
     positionwise_quality: np.ndarray = None,
     quality_thres: float = 30,
     objectify_allele=True,
 ):
     aln_matrix = read_matrix(aln_mat_path)
@@ -251,14 +251,15 @@
         allele = _get_allele_from_alignment(
             ref_aligned,
             query_aligned,
             offset,
             strand,
             start_pos,
             end_pos,
+            chrom,
             positionwise_quality,
             quality_thres,
         )
         for e in allele.edits:
             if e.ref_base == "-":
                 continue
             assert ref_seq[e.rel_pos] == e.ref_base, (
```

### Comparing `crispr-bean-0.2.7/bean/mapping/utils.py` & `crispr-bean-1.0.0/bean/mapping/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,30 +26,84 @@
         return __import__(library_name)
     except ImportError as exc:
         raise ImportError(
             f"You need to install {library_name} module to use CRISPRessoCount!"
         ) from exc
 
 
-def _get_input_parser():
-    """Get the input data"""
-    print(
-        r"""
-    _ _       
-  /  \ '\                       _   
-  |   \  \      __ ___ _  _ _ _| |_ 
-   \   \  |    / _/ _ \ || | ' \  _|
-    `.__|/     \__\___/\_,_|_||_\__|
-    """
+def get_input_parser(parser=None):
+    """Add multi-sample specific arguments to the base parser."""
+    if parser is None:
+        parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-i",
+        "--sample-list",
+        type=str,
+        help="List of fastq and sample ids. Formatted as `R1_filepath,R2_filepath,sample_id`",
+        required=True,
+    )
+    parser = _get_input_parser(parser)
+    parser.add_argument(
+        "-t", "--threads", type=int, help="Number of threads", default=10
     )
+    parser.add_argument(
+        "--guide-start-seqs-file",
+        type=str,
+        help="CSV file path with per-sample `guide_start_seq` to be used."
+        + "Formatted as `sample_id, guide_start_seq`",
+        default=None,
+    )
+    parser.add_argument(
+        "--guide-end-seqs-file",
+        type=str,
+        help="CSV file path with per-sample `guide_end_seq` to be used."
+        + "Formatted as `sample_id,guide_end_seq`",
+        default=None,
+    )
+    parser.add_argument(
+        "--barcode-start-seqs-file",
+        type=str,
+        help="CSV file path with per-sample `barcode_start_seq` to be used."
+        + "Formatted as `sample_id,guide_end_seq`",
+        default=None,
+    )
+
+    parser.add_argument(
+        "--rerun", help="Recount each sample", action="store_true", default=False
+    )
+
+    return parser
 
-    parser = argparse.ArgumentParser(
-        description="CRISPRessoCount parameters",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+
+def get_input_parser_count(parser=None):
+    """Get single-sample specific argument parser."""
+    if parser is None:
+        parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "--R1",
+        type=str,
+        help="FASTQ file path for read 1",
+        required=True,
+    )
+    parser.add_argument(
+        "--R2",
+        type=str,
+        help="FASTQ file path for read 2.",
+        required=True,
     )
+    parser = _get_input_parser(parser)
+    return parser
+
+
+def _get_input_parser(parser=None):
+    if parser is None:
+        parser = argparse.ArgumentParser(
+            description="bean-count parameters",
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        )
 
     parser.add_argument(
         "-b",
         "--edited-base",
         type=str,
         required=True,
         help="For base editors, the base that should be ignored when matching the gRNA sequence",
@@ -61,29 +115,35 @@
         required=True,
         help="""sgRNA description file. The format requires three columns: name, sequence, barcode [ reporter [,strand, target_pos], [start_pos, offset] ].""",
     )
     # optional
     parser.add_argument(
         "--guide-start-seq",
         type=str,
-        help="Guide starts after this sequence in R1",
+        help="Guide starts after this sequence in R1. The start sequence is located by allowing the base transition from `edited_base` (If A to G and if C to T).",
         default="",
     )
     parser.add_argument(
         "--guide-end-seq",
         type=str,
         help="Guide starts after this sequence in R1",
         default="",
     )
     parser.add_argument(
+        "--barcode-start-seq",
+        type=str,
+        help="Barcode + reporter starts after this sequence in R2, denoted as the sense direction (the same sequence direction as R1). The start sequence is located by allowing the base transition from `edited_base` (If A to G and if C to T).",
+        default="",
+    )
+    parser.add_argument(
         "-r", "--count-reporter", help="Count reporter edits.", action="store_true"
     )
     parser.add_argument(
         "-q",
-        "--min_average_read_quality",
+        "--min-average-read-quality",
         type=int,
         help="Minimum average quality score (phred33) to keep a read",
         default=30,
     )
     parser.add_argument(
         "-s",
         "--min-single-bp-quality",
@@ -236,30 +296,35 @@
     #         args.name = clean_name
     sgRNA_info_tbl = pd.read_csv(args.sgRNA_filename)
 
     def _check_sgrna_info_table(args, sgRNA_info_tbl):
         if args.offset:
             if "offset" not in sgRNA_info_tbl.columns:
                 raise InputFileError(
-                    "Offset option is set but the input file doesn't contain the `offset` column."
+                    f"Offset option is set but the input file doesn't contain the `offset` column: Provided {sgRNA_info_tbl.columns}"
                 )
             if len(args.align_fasta) > 0:
                 error_logger("Can't have --offset and --align_fasta option together.")
         if (
             args.match_target_pos
             and args.target_pos_col is not None
             and args.target_pos_col not in sgRNA_info_tbl.columns
         ):
             raise InputFileError(
                 f"Specified target position column '{args.target_pos_col}' not in the input file {args.sgRNA_filename}."
             )
+        if args.count_reporter:
+            if "reporter" not in sgRNA_info_tbl.columns:
+                raise InputFileError(
+                    f"Offset option is set but the input file doesn't contain the `reporter` column: Provided {sgRNA_info_tbl.columns}"
+                )
 
     _check_sgrna_info_table(args, sgRNA_info_tbl)
 
     if args.match_target_pos and (args.target_pos_col not in sgRNA_info_tbl.columns):
         raise InputFileError(
-            "Target position option is set but the input file doesn't contain the target position column."
+            f"Target position option is set as `{args.target_pos_col}` but the input file doesn't contain the target position column: provided {sgRNA_info_tbl.columns}"
         )
 
     info_logger("Done checking input arguments.")
 
     return args
```

### Comparing `crispr-bean-0.2.7/bean/model/model.py` & `crispr-bean-1.0.0/bean/model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,73 +41,91 @@
             )
     mu_center = mu_alleles
     mu = torch.repeat_interleave(mu_center, data.target_lengths, dim=0)
     assert mu.shape == (data.n_guides, 1)
     sd = sd_alleles
     sd = torch.repeat_interleave(sd, data.target_lengths, dim=0)
     assert sd.shape == (data.n_guides, 1)
-
+    if hasattr(data, "sample_covariates"):
+        with pyro.plate("cov_place", data.n_sample_covariates):
+            mu_cov = pyro.sample("mu_cov", dist.Normal(0, 1))
+        assert mu_cov.shape == (data.n_sample_covariates,), mu_cov.shape
     with replicate_plate:
         with bin_plate as b:
             uq = data.upper_bounds[b]
             lq = data.lower_bounds[b]
             assert uq.shape == lq.shape == (data.n_condits,)
-            # with guide_plate, poutine.mask(mask=(data.allele_counts.sum(axis=-1) == 0)):
             with guide_plate:
+                mu = (
+                    mu.unsqueeze(0)
+                    .unsqueeze(0)
+                    .expand((data.n_reps, data.n_condits, -1, -1))
+                )
+                if hasattr(data, "sample_covariates"):
+                    mu = mu + (data.rep_by_cov * mu_cov)[:, 0].unsqueeze(-1).unsqueeze(
+                        -1
+                    ).unsqueeze(-1).expand((-1, data.n_condits, data.n_guides, 1))
+                sd = torch.sqrt(
+                    (
+                        sd.unsqueeze(0)
+                        .unsqueeze(0)
+                        .expand((data.n_reps, data.n_condits, -1, -1))
+                    )
+                )
                 alleles_p_bin = get_std_normal_prob(
-                    uq.unsqueeze(-1).unsqueeze(-1).expand((-1, data.n_guides, 1)),
-                    lq.unsqueeze(-1).unsqueeze(-1).expand((-1, data.n_guides, 1)),
-                    mu.unsqueeze(0).expand((data.n_condits, -1, -1)),
-                    sd.unsqueeze(0).expand((data.n_condits, -1, -1)),
+                    uq.unsqueeze(0)
+                    .unsqueeze(-1)
+                    .unsqueeze(-1)
+                    .expand((data.n_reps, -1, data.n_guides, 1)),
+                    lq.unsqueeze(0)
+                    .unsqueeze(-1)
+                    .unsqueeze(-1)
+                    .expand((data.n_reps, -1, data.n_guides, 1)),
+                    mu,
+                    sd,
                 )
-                assert alleles_p_bin.shape == (data.n_condits, data.n_guides, 1)
-
-            expected_allele_p = alleles_p_bin.unsqueeze(0).expand(
-                data.n_reps, -1, -1, -1
-            )
-            expected_guide_p = expected_allele_p.sum(axis=-1)
+                assert alleles_p_bin.shape == (
+                    data.n_reps,
+                    data.n_condits,
+                    data.n_guides,
+                    1,
+                )
+            expected_guide_p = alleles_p_bin.sum(axis=-1)
             assert expected_guide_p.shape == (
                 data.n_reps,
                 data.n_condits,
                 data.n_guides,
             ), expected_guide_p.shape
 
     with replicate_plate2:
         with pyro.plate("guide_plate3", data.n_guides, dim=-1):
             a = get_alpha(expected_guide_p, data.size_factor, data.sample_mask, data.a0)
-            print(a)
-            print(a.max())
-            print(a.min())
-            a_bcmatch = get_alpha(
-                expected_guide_p,
-                data.size_factor_bcmatch,
-                data.sample_mask,
-                data.a0_bcmatch,
-            )
-            assert (
-                data.X.shape
-                == data.X_bcmatch.shape
-                == (
-                    data.n_reps,
-                    data.n_condits,
-                    data.n_guides,
-                )
+            assert data.X.shape == (
+                data.n_reps,
+                data.n_condits,
+                data.n_guides,
             )
             with poutine.mask(
                 mask=torch.logical_and(
                     data.X_masked.permute(0, 2, 1).sum(axis=-1) > mask_thres,
                     data.repguide_mask,
                 )
             ):
                 pyro.sample(
                     "guide_counts",
                     dist.DirichletMultinomial(a, validate_args=False),
                     obs=data.X_masked.permute(0, 2, 1),
                 )
             if use_bcmatch:
+                a_bcmatch = get_alpha(
+                    expected_guide_p,
+                    data.size_factor_bcmatch,
+                    data.sample_mask,
+                    data.a0_bcmatch,
+                )
                 with poutine.mask(
                     mask=torch.logical_and(
                         data.X_bcmatch_masked.permute(0, 2, 1).sum(axis=-1)
                         > mask_thres,
                         data.repguide_mask,
                     )
                 ):
@@ -160,53 +178,55 @@
                 data.n_condits,
                 data.n_guides,
             ), expected_guide_p.shape
 
     with replicate_plate2:
         with pyro.plate("guide_plate3", data.n_guides, dim=-1):
             a = get_alpha(expected_guide_p, data.size_factor, data.sample_mask, data.a0)
-            a_bcmatch = get_alpha(
-                expected_guide_p,
-                data.size_factor_bcmatch,
-                data.sample_mask,
-                data.a0_bcmatch,
-            )
-            assert (
-                data.X.shape
-                == data.X_bcmatch.shape
-                == (
-                    data.n_reps,
-                    data.n_condits,
-                    data.n_guides,
-                )
+
+            assert data.X.shape == (
+                data.n_reps,
+                data.n_condits,
+                data.n_guides,
             )
             with poutine.mask(
                 mask=torch.logical_and(
                     data.X_masked.permute(0, 2, 1).sum(axis=-1) > mask_thres,
                     data.repguide_mask,
                 )
             ):
                 pyro.sample(
                     "guide_counts",
                     dist.DirichletMultinomial(a, validate_args=False),
                     obs=data.X_masked.permute(0, 2, 1),
                 )
             if use_bcmatch:
-                with poutine.mask(
-                    mask=torch.logical_and(
-                        data.X_bcmatch_masked.permute(0, 2, 1).sum(axis=-1)
-                        > mask_thres,
-                        data.repguide_mask,
-                    )
-                ):
-                    pyro.sample(
-                        "guide_bcmatch_counts",
-                        dist.DirichletMultinomial(a_bcmatch, validate_args=False),
-                        obs=data.X_bcmatch_masked.permute(0, 2, 1),
-                    )
+                a_bcmatch = get_alpha(
+                    expected_guide_p,
+                    data.size_factor_bcmatch,
+                    data.sample_mask,
+                    data.a0_bcmatch,
+                )
+                try:
+                    with poutine.mask(
+                        mask=torch.logical_and(
+                            data.X_bcmatch_masked.permute(0, 2, 1).sum(axis=-1)
+                            > mask_thres,
+                            data.repguide_mask,
+                        )
+                    ):
+                        pyro.sample(
+                            "guide_bcmatch_counts",
+                            dist.DirichletMultinomial(a_bcmatch, validate_args=False),
+                            obs=data.X_bcmatch_masked.permute(0, 2, 1),
+                        )
+                except RuntimeError:
+                    print(data.X_bcmatch_masked.shape)
+                    print(data.repguide_mask.shape)
+                    exit(1)
 
     return alleles_p_bin
 
 
 def MixtureNormalConstPiModel(
     data: VariantSortingScreenData,
     alpha_prior: float = 1,
@@ -492,14 +512,26 @@
             sd_loc = pyro.param("sd_loc", torch.zeros((data.n_targets, 1)))
             sd_scale = pyro.param(
                 "sd_scale",
                 torch.ones((data.n_targets, 1)),
                 constraint=constraints.positive,
             )
             pyro.sample("sd_alleles", dist.LogNormal(sd_loc, sd_scale))
+    if hasattr(data, "sample_covariates"):
+        with pyro.plate("cov_place", data.n_sample_covariates):
+            mu_cov_loc = pyro.param(
+                "mu_cov_loc", torch.zeros((data.n_sample_covariates,))
+            )
+            mu_cov_scale = pyro.param(
+                "mu_cov_scale",
+                torch.ones((data.n_sample_covariates,)),
+                constraint=constraints.positive,
+            )
+            mu_cov = pyro.sample("mu_cov", dist.Normal(mu_cov_loc, mu_cov_scale))
+            assert mu_cov.shape == (data.n_sample_covariates,), mu_cov.shape
 
 
 def MixtureNormalGuide(
     data,
     alpha_prior: float = 1,
     use_bcmatch: bool = True,
     scale_by_accessibility: bool = False,
```

### Comparing `crispr-bean-0.2.7/bean/model/readwrite.py` & `crispr-bean-1.0.0/bean/model/readwrite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Sequence, Optional
+from typing import Union, Sequence, Optional, List
 import numpy as np
 import pandas as pd
 from statistics import NormalDist
 from scipy.special import logit, expit
 from scipy.stats import norm
 
 
@@ -48,55 +48,88 @@
 
 def write_result_table(
     target_info_df: pd.DataFrame,
     param_hist_dict,
     model_label: str,
     prefix: str = "",
     suffix: str = "",
+    negctrl_params=None,
     write_fitted_eff: bool = True,
     adjust_confidence_by_negative_control: bool = True,
     adjust_confidence_negatives: np.ndarray = None,
     guide_index: Optional[Sequence[str]] = None,
     guide_acc: Optional[Sequence] = None,
+    sd_is_fitted: bool = True,
+    sample_covariates: List[str] = None,
     return_result: bool = False,
 ) -> Union[pd.DataFrame, None]:
     """Combine target information and scores to write result table to a csv file or return it."""
-    if param_hist_dict["params"]["mu_loc"].dim() == 2:
-        mu = param_hist_dict["params"]["mu_loc"].detach()[:, 0].cpu().numpy()
-        mu_sd = param_hist_dict["params"]["mu_scale"].detach()[:, 0].cpu().numpy()
-        sd = param_hist_dict["params"]["sd_loc"].detach().exp()[:, 0].cpu().numpy()
-    elif param_hist_dict["params"]["mu_loc"].dim() == 1:
-        mu = param_hist_dict["params"]["mu_loc"].detach().cpu().numpy()
-        mu_sd = param_hist_dict["params"]["mu_scale"].detach().cpu().numpy()
-        sd = param_hist_dict["params"]["sd_loc"].detach().exp().cpu().numpy()
+    if param_hist_dict["mu_loc"].dim() == 2:
+        mu = param_hist_dict["mu_loc"].detach()[:, 0].cpu().numpy()
+        mu_sd = param_hist_dict["mu_scale"].detach()[:, 0].cpu().numpy()
+        if sd_is_fitted:
+            sd = param_hist_dict["sd_loc"].detach().exp()[:, 0].cpu().numpy()
+    elif param_hist_dict["mu_loc"].dim() == 1:
+        mu = param_hist_dict["mu_loc"].detach().cpu().numpy()
+        mu_sd = param_hist_dict["mu_scale"].detach().cpu().numpy()
+        if sd_is_fitted:
+            sd = param_hist_dict["sd_loc"].detach().exp().cpu().numpy()
     else:
         raise ValueError(
-            f'`mu_loc` has invalid shape of {param_hist_dict["params"]["mu_loc"].shape}'
+            f'`mu_loc` has invalid shape of {param_hist_dict["mu_loc"].shape}'
         )
-    fit_df = pd.DataFrame(
-        {
-            "mu": mu,
-            "mu_sd": mu_sd,
-            "mu_z": mu / mu_sd,
-            "sd": sd,
-        }
-    )
-    fit_df["novl"] = get_novl(fit_df, "mu", "mu_sd")
-    if "negctrl" in param_hist_dict.keys():
+    param_dict = {
+        "mu": mu,
+        "mu_sd": mu_sd,
+        "mu_z": mu / mu_sd,
+    }
+    if sd_is_fitted:
+        param_dict["sd"] = sd
+    if sample_covariates is not None:
+        assert (
+            "mu_cov_loc" in param_hist_dict and "mu_cov_scale" in param_hist_dict
+        ), param_hist_dict.keys()
+        for i, sample_cov in enumerate(sample_covariates):
+            param_dict[f"mu_{sample_cov}"] = (
+                mu + param_hist_dict["mu_cov_loc"].detach().cpu().numpy()[i]
+            )
+            param_dict[f"mu_sd_{sample_cov}"] = np.sqrt(
+                mu_sd**2
+                + param_hist_dict["mu_cov_scale"].detach().cpu().numpy()[i] ** 2
+            )
+            param_dict[f"mu_z_{sample_cov}"] = (
+                param_dict[f"mu_{sample_cov}"] / param_dict[f"mu_sd_{sample_cov}"]
+            )
+
+    fit_df = pd.DataFrame(param_dict)
+    if negctrl_params is not None:
         print("Normalizing with common negative control distribution")
-        mu0 = param_hist_dict["negctrl"]["params"]["mu_loc"].detach().cpu().numpy()
-        sd0 = (
-            param_hist_dict["negctrl"]["params"]["sd_loc"].detach().exp().cpu().numpy()
-        )
-        print(f"Fitted mu0={mu0}, sd0={sd0}.")
+        mu0 = negctrl_params["mu_loc"].detach().cpu().numpy()
+        if sd_is_fitted:
+            sd0 = negctrl_params["sd_loc"].detach().exp().cpu().numpy()
+        else:
+            sd0 = 1.0
+        print(f"Fitted mu0={mu0}" + (f", sd0={sd0}." if sd_is_fitted else ""))
         fit_df["mu_scaled"] = (mu - mu0) / sd0
         fit_df["mu_sd_scaled"] = mu_sd / sd0
         fit_df["mu_z_scaled"] = fit_df.mu_scaled / fit_df.mu_sd_scaled
-        fit_df["sd_scaled"] = sd / sd0
+        if sd_is_fitted:
+            fit_df["sd_scaled"] = sd / sd0
         fit_df["novl_scaled"] = get_novl(fit_df, "mu_scaled", "mu_sd_scaled")
+        if sample_covariates is not None:
+            for i, sample_cov in enumerate(sample_covariates):
+                fit_df[f"mu_{sample_cov}_scaled"] = (
+                    fit_df[f"mu_{sample_cov}"] - mu0
+                ) / sd0
+                fit_df[f"mu_sd_{sample_cov}_scaled"] = (
+                    fit_df[f"mu_sd_{sample_cov}"] / sd0
+                )
+                fit_df[f"mu_z_{sample_cov}_scaled"] = (
+                    fit_df[f"mu_{sample_cov}_scaled"] / fit_df["mu_sd_scaled"]
+                )
 
     fit_df = pd.concat(
         [target_info_df.reset_index(), fit_df.reset_index(drop=True)], axis=1
     )
 
     if adjust_confidence_by_negative_control:
         assert adjust_confidence_negatives is not None
@@ -111,36 +144,56 @@
                 _, std = norm.fit(ncvar.mu_z_scaled, floc=0)
             else:
                 _, std = norm.fit(ncvar.mu_z, floc=0)
             fit_df = adjust_normal_params_by_control(
                 fit_df,
                 std,
                 suffix="_adj",
-                mu_adjusted_col="mu_scaled"
-                if "negctrl" in param_hist_dict.keys()
-                else "mu",
-                mu_sd_adjusted_col="mu_sd_scaled"
-                if "negctrl" in param_hist_dict.keys()
-                else "mu_sd",
+                mu_adjusted_col=(
+                    "mu_scaled" if "negctrl" in param_hist_dict.keys() else "mu"
+                ),
+                mu_sd_adjusted_col=(
+                    "mu_sd_scaled" if "negctrl" in param_hist_dict.keys() else "mu_sd"
+                ),
             )
             fit_df = add_credible_interval(fit_df, "mu_adj", "mu_sd_adj")
+            if sample_covariates is not None:
+                for i, sample_cov in enumerate(sample_covariates):
+                    fit_df = adjust_normal_params_by_control(
+                        fit_df,
+                        std,
+                        suffix=f"_{sample_cov}_adj",
+                        mu_adjusted_col=(
+                            f"mu_{sample_cov}_scaled"
+                            if "negctrl" in param_hist_dict.keys()
+                            else f"mu_{sample_cov}"
+                        ),
+                        mu_sd_adjusted_col=(
+                            f"mu_sd_{sample_cov}_scaled"
+                            if "negctrl" in param_hist_dict.keys()
+                            else f"mu_sd_{sample_cov}"
+                        ),
+                    )
+                    fit_df = add_credible_interval(
+                        fit_df, f"mu_{sample_cov}_adj", f"mu_sd_{sample_cov}_adj"
+                    )
 
     if write_fitted_eff or guide_acc is not None:
-        if "alpha_pi" not in param_hist_dict["params"].keys():
+        if "alpha_pi" not in param_hist_dict.keys():
             pi = 1.0
         else:
-            a_fitted = param_hist_dict["params"]["alpha_pi"].detach().cpu().numpy()
+            a_fitted = param_hist_dict["alpha_pi"].detach().cpu().numpy()
             pi = a_fitted[..., 1:].sum(axis=1) / a_fitted.sum(axis=1)
         sgRNA_df = pd.DataFrame({"edit_eff": pi}, index=guide_index)
         if guide_acc is not None:
             sgRNA_df["accessibility"] = guide_acc
             sgRNA_df["scaled_edit_eff"] = _scale_pi(
                 pi,
                 guide_acc,
-                fitted_noise_logit=param_hist_dict["params"]["noise_scale"]
+                fitted_noise_logit=param_hist_dict["noise_scale"]
                 .detach()
                 .cpu()
                 .numpy(),
             )
         sgRNA_df.to_csv(f"{prefix}bean_sgRNA_result.{model_label}{suffix}.csv")
 
     if return_result:
```

### Comparing `crispr-bean-0.2.7/bean/plotting/editing_patterns.py` & `crispr-bean-1.0.0/bean/plotting/editing_patterns.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     guide: str,
     edit_tbl: pd.DataFrame,
     edited_base: str = "A",
     target_alt: str = "G",
 ):
     """If edit is not observed in editable position, add into the edit rate table."""
     editable_positions = np.where(
-        (np.array(list(bdata.guides.loc[guide, "Reporter"])) == edited_base)
+        (np.array(list(bdata.guides.loc[guide, "reporter"])) == edited_base)
     )[0]
     if guide not in edit_tbl.guide.tolist():
         observed_rel_pos = []
     else:
         edited_db = edit_tbl.loc[edit_tbl.guide == guide, :]
         observed_rel_pos = edited_db.rel_pos.tolist()
     edits = []
@@ -56,91 +56,86 @@
         ],
         ignore_index=True,
     )
     return edit_tbl
 
 
 def get_edit_rates(
-    bdata, edit_count_key="edit_counts", add_absent=True, adjust_spacer_pos: bool = True
+    bdata,
+    edit_count_key="edit_counts",
+    adjust_spacer_pos: bool = True,
+    reporter_column: str = "reporter",
 ):
     """
     Obtain position- and context-wise editing rate (context: base preceding the target base position).
     Args
-    bdata (bean.ReporterScreen): input ReporterScreen object to be used for analyzing posiiton-wide editing rate.
+    bdata (bean.reporterScreen): input ReporterScreen object to be used for analyzing posiiton-wide editing rate.
     edit_count_key: key in bdata.uns with edit count DataFrame to be used for analyzing posiiton-wide editing rate.
     """
     edit_rates = bdata.get_normalized_allele_counts(bdata.uns[edit_count_key])
     edit_rates_agg = edit_rates[["guide", "edit"]]
     edit_rates_agg = edit_rates_agg.loc[
         edit_rates_agg.guide.map(lambda s: "CONTROL" not in s)
     ].reset_index(drop=True)
-    try:
-        edit_rates_agg["rep_median"] = edit_rates.iloc[:, 2:].median(axis=1)
-        edit_rates_agg["rep_mean"] = edit_rates.iloc[:, 2:].mean(axis=1)
-        edit_rates_agg["rel_pos"] = edit_rates_agg.edit.map(lambda e: e.rel_pos).astype(
-            int
+    edit_rates_agg["rep_median"] = edit_rates.iloc[:, 2:].median(axis=1)
+    edit_rates_agg["rep_mean"] = edit_rates.iloc[:, 2:].mean(axis=1)
+    edit_rates_agg["rel_pos"] = edit_rates_agg.edit.map(lambda e: e.rel_pos).astype(int)
+
+    for guide in tqdm(
+        edit_rates_agg.guide.unique(),
+        desc="Calibrating edits in editable positions...",
+    ):
+        edit_rates_agg = _add_absent_edits(
+            bdata,
+            guide,
+            edit_rates_agg,
+            edited_base=bdata.base_edited_from,
+            target_alt=bdata.base_edited_to,
         )
-        if add_absent:
-            for guide in tqdm(
-                edit_rates_agg.guide.unique(),
-                desc="Calibrating edits in editable positions...",
-            ):
-                edit_rates_agg = _add_absent_edits(
-                    bdata,
-                    guide,
-                    edit_rates_agg,
-                    edited_base=bdata.base_edited_from,
-                    target_alt=bdata.base_edited_to,
-                )
-        if adjust_spacer_pos:
-            if "guide_len" not in bdata.guides.columns:
-                bdata.guides["guide_len"] = bdata.guides.sequence.map(len)
-            start_pad = (
-                32
-                - 6
-                - bdata.guides.guide_len[edit_rates_agg.guide].reset_index(drop=True)
-            )
-            edit_rates_agg["spacer_pos"] = (edit_rates_agg.rel_pos - start_pad).astype(
-                int
-            )
-            edit_rates_agg = edit_rates_agg[
-                (edit_rates_agg.spacer_pos >= 0) & (edit_rates_agg.spacer_pos < 20)
-            ].reset_index(drop=True)
-            edit_rates_agg.loc[:, "spacer_pos"] = edit_rates_agg["spacer_pos"] + 1
-        else:
-            edit_rates_agg["spacer_pos"] = edit_rates_agg.rel_pos + 1
-        edit_rates_agg["base_change"] = edit_rates_agg.edit.map(
-            lambda e: e.get_base_change()
-        )
-        edit_rates_agg.rel_pos = edit_rates_agg.rel_pos.astype(int)
-        edit_rates_agg["context"] = edit_rates_agg.apply(
-            lambda row: bdata.guides.loc[row.guide, "Reporter"][
-                row.rel_pos - 1 : row.rel_pos + 1
-            ],
-            axis=1,
+
+    if adjust_spacer_pos:
+        if "guide_len" not in bdata.guides.columns:
+            bdata.guides["guide_len"] = bdata.guides.sequence.map(len)
+        start_pad = (
+            32 - 6 - bdata.guides.guide_len[edit_rates_agg.guide].reset_index(drop=True)
         )
-    except Exception as exp:
-        print(exp)
+        edit_rates_agg["spacer_pos"] = (edit_rates_agg.rel_pos - start_pad).astype(int)
+        edit_rates_agg = edit_rates_agg[
+            (edit_rates_agg.spacer_pos >= 0) & (edit_rates_agg.spacer_pos < 20)
+        ].reset_index(drop=True)
+        edit_rates_agg.loc[:, "spacer_pos"] = edit_rates_agg["spacer_pos"] + 1
+    else:
+        edit_rates_agg["spacer_pos"] = edit_rates_agg.rel_pos + 1
+    edit_rates_agg["base_change"] = edit_rates_agg.edit.map(
+        lambda e: e.get_base_change()
+    )
+    edit_rates_agg.rel_pos = edit_rates_agg.rel_pos.astype(int)
+    edit_rates_agg["context"] = edit_rates_agg.apply(
+        lambda row: bdata.guides.loc[row.guide, reporter_column][
+            row.rel_pos - 1 : row.rel_pos + 1
+        ],
+        axis=1,
+    )
     return edit_rates_agg
 
 
 def plot_by_pos_context(
     edit_rates_df: pd.DataFrame,
     target_base="A",
 ):
     target_base_alt = {"A": "G", "C": "T"}[target_base]
     context_to_offset_map = {
         f"A{target_base}": -0.4,
         f"G{target_base}": -0.2,
         f"C{target_base}": 0,
         f"T{target_base}": 0.2,
     }
-    edit_rates_df[
-        "spacer_pos_ctxt"
-    ] = edit_rates_df.spacer_pos + edit_rates_df.context.map(context_to_offset_map)
+    edit_rates_df["spacer_pos_ctxt"] = (
+        edit_rates_df.spacer_pos + edit_rates_df.context.map(context_to_offset_map)
+    )
     fig, ax = plt.subplots(figsize=(6, 3))
     sns.scatterplot(
         edit_rates_df.loc[
             (edit_rates_df.base_change == f"{target_base}>{target_base_alt}")
         ],
         x="spacer_pos_ctxt",
         y="rep_mean",
@@ -182,44 +177,42 @@
 
 
 def _get_norm_rates_df(
     bdata,
     edit_rates_df=None,
     edit_count_key="edit_counts",
     base_changes: Sequence[str] = None,
-    show_list=None,
 ):
     change_by_pos = pd.pivot(
-        edit_rates_df.groupby(["base_change", "spacer_pos"])
+        edit_rates_df[["base_change", "spacer_pos", "rep_mean"]]
+        .groupby(["base_change", "spacer_pos"])
         .sum()["rep_mean"]
         .reset_index(),
         index="spacer_pos",
         columns="base_change",
         values="rep_mean",
     ).fillna(0)
 
     norm_matrix = pd.DataFrame(index=change_by_pos.index, columns=BASES)
     for pos in norm_matrix.index:
-        pos_base = bdata.guides.Reporter.map(
+        pos_base = bdata.guides.reporter.map(
             lambda s: s[pos] if pos < len(s) else " "
         ).values
         for b in BASES:
             norm_matrix.loc[pos, b] = (pos_base == b).sum()
     ref_bases = change_by_pos.columns.map(lambda s: s.split(">")[0])
     change_by_pos = change_by_pos.loc[:, ref_bases.isin(BASES)]
     norm_rate = (
         change_by_pos
         / norm_matrix.loc[
             :, change_by_pos.columns.map(lambda s: s.split(">")[0])
         ].values
     )
-    if show_list is None:
-        show_list = ["A>C", "A>T", "A>G", "C>T", "C>G"]
     # norm_rate_reduced = _combine_complementary_base_changes(norm_rate).astype(float)
-    return norm_rate.astype(float)[show_list]  # _reduced
+    return norm_rate.astype(float)[base_changes]  # _reduced
 
 
 def _get_possible_changes_from_target_base(target_basechange: str):
     """Return base changes strings (ex. A>C) for given the same reference base to edit from to the input target_basechange. ex) returns ['A>C', 'A>T'] given input 'A>G'."""
     if not re.fullmatch(r"[ATCG]>[ATCG]", target_basechange):
         raise ValueError(
             f"Input argument {target_basechange} doesn't conform to the valid format ex. 'A>G'"
@@ -249,48 +242,52 @@
     if not re.fullmatch(r"[ATCG]>[ATCG]", target_basechange):
         raise ValueError(
             f"Input argument {target_basechange} doesn't conform to the valid format ex. 'A>G'"
         )
     if nonref_base_changes is None:
         if target_basechange == "A>G":
             nonref_base_changes = ["C>T", "C>G"]
+        elif target_basechange == "C>T":
+            nonref_base_changes = ["G>A", "G>C"]
         else:
             print("No non-ref base changes specified. not drawing them")
             nonref_base_changes = []
     ref_other_changes = _get_possible_changes_from_target_base(target_basechange)
 
     df_to_draw = _get_norm_rates_df(
         bdata,
         norm_rates_df,
         edit_count_key,
-        base_changes=[
+        base_changes=ref_other_changes
+        + [
             target_basechange,
         ]
-        + ref_other_changes
         + nonref_base_changes,
     )
     fig, ax = plt.subplots(figsize=(3, 7))
 
     vmax = df_to_draw.max().max()
     if normalize:
         df_to_draw = df_to_draw / vmax * 100
         vmax = 100
+
     target_data = df_to_draw.copy()
     target_data.loc[:, target_data.columns != target_basechange] = np.nan
     sns.heatmap(
         target_data,
         ax=ax,
         annot=True,
         cmap="Reds",
         vmax=vmax,
         cbar=False,
         vmin=-0.03,
         fmt=".0f" if normalize else ".2g",
         annot_kws={"fontsize": 8},
     )
+
     ref_data = df_to_draw.copy()
     ref_data.loc[
         :,
         ~ref_data.columns.isin(ref_other_changes),
     ] = np.nan
     sns.heatmap(
         ref_data,
@@ -314,45 +311,45 @@
         vmax=vmax,
         cbar=False,
         fmt=".1g",
         vmin=-0.03,
         annot_kws={"fontsize": 8},
     )
     ax.set_ylabel("Protospacer position")
-    return ax
+    return ax, df_to_draw
 
 
-def get_position_by_pam_rates(bdata, edit_rates_df: pd.DataFrame):
-    edit_rates_df["pam"] = bdata.guides.loc[
-        edit_rates_df.guide, "5-nt PAM"
-    ].reset_index(drop=True)
+def get_position_by_pam_rates(bdata, edit_rates_df: pd.DataFrame, pam_col="5-nt PAM"):
+    edit_rates_df["pam"] = bdata.guides.loc[edit_rates_df.guide, pam_col].reset_index(
+        drop=True
+    )
     edit_rates_df["pam23"] = edit_rates_df.pam.map(lambda s: s[1:3])
-    edit_rates_df["pam2"] = edit_rates_df.pam.map(lambda s: s[1])
-    edit_rates_df["pam3"] = edit_rates_df.pam.map(lambda s: s[2])
-    edit_rates_df["pam12"] = edit_rates_df.pam.map(lambda s: s[:2])
-    edit_rates_df["pam34"] = edit_rates_df.pam.map(lambda s: s[2:4])
     return pd.pivot(
-        edit_rates_df.loc[(edit_rates_df.base_change == bdata.target_base_change)]
+        edit_rates_df.loc[
+            (edit_rates_df.base_change == bdata.target_base_change),
+            ["rep_mean", "pam23", "spacer_pos"],
+        ]
         .groupby(["pam23", "spacer_pos"])
         .mean()
         .reset_index(),
         index="pam23",
         columns="spacer_pos",
         values="rep_mean",
     )
 
 
 def plot_by_pos_pam(
     bdata,
     edit_rates_df,
+    pam_col="5-nt PAM",
     ax=None,
     figsize=(6, 4),
 ):
     """Plot position by PAM"""
-    pos_by_pam = get_position_by_pam_rates(bdata, edit_rates_df)
+    pos_by_pam = get_position_by_pam_rates(bdata, edit_rates_df, pam_col)
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize)
     sns.heatmap(pos_by_pam, ax=ax, cmap="Blues")
     ax.set_yticklabels(ax.get_yticklabels(), rotation=0)
     return pos_by_pam
 
 
@@ -424,23 +421,24 @@
     )
     return pam_pref
 
 
 def plot_pam_preference(
     edit_rates_df,
     bdata=None,
+    pam_col="5-nt PAM",
     edit_start_pos: int = 3,
     edit_end_pos: int = 8,
     ax=None,
     norm=True,
 ):
     """ """
     if "pam2" not in edit_rates_df.columns or "pam3" not in edit_rates_df.columns:
         edit_rates_df["pam"] = bdata.guides.loc[
-            edit_rates_df.guide, "5-nt PAM"
+            edit_rates_df.guide, pam_col
         ].reset_index(drop=True)
         edit_rates_df["pam2"] = edit_rates_df.pam.map(lambda s: s[1])
         edit_rates_df["pam3"] = edit_rates_df.pam.map(lambda s: s[2])
     pam_pref = get_pam_preference(
         edit_rates_df, edit_start_pos, edit_end_pos, norm=norm
     )
     fig, ax = plt.subplots(figsize=(3, 3))
```

### Comparing `crispr-bean-0.2.7/bean/preprocessing/data_class.py` & `crispr-bean-1.0.0/bean/preprocessing/data_class.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import sys
 import abc
-from dataclasses import dataclass
-from typing import Dict, Tuple
 import logging
+from dataclasses import dataclass
+from typing import Optional, Dict, Tuple, List
 from xmlrpc.client import Boolean
 from copy import deepcopy
 import torch
 import numpy as np
 import pandas as pd
 import bean as be
 from .get_alpha0 import get_fitted_alpha0, get_pred_alpha0
 from .get_pi_alpha0 import get_fitted_alpha0 as get_fitted_pi_alpha0
 from .get_pi_alpha0 import get_pred_alpha0 as get_pred_pi_alpha0
 from .utils import (
-    Alias,
     get_accessibility_guides,
     get_edit_to_index_dict,
     _assign_rep_ids_and_sort,
 )
 
 logging.basicConfig(
     level=logging.INFO,
@@ -37,42 +36,70 @@
     def __init__(
         self,
         screen: be.ReporterScreen,
         repguide_mask: str = None,
         sample_mask_column: str = None,
         shrink_alpha: bool = False,
         condition_column: str = "sort",
+        sample_covariate_column: List[str] = [],
         control_condition: str = "bulk",
         accessibility_col: str = None,
         accessibility_bw_path: str = None,
         device: str = None,
-        replicate_column: str = "rep",
-        pi_popt: Tuple[float] = None,
+        replicate_column: str = "replicate",
+        popt: Optional[Tuple[float]] = None,
+        pi_popt: Optional[Tuple[float]] = None,
+        control_can_be_selected: bool = False,
         **kwargs,
     ):
+        """
+        Args
+        condition_column: By default, a single condition column, but you can optionally inlcude sample covariate column
+        control_can_be_selected: If True, screen.samples[condition_column] == control_condition can also be included in effect size inference if its condition column is not NA (Currently only suppoted for prolifertion screens).
+        """
         # TODO: remove replicate with too small number of (ex. only 1) sorting bin
         self.condition_column = condition_column
         self.device = device
         screen.samples["size_factor"] = self.get_size_factor(screen.X)
         if not (
-            "rep" in screen.samples.columns
+            replicate_column in screen.samples.columns
             and condition_column in screen.samples.columns
         ):
-            screen.samples["rep"], screen.samples[condition_column] = zip(
+            screen.samples[replicate_column], screen.samples[condition_column] = zip(
                 *screen.samples.index.map(lambda s: s.rsplit("_", 1))
             )
         if condition_column not in screen.samples.columns:
             screen.samples[condition_column] = screen.samples["index"].map(
                 lambda s: s.split("_")[-1]
             )
-
+        if "sample_covariates" in screen.uns:
+            self.sample_covariates = screen.uns["sample_covariates"]
+            self.n_sample_covariates = len(self.sample_covariates)
+            screen.samples["_rc"] = screen.samples[
+                [replicate_column] + self.sample_covariates
+            ].values.tolist()
+            screen.samples["_rc"] = screen.samples["_rc"].map(
+                lambda slist: ".".join(slist)
+            )
+            self.rep_by_cov = torch.as_tensor(
+                (
+                    screen.samples[["_rc"] + self.sample_covariates]
+                    .drop_duplicates()
+                    .set_index("_rc")
+                    .values.astype(int)
+                )
+            )
+            replicate_column = "_rc"
         self.screen = screen
-        self.screen_selected = screen[
-            :, screen.samples[condition_column] != control_condition
-        ]
+        if not control_can_be_selected:
+            self.screen_selected = screen[
+                :, screen.samples[condition_column] != control_condition
+            ]
+        else:
+            self.screen_selected = screen[:, ~screen.samples[condition_column].isnull()]
 
         self.n_condits = len(
             self.screen_selected.var[condition_column].unique()
         )  # excluding bulk
         self.screen_control = screen[
             :, screen.samples[condition_column] == control_condition
         ]
@@ -83,18 +110,17 @@
         self.accessibility_bw_path = accessibility_bw_path
         self.replicate_column = replicate_column
         self.condition_column = condition_column
         self.control_condition = control_condition
         self.sample_mask_column = sample_mask_column
         self.repguide_mask = repguide_mask
         self.shrink_alpha = shrink_alpha
+        self.popt = popt
 
-    def _post_init(
-        self,
-    ):
+    def _post_init(self):
         # Assign accessibility info
         if self.accessibility_col is not None:
             self.guide_accessibility = torch.as_tensor(
                 self.screen.guides[self.accessibility_col].values
             )
         elif self.accessibility_bw_path is not None:
             self.guide_accessibility = get_accessibility_guides(
@@ -119,29 +145,31 @@
         )  # (n_reps, n_bins, n_guides)
         self.X_masked = self.X * self.sample_mask[:, :, None]
         self.X_control = self.transform_data(self.screen_control.X, 1)
         self.X_control_masked = self.X_control * self.bulk_sample_mask[:, None, None]
         if self.repguide_mask is None:
             self.repguide_mask = ~(self.X == 0).any(axis=1)
         else:
-            print(f"Using repguide mask {self.repguide_mask}")
+            info(
+                f"Using replicate x guide mask in ReporterScreen.uns['{self.repguide_mask}'] to filter out outlier guides."
+            )
             assert (
                 self.repguide_mask in self.screen.uns.keys()
             ), f"{self.repguide_mask} not in screen.uns"
             assert self.screen_selected.uns[self.repguide_mask].shape == (
                 self.n_guides,
                 self.n_reps,
             )
             assert (
                 self.screen_selected.uns[self.repguide_mask].index
                 == self.screen_selected.guides.index
             ).all()
             assert (
                 self.screen_selected.uns[self.repguide_mask].columns
-                == self.screen_selected.samples.rep.unique()
+                == self.screen_selected.samples[self.replicate_column].unique()
             ).all()
             self.repguide_mask = (
                 torch.as_tensor(self.screen_selected.uns[self.repguide_mask].values.T)
                 > 0
             )
             self.repguide_mask = torch.logical_and(
                 self.repguide_mask, ~(self.X == 0).any(axis=1)
@@ -155,34 +183,46 @@
         ).reshape(self.n_reps, 1)
         # Get a0
         fitted_a0, self.popt = get_fitted_alpha0(
             self.X.clone().cpu(),
             self.size_factor.clone().cpu(),
             self.sample_mask.cpu(),
             shrink=self.shrink_alpha,
+            popt=self.popt,
         )
         fitted_a0 = torch.as_tensor(fitted_a0)
         a0 = fitted_a0
         self.a0 = torch.as_tensor(a0)
 
     def __getitem__(self, guide_idx):
         ndata = deepcopy(self)
         ndata.screen_selected = ndata.screen_selected[guide_idx, :]
         ndata.screen_control = ndata.screen_control[guide_idx, :]
         ndata.n_guides = len(guide_idx)
         ndata.X = ndata.X[:, :, guide_idx]  # (n_reps, n_bins, n_guides)
         ndata.X_masked = ndata.X_masked[:, :, guide_idx]
         ndata.X_control = ndata.X_control[:, :, guide_idx]
         ndata.repguide_mask = ndata.repguide_mask[:, guide_idx]
+        if hasattr(ndata, "a0") and self.a0 is not None:
+            ndata.a0 = ndata.a0[guide_idx]
         return ndata
 
     def transform_data(self, X, n_bins=None):
         if n_bins is None:
             n_bins = self.n_condits
-        x = torch.as_tensor(X).T.reshape((self.n_reps, n_bins, self.n_guides)).float()
+        try:
+            x = (
+                torch.as_tensor(X)
+                .T.reshape((self.n_reps, n_bins, self.n_guides))
+                .float()
+            )
+        except RuntimeError:
+            print((self.n_reps, n_bins, self.n_guides))
+            print(X.shape)
+            exit(1)
         if self.device is not None:
             x = x.cuda()
         return x
 
     def get_size_factor(self, X: np.array):
         """
         Get size factor for samples.
@@ -192,32 +232,32 @@
         assert geom_mean_x.shape == (n_guides,)
         norm_count = X / geom_mean_x[:, None]
         size_factor = np.median(norm_count, axis=0)
         assert size_factor.shape == (n_samples,)
         return size_factor
 
     def get_sample_ids_and_sort(self, screen: be.ReporterScreen, condit_id_col: str):
-        screen.samples["rep_id"] = -1
-        for i, rep in enumerate(sorted(screen.samples.rep.unique())):
-            screen.var.loc[screen.samples.rep == rep, "rep_id"] = i
+        screen.samples["replicate_id"] = -1
+        for i, rep in enumerate(sorted(screen.samples.replicate.unique())):
+            screen.var.loc[screen.samples.replicate == rep, "replicate_id"] = i
         if condit_id_col in screen.samples.columns:
             screen = screen[
-                :, screen.samples.sort_values(["rep_id", condit_id_col]).index
+                :, screen.samples.sort_values(["replicate_id", condit_id_col]).index
             ]
         else:
             raise ValueError("AnnData doesn't have condition id provided.")
         return screen
 
 
 @dataclass
 class ReporterScreenData(ScreenData):
     X_bcmatch: torch.Tensor
     size_factor_bcmatch: torch.Tensor
-    X_control_bcmatch: torch.Tensor
-    size_factor_control_bcmatch: torch.Tensor
+    X_bcmatch_control: torch.Tensor
+    size_factor_bcmatch_control: torch.Tensor
     allele_counts: torch.Tensor
     allele_counts_control: torch.Tensor
     a0_bcmatch: torch.Tensor
     a0_allele: torch.Tensor
     pi_a0: torch.Tensor
 
     def __init__(
@@ -328,16 +368,14 @@
         ndata.X_bcmatch = ndata.X_bcmatch[:, :, guide_idx]
         ndata.X_bcmatch_masked = ndata.X_bcmatch_masked[:, :, guide_idx]
         ndata.X_bcmatch_control = ndata.X_bcmatch_control[:, :, guide_idx]
         if hasattr(ndata, "allele_counts"):
             ndata.allele_counts = ndata.allele_counts[:, :, guide_idx, :]
         if hasattr(ndata, "a0_allele"):
             ndata.a0_allele = ndata.a0_allele[guide_idx, :]
-        if hasattr(ndata, "a0") and self.a0 is not None:
-            ndata.a0 = ndata.a0[guide_idx]
         if hasattr(ndata, "pi_a0") and self.pi_a0 is not None:
             ndata.pi_a0 = ndata.pi_a0[guide_idx]
         if hasattr(ndata, "a0_bcmatch") and self.a0_bcmatch is not None:
             ndata.a0_bcmatch = ndata.a0_bcmatch[guide_idx]
         if hasattr(ndata, "pi_a0_bcmatch") and self.pi_a0_bcmatch is not None:
             ndata.pi_a0_bcmatch = ndata.pi_a0_bcmatch[guide_idx]
         return ndata
@@ -436,15 +474,15 @@
             ndata.screen_selected, self.target_col
         )
         return ndata
 
     def get_target_lengths(self, screen, target_col="target"):
         target_len_list = []
         screen.guides[target_col] = screen.guides[target_col].astype("category")
-        cur_item = screen.guides[target_col].cat.codes[0]
+        cur_item = screen.guides[target_col].cat.codes.iloc[0]
         cur_len = 0
         n_targets = 0
         for i in screen.guides[target_col].cat.codes:
             if cur_item == i:
                 cur_len += 1
             else:
                 n_targets += 1
@@ -594,24 +632,24 @@
         Args
             edits_to_index: Dictionary from edit (str) to unique index (int)
             guide_allele_id_to_allele_df: pd.DataFrame of (guide(str), allele_id_for_guide(int)) -> CodingNoncodingAllele
 
         Returns
             allele_edit_assignment: Binary tensor of shape (n_guides, n_max_alleles_per_guide, n_edits. allele_edit_assignment(i, j, k) is 1 if jth allele of ith guide has kth edit.
         """
-        guide_allele_id_to_allele_df[
-            "edits"
-        ] = guide_allele_id_to_allele_df.aa_allele.map(
-            lambda a: list(a.aa_allele.edits) + list(a.nt_allele.edits)
+        guide_allele_id_to_allele_df["edits"] = (
+            guide_allele_id_to_allele_df.aa_allele.map(
+                lambda a: list(a.aa_allele.edits) + list(a.nt_allele.edits)
+            )
         )
         guide_allele_id_to_allele_df = guide_allele_id_to_allele_df.reset_index()
-        guide_allele_id_to_allele_df[
-            "edit_idx"
-        ] = guide_allele_id_to_allele_df.edits.map(
-            lambda es: [edits_to_index[e.get_abs_edit()] for e in es]
+        guide_allele_id_to_allele_df["edit_idx"] = (
+            guide_allele_id_to_allele_df.edits.map(
+                lambda es: [edits_to_index[e.get_abs_edit()] for e in es]
+            )
         )
         guide_allele_id_to_edit_df = guide_allele_id_to_allele_df[
             ["guide", "allele_id_for_guide", "edit_idx"]
         ].set_index(["guide", "allele_id_for_guide"])
         guide_allele_id_to_edit_df = guide_allele_id_to_edit_df.unstack(
             level=1, fill_value=[]
         ).reindex(screen.guides.index, fill_value=[])
@@ -664,20 +702,20 @@
         """
         Transform reindexed allele dataframe reindexed_df of (guide, allele_id_for_guide) -> (per sample count)
         to (n_reps, n_bins, n_guides, n_alleles) tensor.
         """
         allele_tensor = torch.empty(
             (self.n_reps, self.n_condits, self.n_guides, self.n_max_alleles),
         )
-        if not self.device is None:
+        if self.device is not None:
             allele_tensor = allele_tensor.cuda()
         for i in range(self.n_reps):
             for j in range(self.n_condits):
                 condit_idx = np.where(
-                    (adata.samples.rep_id == i)
+                    (adata.samples.replicate_id == i)
                     & (adata.samples[f"{self.condition_column}_id"] == j)
                 )[0]
                 assert len(condit_idx) == 1, print(i, j, condit_idx)
                 condit_idx = condit_idx.item()
                 condit_name = adata.samples.index[condit_idx]
                 condit_allele_df = (
                     reindexed_df.loc[:, condit_name]
@@ -706,32 +744,32 @@
                     self.n_guides,
                     self.n_max_alleles,
                 )
                 allele_tensor[i, j, :, :] = torch.as_tensor(condit_allele_df.to_numpy())
 
         try:
             assert (allele_tensor >= 0).all(), allele_tensor[allele_tensor < 0]
-        except:
+        except AssertionError:
             print("Allele tensor doesn't match condit_allele_df")
             return (allele_tensor, reindexed_df)
         return allele_tensor
 
     def transform_allele_control(self, adata, reindexed_df):
         """
         Transform reindexed allele dataframe reindexed_df of (guide, allele_id_for_guide) -> (per sample count)
         to (n_reps, n_bins, n_guides, n_alleles) tensor.
         """
 
         allele_tensor = torch.empty(
             (self.n_reps, 1, self.n_guides, self.n_max_alleles),
         )
-        if not self.device is None:
+        if self.device is not None:
             allele_tensor = allele_tensor.cuda()
         for i in range(self.n_reps):
-            condit_idx = np.where(adata.samples.rep_id == i)[0]
+            condit_idx = np.where(adata.samples.replicate_id == i)[0]
             assert len(condit_idx) == 1, print(i, self.control_condition, condit_idx)
             condit_idx = condit_idx.item()
             condit_name = adata.samples.index[condit_idx]
             condit_allele_df = (
                 reindexed_df.loc[:, condit_name]
                 .unstack(level=1, fill_value=0)
                 .astype(int)
@@ -757,22 +795,18 @@
                 "allele_id_for_guide", axis=1, ascending=True
             )
             assert all(condit_allele_df.columns == list(range(self.n_max_alleles)))
             assert condit_allele_df.to_numpy().shape == (
                 self.n_guides,
                 self.n_max_alleles,
             )
-            try:
-                allele_tensor[i, 0, :, :] = torch.as_tensor(condit_allele_df.to_numpy())
-            except:
-                print("Allele tensor doesn't match condit_allele_df")
-                return (allele_tensor, torch.as_tensor(condit_allele_df.to_numpy()))
+            allele_tensor[i, 0, :, :] = torch.as_tensor(condit_allele_df.to_numpy())
         try:
             assert (allele_tensor >= 0).all(), allele_tensor[allele_tensor < 0]
-        except:
+        except AssertionError:
             print("Negative values in allele_tensor")
             return (allele_tensor, reindexed_df)
         return allele_tensor
 
     def get_allele_mask(
         self, adata, guide_allele_id_to_allele_df, keep_one_allele: bool = False
     ):
@@ -792,73 +826,32 @@
         mask = torch.zeros((self.n_guides, self.n_max_alleles))
         for i in range(mask.shape[0]):
             mask[i, 0] = 1
             for j in range(n_valid_allele[i]):
                 mask[i, j + 1] = 1
         return mask.bool()
 
-    def get_allele_to_edit_tensor(
-        self,
-        adata,
-        edits_to_index: Dict[str, int],
-        guide_allele_id_to_allele_df: pd.DataFrame,
-    ):
-        """
-        Convert (guide, allele_id_for_guide) -> allele DataFrame into the tensor with shape (n_guides, n_max_alleles_per_guide, n_edits) tensor.
-        -----
-        Arguments
-        edits_to_index (dict) -- Dictionary from edit (str) to unique index (int)
-        guide_allele_id_to_allele_df (pd.DataFrame) -- pd.DataFrame of (guide(str), allele_id_for_guide(int)) -> CodingNoncodingAllele
-        -----
-        Returns
-        allele_edit_assignment (torch.Tensor) -- Binary tensor of shape (n_guides, n_max_alleles_per_guide, n_edits).
-        allele_edit_assignment(i, j, k) is 1 if jth allele of ith guide has kth edit.
-        """
-        guide_allele_id_to_allele_df[
-            "edits"
-        ] = guide_allele_id_to_allele_df.aa_allele.map(
-            lambda a: list(a.aa_allele.edits) + list(a.nt_allele.edits)
-        )
-        guide_allele_id_to_allele_df = guide_allele_id_to_allele_df.reset_index()
-        guide_allele_id_to_allele_df[
-            "edit_idx"
-        ] = guide_allele_id_to_allele_df.edits.map(
-            lambda es: [edits_to_index[e.get_abs_edit()] for e in es]
-        )
-        guide_allele_id_to_edit_df = guide_allele_id_to_allele_df[
-            ["guide", "allele_id_for_guide", "edit_idx"]
-        ].set_index(["guide", "allele_id_for_guide"])
-        guide_allele_id_to_edit_df = guide_allele_id_to_edit_df.unstack(
-            level=1, fill_value=[]
-        ).reindex(adata.guides.index, fill_value=[])
-        allele_edit_assignment = torch.zeros(
-            (len(adata.guides), self.n_max_alleles - 1, len(edits_to_index.keys()))
-        )
-        for i in range(len(guide_allele_id_to_edit_df)):
-            for j in range(len(guide_allele_id_to_edit_df.columns)):
-                allele_edit_assignment[i, j, guide_allele_id_to_edit_df.iloc[i, j]] = 1
-        return allele_edit_assignment
-
 
 @dataclass
 class SortingScreenData(ScreenData):
     upper_bounds: torch.Tensor
     lower_bounds: torch.Tensor
 
     def __init__(
         self,
         screen: be.ReporterScreen,
         repguide_mask: str = None,
         sample_mask_column: str = None,
         shrink_alpha: bool = False,
         condition_column: str = "sort",
+        sample_covariate_column: List[str] = [],
         control_condition: str = "bulk",
         lower_quantile_column: str = "lower_quantile",
         upper_quantile_column: str = "upper_quantile",
-        replicate_column: str = "rep",
+        replicate_column: str = "replicate",
         **kwargs,
     ):
         """
         Args
         ---
         lower_quantile_column: column in screen.samples that indicate lower quantile threshold of sorting bin.
         upper_quantile_column: column in screen.samples that indicate upper quantile threshold of sorting bin.
@@ -905,15 +898,15 @@
         if not (
             self.screen.samples.groupby(
                 [upper_quantile_column, lower_quantile_column]
             ).size()
             == len(self.screen.samples[self.replicate_column].unique())
         ).all():
             raise ValueError(
-                "Not all replicate share same quantile bin definition. If you have missing bin data, add the sample and add 'mask' column in 'screen.samples'."
+                "Not all replicate share same quantile bin definition. If you have missing bin data, add the sample and add 'mask' column in 'screen.samples' or run `bean-qc` that automatically handles this."
             )
         sorting_bins = self.screen_selected.samples.sort_values(
             [upper_quantile_column, lower_quantile_column]
         )[[upper_quantile_column, lower_quantile_column]].drop_duplicates()
         for j, (idx, row) in enumerate(sorting_bins.iterrows()):
             self.screen_selected.samples.loc[
                 (
@@ -931,14 +924,23 @@
         self.screen.samples[f"{self.condition_column}_id"] = -1
         self.screen.samples.loc[
             self.screen_selected.samples.index, f"{self.condition_column}_id"
         ] = self.screen_selected.samples[f"{self.condition_column}_id"]
         self.screen = _assign_rep_ids_and_sort(
             self.screen, self.replicate_column, self.condition_column
         )
+        if hasattr(self, "sample_covariates"):
+            self.rep_by_cov = torch.as_tensor(
+                (
+                    self.screen.samples[["_rc"] + self.sample_covariates]
+                    .drop_duplicates()
+                    .set_index("_rc")
+                    .values.astype(int)
+                )
+            )
         self.screen_selected = _assign_rep_ids_and_sort(
             self.screen_selected, self.replicate_column, self.condition_column
         )
         self.screen_control = _assign_rep_ids_and_sort(
             self.screen_control,
             self.replicate_column,
         )
@@ -948,48 +950,105 @@
 class SurvivalScreenData(ScreenData):
     def __init__(
         self,
         screen: be.ReporterScreen,
         repguide_mask: str = None,
         sample_mask_column: str = None,
         shrink_alpha: bool = False,
-        condition_column: str = "time",
+        condition_column: str = "condition",
         control_condition: str = "bulk",
-        accessibility_col: str = None,
-        accessibility_bw_path: str = None,
+        control_can_be_selected=True,
+        time_column: str = "time",
+        replicate_column: str = "replicate",
         **kwargs,
     ):
+        self._pre_init(condition_column)
         super().__init__(
             screen=screen,
             repguide_mask=repguide_mask,
             sample_mask_column=sample_mask_column,
             shrink_alpha=shrink_alpha,
             condition_column=condition_column,
             control_condition=control_condition,
-            accessibility_col=accessibility_col,
-            accessibility_bw_path=accessibility_bw_path,
+            control_can_be_selected=control_can_be_selected,
             **kwargs,
         )
+        self._post_init()
+
+    def _pre_init(self, time_column: str, condition_column: str):
+        self.time_column = time_column
+        try:
+            self.screen.samples[time_column] = self.screen.samples[time_column].astype(
+                float
+            )
+        except ValueError as e:
+            raise ValueError(
+                f"Invalid timepoint value({self.screen.samples[time_column]}) in screen.samples[{time_column}]: check input."
+            ) from e
+
+        if not (
+            self.screen.samples.groupby(condition_column).size()
+            == len(self.screen.samples[self.replicate_column].unique())
+        ).all():
+            raise ValueError(
+                f"Not all replicate share same timepoint definition. If you have missing bin data, add the sample and add 'mask' column in 'screen.samples', or run `bean-qc` that automatically handles this. \n{self.screen.samples}"
+            )
+
+    def _post_init(
+        self,
+    ):
         self.timepoints = torch.as_tensor(
-            self.screen.samples[condition_column].unique()
+            self.screen_selected.samples[self.time_column].unique()
+        )
+        self.n_timepoints = self.n_condits
+        timepoints = self.screen_selected.samples.sort_values(self.time_column)[
+            self.time_column
+        ].drop_duplicates()
+        if timepoints.isnull().any():
+            raise ValueError(
+                f"NaN values in time points provided in input: {self.screen_selected.samples[self.time_column]}"
+            )
+        for j, time in enumerate(timepoints):
+            self.screen_selected.samples.loc[
+                self.screen_selected.samples[self.time_column] == time,
+                f"{self.time_column}_id",
+            ] = j
+        self.screen.samples[f"{self.time_column}_id"] = -1
+        self.screen.samples.loc[
+            self.screen_selected.samples.index, f"{self.time_column}_id"
+        ] = self.screen_selected.samples[f"{self.time_column}_id"]
+        self.screen = _assign_rep_ids_and_sort(
+            self.screen, self.replicate_column, self.time_column
+        )
+        if hasattr(self, "sample_covariates"):
+            self.rep_by_cov = self.screen.samples.groupby(self.replicate_column)[
+                self.sample_covariates
+            ].values
+        self.screen_selected = _assign_rep_ids_and_sort(
+            self.screen_selected,
+            self.replicate_column,
+            self.time_column,
+        )
+        self.screen_control = _assign_rep_ids_and_sort(
+            self.screen_control,
+            self.replicate_column,
         )
-        self.timepoints = Alias("n_condits")
 
 
 @dataclass
 class VariantReporterScreenData(VariantScreenData, ReporterScreenData):
     def __init__(
         self,
         screen: be.ReporterScreen,
         repguide_mask: str = None,
         sample_mask_column: str = None,
         pi_popt: Tuple[float] = None,
         impute_pi_popt: bool = False,
         shrink_alpha: bool = False,
-        condition_column: str = "time",
+        condition_column: str = "condition",
         control_condition: str = "bulk",
         accessibility_col: str = None,
         accessibility_bw_path: str = None,
         use_const_pi: bool = False,
         pi_prior_count: int = 10,
         **kwargs,
     ):
@@ -1019,35 +1078,100 @@
 class VariantSortingScreenData(VariantScreenData, SortingScreenData):
     def __init__(
         self,
         screen,
         *args,
         lower_quantile_column="lower_quantile",
         upper_quantile_column="upper_quantile",
-        replicate_column="rep",
+        replicate_column="replicate",
         condition_column="bin",
+        target_col="target",
+        sample_mask_column="mask",
+        shrink_alpha: bool = False,
+        use_bcmatch=False,
         **kwargs,
     ):
+        ScreenData.__init__(
+            self,
+            screen,
+            *args,
+            sample_mask_column=sample_mask_column,
+            replicate_column=replicate_column,
+            condition_column=condition_column,
+            shrink_alpha=shrink_alpha,
+            **kwargs,
+        )
         SortingScreenData._pre_init(
             self,
             lower_quantile_column,
             upper_quantile_column,
         )
-        VariantScreenData.__init__(self, *args, **kwargs)
+        ScreenData._post_init(self)
+        VariantScreenData._post_init(self, target_col)
+        if use_bcmatch:
+            self.set_bcmatch(
+                screen,
+            )
+
+    def set_bcmatch(self, screen):
+        screen.samples["size_factor_bcmatch"] = self.get_size_factor(
+            screen.layers["X_bcmatch"]
+        )
+        self.screen_selected.samples["size_factor_bcmatch"] = screen.samples.loc[
+            self.screen_selected.samples.index, "size_factor_bcmatch"
+        ]
+        self.screen_control.samples["size_factor_bcmatch"] = screen.samples.loc[
+            self.screen_control.samples.index, "size_factor_bcmatch"
+        ]
+        self.X_bcmatch = self.transform_data(self.screen_selected.layers["X_bcmatch"])
+        self.X_bcmatch_masked = self.X_bcmatch * self.sample_mask[:, :, None]
+        self.X_bcmatch_control = self.transform_data(
+            self.screen_control.layers["X_bcmatch"], 1
+        )
+        self.X_bcmatch_control_masked = (
+            self.X_bcmatch_control * self.bulk_sample_mask[:, None, None]
+        )
+        self.size_factor_bcmatch = torch.as_tensor(
+            self.screen_selected.samples["size_factor_bcmatch"].to_numpy()
+        ).reshape(self.n_reps, self.n_condits)
+        self.size_factor_bcmatch_control = torch.as_tensor(
+            self.screen_control.samples["size_factor_bcmatch"].to_numpy()
+        ).reshape(self.n_reps, 1)
+        a0_bcmatch = get_pred_alpha0(
+            self.X_bcmatch.clone().cpu(),
+            self.size_factor_bcmatch.clone().cpu(),
+            self.popt,
+            self.sample_mask.cpu(),
+        )
+        self.a0_bcmatch = torch.as_tensor(a0_bcmatch)
+
+    def __getitem__(self, guide_idx):
+        ndata = super().__getitem__(guide_idx)
+        if hasattr(ndata, "X_bcmatch"):
+            ndata.X_bcmatch = ndata.X_bcmatch[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_masked"):
+            ndata.X_bcmatch_masked = ndata.X_bcmatch_masked[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_control"):
+            ndata.X_bcmatch_control = ndata.X_bcmatch_control[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_control_masked"):
+            ndata.X_bcmatch_control_masked = ndata.X_bcmatch_control_masked[
+                :, :, guide_idx
+            ]
+        return ndata
 
 
 @dataclass
 class VariantSortingReporterScreenData(VariantReporterScreenData, SortingScreenData):
     def __init__(
         self,
         screen,
         *args,
         lower_quantile_column="lower_quantile",
         upper_quantile_column="upper_quantile",
-        replicate_column="rep",
+        replicate_column="replicate",
         condition_column="bin",
         target_col="target",
         sample_mask_column="mask",
         use_const_pi: bool = False,
         impute_pi_popt: bool = False,
         pi_prior_count: int = 10,
         shrink_alpha: bool = False,
@@ -1055,16 +1179,16 @@
         **kwargs,
     ):
         ScreenData.__init__(
             self,
             screen,
             *args,
             sample_mask_column=sample_mask_column,
-            replicate_column="rep",
-            condition_column="bin",
+            replicate_column=replicate_column,
+            condition_column=condition_column,
             shrink_alpha=shrink_alpha,
             **kwargs,
         )
         SortingScreenData._pre_init(
             self,
             lower_quantile_column,
             upper_quantile_column,
@@ -1086,15 +1210,15 @@
 class TilingSortingReporterScreenData(TilingReporterScreenData, SortingScreenData):
     def __init__(
         self,
         screen,
         *args,
         lower_quantile_column="lower_quantile",
         upper_quantile_column="upper_quantile",
-        replicate_column="rep",
+        replicate_column="replicate",
         condition_column="bin",
         sample_mask_column="mask",
         use_const_pi: bool = False,
         impute_pi_popt: bool = False,
         pi_prior_count: int = 10,
         shrink_alpha: bool = False,
         pi_popt: Tuple[float] = None,
@@ -1104,16 +1228,16 @@
         **kwargs,
     ):
         ScreenData.__init__(
             self,
             screen,
             *args,
             sample_mask_column=sample_mask_column,
-            replicate_column="rep",
-            condition_column="bin",
+            replicate_column=replicate_column,
+            condition_column=condition_column,
             shrink_alpha=shrink_alpha,
             **kwargs,
         )
         SortingScreenData._pre_init(
             self,
             lower_quantile_column,
             upper_quantile_column,
@@ -1132,9 +1256,205 @@
             pi_prior_count,
             shrink_alpha,
             pi_popt,
         )
 
 
 @dataclass
+class VariantSurvivalScreenData(VariantScreenData, SurvivalScreenData):
+    def __init__(
+        self,
+        screen,
+        *args,
+        replicate_column="replicate",
+        condition_column="condition",
+        time_column="time",
+        control_can_be_selected=True,
+        target_col="target",
+        sample_mask_column="mask",
+        shrink_alpha: bool = False,
+        use_bcmatch=False,
+        **kwargs,
+    ):
+        ScreenData.__init__(
+            self,
+            screen,
+            *args,
+            sample_mask_column=sample_mask_column,
+            replicate_column=replicate_column,
+            condition_column=condition_column,
+            time_column=time_column,
+            shrink_alpha=shrink_alpha,
+            control_can_be_selected=control_can_be_selected,
+            **kwargs,
+        )
+        SurvivalScreenData._pre_init(self, time_column, condition_column)
+        ScreenData._post_init(self)
+        SurvivalScreenData._post_init(self)
+        VariantScreenData._post_init(self, target_col)
+        if use_bcmatch:
+            self.set_bcmatch(
+                screen,
+            )
+
+    def __getitem__(self, guide_idx):
+        ndata = super().__getitem__(guide_idx)
+        if hasattr(ndata, "X_bcmatch"):
+            ndata.X_bcmatch = ndata.X_bcmatch[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_masked"):
+            ndata.X_bcmatch_masked = ndata.X_bcmatch_masked[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_control"):
+            ndata.X_bcmatch_control = ndata.X_bcmatch_control[:, :, guide_idx]
+        if hasattr(ndata, "X_bcmatch_control_masked"):
+            ndata.X_bcmatch_control_masked = ndata.X_bcmatch_control_masked[
+                :, :, guide_idx
+            ]
+        return ndata
+
+    def set_bcmatch(self, screen):
+        screen.samples["size_factor_bcmatch"] = self.get_size_factor(
+            screen.layers["X_bcmatch"]
+        )
+        self.screen_selected.samples["size_factor_bcmatch"] = screen.samples.loc[
+            self.screen_selected.samples.index, "size_factor_bcmatch"
+        ]
+        self.screen_control.samples["size_factor_bcmatch"] = screen.samples.loc[
+            self.screen_control.samples.index, "size_factor_bcmatch"
+        ]
+        self.X_bcmatch = self.transform_data(self.screen_selected.layers["X_bcmatch"])
+        self.X_bcmatch_masked = self.X_bcmatch * self.sample_mask[:, :, None]
+        self.X_bcmatch_control = self.transform_data(
+            self.screen_control.layers["X_bcmatch"], 1
+        )
+        self.X_bcmatch_control_masked = (
+            self.X_bcmatch_control * self.bulk_sample_mask[:, None, None]
+        )
+        self.size_factor_bcmatch = torch.as_tensor(
+            self.screen_selected.samples["size_factor_bcmatch"].to_numpy()
+        ).reshape(self.n_reps, self.n_condits)
+        self.size_factor_bcmatch_control = torch.as_tensor(
+            self.screen_control.samples["size_factor_bcmatch"].to_numpy()
+        ).reshape(self.n_reps, 1)
+        a0_bcmatch = get_pred_alpha0(
+            self.X_bcmatch.clone().cpu(),
+            self.size_factor_bcmatch.clone().cpu(),
+            self.popt,
+            self.sample_mask.cpu(),
+        )
+        self.a0_bcmatch = torch.as_tensor(a0_bcmatch)
+
+
+@dataclass
 class VariantSurvivalReporterScreenData(VariantReporterScreenData, SurvivalScreenData):
-    pass
+    def __init__(
+        self,
+        screen,
+        *args,
+        replicate_column="replicate",
+        condition_column="condition",
+        time_column="time",
+        control_can_be_selected=True,
+        target_col="target",
+        sample_mask_column="mask",
+        use_const_pi: bool = False,
+        impute_pi_popt: bool = False,
+        pi_prior_count: int = 10,
+        shrink_alpha: bool = False,
+        pi_popt: Tuple[float] = None,
+        **kwargs,
+    ):
+        ScreenData.__init__(
+            self,
+            screen,
+            *args,
+            sample_mask_column=sample_mask_column,
+            replicate_column=replicate_column,
+            condition_column=condition_column,
+            time_column=time_column,
+            shrink_alpha=shrink_alpha,
+            control_can_be_selected=control_can_be_selected,
+            **kwargs,
+        )
+        SurvivalScreenData._pre_init(self, time_column, condition_column)
+        ScreenData._post_init(self)
+        SurvivalScreenData._post_init(self)
+        VariantScreenData._post_init(self, target_col)
+        ReporterScreenData._post_init(
+            self,
+            screen,
+            use_const_pi,
+            impute_pi_popt,
+            pi_prior_count,
+            shrink_alpha,
+            pi_popt,
+        )
+
+
+@dataclass
+class TilingSurvivalReporterScreenData(TilingReporterScreenData, SurvivalScreenData):
+    def __init__(
+        self,
+        screen,
+        *args,
+        replicate_column="replicate",
+        condition_column="condition",
+        time_column="time",
+        control_can_be_selected=True,
+        sample_mask_column="mask",
+        use_const_pi: bool = False,
+        impute_pi_popt: bool = False,
+        pi_prior_count: int = 10,
+        shrink_alpha: bool = False,
+        pi_popt: Tuple[float] = None,
+        allele_df_key: str = None,
+        allele_col: str = None,
+        control_guide_tag: str = None,
+        **kwargs,
+    ):
+        ScreenData.__init__(
+            self,
+            screen,
+            *args,
+            sample_mask_column=sample_mask_column,
+            replicate_column=replicate_column,
+            condition_column=condition_column,
+            time_column=time_column,
+            shrink_alpha=shrink_alpha,
+            control_can_be_selected=control_can_be_selected,
+            **kwargs,
+        )
+        SurvivalScreenData._pre_init(self, time_column, condition_column)
+        ScreenData._post_init(self)
+        SurvivalScreenData._post_init(self)
+        TilingReporterScreenData._post_init(
+            self,
+            allele_df_key=allele_df_key,
+            control_guide_tag=control_guide_tag,
+        )
+        ReporterScreenData._post_init(
+            self,
+            screen,
+            use_const_pi,
+            impute_pi_popt,
+            pi_prior_count,
+            shrink_alpha,
+            pi_popt,
+        )
+
+
+DATACLASS_DICT = {
+    "sorting": {
+        "Normal": VariantSortingScreenData,
+        "MixtureNormal": VariantSortingReporterScreenData,
+        "MixtureNormal+Acc": VariantSortingReporterScreenData,
+        "MixtureNormalConstPi": VariantSortingScreenData,
+        "MultiMixtureNormal": TilingSortingReporterScreenData,
+        "MultiMixtureNormal+Acc": TilingSortingReporterScreenData,
+    },
+    "survival": {
+        "Normal": VariantSurvivalScreenData,
+        "MixtureNormal": VariantSurvivalReporterScreenData,
+        "MixtureNormal+Acc": VariantSurvivalReporterScreenData,
+        "MultiMixtureNormal": TilingSurvivalReporterScreenData,
+        "MultiMixtureNormal+Acc": TilingSurvivalReporterScreenData,
+    },
+}
```

### Comparing `crispr-bean-0.2.7/bean/preprocessing/get_alpha0.py` & `crispr-bean-1.0.0/bean/preprocessing/get_alpha0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional, Tuple
 import numpy as np
 import torch
 from scipy.optimize import curve_fit
 
 """
 Returns fitted alpha 0 (sum of concentration) of Dirichlet-Multinomial
 For the notation, see DESeq paper
@@ -67,23 +68,25 @@
 
 
 def get_fitted_alpha0(
     X,
     sample_size_factors,
     sample_mask=None,
     fit_quantile: float = None,
-    shrink=False,
-    shrink_prior_var=1.0,
+    shrink: bool = False,
+    shrink_prior_var: float = 1.0,
+    popt: Optional[Tuple[float, float]] = None,
 ):
     """Fits sum of concentration of DirichletMultinomial distribution.
 
     Args:
         fit: if False, return the raw value
         fit_quantile: if not None, alpha is fitted conservatively with lowest `fit_quantile`
             guides.
+        popt: Regression coefficient (b0, b1) of log(a0) ~ log(q) that will be used if fitting dispersion on the data fails
     """
     n_reps, n_condits, n_guides = X.shape
     if sample_mask is None:
         sample_mask = torch.ones((n_reps, n_condits), device="cpu")
     elif (sample_mask.sum(axis=0) == 0).any():
         raise ValueError("Some bins have no data.")
     w = get_w(X + 1, sample_size_factors, sample_mask=sample_mask)
@@ -94,15 +97,16 @@
     p = q / n[None, :]  # depth-normalized p for Multinomial
     multinom_var = n[None, :] * p * (1 - p)  # theoretical Multinomial variance
     r = (w - q) / multinom_var
     a0 = ((n - 1) / (r - 1 + 1 / (1 - p)) - 1).mean(axis=0)
 
     x, y = get_valid_vals(n.log(), a0.log())
     if len(y) < 10:
-        popt = (-1.510, 0.7861)
+        if popt is None:
+            popt = (-1.510, 0.7861)
         print(
             f"Cannot fit log(a0) ~ log(q): data too sparse! Using pre-fitted values [b0, b1]={popt}"
         )
     else:
         popt, pcov = curve_fit(linear, x, y)
         print("Linear fit of log(a0) ~ log(q): [b0, b1]={}, cov={}".format(popt, pcov))
     log_a0_est = torch.as_tensor(linear(n.log().cpu().numpy(), *popt))
```

### Comparing `crispr-bean-0.2.7/bean/preprocessing/get_pi_alpha0.py` & `crispr-bean-1.0.0/bean/preprocessing/get_pi_alpha0.py`

 * *Files identical despite different names*

### Comparing `crispr-bean-0.2.7/bean/preprocessing/utils.py` & `crispr-bean-1.0.0/bean/preprocessing/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 import torch
 import numpy as np
 import pyBigWig
 import pandas as pd
-import anndata as ad
 import bean as be
+from bean.qc.guide_qc import filter_no_info_target
 
 
 class Alias:
     def __init__(self, source_name):
         self.source_name = source_name
 
     def __get__(self, obj, objtype=None):
@@ -17,14 +17,41 @@
             return self
         return getattr(obj, self.source_name)
 
     def __set__(self, obj, value):
         setattr(obj, self.source_name, value)
 
 
+def prepare_bdata(bdata: be.ReporterScreen, args, warn, prefix: str):
+    """Utility function for formatting bdata for bean-run"""
+    bdata = bdata.copy()
+    bdata.samples["replicate"] = bdata.samples[args.replicate_col].astype("category")
+    bdata.guides = bdata.guides.loc[:, ~bdata.guides.columns.duplicated()].copy()
+    if args.library_design == "variant":
+        if bdata.guides[args.target_col].isnull().any():
+            raise ValueError(
+                f"Some target column (bdata.guides[{args.target_col}]) value is null. Check your input file."
+            )
+        bdata = bdata[bdata.guides[args.target_col].argsort(), :]
+        n_no_support_targets, bdata = filter_no_info_target(
+            bdata,
+            condit_col=args.condition_col,
+            control_condition=args.control_condition,
+            target_col=args.target_col,
+            write_no_support_targets=True,
+            no_support_target_write_path=f"{prefix}/no_support_targets.csv",
+        )
+        if n_no_support_targets > 0:
+            warn(
+                f"Ignoring {n_no_support_targets} targets with 0 gRNA counts across all non-control samples. Ignored targets are written in {prefix}/no_support_targets.csv."
+            )
+        return bdata
+    return bdata
+
+
 def _get_accessibility_single(
     pos: int,
     track,
     chrom: str = "chr19",
     guide_start_pos=0,
     half_window_size: int = 100,
 ):
@@ -181,24 +208,28 @@
                 prev_item = item
 
 
 def _assign_rep_ids_and_sort(
     screen: be.ReporterScreen, rep_col: str, condition_column: str = None
 ) -> be.ReporterScreen:
     """Assign replicate IDs to samples and sort them accordingly."""
+    if rep_col not in screen.samples.columns:
+        raise ValueError(
+            f"{rep_col} not in columns of ReporterScreen.samples with following columns: {screen.samples.columns}. Check your input or adjust `--replicate-col` of `bean-run` command as the existing column name specifying experimental replicates."
+        )
     for i, rep in enumerate(sorted(screen.samples[rep_col].unique())):
         screen.samples.loc[screen.samples[rep_col] == rep, f"{rep_col}_id"] = i
-        if condition_column is None:
-            sort_key = f"{rep_col}_id"
-        else:
-            sort_key = [f"{rep_col}_id", f"{condition_column}_id"]
-        screen = screen[
-            :,
-            screen.samples.sort_values(sort_key).index,
-        ]
+    if condition_column is None:
+        sort_key = f"{rep_col}_id"
+    else:
+        sort_key = [f"{rep_col}_id", f"{condition_column}_id"]
+    screen = screen[
+        :,
+        screen.samples.sort_values(sort_key).index,
+    ]
     return screen
 
 
 def _obtain_effective_edit_rate(ndata, count_thres=10):
     """Calculates effective editing rate of each variant for tiling screen.
 
     Allele count
@@ -224,7 +255,18 @@
         ndata.n_edits,
     )
     return (mean_allele_rates[:, :, None] * allele_to_edit_normed).nansum(axis=(0, 1))
 
 
 def _obtain_n_guides_alleles_per_variant(ndata):
     return (ndata.allele_to_edit.sum(axis=1) > 0).sum(axis=0)
+
+
+def _obtain_n_cooccurring_variants(ndata) -> np.ndarray:
+    """Obtain the number of co-occurring variants in any allele produced by any guides."""
+    allele_to_edit = ndata.allele_to_edit.cpu()
+    n_coedited_vars_edits = []
+    for edit_idx in range(allele_to_edit.shape[-1]):
+        gidx, aidx = torch.where(allele_to_edit[:, :, edit_idx] > 0)
+        n_coedited_vars = (allele_to_edit[gidx, aidx, :].sum(axis=0) > 0).sum() - 1
+        n_coedited_vars_edits.append(n_coedited_vars)
+    return np.array(n_coedited_vars_edits)
```

### Comparing `crispr-bean-0.2.7/bean/qc/sample_qc.py` & `crispr-bean-1.0.0/bean/qc/sample_qc.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,39 @@
         fig, ax = plt.subplots(figsize=figsize)
     sns.histplot(bdata.guides.edit_rate, bins=n_bins)
     ax.set_title(title)
     ax.set_xlabel("Editing rate")
     return ax
 
 
-def plot_sample_edit_rates(
-    bdata, ax=None, figsize=(5, 3), title="", agg_method="median"
-):
+def plot_sample_edit_rates(bdata, ax=None, figsize=(5, 3), title="", agg_method="mean"):
+    if agg_method == "median":
+        agg = np.nanmedian
+    elif agg_method == "mean":
+        agg = np.nanmean
+    else:
+        raise ValueError(
+            "Invalid aggregation method provided. Please pass one of 'median' or 'mean'."
+        )
     set_sample_edit_rates(bdata, agg_method)
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize)
     for i, sample in enumerate(bdata.samples.index):
         sns.kdeplot(
             bdata.layers["edit_rate"][:, i],
-            label=f"{sample}(median {np.nanmedian(bdata.layers['edit_rate'][:, i]):.2f})",
+            label=f"{sample}({agg_method} {agg(bdata.layers['edit_rate'][:, i]):.2f})",
             linestyle=linestyles[(i // 10) % 4],
             clip=(0, 1),
         )
     sns.kdeplot(
-        bdata.guides.edit_rate, linewidth=2, c="black", label="Bulk median", clip=(0, 1)
+        bdata.guides.edit_rate,
+        linewidth=2,
+        c="black",
+        label=f"Bulk {agg_method}",
+        clip=(0, 1),
     )
     ax.set_xlabel("Editing rate")
     ax.set_title(title)
     ax.legend(bbox_to_anchor=(1, 1))
     return ax
```

### Comparing `crispr-bean-0.2.7/bean/qc/utils.py` & `crispr-bean-1.0.0/bean/qc/parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,188 +1,153 @@
-import numpy as np
-import pandas as pd
-from copy import deepcopy
 import argparse
-from ..framework.ReporterScreen import ReporterScreen, concat
 
 
-def parse_args():
-    print("  \n~~~BEANQC~~~")
-    print("-Check guide/sample level quality and mask / discard-")
-    print(
-        r"""
-    _ _       
-  /  \ '\        ___   ___ 
-  |   \  \      / _ \ / __|
-   \   \  |    | (_) | (__ 
-    `.__|/      \__\_\\___|
-    """
-    )
-    parser = argparse.ArgumentParser()
+def str2bool(v):
+    if isinstance(v, bool):
+        return v
+    if v.lower() in ("yes", "true", "t", "y", "1"):
+        return True
+    elif v.lower() in ("no", "false", "f", "n", "0"):
+        return False
+    else:
+        raise argparse.ArgumentTypeError("Boolean value expected.")
+
+
+def parse_args(parser=None):
+    if parser is None:
+        parser = argparse.ArgumentParser()
     parser.add_argument(
         "bdata_path", help="Path to the ReporterScreen object to run QC on", type=str
     )
+    thres_parser = parser.add_argument_group("QC thresholds")
+    run_parser = parser.add_argument_group("Run options")
+    input_parser = parser.add_argument_group("Input .h5ad formatting")
+
+    thres_parser.add_argument(
+        "--count-correlation-thres",
+        help="Correlation threshold to mask out.",
+        type=float,
+        default=0.7,
+    )
+    thres_parser.add_argument(
+        "--edit-rate-thres",
+        help="Mean editing rate threshold per sample to mask out.",
+        type=float,
+        default=0.1,
+    )
+    thres_parser.add_argument(
+        "--lfc-thres",
+        help="Positive guides' correlation threshold to filter out.",
+        type=float,
+        default=-0.1,
+    )
+
     parser.add_argument(
         "-o",
         "--out-screen-path",
         help="Path where quality-filtered ReporterScreen object to be written to",
         type=str,
     )
     parser.add_argument(
+        "-r",
+        "--out-report-prefix",
+        help="Output prefix of qc report (prefix.html, prefix.ipynb)",
+        type=str,
+    )
+
+    run_parser.add_argument(
+        "-b",
+        "--remove-bad-replicates",
+        help="Remove replicates with at least two of its samples meet the QC threshold.",
+        action="store_true",
+    )
+    run_parser.add_argument(
         "-i",
         "--ignore-missing-samples",
         help="If the flag is not provided, if the ReporterScreen object does not contain all condiitons for each replicate, make fake empty samples. If the flag is provided, don't add dummy samples.",
         action="store_true",
     )
-    parser.add_argument(
-        "-r",
-        "--out-report-prefix",
-        help="Output prefix of qc report (prefix.html, prefix.ipynb)",
-        type=str,
+    run_parser.add_argument(
+        "--no-editing",
+        help="Ignore QC about editing. Can be used for QC of other editing modalities.",
+        action="store_true",
     )
-    parser.add_argument(
+    run_parser.add_argument(
+        "--dont-recalculate-edits",
+        help="When ReporterScreen.layers['edit_count'] exists, do not recalculate the edit counts from ReporterScreen.uns['allele_count'].",
+        action="store_true",
+    )
+
+    input_parser.add_argument(
+        "--tiling",
+        dest="tiling",
+        type=str2bool,
+        help="Specify that the guide library is tiling library without 'n guides per target' design",
+    )
+    input_parser.add_argument(
         "--replicate-label",
         help="Label of column in `bdata.samples` that describes replicate ID.",
         type=str,
-        default="rep",
+        default="replicate",
     )
-    parser.add_argument(
+    input_parser.add_argument(
+        "--sample-covariates",
+        help="Comma-separated list of column names in `bdata.samples` that describes non-selective experimental condition. (drug treatment, etc.)",
+        type=str,
+        default=None,
+    )
+    input_parser.add_argument(
         "--condition-label",
         help="Label of column in `bdata.samples` that describes experimental condition. (sorting bin, time, etc.)",
         type=str,
-        default="bin",
+        default="condition",
     )
-    parser.add_argument(
+    input_parser.add_argument(
         "--target-pos-col",
         help="Target position column in `bdata.guides` specifying target edit position in reporter",
         type=str,
         default="target_pos",
     )
-    parser.add_argument(
+    input_parser.add_argument(
         "--rel-pos-is-reporter",
         help="Specifies whether `edit_start_pos` and `edit_end_pos` are relative to reporter position. If `False`, those are relative to spacer position.",
         action="store_true",
         default=False,
     )
-    parser.add_argument(
+    input_parser.add_argument(
         "--edit-start-pos",
         help="Edit start position to quantify editing rate on, 0-based inclusive.",
         default=2,
     )
-    parser.add_argument(
+    input_parser.add_argument(
         "--edit-end-pos",
         help="Edit end position to quantify editing rate on, 0-based exclusive.",
         default=7,
     )
-    parser.add_argument(
-        "--count-correlation-thres",
-        help="Correlation threshold to mask out.",
-        type=float,
-        default=0.8,
-    )
-    parser.add_argument(
-        "--edit-rate-thres",
-        help="Median editing rate threshold per sample to mask out.",
-        type=float,
-        default=0.1,
-    )
-    parser.add_argument(
+
+    input_parser.add_argument(
         "--posctrl-col",
-        help="Column name in ReporterScreen.guides DataFrame that specifies guide category.",
+        help="Column name in ReporterScreen.guides DataFrame that specifies guide category. To use all gRNAs, feed empty string ''.",
         type=str,
         default="target_group",
     )
-    parser.add_argument(
+    input_parser.add_argument(
         "--posctrl-val",
         help="Value in ReporterScreen.guides[`posctrl_col`] that specifies guide will be used as the positive control in calculating log fold change.",
         type=str,
         default="PosCtrl",
     )
-    parser.add_argument(
-        "--lfc-thres",
-        help="Positive guides' correlation threshold to filter out.",
-        type=float,
-        default=-0.1,
-    )
-    parser.add_argument(
+
+    input_parser.add_argument(
         "--lfc-conds",
         help="Values in of column in `ReporterScreen.samples[condition_label]` for LFC will be calculated between, delimited by comma",
         type=str,
         default="top,bot",
     )
-    parser.add_argument(
-        "--recalculate-edits",
-        help="Even when ReporterScreen.layers['edit_count'] exists, recalculate the edit counts from ReporterScreen.uns['allele_count'].",
-        action="store_true",
+    input_parser.add_argument(
+        "--control-condition",
+        help="Values in of column in `ReporterScreen.samples[condition_label]` for guide-level editing rate to be calculated",
+        type=str,
+        default="bulk",
     )
-    args = parser.parse_args()
-    if args.out_screen_path is None:
-        args.out_screen_path = f"{args.bdata_path.rsplit('.h5ad', 1)[0]}.filtered.h5ad"
-    if args.out_report_prefix is None:
-        args.out_report_prefix = f"{args.bdata_path.rsplit('.h5ad', 1)[0]}.qc_report"
-    return args
-
-
-def check_args(args):
-    lfc_conds = args.lfc_conds.split(",")
-    if not len(lfc_conds) == 2:
-        raise ValueError(
-            f"lfc_conds must be two condition labels delimited by comma. Provided {args.lfc_conds}"
-        )
-    args.lfc_cond1 = lfc_conds[0]
-    args.lfc_cond2 = lfc_conds[1]
-    return args
-
-
-def _add_dummy_sample(bdata, rep, cond, condition_label: str, replicate_label: str):
-    sample_id = f"{rep}_{cond}"
-    cond_df = deepcopy(bdata.samples)
-    cond_df[replicate_label] = np.nan
-    cond_df = cond_df.drop_duplicates()
-    cond_row = cond_df.loc[cond_df[condition_label] == cond, :]
-    if not len(cond_row) == 1:
-        raise ValueError(
-            f"Non-unique condition specification in ReporterScreen.samples: {cond_row}"
-        )
-    cond_row.index = [sample_id]
-    cond_row.loc[:, replicate_label] = rep
-    dummy_sample_bdata = ReporterScreen(
-        X=np.zeros((bdata.n_obs, 1)),
-        X_bcmatch=np.zeros((bdata.n_obs, 1)),
-        guides=bdata.guides,
-        samples=cond_row,
-    )
-    for k in bdata.uns.keys():
-        if isinstance(bdata.uns[k], pd.DataFrame):
-            dummy_sample_bdata.uns[k] = pd.DataFrame(
-                columns=bdata.uns[k].columns.tolist()[:2] + [sample_id]
-            )
-        else:
-            dummy_sample_bdata.uns[k] = bdata.uns[k]
-    bdata = concat([bdata, dummy_sample_bdata])
-    return bdata
-
-
-def fill_in_missing_samples(bdata, condition_label: str, replicate_label: str):
-    """If not all condition exists for every replicate in bdata, fill in fake sample"""
-    added_dummy = False
-    for rep in bdata.samples[replicate_label].unique():
-        for cond in bdata.samples[condition_label].unique():
-            if (
-                len(
-                    np.where(
-                        (bdata.samples[replicate_label] == rep)
-                        & (bdata.samples[condition_label] == cond)
-                    )[0]
-                )
-                != 1
-            ):
-                bdata = _add_dummy_sample(
-                    bdata, rep, cond, condition_label, replicate_label
-                )
-                if not added_dummy:
-                    added_dummy = True
-    if added_dummy:
-        bdata = bdata[
-            :, bdata.samples.sort_values([replicate_label, condition_label]).index
-        ]
-    return bdata
+
+    return parser
```

### Comparing `crispr-bean-0.2.7/bin/bean-count` & `crispr-bean-1.0.0/bean/cli/count.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,90 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Count guides, optionally with reporter and alleles of a single sequencing sample."""
-
-import logging
-import os
-import sys
-
-import bean
-from bean.mapping.utils import (
-    _check_arguments,
-    _get_input_parser,
-    _check_file,
-    _get_first_read_length,
-    _check_read_length,
-)
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(levelname)-5s @ %(asctime)s:\n\t %(message)s \n",
-    datefmt="%a, %d %b %Y %H:%M:%S",
-    stream=sys.stderr,
-    filemode="w",
-)
-error = logging.critical
-warn = logging.warning
-debug = logging.debug
-info = logging.info
-
-
-_ROOT = os.path.abspath(os.path.dirname(__file__))
-
-
-def get_input_parser():
-    """Get single-sample specific argument parser."""
-    parser = _get_input_parser()
-    parser.add_argument(
-        "--R1",
-        type=str,
-        help="fastq file for read 1",
-        required=True,
-        default="Fastq filename",
-    )
-    parser.add_argument(
-        "--R2",
-        type=str,
-        help="fastq file for read 2, sorted as the same name order as in --R1 file.",
-        required=True,
-        default="Fastq filename",
-    )
-    return parser
-
-
-def check_arguments(args, info_logger, warn_logger, error_logger):
-    args = _check_arguments(
-        args, info_logger=info, warn_logger=warn, error_logger=error
-    )
-    _check_file(args.R1)
-    _check_file(args.R2)
-    read_length = _get_first_read_length(args.R1)
-    _check_read_length(args, read_length, warn)
-    return args
-
-
-def main():
-    parser = get_input_parser()
-    args = parser.parse_args()
-
-    args = check_arguments(args, info_logger=info, warn_logger=warn, error_logger=error)
-    args_dict = vars(args)
-
-    edited_from = args_dict["edited_base"]
-    match_target_pos = args_dict["match_target_pos"]
-
-    counter = bean.mp.GuideEditCounter(**args_dict)
-    counter.check_filter_fastq()
-
-    counter.get_counts()
-    if counter.count_reporter_edits:
-        counter.screen.uns["allele_counts"] = counter.screen.uns["allele_counts"].loc[
-            counter.screen.uns["allele_counts"].allele.map(str) != "", :
-        ]
-        if match_target_pos:
-            base_editing_map = {"A": "G", "C": "T"}
-            edited_to = base_editing_map[edited_from]
-            counter.screen.get_edit_mat_from_uns(
-                edited_from, edited_to, match_target_pos
-            )
-    counter.screen.write(f"{counter.output_dir}.h5ad")
-    counter.screen.to_Excel(f"{counter.output_dir}.xlsx")
-    info(f"Output written at:\n {counter.output_dir}.h5ad,\n {counter.output_dir}.xlsx")
-    info("All Done!")
-    print(
-        r"""
-    _ _       
-  /  \ '\                       _   
-  |   \  \      __ ___ _  _ _ _| |_ 
-   \   \  |    / _/ _ \ || | ' \  _|
-    `.__|/     \__\___/\_,_|_||_\__|
-    """
-    )
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""Count guides, optionally with reporter and alleles of a single sequencing sample."""
+
+import logging
+import os
+import sys
+
+import bean
+from bean.mapping.utils import (
+    _check_arguments,
+    _check_file,
+    _get_first_read_length,
+    _check_read_length,
+)
+
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(levelname)-5s @ %(asctime)s:\n\t %(message)s \n",
+    datefmt="%a, %d %b %Y %H:%M:%S",
+    stream=sys.stderr,
+    filemode="w",
+)
+error = logging.critical
+warn = logging.warning
+debug = logging.debug
+info = logging.info
+
+
+_ROOT = os.path.abspath(os.path.dirname(__file__))
+
+
+
+
+
+def check_arguments(args, info_logger, warn_logger, error_logger):
+    args = _check_arguments(
+        args, info_logger=info, warn_logger=warn, error_logger=error
+    )
+    _check_file(args.R1)
+    _check_file(args.R2)
+    read_length = _get_first_read_length(args.R1)
+    _check_read_length(args, read_length, warn)
+    return args
+
+
+def main(args):
+    """Get the input data"""
+    print(
+        r"""
+    _ _       
+  /  \ '\                       _   
+  |   \  \      __ ___ _  _ _ _| |_ 
+   \   \  |    / _/ _ \ || | ' \  _|
+    `.__|/     \__\___/\_,_|_||_\__|
+    """
+    )
+    args = check_arguments(args, info_logger=info, warn_logger=warn, error_logger=error)
+    args_dict = vars(args)
+
+    edited_from = args_dict["edited_base"]
+    match_target_pos = args_dict["match_target_pos"]
+
+    counter = bean.mp.GuideEditCounter(**args_dict)
+    counter.check_filter_fastq()
+
+    counter.get_counts()
+    if counter.count_reporter_edits:
+        counter.screen.uns["allele_counts"] = counter.screen.uns["allele_counts"].loc[
+            counter.screen.uns["allele_counts"].allele.map(str) != "", :
+        ]
+        if match_target_pos:
+            base_editing_map = {"A": "G", "C": "T"}
+            edited_to = base_editing_map[edited_from]
+            counter.screen.get_edit_mat_from_uns(
+                edited_from, edited_to, match_target_pos
+            )
+    counter.screen.write(f"{counter.output_dir}.h5ad")
+    counter.screen.to_Excel(f"{counter.output_dir}.xlsx")
+    info(f"Output written at:\n {counter.output_dir}.h5ad,\n {counter.output_dir}.xlsx")
+    info("All Done!")
+    print(
+        r"""
+    _ _       
+  /  \ '\                       _   
+  |   \  \      __ ___ _  _ _ _| |_ 
+   \   \  |    / _/ _ \ || | ' \  _|
+    `.__|/     \__\___/\_,_|_||_\__|
+    """
+    )
```

### Comparing `crispr-bean-0.2.7/bin/bean-count-samples` & `crispr-bean-1.0.0/bean/cli/count_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from multiprocessing import Pool
 
 import bean
 import pandas as pd
 from bean.mapping.utils import (
     InputFileError,
     _check_arguments,
-    _get_input_parser,
     _get_first_read_length,
     _check_read_length,
 )
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)-5s @ %(asctime)s:\n\t %(message)s \n",
@@ -28,49 +27,14 @@
 )
 error = logging.critical
 warn = logging.warning
 debug = logging.debug
 info = logging.info
 
 
-def get_input_parser() -> argparse.Namespace:
-    """Add multi-sample specific arguments to the base parser."""
-    parser = _get_input_parser()
-    parser.add_argument(
-        "-i",
-        "--input",
-        type=str,
-        help="List of fastq and sample ids. Formatted as `R1_filepath,R2_filepath,sample_id`",
-        required=True,
-    )
-    parser.add_argument(
-        "-t", "--threads", type=int, help="Number of threads", default=10
-    )
-    parser.add_argument(
-        "--guide-start-seqs-file",
-        type=str,
-        help="CSV file path with per-sample `guide_start_seq` to be used."
-        + "Formatted as `sample_id, guide_start_seq`",
-        default=None,
-    )
-    parser.add_argument(
-        "--guide-end-seqs-file",
-        type=str,
-        help="CSV file path with per-sample `guide_end_seq` to be used."
-        + "Formatted as `sample_id,guide_end_seq`",
-        default=None,
-    )
-
-    parser.add_argument(
-        "--rerun", help="Recount each sample", action="store_true", default=False
-    )
-
-    return parser
-
-
 def count_sample(R1: str, R2: str, sample_id: str, args: argparse.Namespace):
     """Count single sample given R1 and R2 paths.
     Arguments are modified accordingly to the provided sample_id before being passed to GuideEditCounter.
     """
     args_dict = deepcopy(vars(args))
     args_dict["R1"] = R1
     args_dict["R2"] = R2
@@ -87,14 +51,21 @@
     ):
         args_dict["guide_start_seq"] = str(args_dict["guide_start_seqs_tbl"][sample_id])
     if (
         "guide_end_seqs_tbl" in args_dict
         and args_dict["guide_end_seqs_tbl"] is not None
     ):
         args_dict["guide_end_seq"] = args_dict["guide_end_seqs_tbl"][sample_id]
+    if (
+        "barcode_start_seqs_tbl" in args_dict
+        and args_dict["barcode_start_seqs_tbl"] is not None
+    ):
+        args_dict["barcode_start_seq"] = str(
+            args_dict["barcode_start_seqs_tbl"][sample_id]
+        )
     counter = bean.mp.GuideEditCounter(**args_dict)
     if os.path.exists(f"{counter.output_dir}.h5ad") and not args_dict["rerun"]:
         screen = bean.read_h5ad(f"{counter.output_dir}.h5ad")
         if counter.count_reporter_edits and match_target_pos:
             screen.uns["allele_counts"] = screen.uns["allele_counts"].loc[
                 screen.uns["allele_counts"].allele.map(str) != "", :
             ]
@@ -124,76 +95,88 @@
             ]
             screen.get_edit_from_allele("allele_counts", "allele")
             screen.get_edit_mat_from_uns(edited_from, edited_to, match_target_pos)
         info(
             f"Done for {sample_id}. \n\
             Output written at {counter.output_dir}.h5ad"
         )
-
+    del counter
     return screen
 
 
 def check_arguments(args: argparse.Namespace) -> argparse.Namespace:
     """Checks the validity of the argument."""
     args = _check_arguments(args, info, warn, error)
-    sample_tbl = pd.read_csv(args.input)
+    sample_tbl = pd.read_csv(args.sample_list)
     if len(sample_tbl.iloc[:, 2].unique()) != len(sample_tbl.iloc[:, 2]):
         raise InputFileError(
-            f"Sample ID not unique. Please check your input file {args.input}."
+            f"Sample ID not unique. Please check your input file {args.sample_list}."
         )
     first_read_lengths = [
         _get_first_read_length(fastq_R1) for fastq_R1 in sample_tbl.iloc[:, 0]
     ]
     for read_length in first_read_lengths:
         _check_read_length(args, read_length, warn)
 
-    def _check_return_guide_seqs_tbl(guide_seqs_file, sample_tbl):
+    def _check_return_guide_seqs_tbl(guide_seqs_file, sample_tbl, label):
         """Check if the provided `guide_[start,end]_seqs_file` contains information about all samples in `sample_tbl`."""
         guide_seqs_tbl = pd.read_csv(guide_seqs_file, header=None, dtype=str).fillna("")
         if len(guide_seqs_tbl.columns) == 1:
             info("No guide start seq provided. Ignoring the file.")
             return None
         sample_has_seq = sample_tbl.iloc[:, 2].isin(guide_seqs_tbl[0])
         if not sample_has_seq.all():
             raise InputFileError(
-                f"Sample ID(s) {sample_tbl.iloc[:,2][~sample_has_seq]} not in guides_seqs_file {guide_seqs_tbl}"
+                f"Sample ID(s) {sample_tbl.iloc[:,2][~sample_has_seq]} not in {label}_seqs_file {guide_seqs_tbl}"
             )
         guide_seqs_tbl.columns = ["sample", "seq"]
         return guide_seqs_tbl.set_index("sample")["seq"]
 
     if args.guide_start_seqs_file is not None:
         args.guide_start_seqs_tbl = _check_return_guide_seqs_tbl(
-            args.guide_start_seqs_file, sample_tbl
+            args.guide_start_seqs_file, sample_tbl, "guide_start"
         )
     if args.guide_end_seqs_file is not None:
         args.guide_end_seqs_tbl = _check_return_guide_seqs_tbl(
-            args.guide_end_seqs_file, sample_tbl
+            args.guide_end_seqs_file, sample_tbl, "guide_end"
+        )
+    if args.barcode_start_seqs_file is not None:
+        args.barcode_start_seqs_tbl = _check_return_guide_seqs_tbl(
+            args.barcode_start_seqs_file, sample_tbl, "barcode_start"
         )
     return args
 
 
-def main():
-    parser = get_input_parser()
-    args = parser.parse_args()
+def main(args):
+    """Get the input data"""
+    print(
+        r"""
+    _ _       
+  /  \ '\                       _   
+  |   \  \      __ ___ _  _ _ _| |_ 
+   \   \  |    / _/ _ \ || | ' \  _|
+    `.__|/     \__\___/\_,_|_||_\__|
+    """
+    )
     args = check_arguments(args)
-    sample_tbl = pd.read_csv(args.input)  # R1_filepath, R2_filepath, sample_name
+    sample_tbl = pd.read_csv(args.sample_list)  # R1_filepath, R2_filepath, sample_name
     sample_tbl_input = sample_tbl.iloc[:, :3]
     sample_info_tbl = sample_tbl.iloc[:, 2:].set_index(sample_tbl.columns[2])
-    with Pool(processes=args.threads) as p:
+    with Pool(processes=args.threads, maxtasksperchild=1) as p:
         result = p.starmap(
             count_sample,
             [
                 list(tup) + [args]
                 for tup in list(sample_tbl_input.to_records(index=False))
             ],
         )
         # result = p.starmap(count_sample, sample_tbl[0], sample_tbl[1], sample_tbl[2])
 
     screen = bean.concat(result, axis=1)
-    database_id = args.name or os.path.basename(args.input).split(".")[0]
+    database_id = args.name or os.path.basename(args.sample_list).split(".")[0]
     output_path = os.path.join(
         os.path.abspath(args.output_folder), f"bean_count_{database_id}"
     )
     if not os.path.exists(args.output_folder):
         os.makedirs(args.output_folder)
     try:
         screen.samples = screen.samples.join(sample_info_tbl, how="left")
@@ -210,11 +193,7 @@
     _ _       
   /  \ '\                       _   
   |   \  \      __ ___ _  _ _ _| |_ 
    \   \  |    / _/ _ \ || | ' \  _|
     `.__|/     \__\___/\_,_|_||_\__|
     """
     )
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `crispr-bean-0.2.7/bin/bean-filter` & `crispr-bean-1.0.0/bean/cli/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import os
 import sys
-import argparse
+
 import logging
 import pandas as pd
 import bean as be
-from bean.plotting.allele_stats import plot_n_alleles_per_guide, plot_n_guides_per_edit
+import bean.annotate.filter_alleles as filter_alleles
+from bean.plotting.allele_stats import (
+    plot_allele_stats,
+)
+from bean.annotate.translate_allele import get_mismatch_df
+from bean.annotate.utils import check_args
 import matplotlib.pyplot as plt
 
 plt.style.use("default")
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)-5s @ %(asctime)s:\n\t %(message)s \n",
     datefmt="%a, %d %b %Y %H:%M:%S",
@@ -19,215 +23,77 @@
 )
 error = logging.critical
 warn = logging.warning
 debug = logging.debug
 info = logging.info
 
 
-def parse_args():
+def main(args):
     """Get the input arguments"""
     print(
         r"""
     _ _         
   /  \ '\       __ _ _ _           
   |   \  \     / _(_) | |_ ___ _ _ 
    \   \  |   |  _| | |  _/ -_) '_|
     `.__|/    |_| |_|_|\__\___|_|  
     """
     )
     print("bean-filter: filter alleles")
-    parser = argparse.ArgumentParser(
-        prog="allele_filter",
-        description="Filter alleles based on edit position in spacer and frequency across samples.",
-    )
-    parser.add_argument(
-        "bdata_path",
-        type=str,
-        help="Input ReporterScreen file of which allele will be filtered out.",
-    )
-    parser.add_argument(
-        "--output-prefix",
-        "-o",
-        type=str,
-        default=None,
-        help="Output prefix for log and ReporterScreen file with allele assignment",
-    )
-    parser.add_argument(
-        "--plasmid-path",
-        "-p",
-        type=str,
-        default=None,
-        help="Plasmid ReporterScreen object path. If provided, alleles are filtered based on if a nucleotide edit is more significantly enriched in sample compared to the plasmid data. Negative control data where no edit is expected can be fed in instead of plasmid library.",
-    )
-    parser.add_argument(
-        "--edit-start-pos",
-        "-s",
-        type=int,
-        default=2,
-        help="0-based start posiiton (inclusive) of edit relative to the start of guide spacer.",
-    )
-    parser.add_argument(
-        "--edit-end-pos",
-        "-e",
-        type=int,
-        default=7,
-        help="0-based end position (exclusive) of edit relative to the start of guide spacer.",
-    )
-    parser.add_argument(
-        "--jaccard-threshold",
-        "-j",
-        type=float,
-        help="Jaccard Index threshold when the alleles are mapped to the most similar alleles. In each filtering step, allele counts of filtered out alleles will be mapped to the most similar allele only if they have Jaccard Index of shared edit higher than this threshold.",
-        default=0.3,
-    )
-    parser.add_argument(
-        "--filter-window",
-        "-w",
-        help="Only consider edit within window provided by (edit-start-pos, edit-end-pos). If this flag is not provided, `--edit-start-pos` and `--edit-end-pos` flags are ignored.",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--filter-target-basechange",
-        "-b",
-        help="Only consider target edit (stored in bdata.uns['target_base_change'])",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--translate", "-t", help="Translate alleles", action="store_true"
-    )
-    parser.add_argument(
-        "--translate-fasta",
-        "-f",
-        type=str,
-        help="fasta file path with exon positions. If not provided, LDLR hg19 coordinates will be used.",
-        default=None,
-    )
-    parser.add_argument(
-        "--translate-fastas-csv",
-        "-fs",
-        type=str,
-        help=".csv with two columns with gene IDs and FASTA file path corresponding to each gene.",
-        default=None,
-    )
-    parser.add_argument(
-        "--filter-allele-proportion",
-        "-ap",
-        type=float,
-        default=0.05,
-        help="If provided, alleles that exceed `filter_allele_proportion` in `filter-sample-proportion` will be retained.",
-    )
-    parser.add_argument(
-        "--filter-allele-count",
-        "-ac",
-        type=int,
-        default=5,
-        help="If provided, alleles that exceed `filter_allele_proportion` AND `filter_allele_count` in `filter-sample-proportion` will be retained.",
-    )
-    parser.add_argument(
-        "--filter-sample-proportion",
-        "-sp",
-        type=float,
-        default=0.2,
-        help="If `filter_allele_proportion` is provided, alleles that exceed `filter_allele_proportion` in `filter-sample-proportion` will be retained.",
-    )
-    return parser.parse_args()
-
-
-def check_args(args):
-    if args.output_prefix is None:
-        args.output_prefix = args.bdata_path.rsplit(".h5ad", 1)[0] + "_alleleFiltered"
-    info(f"Saving results to {args.output_prefix}")
-    if args.filter_window:
-        if args.edit_start_pos is None and args.edit_end_pos is None:
-            raise ValueError(
-                "Invalid arguments: --filter-window option set but none of --edit-start-pos and --edit-end-pos specified."
+    args = check_args(args)
+    if not args.load_tmp:
+        bdata = be.read_h5ad(args.bdata_path)
+        allele_df_keys = ["allele_counts"]
+        info(
+            f"Starting from .uns['allele_counts'] with {len(bdata.uns['allele_counts'])} alleles."
+        )
+        if args.plasmid_path is not None:
+            info(
+                "Filtering significantly more edited nucleotide per guide compared to plasmid library..."
             )
-        if args.edit_start_pos is None:
-            warn(
-                "--filter-window option set but none of --edit-start-pos not provided. Using 0 as its value."
+            plasmid_adata = be.read_h5ad(args.plasmid_path)
+            plasmid_adata.uns[allele_df_keys[-1]] = plasmid_adata.uns[
+                allele_df_keys[-1]
+            ].loc[plasmid_adata.uns[allele_df_keys[-1]].allele.map(str) != "", :]
+
+            (
+                q_val_each,
+                sig_allele_df,
+            ) = filter_alleles.filter_alleles(
+                bdata, plasmid_adata, filter_each_sample=True, run_parallel=True
             )
-            args.edit_start_pos = 0
-        if args.edit_end_pos is None:
-            warn(
-                "--filter-window option set but none of --edit-end-pos not provided. Using 20 as its value."
+            bdata.uns["sig_allele_counts"] = sig_allele_df.reset_index(drop=True)
+            allele_df_keys.append("sig_allele_counts")
+            info(f"Filtered down to {len(bdata.uns['sig_allele_counts'])} alleles.")
+
+        print(len(bdata.uns[allele_df_keys[-1]]))
+        if len(bdata.uns[allele_df_keys[-1]]) >= 1:
+            info("Filtering out edits outside spacer position...")
+            bdata.uns[f"{allele_df_keys[-1]}_spacer"] = (
+                bdata.filter_allele_counts_by_pos(
+                    rel_pos_start=0,
+                    rel_pos_end=20,
+                    rel_pos_is_reporter=False,
+                    map_to_filtered=True,
+                    allele_uns_key=allele_df_keys[-1],
+                    jaccard_threshold=0.2,
+                ).reset_index(drop=True)
             )
-            args.edit_end_pos = 20
-    if args.filter_allele_proportion is not None and (
-        args.filter_allele_proportion < 0 or args.filter_allele_proportion > 1
-    ):
-        raise ValueError(
-            "Invalid arguments: filter-allele-proportion should be in range [0, 1]."
-        )
-    if args.filter_sample_proportion < 0 or args.filter_sample_proportion > 1:
-        raise ValueError(
-            "Invalid arguments: filter-sample-proportion should be in range [0, 1]."
-        )
-    if args.translate_fasta and args.translate_fastas_csv:
-        raise ValueError(
-            "Invalid arguments: You can only specify one of --translate-fasta (single gene) or --translate-fastas-csv (multiple genes)."
-        )
-    if args.translate_fastas_csv:
-        tbl = pd.read_csv(
-            args.translate_fastas_csv,
-            header=None,
-        )
-        if len(tbl) == 0 or len(tbl.columns != 2):
-            raise ValueError(
-                "Invalid arguments: Table should have two columns and more than 0 entry"
+            info(
+                f"Filtered down to {len(bdata.uns[f'{allele_df_keys[-1]}_spacer'])} alleles."
             )
-        for path in tbl.iloc[:, 2].tolist():
-            if not os.path.isfile(path):
-                raise FileNotFoundError(
-                    f"Invalid input file: {path} does not exist. Check your input in {args.translate_fastas_csv}"
-                )
-
-
-if __name__ == "__main__":
-    args = parse_args()
-    check_args(args)
-    bdata = be.read_h5ad(args.bdata_path)
-    allele_df_keys = ["allele_counts"]
-    info(
-        f"Starting from .uns['allele_counts'] with {len(bdata.uns['allele_counts'])} alleles."
-    )
-
-    if args.plasmid_path is not None:
-        info(
-            "Filtering significantly more edited nucleotide per guide compared to plasmid library..."
-        )
-        plasmid_adata = be.read_h5ad(args.plasmid_path)
-        plasmid_adata.uns[allele_df_keys[-1]] = plasmid_adata.uns[
-            allele_df_keys[-1]
-        ].loc[plasmid_adata.uns[allele_df_keys[-1]].allele.map(str) != "", :]
-
-        (
-            q_val_each,
-            sig_allele_df,
-        ) = be.an.filter_alleles.filter_alleles(
-            bdata, plasmid_adata, filter_each_sample=True, run_parallel=True
-        )
-        bdata.uns["sig_allele_counts"] = sig_allele_df.reset_index(drop=True)
-        allele_df_keys.append("sig_allele_counts")
-        info(f"Filtered down to {len(bdata.uns['sig_allele_counts'])} alleles.")
-
-    print(len(bdata.uns[allele_df_keys[-1]]))
-    if len(bdata.uns[allele_df_keys[-1]]) >= 1:
-        info("Filtering out edits outside spacer position...")
-        bdata.uns[f"{allele_df_keys[-1]}_spacer"] = bdata.filter_allele_counts_by_pos(
-            rel_pos_start=0,
-            rel_pos_end=20,
-            rel_pos_is_reporter=False,
-            map_to_filtered=True,
-            allele_uns_key=allele_df_keys[-1],
-            jaccard_threshold=0.2,
-        ).reset_index(drop=True)
-        info(
-            f"Filtered down to {len(bdata.uns[f'{allele_df_keys[-1]}_spacer'])} alleles."
-        )
-        allele_df_keys.append(f"{allele_df_keys[-1]}_spacer")
+            allele_df_keys.append(f"{allele_df_keys[-1]}_spacer")
+            bdata.write(f"{args.output_prefix}.tmp.h5ad")
+    else:
+        bdata = be.read_h5ad(f"{args.output_prefix}.tmp.h5ad")
+        allele_df_keys = ["allele_counts"]
+        if "sig_allele_counts" in bdata.uns.keys():
+            allele_df_keys += ["sig_allele_counts"]
+        if f"{allele_df_keys[-1]}_spacer" in bdata.uns.keys():
+            allele_df_keys += [f"{allele_df_keys[-1]}_spacer"]
 
     if len(bdata.uns[allele_df_keys[-1]]) > 0 and args.filter_window:
         info(
             f"Filtering out edits based on relatvie position in spacer: 0-based [{args.edit_start_pos},{args.edit_end_pos})..."
         )
         filtered_key = f"{allele_df_keys[-1]}_{args.edit_start_pos}_{args.edit_end_pos}"
         bdata.uns[filtered_key] = bdata.filter_allele_counts_by_pos(
@@ -237,14 +103,26 @@
             map_to_filtered=True,
             allele_uns_key=allele_df_keys[-1],
             jaccard_threshold=args.jaccard_threshold,
         ).reset_index(drop=True)
         allele_df_keys.append(filtered_key)
         info(f"Filtered down to {len(bdata.uns[filtered_key])} alleles.")
 
+    if len(bdata.uns[allele_df_keys[-1]]) > 0 and not args.keep_indels:
+        filtered_key = f"{allele_df_keys[-1]}_noindels"
+        info(f"Filtering out indels...")
+        bdata.uns[filtered_key] = bdata.filter_allele_counts_by_base(
+            ["A", "T", "G", "C"],
+            ["A", "T", "G", "C"],
+            map_to_filtered=False,
+            allele_uns_key=allele_df_keys[-1],
+        ).reset_index(drop=True)
+        info(f"Filtered down to {len(bdata.uns[filtered_key])} alleles.")
+        allele_df_keys.append(filtered_key)
+
     if len(bdata.uns[allele_df_keys[-1]]) > 0 and args.filter_target_basechange:
         filtered_key = (
             f"{allele_df_keys[-1]}_{bdata.base_edited_from}.{bdata.base_edited_to}"
         )
         info(f"Filtering out non-{bdata.uns['target_base_change']} edits...")
         bdata.uns[filtered_key] = bdata.filter_allele_counts_by_base(
             bdata.base_edited_from,
@@ -266,18 +144,24 @@
             fasta_dict = None
         info(
             "Translating alleles..."
         )  # TODO: Check & document custom fasta file for translation
         filtered_key = f"{allele_df_keys[-1]}_translated"
         bdata.uns[filtered_key] = be.translate_allele_df(
             bdata.uns[allele_df_keys[-1]],
+            gene_name=args.translate_gene,
+            gene_names=args.translate_genes_list,
             fasta_file=args.translate_fasta,
             fasta_file_dict=fasta_dict,
         ).rename(columns={"allele": "aa_allele"})
+        get_mismatch_df().to_csv(f"{args.output_prefix}.translation_ref_mismatches.csv")
+
         allele_df_keys.append(filtered_key)
+        if not any(bdata.uns[filtered_key].aa_allele.map(lambda a: a.has_coding)):
+            warn("WARNING: No alleles have been translated. Check your gene input(s).")
         info(f"Filtered down to {len(bdata.uns[filtered_key])} alleles.")
 
     if (
         len(bdata.uns[allele_df_keys[-1]]) > 0
         and args.filter_allele_proportion is not None
     ):
         info(
@@ -299,20 +183,54 @@
         allele_df_keys.append(filtered_key)
         info(f"Filtered down to {len(bdata.uns[filtered_key])} alleles.")
         info("Done filtering!")
     info(f"Saving ReporterScreen with filtered alleles at {args.output_prefix}.h5ad...")
     bdata.write(f"{args.output_prefix}.h5ad")
 
     info("Plotting allele stats for each filtering step...")
-    fig, ax = plt.subplots(len(allele_df_keys), 2, figsize=(6, 3 * len(allele_df_keys)))
-    for i, key in enumerate(allele_df_keys):
-        if len(bdata.uns[key]) > 0:
-            plot_n_alleles_per_guide(bdata, key, bdata.uns[key].columns[1], ax[i, 0])
-            plot_n_guides_per_edit(bdata, key, bdata.uns[key].columns[1], ax[i, 1])
-    plt.tight_layout()
-    plt.savefig(f"{args.output_prefix}.filtered_allele_stats.pdf", bbox_inches="tight")
+    plot_allele_stats(
+        bdata, allele_df_keys, f"{args.output_prefix}.filtered_allele_stats.pdf"
+    )
     info(
         f"Saving plotting result and log at {args.output_prefix}.[filtered_allele_stats.pdf, filter_log.txt]."
     )
     with open(f"{args.output_prefix}.filter_log.txt", "w") as out_log:
+        out_log.write(
+            "filter_step\tn_alleles\tn_var\tn_noncoding_var\tn_coding_var\tn_synonymous_var\n"
+        )
         for key in allele_df_keys:
-            out_log.write(f"{key}\t{len(bdata.uns[key])}\n")
+            if "translate" in key:
+                n_coding_vars = len(
+                    set().union(
+                        *bdata.uns[key]
+                        .aa_allele.map(lambda a: list(a.aa_allele.edits))
+                        .tolist()
+                    )
+                )
+                n_syn_vars = len(
+                    set().union(
+                        *bdata.uns[key]
+                        .aa_allele.map(
+                            lambda a: {e for e in a.aa_allele.edits if e.ref == e.alt}
+                        )
+                        .tolist()
+                    )
+                )
+                n_noncoding_vars = len(
+                    set().union(
+                        *bdata.uns[key]
+                        .aa_allele.map(lambda a: list(a.nt_allele.edits))
+                        .tolist()
+                    )
+                )
+                out_log.write(
+                    f"{key}\t{len(bdata.uns[key])}\t{n_coding_vars + n_noncoding_vars}\t{n_noncoding_vars}\t{n_coding_vars}\t{n_syn_vars}\n"
+                )
+            else:
+                n_noncoding_vars = len(
+                    set().union(
+                        *bdata.uns[key].allele.map(lambda a: list(a.edits)).tolist()
+                    )
+                )
+                out_log.write(
+                    f"{key}\t{len(bdata.uns[key])}\t{n_noncoding_vars}\t{n_noncoding_vars}\t{0}\t{0}\n"
+                )
```

### Comparing `crispr-bean-0.2.7/bin/bean-qc` & `crispr-bean-1.0.0/bean/cli/qc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-#!/usr/bin/env python
-import os
-import papermill as pm
-import bean as be
-from bean.qc.utils import parse_args, check_args
-
-
-def main():
-    args = parse_args()
-    args = check_args(args)
-    os.system(
-        "python -m ipykernel install --user --name bean_python3 --display-name bean_python3"
-    )
-    pm.execute_notebook(
-        f"{os.path.dirname(be.__file__)}/../notebooks/sample_quality_report.ipynb",
-        f"{args.out_report_prefix}.ipynb",
-        parameters=dict(
-            bdata_path=args.bdata_path,
-            out_bdata_path=args.out_screen_path,
-            edit_quantification_start_pos=args.edit_start_pos,
-            edit_quantification_end_pos=args.edit_end_pos,
-            target_pos_col=args.target_pos_col,
-            rel_pos_is_reporter=args.rel_pos_is_reporter,
-            corr_X_thres=args.count_correlation_thres,
-            edit_rate_thres=args.edit_rate_thres,
-            posctrl_col=args.posctrl_col,
-            posctrl_val=args.posctrl_val,
-            lfc_thres=args.lfc_thres,
-            replicate_label=args.replicate_label,
-            condition_label=args.condition_label,
-            comp_cond1=args.lfc_cond1,
-            comp_cond2=args.lfc_cond2,
-            exp_id=args.out_report_prefix,
-            recalculate_edits=args.recalculate_edits,
-        ),
-        kernel_name="bean_python3",
-    )
-    os.system(f"jupyter nbconvert --to html {args.out_report_prefix}.ipynb")
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+import os
+import papermill as pm
+import bean as be
+from bean.qc.utils import check_args
+
+
+def main(args):
+    print("  \n~~~BEANQC~~~")
+    print("-Check guide/sample level quality and mask / discard-")
+    print(
+        r"""
+    _ _       
+  /  \ '\        ___   ___ 
+  |   \  \      / _ \ / __|
+   \   \  |    | (_) | (__ 
+    `.__|/      \__\_\\___|
+    """
+    )
+    if args.out_screen_path is None:
+        args.out_screen_path = f"{args.bdata_path.rsplit('.h5ad', 1)[0]}.filtered.h5ad"
+    if args.out_report_prefix is None:
+        args.out_report_prefix = f"{args.bdata_path.rsplit('.h5ad', 1)[0]}.qc_report"
+    args = check_args(args)
+    os.system(
+        "python -m ipykernel install --user --name bean_python3 --display-name bean_python3"
+    )
+    pm.execute_notebook(
+        f"{os.path.dirname(be.__file__)}/../notebooks/sample_quality_report.ipynb",
+        f"{args.out_report_prefix}.ipynb",
+        parameters=dict(
+            bdata_path=args.bdata_path,
+            out_bdata_path=args.out_screen_path,
+            tiling=args.tiling,
+            edit_quantification_start_pos=args.edit_start_pos,
+            edit_quantification_end_pos=args.edit_end_pos,
+            target_pos_col=args.target_pos_col,
+            rel_pos_is_reporter=args.rel_pos_is_reporter,
+            corr_X_thres=args.count_correlation_thres,
+            edit_rate_thres=args.edit_rate_thres,
+            posctrl_col=args.posctrl_col,
+            posctrl_val=args.posctrl_val,
+            lfc_thres=args.lfc_thres,
+            replicate_label=args.replicate_label,
+            condition_label=args.condition_label,
+            comp_cond1=args.lfc_cond1,
+            comp_cond2=args.lfc_cond2,
+            ctrl_cond=args.control_condition,
+            exp_id=args.out_report_prefix,
+            recalculate_edits=~args.dont_recalculate_edits,
+            base_edit_data=args.base_edit_data,
+            remove_bad_replicates=args.remove_bad_replicates,
+        ),
+        kernel_name="bean_python3",
+    )
+    os.system(f"jupyter nbconvert --to html {args.out_report_prefix}.ipynb")
```

### Comparing `crispr-bean-0.2.7/bin/bean-run` & `crispr-bean-1.0.0/bean/model/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,215 @@
-#!/usr/bin/env python
 import os
 import sys
+
+from tqdm import tqdm
+import pickle as pkl
+import pandas as pd
 import logging
-from copy import deepcopy
 from functools import partial
-import numpy as np
-import pandas as pd
-
-import torch
 import pyro
-import pyro.infer
-import pyro.optim
-import pickle as pkl
+import bean.model.model as sorting_model
+import bean.model.survival_model as survival_model
 
-import bean.model.model as m
-from bean.model.readwrite import write_result_table
-from bean.preprocessing.data_class import (
-    VariantSortingScreenData,
-    VariantSortingReporterScreenData,
-    TilingSortingReporterScreenData,
-)
-from bean.preprocessing.utils import (
-    _obtain_effective_edit_rate,
-    _obtain_n_guides_alleles_per_variant,
-)
-
-import bean as be
-from bean.model.utils import (
-    run_inference,
-    _get_guide_target_info,
-    parse_args,
-    check_args,
-)
+# import bean.model.survival_model as survival_model
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(levelname)-5s @ %(asctime)s:\n\t %(message)s \n",
     datefmt="%a, %d %b %Y %H:%M:%S",
     stream=sys.stderr,
     filemode="w",
 )
 error = logging.critical
 warn = logging.warning
 debug = logging.debug
 info = logging.info
 pyro.set_rng_seed(101)
 
-DATACLASS_DICT = {
-    "Normal": VariantSortingReporterScreenData,
-    "MixtureNormal": VariantSortingReporterScreenData,
-    "_MixtureNormal+Acc": VariantSortingReporterScreenData,  # TODO: old
-    "MixtureNormal+Acc": VariantSortingReporterScreenData,
-    "MixtureNormalConstPi": VariantSortingScreenData,
-    "MultiMixtureNormal": TilingSortingReporterScreenData,
-    "MultiMixtureNormal+Acc": TilingSortingReporterScreenData,
-}
+
+def check_args(args, bdata):
+    args.adjust_confidence_by_negative_control = (
+        not args.dont_adjust_confidence_by_negative_control
+    )
+    if args.scale_by_acc:
+        if args.acc_col is None and args.acc_bw_path is None:
+            raise ValueError(
+                "--scale-by-acc not accompanied by --acc-col nor --acc-bw-path to use. Pass either one."
+            )
+        elif args.acc_col is not None and args.acc_bw_path is not None:
+            warn(
+                "Both --acc-col and --acc-bw-path is specified. --acc-bw-path is ignored."
+            )
+            args.acc_bw_path = None
+    if args.outdir is None:
+        args.outdir = os.path.dirname(args.bdata_path)
+    if args.library_design == "variant":
+        pass
+    elif args.library_design == "tiling":
+        if args.allele_df_key is None:
+            key_to_use = "allele_counts"
+            n_alleles = len(bdata.uns[key_to_use])
+            for key, df in bdata.uns.items():
+                if "allele_counts" not in key or not isinstance(df, pd.DataFrame):
+                    continue
+                if len(df) < n_alleles:
+                    key_to_use = key
+                    n_alleles = len(df)
+            warn(
+                f"--allele-df-key not provided for tiling screen. Using the most filtered allele counts with {n_alleles} alleles stored in {key_to_use}."
+            )
+            args.allele_df_key = key_to_use
+        elif args.allele_df_key not in bdata.uns:
+            raise ValueError(
+                f"--allele-df-key {args.allele_df_key} not in ReporterScreen.uns. Check your input."
+            )
+    else:
+        raise ValueError(
+            "Invalid library_design provided. Select either 'variant' or 'tiling'."
+        )  # TODO: change this into discrete modes via argparse
+    if args.fit_negctrl:
+        n_negctrl = (
+            bdata.guides[args.negctrl_col].map(lambda s: s.lower())
+            == args.negctrl_col_value.lower()
+        ).sum()
+        if not n_negctrl >= 10:
+            raise ValueError(
+                f"Not enough negative control guide in the input data: {n_negctrl}. Check your input arguments."
+            )
+    if args.repguide_mask is not None and args.repguide_mask not in bdata.uns.keys():
+        bdata.uns[args.repguide_mask] = pd.DataFrame(
+            index=bdata.guides.index, columns=bdata.samples[args.replicate_col].unique()
+        ).fillna(1)
+        warn(
+            f"{args.bdata_path} does not have replicate x guide outlier mask. All guides are included in analysis."
+        )
+    if args.sample_mask_col is not None:
+        if args.sample_mask_col not in bdata.samples.columns.tolist():
+            raise ValueError(
+                f"{args.bdata_path} does not have specified sample mask column {args.sample_mask_col} in .samples"
+            )
+    if args.condition_col not in bdata.samples.columns:
+        raise ValueError(
+            f"Condition column set by `--condition-col` {args.condition_col} not in ReporterScreen.samples.columns:{bdata.samples.columns}. Check your input."
+        )
+    if args.control_condition not in bdata.samples[args.condition_col].tolist():
+        raise ValueError(
+            f"No sample has control label (set by `--control-condition`) {args.control_condition} in ReporterScreen.samples[{args.condition_col}]: {bdata.samples[args.condition_col]}. Check your input."
+        )
+    if args.replicate_col not in bdata.samples.columns:
+        raise ValueError(
+            f"Condition column set by `--replicate-col` {args.replicate_col} not in ReporterScreen.samples.columns:{bdata.samples.columns}. Check your input."
+        )
+    if args.control_guide_tag is not None:
+        if args.library_design == "variant":
+            raise ValueError(
+                "`--control-guide-tag` is not used for the variant mode. Make sure you provide the separate `target` column for negative control guide that targets different negative control variant."
+            )
+        elif not bdata.guides.index.map(lambda s: args.control_guide_tag in s).any():
+            raise ValueError(
+                f"Negative control guide label {args.control_guide_tag} provided by `--control-guide-tag` doesn't appear in any of the guide names. Check your input."
+            )
+    if args.alpha_if_overdispersion_fitting_fails is not None:
+        try:
+            b0, b1 = args.alpha_if_overdispersion_fitting_fails.split(",")
+            args.popt = (float(b0), float(b1))
+        except TypeError as e:
+            raise ValueError(
+                f"Input --alpha-if-overdispersion-fitting-fails {args.alpha_if_overdispersion_fitting_fails} is malformatted! Provide [float].[float] format."
+            )
+    else:
+        args.popt = None
+    return args, bdata
+
+
+def _get_guide_target_info(bdata, args, cols_include=[]):
+    guide_info = bdata.guides.copy()
+    target_info = (
+        guide_info[
+            [args.target_col]
+            + [
+                col
+                for col in guide_info.columns
+                if (
+                    (
+                        (col.startswith("target_"))
+                        and len(guide_info[[args.target_col, col]].drop_duplicates())
+                        == len(guide_info[args.target_col].unique())
+                    )
+                    or col in cols_include
+                )
+                and col != args.target_col
+            ]
+        ]
+        .drop_duplicates()
+        .set_index(args.target_col, drop=True)
+    )
+    target_info["n_guides"] = guide_info.groupby("target").size()
+
+    if "edit_rate" in guide_info.columns.tolist():
+        edit_rate_info = (
+            guide_info[[args.target_col, "edit_rate"]]
+            .groupby(args.target_col, sort=False)
+            .agg({"edit_rate": ["mean", "std"]})
+        )
+        edit_rate_info.columns = edit_rate_info.columns.get_level_values(1)
+        edit_rate_info = edit_rate_info.rename(
+            columns={"mean": "edit_rate_mean", "std": "edit_rate_std"}
+        )
+        target_info = target_info.join(edit_rate_info)
+    return target_info
+
+
+def run_inference(
+    model, guide, data, initial_lr=0.01, gamma=0.1, num_steps=2000, autoguide=False
+):
+    pyro.clear_param_store()
+    lrd = gamma ** (1 / num_steps)
+    svi = pyro.infer.SVI(
+        model=model,
+        guide=guide,
+        optim=pyro.optim.ClippedAdam({"lr": initial_lr, "lrd": lrd}),
+        loss=pyro.infer.Trace_ELBO(),
+    )
+    losses = []
+    try:
+        for t in tqdm(range(num_steps)):
+            loss = svi.step(data)
+            if t % 100 == 0:
+                print(f"loss {loss} @ iter {t}")
+            losses.append(loss)
+    except ValueError as exc:
+        error(
+            "Error occurred during fitting. Saving temporary output at tmp_result.pkl."
+        )
+        with open("tmp_result.pkl", "wb") as handle:
+            pkl.dump({"param": pyro.get_param_store()}, handle)
+
+        raise ValueError(
+            f"Fitting halted for command: {' '.join(sys.argv)} with following error: \n {exc}"
+        )
+    return pyro.get_param_store(), {
+        "loss": losses,
+        "params": pyro.get_param_store().get_state(),
+    }
 
 
 def identify_model_guide(args):
-    if args.mode == "tiling":
+    if args.selection == "sorting":
+        m = sorting_model
+    else:
+        m = survival_model
+    if args.library_design == "tiling":
         info("Using Mixture Normal model...")
         return (
             f"MultiMixtureNormal{'+Acc' if args.scale_by_acc else ''}",
             partial(
                 m.MultiMixtureNormalModel,
                 scale_by_accessibility=args.scale_by_acc,
-                use_bcmatch=~args.ignore_bcmatch,
+                use_bcmatch=(not args.ignore_bcmatch,),
             ),
             partial(
                 m.MultiMixtureNormalGuide,
                 scale_by_accessibility=args.scale_by_acc,
                 fit_noise=~args.dont_fit_noise,
             ),
         )
@@ -77,166 +217,55 @@
         if args.guide_activity_col is not None:
             raise ValueError(
                 "Can't use the guide activity column while constraining uniform edit."
             )
         info("Using Normal model...")
         return (
             "Normal",
-            partial(m.NormalModel, use_bcmatch=~args.ignore_bcmatch),
+            partial(m.NormalModel, use_bcmatch=(not args.ignore_bcmatch)),
             m.NormalGuide,
         )
     elif args.const_pi:
         if args.guide_activity_col is not None:
             raise ValueError(
                 "--guide-activity-col to be used as constant pi is not provided."
             )
         info("Using Mixture Normal model with constant weight ...")
         return (
             "MixtureNormalConstPi",
-            partial(m.MixtureNormalConstPiModel, use_bcmatch=~args.ignore_bcmatch),
+            partial(m.MixtureNormalConstPiModel, use_bcmatch=(not args.ignore_bcmatch)),
             m.MixtureNormalGuide,
         )
     else:
         info(
             f"Using Mixture Normal model {'with accessibility normalization' if args.scale_by_acc else ''}..."
         )
         return (
             f"{'_' if args.dont_fit_noise else ''}MixtureNormal{'+Acc' if args.scale_by_acc else ''}",
             partial(
                 m.MixtureNormalModel,
                 scale_by_accessibility=args.scale_by_acc,
-                use_bcmatch=~args.ignore_bcmatch,
+                use_bcmatch=(not args.ignore_bcmatch,),
             ),
             partial(
                 m.MixtureNormalGuide,
                 scale_by_accessibility=args.scale_by_acc,
-                fit_noise=~args.dont_fit_noise,
+                fit_noise=(not args.dont_fit_noise),
             ),
         )
 
 
-def main(args, bdata):
-    if args.cuda:
-        os.environ["CUDA_VISIBLE_DEVICES"] = "1"
-        torch.set_default_tensor_type(torch.cuda.FloatTensor)
+def identify_negctrl_model_guide(args, data_has_bcmatch):
+    if args.selection == "sorting":
+        m = sorting_model
     else:
-        torch.set_default_tensor_type(torch.FloatTensor)
-    prefix = (
-        args.outdir
-        + "/bean_run_result."
-        + os.path.basename(args.bdata_path).rsplit(".", 1)[0]
-    )
-    os.makedirs(prefix, exist_ok=True)
-    model_label, model, guide = identify_model_guide(args)
-    guide_index = bdata.guides.index
-    info("Done loading data. Preprocessing...")
-    bdata.samples["rep"] = bdata.samples["rep"].astype("category")
-    bdata.guides = bdata.guides.loc[:, ~bdata.guides.columns.duplicated()].copy()
-    if args.mode == "variant":
-        if bdata.guides[args.target_col].isnull().any():
-            raise ValueError(
-                f"Some target column (bdata.guides[{args.target_col}]) value is null. Check your input file."
-            )
-        bdata = bdata[bdata.guides[args.target_col].argsort(), :]
-    ndata = DATACLASS_DICT[model_label](
-        screen=bdata,
-        device=args.device,
-        repguide_mask=args.repguide_mask,
-        sample_mask_column=args.sample_mask_col,
-        accessibility_col=args.acc_col,
-        accessibility_bw_path=args.acc_bw_path,
-        use_const_pi=args.const_pi,
-        condition_column=args.condition_col,
-        allele_df_key=args.allele_df_key,
-        control_guide_tag=args.control_guide_tag,
-        target_col=args.target_col,
-        shrink_alpha=args.shrink_alpha,
-        replicate_col=args.replicate_col,
+        m = survival_model
+    negctrl_model = partial(
+        m.ControlNormalModel,
+        use_bcmatch=(not args.ignore_bcmatch and data_has_bcmatch),
     )
-    print(ndata.a0)
-    adj_negctrl_idx = None
-    if args.mode == "variant":
-        if "edit_rate" not in bdata.guides.columns:
-            bdata.get_edit_from_allele()
-            bdata.get_edit_mat_from_uns(rel_pos_is_reporter=True)
-            bdata.get_guide_edit_rate()
-        target_info_df = _get_guide_target_info(
-            ndata.screen, args, cols_include=[args.negctrl_col]
-        )
-        print(target_info_df.columns)
-        if args.adjust_confidence_by_negative_control:
-            adj_negctrl_idx = np.where(
-                target_info_df[args.negctrl_col].map(lambda s: s.lower())
-                == args.negctrl_col_value.lower()
-            )[0]
-    else:
-        if args.splice_site_path is not None:
-            splice_site = pd.read_csv(args.splice_site_path).pos
-        target_info_df = be.an.translate_allele.annotate_edit(
-            pd.DataFrame(pd.Series(ndata.edit_index))
-            .reset_index()
-            .rename(columns={"index": "edit"}),
-            splice_sites=None if args.splice_site_path is None else splice_site,
-        )
-        target_info_df["effective_edit_rate"] = _obtain_effective_edit_rate(ndata).cpu()
-        target_info_df["n_guides"] = _obtain_n_guides_alleles_per_variant(ndata).cpu()
-        if args.adjust_confidence_by_negative_control:
-            adj_negctrl_idx = np.where(target_info_df.ref == target_info_df.alt)[0]
-
-    guide_info_df = ndata.screen.guides
-    del bdata
-
-    info(f"Running inference for {model_label}...")
-
-    if args.load_existing:
-        with open(f"{prefix}/{model_label}.result.pkl", "rb") as handle:
-            param_history_dict = pkl.load(handle)
-    else:
-        param_history_dict = deepcopy(run_inference(model, guide, ndata))
-        if args.fit_negctrl:
-            negctrl_model = m.ControlNormalModel
-            negctrl_guide = m.ControlNormalGuide
-            negctrl_idx = np.where(
-                guide_info_df[args.negctrl_col].map(lambda s: s.lower())
-                == args.negctrl_col_value.lower()
-            )[0]
-            print(len(negctrl_idx))
-            print(negctrl_idx.shape)
-            ndata_negctrl = ndata[negctrl_idx]
-            param_history_dict["negctrl"] = run_inference(
-                negctrl_model, negctrl_guide, ndata_negctrl
-            )
 
-    outfile_path = (
-        f"{prefix}/bean_element[sgRNA]_result.{model_label}{args.result_suffix}.csv"
+    negctrl_guide = partial(
+        m.ControlNormalGuide,
+        use_bcmatch=(not args.ignore_bcmatch and data_has_bcmatch),
     )
-    info(f"Done running inference. Writing result at {outfile_path}...")
-    if not os.path.exists(prefix):
-        os.makedirs(prefix)
-    with open(f"{prefix}/{model_label}.result{args.result_suffix}.pkl", "wb") as handle:
-        try:
-            pkl.dump(param_history_dict, handle)
-        except TypeError as exc:
-            print(exc.message)
-            # print(param_history_dict)
-    write_result_table(
-        target_info_df,
-        param_history_dict,
-        model_label=model_label,
-        prefix=f"{prefix}/",
-        suffix=args.result_suffix,
-        guide_index=guide_index,
-        guide_acc=ndata.guide_accessibility.cpu().numpy()
-        if hasattr(ndata, "guide_accessibility")
-        and ndata.guide_accessibility is not None
-        else None,
-        adjust_confidence_by_negative_control=args.adjust_confidence_by_negative_control,
-        adjust_confidence_negatives=adj_negctrl_idx,
-    )
-    info("Done!")
-
-
-if __name__ == "__main__":
-    args = parse_args()
-    bdata = be.read_h5ad(args.bdata_path)
-    args, bdata = check_args(args, bdata)
-    main(args, bdata)
+    return negctrl_model, negctrl_guide
```

### Comparing `crispr-bean-0.2.7/setup.py` & `crispr-bean-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
-from setuptools import setup, Extension, find_packages
+from setuptools import setup, find_packages
 from Cython.Build import cythonize
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="crispr-bean",
-    version="0.2.7",
+    version="1.0.0",
     python_requires=">=3.8.0",
     author="Jayoung Ryu",
     author_email="jayoung_ryu@g.harvard.edu",
     description="Base Editor screen analysis [Bayesian Estimation of variant effect] with guide Activity Normalization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pinellolab/crispr-bean",
@@ -20,39 +20,43 @@
     ext_modules=cythonize(["bean/mapping/CRISPResso2Align.pyx"]),
     include_dirs=np.get_include(),
     setup_requires=[
         "setuptools>=18.0",
         "Cython",
     ],
     scripts=[
-        "bin/bean-count",
-        "bin/bean-count-samples",
-        "bin/bean-qc",
-        "bin/bean-filter",
-        "bin/bean-run",  # TODO: prevent error when extra requirements are not met.
+        "bin/bean"
+        # "bin/bean-count",
+        # "bin/bean-count-samples",
+        # "bin/bean-create-screen",
+        # "bin/bean-profile",
+        # "bin/bean-qc",
+        # "bin/bean-filter",
+        # "bin/bean-run",  # TODO: prevent error when extra requirements are not met.
     ],
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
-        "perturb-tools>=0.2.6",
+        "perturb-tools>=0.3.0",
         "matplotlib",
-        "seaborn",
+        "seaborn>=0.13.0",
         "tqdm",
         "bio",
         "liftover",
         "openpyxl>=3.0.10",
         "papermill>=2.4.0",
         "pyBigWig>=0.3.18",
-        "pyro-ppl==1.8.1",
+        "pyro-ppl>=1.8.5",
         "scikit-learn",
         "statsmodels>=0.12.1",
         "ipykernel",
         "pytest-order",
         "nbconvert",
+        "logomaker",
     ],
     extras_require={"model": ["pyBigWig", "pyro-ppl<=1.8.1", "statsmodels", "torch<2"]},
     include_package_data=True,
     package_data={
         "": [
             "bean/annotate/ldlr_exons.fa",
             "notebooks/sample_quality_report.ipynb",
```

