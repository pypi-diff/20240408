# Comparing `tmp/lib_pcg_algopy-0.2.2.tar.gz` & `tmp/lib_pcg_algopy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_pcg_algopy-0.2.2.tar", max compression
+gzip compressed data, was "lib_pcg_algopy-0.2.3.tar", max compression
```

## Comparing `lib_pcg_algopy-0.2.2.tar` & `lib_pcg_algopy-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.2.2/README.md
--rw-r--r--   0        0        0      303 2024-04-06 15:54:14.290298 lib_pcg_algopy-0.2.2/lib_pcg/__init__.py
--rw-r--r--   0        0        0      251 2024-04-06 13:55:27.698575 lib_pcg_algopy-0.2.2/lib_pcg/consts.py
--rw-r--r--   0        0        0        0 2024-04-07 17:16:51.217844 lib_pcg_algopy-0.2.2/lib_pcg/py.typed
--rw-r--r--   0        0        0     2844 2024-04-07 16:32:17.909072 lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_64_32.py
--rw-r--r--   0        0        0     2364 2024-04-06 13:56:18.658332 lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_double_64_32.py
--rw-r--r--   0        0        0     4599 2024-04-08 11:13:49.533120 lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_quadruple_64_32.py
--rw-r--r--   0        0        0     1549 2024-04-08 11:15:32.600635 lib_pcg_algopy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.2.3/README.md
+-rw-r--r--   0        0        0      303 2024-04-06 15:54:14.290298 lib_pcg_algopy-0.2.3/lib_pcg/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-06 13:55:27.698575 lib_pcg_algopy-0.2.3/lib_pcg/consts.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:16:51.217844 lib_pcg_algopy-0.2.3/lib_pcg/py.typed
+-rw-r--r--   0        0        0     2844 2024-04-07 16:32:17.909072 lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_64_32.py
+-rw-r--r--   0        0        0     2364 2024-04-06 13:56:18.658332 lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_double_64_32.py
+-rw-r--r--   0        0        0     4262 2024-04-08 12:06:40.001050 lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_quadruple_64_32.py
+-rw-r--r--   0        0        0     1549 2024-04-08 12:10:33.755538 lib_pcg_algopy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.2.3/PKG-INFO
```

### Comparing `lib_pcg_algopy-0.2.2/README.md` & `lib_pcg_algopy-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_64_32.py` & `lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_64_32.py`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_double_64_32.py` & `lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_double_64_32.py`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.2/lib_pcg/xsh_rr_quadruple_64_32.py` & `lib_pcg_algopy-0.2.3/lib_pcg/xsh_rr_quadruple_64_32.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,36 +106,30 @@
         for i in urange(length):  # noqa: B007
             state1, state2, state3, state4, n = __pcg128_random(
                 (state1, state2, state3, state4)
             )
 
             result += n.bytes
     else:
-        # We write the bound condition on the length of the underlying bytes because
-        #  it's important that it doesn't just exceed in value but in length.
-        # BigUInt arithmetic will pad with 0 the shortest string potentially increasing
-        #  the length of our results beyond 16 bytes.
-        assert lower_bound.bytes.length <= 16
-        assert upper_bound.bytes.length <= 16
-
         if upper_bound != 0:
             assert upper_bound > BigUInt(1)
+            assert upper_bound < BigUInt(2**128)
             assert lower_bound < upper_bound - BigUInt(1)
 
             absolute_bound = upper_bound - lower_bound
         else:
-            assert lower_bound < BigUInt(2**256 - 1)
+            assert lower_bound < BigUInt(2**128 - 1)
 
-            absolute_bound = BigUInt(2**256) - lower_bound
+            absolute_bound = BigUInt(2**128) - lower_bound
 
         threshold = __pcg128_twos(absolute_bound) % absolute_bound
 
         for i in urange(length):  # noqa: B007
             while True:
                 state1, state2, state3, state4, candidate = __pcg128_random(
                     (state1, state2, state3, state4)
                 )
                 if candidate >= threshold:
                     break
-            result += ((candidate % absolute_bound) + lower_bound).bytes
+            result += arc4.UInt128((candidate % absolute_bound) + lower_bound).bytes
 
     return state1, state2, state3, state4, result
```

### Comparing `lib_pcg_algopy-0.2.2/pyproject.toml` & `lib_pcg_algopy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-pcg-algopy"
-version = "0.2.2"
+version = "0.2.3"
 description = "PCG library implemented using Algorand Python"
 authors = ["CiottiGiorgio <giorgio.ciotti@algorand.foundation>"]
 readme = "README.md"
 packages = [{include = "lib_pcg"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `lib_pcg_algopy-0.2.2/PKG-INFO` & `lib_pcg_algopy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pcg-algopy
-Version: 0.2.2
+Version: 0.2.3
 Summary: PCG library implemented using Algorand Python
 Author: CiottiGiorgio
 Author-email: giorgio.ciotti@algorand.foundation
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: algokit-utils (>=2.2.0,<3.0.0)
```

