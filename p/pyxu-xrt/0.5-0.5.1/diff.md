# Comparing `tmp/pyxu_xrt-0.5-py3-none-any.whl.zip` & `tmp/pyxu_xrt-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14180 bytes, number of entries: 10
+Zip file size: 13569 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       80 b- defN 20-Feb-02 00:00 pyxu_xrt/__init__.py
--rw-r--r--  2.0 unx       88 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/__init__.py
+-rw-r--r--  2.0 unx       42 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/linop/__init__.py
 -rw-r--r--  2.0 unx    16687 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/linop/_drjit.py
--rw-r--r--  2.0 unx      149 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/linop/fourier.py
--rw-r--r--  2.0 unx    20792 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/linop/ray.py
-?rw-r--r--  2.0 unx     4314 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      816 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.dist-info/RECORD
-10 files, 44095 bytes uncompressed, 12782 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    18440 b- defN 20-Feb-02 00:00 pyxu_xrt/operator/linop/ray.py
+?rw-r--r--  2.0 unx     4348 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx       50 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1082 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      830 b- defN 20-Feb-02 00:00 pyxu_xrt-0.5.1.dist-info/RECORD
+10 files, 41646 bytes uncompressed, 12141 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pyxu_xrt/operator/linop/__init__.py
 Comment: 
 
 Filename: pyxu_xrt/operator/linop/_drjit.py
 Comment: 
 
-Filename: pyxu_xrt/operator/linop/fourier.py
+Filename: pyxu_xrt/operator/linop/ray.py
 Comment: 
 
-Filename: pyxu_xrt/operator/linop/ray.py
+Filename: pyxu_xrt-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: pyxu_xrt-0.5.dist-info/METADATA
+Filename: pyxu_xrt-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyxu_xrt-0.5.dist-info/WHEEL
+Filename: pyxu_xrt-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyxu_xrt-0.5.dist-info/licenses/LICENSE
+Filename: pyxu_xrt-0.5.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pyxu_xrt-0.5.dist-info/RECORD
+Filename: pyxu_xrt-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxu_xrt/operator/__init__.py

```diff
@@ -1,2 +1 @@
-from pyxu_xrt.operator.linop.fourier import *
 from pyxu_xrt.operator.linop.ray import *
```

## pyxu_xrt/operator/linop/ray.py

```diff
@@ -48,16 +48,19 @@
     .. image:: /_static/api/xray/xray_parametrization.svg
        :alt: 2D XRay Geometry
        :width: 50%
        :align: center
 
     Notes
     -----
-    * :py:class:`~pyxu_xrt.operator.RayXRT` requires LLVM installed on the system. See the `Dr.Jit documentation
-      <https://drjit.readthedocs.io/en/latest/index.html>`_ for details.
+    * Using :py:class:`~pyxu_xrt.operator.RayXRT` on the CPU requires LLVM.
+      See the `Dr.Jit documentation <https://drjit.readthedocs.io/en/latest/index.html>`_ for details.
+    * Using :py:class:`~pyxu_xrt.operator.RayXRT` on the GPU requires installing Pyxu with GPU add-ons.
+      See the `Pyxu install guide
+      <https://pyxu-org.github.io/intro/installation.html#installation-with-optional-dependencies>`_ for details.
     """
 
     def __init__(
         self,
         dim_shape: pxt.NDArrayShape,
         n_spec: pxt.NDArray,
         t_spec: pxt.NDArray,
@@ -81,14 +84,15 @@
         enable_warnings: bool
             If ``True``, emit a warning in case of precision mis-match issues.
 
         Notes
         -----
         * :py:class:`~pyxu_xrt.operator.RayXRT` instances are **not arraymodule-agnostic**: they will only work with
           NDArrays belonging to the same array module as (`n_spec`, `t_spec`).
+          Dask arrays are currently not supported.
         * :py:class:`~pyxu_xrt.operator.RayXRT` is **not** precision-agnostic: it will only work on NDArrays in
           single-precision. A warning is emitted if inputs must be cast.
         """
         super().__init__(
             dim_shape=dim_shape,
             codim_shape=len(n_spec),
         )
@@ -148,14 +152,16 @@
         # Run-time vs. Init-time Setup ----------------------------------------
         if ndi == pxd.NDArrayInfo.DASK:
             # Build data structures at runtime; just validate (n_spec, t_spec)
             assert self._n_spec.chunks == self._t_spec.chunks, "[n_spec,t_spec] Must have same chunk sizes."
             assert self._n_spec.chunks[1] == (
                 self.dim_rank,
             ), "[n_spec,t_spec] Chunking along last dimension unsupported."
+
+            raise NotImplementedError  # will change in a future release.
         else:  # init-time instantiation: create drjit variables
             self._dr = self._init_dr_metadata()
 
     @pxrt.enforce_precision(i="arr")
     def apply(self, arr: pxt.NDArray) -> pxt.NDArray:
         r"""
         Parameters
@@ -191,49 +197,15 @@
             # * origin: (Bi1,...,BiD, D), (Bi1,...,BiD, 1), (1,...,D, D+2)
             # * parts: [ this is the output of blockwise() ]
             #       (N_ray, Bi1,...,BiD),
             #       (Bp,    Bi1,...,BiD), -> we 'sumed' over the single-block axes (D+1, D+2)
             #       ( 0,      1,...,  D)
             # * out [ = parts.sum(axis=(-D,...,-1)) ]
             #       (N_ray,), (Bp,)
-
-            # Compute `origin` info.
-            offset = [np.r_[0, chks].cumsum()[:-1] for chks in arr.chunks]
-            offset = np.stack(  # (Bi1,...,BiD, D)
-                np.meshgrid(*offset, indexing="ij"),
-                axis=-1,
-            )
-            origin = xp.asarray(  # (Bi1,...,BiD, D)
-                np.r_[self._origin] + np.r_[self._pitch] * offset,
-                chunks=(1,) * self.dim_rank + (self.dim_rank,),
-            )
-
-            # Compute (I,n,t,orig,o)_ind & output chunks
-            I_ind = tuple(range(1, self.dim_rank + 1))
-            n_ind = (0, self.dim_rank + 1)
-            t_ind = (0, self.dim_rank + 1)
-            orig_ind = (*range(1, self.dim_rank + 1), self.dim_rank + 2)
-            o_ind = tuple(range(self.dim_rank + 1))
-            o_chunks = {d: 1 for d in range(1, self.dim_rank + 1)}
-
-            parts = xp.blockwise(
-                # shape:  (N_ray | Bi1,...,BiD)
-                # bcount: (Bp    | Bi1,...,BiD)
-                *(self._blockwise_apply, o_ind),
-                *(arr, I_ind),
-                *(self._n_spec, n_ind),
-                *(self._t_spec, t_ind),
-                *(origin, orig_ind),
-                dtype=dtype,
-                adjust_chunks=o_chunks,
-                align_arrays=False,
-                concatenate=True,
-                meta=arr._meta,
-            )
-            out = parts.sum(axis=tuple(range(-self.dim_rank, 0)))  # (N_ray,)
+            raise NotImplementedError
         else:  # NUMPY/CUPY
             from . import _drjit as drh
 
             # Load the right drjit function
             drb = drh._load_dr_variant(ndi)
             fwd, _ = drh._build_xrt(drb, D=self.dim_rank, weighted=False)
 
@@ -516,45 +488,7 @@
             N=Arrayu(*self.dim_shape),
             r=Rayf(
                 o=Arrayf(*[drh._xp2dr(_) for _ in self._t_spec.T]),
                 d=Arrayf(*[drh._xp2dr(_) for _ in self._n_spec.T]),
             ),
         )
         return meta
-
-    def _blockwise_apply(self, I, n_spec, t_spec, origin) -> pxt.NDArray:
-        # Project rays through sub-volume.
-        # [All arrays are NUMPY/CUPY.]
-        #
-        # Parameters
-        # ----------
-        # I: NDArray[float32]
-        #     (S1,...,SD) sub-volume entries.
-        # n_spec: NDArray[float32]
-        #     (L, D) ray directions :math:`\mathbf{n} \in \mathbb{S}^{D-1}`.
-        # t_spec: NDArray[float32]
-        #     (L, D) offset specifiers :math:`\mathbf{t} \in \mathbb{R}^{D}`.
-        # origin: NDArray[float]
-        #     (<D 1s>, D) bottom-left coordinate of sub-volume.
-        #
-        # Returns
-        # -------
-        # P: NDArray[float32]
-        #     (L, <D 1s>) projection weights.
-        #
-        #     [Note the trailing size-1 dims; these are required since blockwise() expects to
-        #      stack these outputs given how it was called.]
-        select = (0,) * self.dim_rank
-        origin = origin[*select]  # (D,)
-
-        op = RayXRT(
-            dim_shape=I.shape,
-            n_spec=n_spec,
-            t_spec=t_spec,
-            origin=origin,
-            pitch=self._pitch,
-            enable_warnings=self._enable_warnings,
-        )
-        P = op.apply(I)  # (L,)
-
-        expand = (np.newaxis,) * self.dim_rank
-        return P[..., *expand]  # (L, <D 1s>)
```

## Comparing `pyxu_xrt-0.5.dist-info/METADATA` & `pyxu_xrt-0.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: pyxu_xrt
-Version: 0.5
+Version: 0.5.1
 Summary: Pyxu X-Ray Transform Operators.
 Project-URL: download, https://github.com/pyxu-org/pyxu_xrt
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

## Comparing `pyxu_xrt-0.5.dist-info/licenses/LICENSE` & `pyxu_xrt-0.5.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pyxu_xrt-0.5.dist-info/RECORD` & `pyxu_xrt-0.5.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyxu_xrt/__init__.py,sha256=tqbIMaLsTGWuU8ef6IZgyUaLDt3tHvJiHEkzmMNTyXk,80
-pyxu_xrt/operator/__init__.py,sha256=0la1ubuqN2pPTweZK6ANyx3N1PrXtQOh1t5NncuJB6E,88
+pyxu_xrt/operator/__init__.py,sha256=2UZSKtjDZ8FaH7vEgjnr7FWe1LqDoDQ3JXmy_y991m4,42
 pyxu_xrt/operator/linop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyxu_xrt/operator/linop/_drjit.py,sha256=IrcaF9FajfM0TFqodUT4floxkruScXBVXEyjufeYZAo,16687
-pyxu_xrt/operator/linop/fourier.py,sha256=bhfhPrEiHQad5KmXpO0NRVgSHX9TPDfw7oTzXjgmRbo,149
-pyxu_xrt/operator/linop/ray.py,sha256=eFcAh7Z1A9LRGqOvfNwlJXClP7oMKA8LszXJrBK_z30,20792
-pyxu_xrt-0.5.dist-info/METADATA,sha256=3tUUUBJAj0WvrmAHNE8x8a8Fxvbfk1FakuVEdZmBniE,4314
-pyxu_xrt-0.5.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-pyxu_xrt-0.5.dist-info/licenses/LICENSE,sha256=_kI8k_5LWv06zr2vd5F2cE4_O7w8H5gxAWEUVqhwRck,1082
-pyxu_xrt-0.5.dist-info/RECORD,,
+pyxu_xrt/operator/linop/ray.py,sha256=WGCFfqjCTg-vnaqexmL5zwY_8KICOMpNKePC0RXP_Zc,18440
+pyxu_xrt-0.5.1.dist-info/METADATA,sha256=f1SlqYKMPLp-pXlvymt42bscnxsvJJP_UxWJWM-IhR8,4348
+pyxu_xrt-0.5.1.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
+pyxu_xrt-0.5.1.dist-info/entry_points.txt,sha256=ZmX79tv1LPVv6VaPz7V2VYaFKiZXA_i1ywcvmjLESWU,50
+pyxu_xrt-0.5.1.dist-info/licenses/LICENSE,sha256=_kI8k_5LWv06zr2vd5F2cE4_O7w8H5gxAWEUVqhwRck,1082
+pyxu_xrt-0.5.1.dist-info/RECORD,,
```

