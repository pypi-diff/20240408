# Comparing `tmp/pyxu_finufft-1.0-py3-none-any.whl.zip` & `tmp/pyxu_finufft-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 7775 bytes, number of entries: 8
+Zip file size: 8081 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       84 b- defN 20-Feb-02 00:00 pyxu_finufft/__init__.py
 -rw-r--r--  2.0 unx       48 b- defN 20-Feb-02 00:00 pyxu_finufft/operator/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 pyxu_finufft/operator/linop/__init__.py
 -rw-r--r--  2.0 unx    24746 b- defN 20-Feb-02 00:00 pyxu_finufft/operator/linop/nufft.py
-?rw-r--r--  2.0 unx     2720 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      669 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.dist-info/RECORD
-8 files, 29436 bytes uncompressed, 6595 bytes compressed:  77.6%
+?rw-r--r--  2.0 unx     2754 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      130 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      778 b- defN 20-Feb-02 00:00 pyxu_finufft-1.0.1.dist-info/RECORD
+9 files, 29709 bytes uncompressed, 6719 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -6,20 +6,23 @@
 
 Filename: pyxu_finufft/operator/linop/__init__.py
 Comment: 
 
 Filename: pyxu_finufft/operator/linop/nufft.py
 Comment: 
 
-Filename: pyxu_finufft-1.0.dist-info/METADATA
+Filename: pyxu_finufft-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pyxu_finufft-1.0.dist-info/WHEEL
+Filename: pyxu_finufft-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyxu_finufft-1.0.dist-info/licenses/LICENSE
+Filename: pyxu_finufft-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyxu_finufft-1.0.dist-info/RECORD
+Filename: pyxu_finufft-1.0.1.dist-info/licenses/LICENSE
+Comment: 
+
+Filename: pyxu_finufft-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyxu_finufft-1.0.dist-info/METADATA` & `pyxu_finufft-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: pyxu_finufft
-Version: 1.0
+Version: 1.0.1
 Summary: Pyxu bindings to the Flatiron Institute Non-uniform Fast Fourier Transform (FINUFFT) library.
 Project-URL: download, https://github.com/pyxu-org/pyxu_finufft
 Author-email: "S. Kashani" <sepand@kashani.ch>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Pycsou
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
```

## Comparing `pyxu_finufft-1.0.dist-info/licenses/LICENSE` & `pyxu_finufft-1.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pyxu_finufft-1.0.dist-info/RECORD` & `pyxu_finufft-1.0.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 pyxu_finufft/__init__.py,sha256=c-rC6KxhR5u4F1r7Wvp0HdAHzZ48hJ5yNvrWQKQOhBo,84
 pyxu_finufft/operator/__init__.py,sha256=HKHT_Dgqz5WKgYw2ECXENzOHLsk4NGfblQqmtTnFo2U,48
 pyxu_finufft/operator/linop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyxu_finufft/operator/linop/nufft.py,sha256=FGn0T_bS002L0Y8DuWzMCgLrPFJYHDhEMBV7VjH9leY,24746
-pyxu_finufft-1.0.dist-info/METADATA,sha256=aqgvwanbjGtdBOGrpiUhxb_yQpEyuhCxbMuZuqRlO0I,2720
-pyxu_finufft-1.0.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-pyxu_finufft-1.0.dist-info/licenses/LICENSE,sha256=_kI8k_5LWv06zr2vd5F2cE4_O7w8H5gxAWEUVqhwRck,1082
-pyxu_finufft-1.0.dist-info/RECORD,,
+pyxu_finufft-1.0.1.dist-info/METADATA,sha256=S7zyYOM6QPS0SPepUSq78V05qYXzvdAXFQUHGiLZX50,2754
+pyxu_finufft-1.0.1.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+pyxu_finufft-1.0.1.dist-info/entry_points.txt,sha256=pgJTaGVpMfrA0POfN_Sp07CCbwBiH9QxnMO1-mHnqDg,130
+pyxu_finufft-1.0.1.dist-info/licenses/LICENSE,sha256=_kI8k_5LWv06zr2vd5F2cE4_O7w8H5gxAWEUVqhwRck,1082
+pyxu_finufft-1.0.1.dist-info/RECORD,,
```

