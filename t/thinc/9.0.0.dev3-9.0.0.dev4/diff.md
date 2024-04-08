# Comparing `tmp/thinc-9.0.0.dev3.tar.gz` & `tmp/thinc-9.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinc-9.0.0.dev3.tar", last modified: Wed Mar 22 15:38:49 2023, max compression
+gzip compressed data, was "thinc-9.0.0.dev4.tar", last modified: Tue Jan 16 12:08:16 2024, max compression
```

## Comparing `thinc-9.0.0.dev3.tar` & `thinc-9.0.0.dev4.tar`

### file list

```diff
@@ -1,206 +1,207 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1123 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      222 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    11536 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3442 2023-03-22 15:38:49.050978 thinc-9.0.0.dev3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3829 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.026977 thinc-9.0.0.dev3/thinc/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      214 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/about.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5853 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/api.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.030977 thinc-9.0.0.dev3/thinc/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5404 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2200 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_cupy_allocators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18263 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_custom_kernels.cu
--rw-r--r--   0 vsts      (1001) docker     (122)    21936 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_custom_kernels.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5210 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_murmur3.cu
--rw-r--r--   0 vsts      (1001) docker     (122)     2741 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/_param_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2027 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cblas.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2052 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cblas.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    14601 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cpu_kernels.hh
--rw-r--r--   0 vsts      (1001) docker     (122)    11756 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/cupy_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)      581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/mps_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1989 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/numpy_ops.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    37228 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/numpy_ops.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    58365 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/backends/ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2474 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3833 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/initializers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)     4315 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2246 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/add.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1587 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/array_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/bidirectional.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1741 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/cauchysimilarity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3445 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/chain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4447 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/clipped_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)      649 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/clone.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5181 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/concatenate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2113 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/dish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2956 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2691 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/embed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1641 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/expand_window.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2120 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/gelu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2147 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hard_swish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2194 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hard_swish_mobilenet.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/hashembed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1721 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)      878 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2array.py
--rw-r--r--   0 vsts      (1001) docker     (122)      623 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2padded.py
--rw-r--r--   0 vsts      (1001) docker     (122)      864 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/list2ragged.py
--rw-r--r--   0 vsts      (1001) docker     (122)      610 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/logistic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6450 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/lstm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1027 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/map_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2595 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/maxout.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2270 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/mish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1769 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/multisoftmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4299 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/mxnetwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      512 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)      703 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/padded2list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2105 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/parametricattention.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/premap_ids.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    12428 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/pytorchwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      774 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/ragged2list.py
--rw-r--r--   0 vsts      (1001) docker     (122)      816 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_first.py
--rw-r--r--   0 vsts      (1001) docker     (122)      796 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_last.py
--rw-r--r--   0 vsts      (1001) docker     (122)      721 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_max.py
--rw-r--r--   0 vsts      (1001) docker     (122)      713 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_mean.py
--rw-r--r--   0 vsts      (1001) docker     (122)      707 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/reduce_sum.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/relu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3091 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/remap_ids.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2092 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/residual.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2755 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/resizable.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1615 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/siamese.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1946 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sigmoid.py
--rw-r--r--   0 vsts      (1001) docker     (122)      652 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sigmoid_activation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3238 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/softmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/softmax_activation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8161 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/sparselinear.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      805 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/strings2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2128 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/swish.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6516 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/tensorflowwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3286 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2018 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/tuplify.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2061 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3579 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_array.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4137 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_array2d.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1426 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_cpu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1333 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1954 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_flatten_v2.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1168 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2893 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1293 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_nvtx_range.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4857 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_padded.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4447 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_ragged.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1792 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_reshape.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1512 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/layers/with_signpost_interval.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)      201 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11358 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/legacy/loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22962 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11466 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/mypy.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)    11359 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/schedules.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.038977 thinc-9.0.0.dev3/thinc/shims/
--rw-r--r--   0 vsts      (1001) docker     (122)      463 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4285 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/mxnet.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9354 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/pytorch.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6060 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2482 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10581 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/tensorflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2261 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/shims/torchscript.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.042977 thinc-9.0.0.dev3/thinc/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.042977 thinc-9.0.0.dev3/thinc/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      358 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/test_mem.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48394 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/backends/test_ops.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2208 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2426 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_basic_tagger.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7807 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_combinators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5439 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_feed_forward.py
--rw-r--r--   0 vsts      (1001) docker     (122)      532 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_hash_embed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9830 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_layers_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7341 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5669 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_lstm.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1649 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mappers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3673 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mnist.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6275 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_mxnet_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6991 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_pytorch_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3694 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_reduce.py
--rw-r--r--   0 vsts      (1001) docker     (122)      872 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_resizable.py
--rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2869 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_softmax.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2289 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_sparse_linear.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13090 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_tensorflow_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      810 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1975 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_transforms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2251 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (122)      801 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10166 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/layers/test_with_transforms.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/model/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19914 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1369 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/model/test_validation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/configs/
--rw-r--r--   0 vsts      (1001) docker     (122)      195 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0 vsts      (1001) docker     (122)      217 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/configs/mypy-plugin.ini
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/modules/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      565 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     2416 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      576 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/mypy/test_mypy.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/regression/issue519/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/program.py
--rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/issue519/test_issue519.py
--rw-r--r--   0 vsts      (1001) docker     (122)      328 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/test_issue208.py
--rw-r--r--   0 vsts      (1001) docker     (122)      520 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/regression/test_issue564.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.046977 thinc-9.0.0.dev3/thinc/tests/shims/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3349 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/shims/test_pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3586 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/strategies.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5702 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1749 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1800 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_import__all__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1895 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_indexing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      983 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_initializers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    27480 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_loss.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4997 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3491 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_schedules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6771 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1306 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6573 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3598 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)    47781 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20964 2023-03-22 15:38:19.000000 thinc-9.0.0.dev3/thinc/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 15:38:49.026977 thinc-9.0.0.dev3/thinc.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    13235 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-03-22 15:38:49.000000 thinc-9.0.0.dev3/thinc.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)     1092 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-03-22 15:38:48.000000 thinc-9.0.0.dev3/thinc.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.163423 thinc-9.0.0.dev4/thinc/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)      213 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/about.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5915 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/api.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.167423 thinc-9.0.0.dev4/thinc/backends/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     5320 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_cupy_allocators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18822 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_custom_kernels.cu
+-rw-r--r--   0 vsts      (1001) docker     (127)    25370 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_custom_kernels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_murmur3.cu
+-rw-r--r--   0 vsts      (1001) docker     (127)     2740 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_param_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2026 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cblas.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     2076 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cblas.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    14601 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cpu_kernels.hh
+-rw-r--r--   0 vsts      (1001) docker     (127)    12947 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cupy_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/mps_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/numpy_ops.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)    38254 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/numpy_ops.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    58702 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3092 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/initializers.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.175423 thinc-9.0.0.dev4/thinc/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4396 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2245 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1587 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/array_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/bidirectional.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1740 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/cauchysimilarity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3444 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/chain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/clipped_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      648 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5188 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/concatenate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2113 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/dish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2955 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/dropout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2690 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1640 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/expand_window.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2120 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/gelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2147 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hard_swish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2194 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hard_swish_mobilenet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3615 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hashembed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2534 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1720 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      877 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      622 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2padded.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      609 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/logistic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6451 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/map_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2594 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/maxout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2269 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/mish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1768 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/multisoftmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4281 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/mxnetwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      511 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/padded2list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/parametricattention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2972 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/parametricattention_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/premap_ids.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    12439 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/pytorchwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      773 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/ragged2list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      815 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_first.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_last.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      720 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_max.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      712 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_mean.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_sum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2057 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/relu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/remap_ids.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2092 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/residual.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2755 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/siamese.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1945 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sigmoid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      652 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sigmoid_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3237 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/softmax_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8175 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sparselinear.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/strings2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2128 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/swish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6549 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/tensorflowwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3276 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2018 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/tuplify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_array2d.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_cpu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1674 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_flatten_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2893 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_nvtx_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4856 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_padded.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4446 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1791 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_reshape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_signpost_interval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16308 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/loss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34919 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11467 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/mypy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14580 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)    11342 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/schedules.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.175423 thinc-9.0.0.dev4/thinc/shims/
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4315 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/mxnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9340 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/pytorch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6060 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2482 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/shim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10604 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/tensorflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2457 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/torchscript.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.179423 thinc-9.0.0.dev4/thinc/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.179423 thinc-9.0.0.dev4/thinc/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/test_mem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52692 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/test_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2209 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       92 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/enable_mxnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/enable_tensorflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_basic_tagger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_combinators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5441 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_feed_forward.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_hash_embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9974 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_layers_api.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7342 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5650 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1650 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mappers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3669 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mnist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mxnet_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_parametric_attention_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6951 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_pytorch_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3695 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_reduce.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      874 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2869 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_sparse_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13111 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_tensorflow_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_transforms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2252 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      802 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      871 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10169 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_transforms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/model/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19918 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1386 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/test_validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/configs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      195 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/configs/mypy-plugin.ini
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/modules/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      831 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     2416 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      576 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      494 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/test_mypy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/regression/issue519/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/program.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      817 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/test_issue519.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      328 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/test_issue208.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/test_issue564.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/shims/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/shims/test_pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3587 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/strategies.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5833 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1800 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_import__all__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1896 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_indexing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_initializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12083 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_loss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4997 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3471 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6788 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1559 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5647 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47816 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21106 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5528 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/top_level.txt
```

### Comparing `thinc-9.0.0.dev3/LICENSE` & `thinc-9.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/PKG-INFO` & `thinc-9.0.0.dev4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev3
+Version: 9.0.0.dev4
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,115 +18,172 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: blis<0.8.0,>=0.7.8
+Requires-Dist: murmurhash<1.1.0,>=1.0.2
+Requires-Dist: cymem<2.1.0,>=2.0.2
+Requires-Dist: preshed<3.1.0,>=3.0.2
+Requires-Dist: wasabi<1.2.0,>=0.8.1
+Requires-Dist: srsly<3.0.0,>=2.4.0
+Requires-Dist: catalogue<2.1.0,>=2.0.4
+Requires-Dist: confection<1.0.0,>=0.0.1
+Requires-Dist: setuptools
+Requires-Dist: numpy>=1.15.0; python_version < "3.9"
+Requires-Dist: numpy>=1.19.0; python_version >= "3.9"
+Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
+Requires-Dist: packaging>=20.0
+Requires-Dist: dataclasses<1.0,>=0.6; python_version < "3.7"
+Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1; python_version < "3.8"
+Requires-Dist: contextvars<3,>=2.4; python_version < "3.7"
 Provides-Extra: cuda
+Requires-Dist: cupy>=5.0.0b4; extra == "cuda"
 Provides-Extra: cuda80
+Requires-Dist: cupy-cuda80>=5.0.0b4; extra == "cuda80"
 Provides-Extra: cuda90
+Requires-Dist: cupy-cuda90>=5.0.0b4; extra == "cuda90"
 Provides-Extra: cuda91
+Requires-Dist: cupy-cuda91>=5.0.0b4; extra == "cuda91"
 Provides-Extra: cuda92
+Requires-Dist: cupy-cuda92>=5.0.0b4; extra == "cuda92"
 Provides-Extra: cuda100
+Requires-Dist: cupy-cuda100>=5.0.0b4; extra == "cuda100"
 Provides-Extra: cuda101
+Requires-Dist: cupy-cuda101>=5.0.0b4; extra == "cuda101"
 Provides-Extra: cuda102
+Requires-Dist: cupy-cuda102>=5.0.0b4; extra == "cuda102"
 Provides-Extra: cuda110
+Requires-Dist: cupy-cuda110>=5.0.0b4; extra == "cuda110"
 Provides-Extra: cuda111
+Requires-Dist: cupy-cuda111>=5.0.0b4; extra == "cuda111"
 Provides-Extra: cuda112
+Requires-Dist: cupy-cuda112>=5.0.0b4; extra == "cuda112"
 Provides-Extra: cuda113
+Requires-Dist: cupy-cuda113>=5.0.0b4; extra == "cuda113"
 Provides-Extra: cuda114
+Requires-Dist: cupy-cuda114>=5.0.0b4; extra == "cuda114"
 Provides-Extra: cuda115
+Requires-Dist: cupy-cuda115>=5.0.0b4; extra == "cuda115"
 Provides-Extra: cuda116
+Requires-Dist: cupy-cuda116>=5.0.0b4; extra == "cuda116"
 Provides-Extra: cuda117
+Requires-Dist: cupy-cuda117>=5.0.0b4; extra == "cuda117"
 Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x>=11.0.0; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x>=11.5.0; extra == "cuda12x"
 Provides-Extra: cuda-autodetect
+Requires-Dist: cupy-wheel>=11.0.0; extra == "cuda-autodetect"
 Provides-Extra: datasets
+Requires-Dist: ml_datasets<0.3.0,>=0.2.0; extra == "datasets"
 Provides-Extra: torch
+Requires-Dist: torch>=1.6.0; extra == "torch"
 Provides-Extra: tensorflow
+Requires-Dist: tensorflow<2.6.0,>=2.0.0; extra == "tensorflow"
 Provides-Extra: mxnet
-License-File: LICENSE
+Requires-Dist: mxnet<1.6.0,>=1.5.1; extra == "mxnet"
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Thinc: A refreshing functional take on deep learning, compatible with your favorite libraries
 
 ### From the makers of [spaCy](https://spacy.io) and [Prodigy](https://prodi.gy)
 
-[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers an elegant,
-type-checked, functional-programming API for **composing models**, with support
-for layers defined in other frameworks such as **PyTorch, TensorFlow and MXNet**. You
-can use Thinc as an interface layer, a standalone toolkit or a flexible way to
-develop new models. Previous versions of Thinc have been running quietly in
-production in thousands of companies, via both [spaCy](https://spacy.io) and
-[Prodigy](https://prodi.gy). We wrote the new version to let users **compose,
-configure and deploy custom models** built with their favorite framework.
+[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers
+an elegant, type-checked, functional-programming API for **composing models**,
+with support for layers defined in other frameworks such as **PyTorch,
+TensorFlow and MXNet**. You can use Thinc as an interface layer, a standalone
+toolkit or a flexible way to develop new models. Previous versions of Thinc have
+been running quietly in production in thousands of companies, via both
+[spaCy](https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the new
+version to let users **compose, configure and deploy custom models** built with
+their favorite framework.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/7/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=7)
+[![tests](https://github.com/explosion/thinc/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/thinc/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)](https://github.com/explosion/thinc/releases)
 [![PyPi Version](https://img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/thinc)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 [![Open demo in Colab][colab]][intro_to_thinc_colab]
 
 ## 🔥 Features
 
-- **Type-check** your model definitions with custom types and [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
+- **Type-check** your model definitions with custom types and
+  [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
 - Wrap **PyTorch**, **TensorFlow** and **MXNet** models for use in your network.
-- Concise **functional-programming** approach to model definition, using composition rather than inheritance.
+- Concise **functional-programming** approach to model definition, using
+  composition rather than inheritance.
 - Optional custom infix notation via **operator overloading**.
 - Integrated **config system** to describe trees of objects and hyperparameters.
 - Choice of **extensible backends**.
 - **[Read more &rarr;](https://thinc.ai/docs)**
 
 ## 🚀 Quickstart
 
-Thinc is compatible with **Python 3.6+** and runs on **Linux**,
-**macOS** and **Windows**. The latest releases with binary wheels are available from
+Thinc is compatible with **Python 3.6+** and runs on **Linux**, **macOS** and
+**Windows**. The latest releases with binary wheels are available from
 [pip](https://pypi.python.org/pypi/thinc). Before you install Thinc and its
 dependencies, make sure that your `pip`, `setuptools` and `wheel` are up to
 date. For the most recent releases, pip 19.3 or newer is recommended.
 
 ```bash
 pip install -U pip setuptools wheel
 pip install thinc
 ```
 
-See the [extended installation docs](https://thinc.ai/docs/install#extended) for details on optional dependencies for different backends and GPU. You might also want to [set up static type checking](https://thinc.ai/docs/install#type-checking) to take advantage of Thinc's type system.
+See the [extended installation docs](https://thinc.ai/docs/install#extended) for
+details on optional dependencies for different backends and GPU. You might also
+want to
+[set up static type checking](https://thinc.ai/docs/install#type-checking) to
+take advantage of Thinc's type system.
 
 > ⚠️ If you have installed PyTorch and you are using Python 3.7+, uninstall the
-> package `dataclasses` with `pip uninstall dataclasses`, since it may have
-> been installed by PyTorch and is incompatible with Python 3.7+.
+> package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+.
 
 ### 📓 Selected examples and notebooks
 
-Also see the [`/examples`](examples) directory and [usage documentation](https://thinc.ai/docs) for more examples. Most examples are Jupyter notebooks – to launch them on [Google Colab](https://colab.research.google.com) (with GPU support!) click on the button next to the notebook name.
+Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks – to launch them on
+[Google Colab](https://colab.research.google.com) (with GPU support!) click on
+the button next to the notebook name.
 
 | Notebook                                                                                                              | Description                                                                                                                                                                                       |
 | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [`intro_to_thinc`][intro_to_thinc]<br />[![Open in Colab][colab]][intro_to_thinc_colab]                               | Everything you need to know to get started. Composing and training a model on the MNIST data, using config files, registering custom functions and wrapping PyTorch, TensorFlow and MXNet models. |
 | [`transformers_tagger_bert`][transformers_tagger_bert]<br />[![Open in Colab][colab]][transformers_tagger_bert_colab] | How to use Thinc, `transformers` and PyTorch to train a part-of-speech tagger. From model definition and config to the training loop.                                                             |
 | [`pos_tagger_basic_cnn`][pos_tagger_basic_cnn]<br />[![Open in Colab][colab]][pos_tagger_basic_cnn_colab]             | Implementing and training a basic CNN for part-of-speech tagging model without external dependencies and using different levels of Thinc's config system.                                         |
 | [`parallel_training_ray`][parallel_training_ray]<br />[![Open in Colab][colab]][parallel_training_ray_colab]          | How to set up synchronous and asynchronous parameter server training with Thinc and [Ray](https://ray.readthedocs.io/en/latest/).                                                                 |
 
 **[View more &rarr;](examples)**
 
-[colab]: https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
+[colab]:
+  https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
 [intro_to_thinc]: examples/00_intro_to_thinc.ipynb
-[intro_to_thinc_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
+[intro_to_thinc_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
 [transformers_tagger_bert]: examples/02_transformers_tagger_bert.ipynb
-[transformers_tagger_bert_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
+[transformers_tagger_bert_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
 [pos_tagger_basic_cnn]: examples/03_pos_tagger_basic_cnn.ipynb
-[pos_tagger_basic_cnn_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
+[pos_tagger_basic_cnn_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
 [parallel_training_ray]: examples/04_parallel_training_ray.ipynb
-[parallel_training_ray_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
+[parallel_training_ray_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
 
 ### 📖 Documentation & usage guides
 
 | Documentation                                                                     | Description                                           |
 | --------------------------------------------------------------------------------- | ----------------------------------------------------- |
 | [Introduction](https://thinc.ai/docs)                                             | Everything you need to know.                          |
 | [Concept & Design](https://thinc.ai/docs/concept)                                 | Thinc's conceptual model and how it works.            |
@@ -150,15 +207,20 @@
 | [`thinc.schedules`](thinc/schedules.py)   | Generators for different rates, schedules, decays or series.                      |
 | [`thinc.backends`](thinc/backends)        | Backends for `numpy` and `cupy`.                                                  |
 | [`thinc.config`](thinc/config.py)         | Config parsing and validation and function registry system.                       |
 | [`thinc.util`](thinc/util.py)             | Utilities and helper functions.                                                   |
 
 ## 🐍 Development notes
 
-Thinc uses [`black`](https://github.com/psf/black) for auto-formatting, [`flake8`](http://flake8.pycqa.org/en/latest/) for linting and [`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is written compatible with **Python 3.6+**, with type hints wherever possible. See the [type reference](https://thinc.ai/docs/api-types) for more details on Thinc's custom types.
+Thinc uses [`black`](https://github.com/psf/black) for auto-formatting,
+[`flake8`](http://flake8.pycqa.org/en/latest/) for linting and
+[`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is
+written compatible with **Python 3.6+**, with type hints wherever possible. See
+the [type reference](https://thinc.ai/docs/api-types) for more details on
+Thinc's custom types.
 
 ### 👷‍♀️ Building Thinc from source
 
 Building Thinc from source requires the full dependencies listed in
 [`requirements.txt`](requirements.txt) to be installed. You'll also need a
 compiler to build the C extensions.
 
@@ -185,16 +247,20 @@
 export PYTHONPATH=`pwd`
 pip install -r requirements.txt
 python setup.py build_ext --inplace
 ```
 
 ### 🚦 Running tests
 
-Thinc comes with an [extensive test suite](thinc/tests). The following should all pass and not report any warnings or errors:
+Thinc comes with an [extensive test suite](thinc/tests). The following should
+all pass and not report any warnings or errors:
 
 ```bash
 python -m pytest thinc    # test suite
 python -m mypy thinc      # type checks
 python -m flake8 thinc    # linting
 ```
 
-To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim for a 100% test coverage. This doesn't mean that we meticulously write tests for every single line – we ignore blocks that are not relevant or difficult to test and make sure that the tests execute all code paths.
+To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim
+for a 100% test coverage. This doesn't mean that we meticulously write tests for
+every single line – we ignore blocks that are not relevant or difficult to test
+and make sure that the tests execute all code paths.
```

#### html2text {}

```diff
@@ -1,45 +1,72 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev3 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev4 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: cuda Provides-Extra: cuda80 Provides-Extra: cuda90
-Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-Extra: cuda100 Provides-
-Extra: cuda101 Provides-Extra: cuda102 Provides-Extra: cuda110 Provides-Extra:
-cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113 Provides-Extra: cuda114
-Provides-Extra: cuda115 Provides-Extra: cuda116 Provides-Extra: cuda117
-Provides-Extra: cuda11x Provides-Extra: cuda-autodetect Provides-Extra:
-datasets Provides-Extra: torch Provides-Extra: tensorflow Provides-Extra: mxnet
-License-File: LICENSE _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# Thinc: A
-refreshing functional take on deep learning, compatible with your favorite
-libraries ### From the makers of [spaCy](https://spacy.io) and [Prodigy](https:
-//prodi.gy) [Thinc](https://thinc.ai) is a **lightweight deep learning
-library** that offers an elegant, type-checked, functional-programming API for
-**composing models**, with support for layers defined in other frameworks such
-as **PyTorch, TensorFlow and MXNet**. You can use Thinc as an interface layer,
-a standalone toolkit or a flexible way to develop new models. Previous versions
-of Thinc have been running quietly in production in thousands of companies, via
-both [spaCy](https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the
-new version to let users **compose, configure and deploy custom models** built
-with their favorite framework. [![Azure Pipelines](https://img.shields.io/
-azure-devops/build/explosion-ai/public/7/master.svg?logo=azure-
-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/
-_build?definitionId=7) [![Current Release Version](https://img.shields.io/
-github/v/release/explosion/
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: blis<0.8.0,>=0.7.8 Requires-Dist:
+murmurhash<1.1.0,>=1.0.2 Requires-Dist: cymem<2.1.0,>=2.0.2 Requires-Dist:
+preshed<3.1.0,>=3.0.2 Requires-Dist: wasabi<1.2.0,>=0.8.1 Requires-Dist:
+srsly<3.0.0,>=2.4.0 Requires-Dist: catalogue<2.1.0,>=2.0.4 Requires-Dist:
+confection<1.0.0,>=0.0.1 Requires-Dist: setuptools Requires-Dist:
+numpy>=1.15.0; python_version < "3.9" Requires-Dist: numpy>=1.19.0;
+python_version >= "3.9" Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
+Requires-Dist: packaging>=20.0 Requires-Dist: dataclasses<1.0,>=0.6;
+python_version < "3.7" Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1;
+python_version < "3.8" Requires-Dist: contextvars<3,>=2.4; python_version <
+"3.7" Provides-Extra: cuda Requires-Dist: cupy>=5.0.0b4; extra == "cuda"
+Provides-Extra: cuda80 Requires-Dist: cupy-cuda80>=5.0.0b4; extra == "cuda80"
+Provides-Extra: cuda90 Requires-Dist: cupy-cuda90>=5.0.0b4; extra == "cuda90"
+Provides-Extra: cuda91 Requires-Dist: cupy-cuda91>=5.0.0b4; extra == "cuda91"
+Provides-Extra: cuda92 Requires-Dist: cupy-cuda92>=5.0.0b4; extra == "cuda92"
+Provides-Extra: cuda100 Requires-Dist: cupy-cuda100>=5.0.0b4; extra ==
+"cuda100" Provides-Extra: cuda101 Requires-Dist: cupy-cuda101>=5.0.0b4; extra
+== "cuda101" Provides-Extra: cuda102 Requires-Dist: cupy-cuda102>=5.0.0b4;
+extra == "cuda102" Provides-Extra: cuda110 Requires-Dist: cupy-
+cuda110>=5.0.0b4; extra == "cuda110" Provides-Extra: cuda111 Requires-Dist:
+cupy-cuda111>=5.0.0b4; extra == "cuda111" Provides-Extra: cuda112 Requires-
+Dist: cupy-cuda112>=5.0.0b4; extra == "cuda112" Provides-Extra: cuda113
+Requires-Dist: cupy-cuda113>=5.0.0b4; extra == "cuda113" Provides-Extra:
+cuda114 Requires-Dist: cupy-cuda114>=5.0.0b4; extra == "cuda114" Provides-
+Extra: cuda115 Requires-Dist: cupy-cuda115>=5.0.0b4; extra == "cuda115"
+Provides-Extra: cuda116 Requires-Dist: cupy-cuda116>=5.0.0b4; extra ==
+"cuda116" Provides-Extra: cuda117 Requires-Dist: cupy-cuda117>=5.0.0b4; extra
+== "cuda117" Provides-Extra: cuda11x Requires-Dist: cupy-cuda11x>=11.0.0; extra
+== "cuda11x" Provides-Extra: cuda12x Requires-Dist: cupy-cuda12x>=11.5.0; extra
+== "cuda12x" Provides-Extra: cuda-autodetect Requires-Dist: cupy-wheel>=11.0.0;
+extra == "cuda-autodetect" Provides-Extra: datasets Requires-Dist:
+ml_datasets<0.3.0,>=0.2.0; extra == "datasets" Provides-Extra: torch Requires-
+Dist: torch>=1.6.0; extra == "torch" Provides-Extra: tensorflow Requires-Dist:
+tensorflow<2.6.0,>=2.0.0; extra == "tensorflow" Provides-Extra: mxnet Requires-
+Dist: mxnet<1.6.0,>=1.5.1; extra == "mxnet" _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
+_l_o_g_o_._s_v_g_]# Thinc: A refreshing functional take on deep learning, compatible
+with your favorite libraries ### From the makers of [spaCy](https://spacy.io)
+and [Prodigy](https://prodi.gy) [Thinc](https://thinc.ai) is a **lightweight
+deep learning library** that offers an elegant, type-checked, functional-
+programming API for **composing models**, with support for layers defined in
+other frameworks such as **PyTorch, TensorFlow and MXNet**. You can use Thinc
+as an interface layer, a standalone toolkit or a flexible way to develop new
+models. Previous versions of Thinc have been running quietly in production in
+thousands of companies, via both [spaCy](https://spacy.io) and [Prodigy](https:
+//prodi.gy). We wrote the new version to let users **compose, configure and
+deploy custom models** built with their favorite framework. [![tests](https://
+github.com/explosion/thinc/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/thinc/actions/workflows/tests.yml) [![Current Release
+Version](https://img.shields.io/github/v/release/explosion/
 thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)]
 (https://github.com/explosion/thinc/releases) [![PyPi Version](https://
 img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc) [![conda
 Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-
 square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
 thinc) [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
@@ -61,19 +88,19 @@
 `setuptools` and `wheel` are up to date. For the most recent releases, pip 19.3
 or newer is recommended. ```bash pip install -U pip setuptools wheel pip
 install thinc ``` See the [extended installation docs](https://thinc.ai/docs/
 install#extended) for details on optional dependencies for different backends
 and GPU. You might also want to [set up static type checking](https://thinc.ai/
 docs/install#type-checking) to take advantage of Thinc's type system. > â ï¸
 If you have installed PyTorch and you are using Python 3.7+, uninstall the >
-package `dataclasses` with `pip uninstall dataclasses`, since it may have >
-been installed by PyTorch and is incompatible with Python 3.7+. ### ð
-Selected examples and notebooks Also see the [`/examples`](examples) directory
-and [usage documentation](https://thinc.ai/docs) for more examples. Most
-examples are Jupyter notebooks â to launch them on [Google Colab](https://
+package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+. ### ð Selected
+examples and notebooks Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks â to launch them on [Google Colab](https://
 colab.research.google.com) (with GPU support!) click on the button next to the
 notebook name. | Notebook | Description | | -----------------------------------
 -------------------------------------------------------------------------------
 --- | -------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------- | | [`intro_to_thinc`]
 [intro_to_thinc]
```

### Comparing `thinc-9.0.0.dev3/README.md` & `thinc-9.0.0.dev4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Thinc: A refreshing functional take on deep learning, compatible with your favorite libraries
 
 ### From the makers of [spaCy](https://spacy.io) and [Prodigy](https://prodi.gy)
 
-[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers an elegant,
-type-checked, functional-programming API for **composing models**, with support
-for layers defined in other frameworks such as **PyTorch, TensorFlow and MXNet**. You
-can use Thinc as an interface layer, a standalone toolkit or a flexible way to
-develop new models. Previous versions of Thinc have been running quietly in
-production in thousands of companies, via both [spaCy](https://spacy.io) and
-[Prodigy](https://prodi.gy). We wrote the new version to let users **compose,
-configure and deploy custom models** built with their favorite framework.
+[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers
+an elegant, type-checked, functional-programming API for **composing models**,
+with support for layers defined in other frameworks such as **PyTorch,
+TensorFlow and MXNet**. You can use Thinc as an interface layer, a standalone
+toolkit or a flexible way to develop new models. Previous versions of Thinc have
+been running quietly in production in thousands of companies, via both
+[spaCy](https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the new
+version to let users **compose, configure and deploy custom models** built with
+their favorite framework.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/7/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=7)
+[![tests](https://github.com/explosion/thinc/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/thinc/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)](https://github.com/explosion/thinc/releases)
 [![PyPi Version](https://img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/thinc)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 [![Open demo in Colab][colab]][intro_to_thinc_colab]
 
 ## 🔥 Features
 
-- **Type-check** your model definitions with custom types and [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
+- **Type-check** your model definitions with custom types and
+  [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
 - Wrap **PyTorch**, **TensorFlow** and **MXNet** models for use in your network.
-- Concise **functional-programming** approach to model definition, using composition rather than inheritance.
+- Concise **functional-programming** approach to model definition, using
+  composition rather than inheritance.
 - Optional custom infix notation via **operator overloading**.
 - Integrated **config system** to describe trees of objects and hyperparameters.
 - Choice of **extensible backends**.
 - **[Read more &rarr;](https://thinc.ai/docs)**
 
 ## 🚀 Quickstart
 
-Thinc is compatible with **Python 3.6+** and runs on **Linux**,
-**macOS** and **Windows**. The latest releases with binary wheels are available from
+Thinc is compatible with **Python 3.6+** and runs on **Linux**, **macOS** and
+**Windows**. The latest releases with binary wheels are available from
 [pip](https://pypi.python.org/pypi/thinc). Before you install Thinc and its
 dependencies, make sure that your `pip`, `setuptools` and `wheel` are up to
 date. For the most recent releases, pip 19.3 or newer is recommended.
 
 ```bash
 pip install -U pip setuptools wheel
 pip install thinc
 ```
 
-See the [extended installation docs](https://thinc.ai/docs/install#extended) for details on optional dependencies for different backends and GPU. You might also want to [set up static type checking](https://thinc.ai/docs/install#type-checking) to take advantage of Thinc's type system.
+See the [extended installation docs](https://thinc.ai/docs/install#extended) for
+details on optional dependencies for different backends and GPU. You might also
+want to
+[set up static type checking](https://thinc.ai/docs/install#type-checking) to
+take advantage of Thinc's type system.
 
 > ⚠️ If you have installed PyTorch and you are using Python 3.7+, uninstall the
-> package `dataclasses` with `pip uninstall dataclasses`, since it may have
-> been installed by PyTorch and is incompatible with Python 3.7+.
+> package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+.
 
 ### 📓 Selected examples and notebooks
 
-Also see the [`/examples`](examples) directory and [usage documentation](https://thinc.ai/docs) for more examples. Most examples are Jupyter notebooks – to launch them on [Google Colab](https://colab.research.google.com) (with GPU support!) click on the button next to the notebook name.
+Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks – to launch them on
+[Google Colab](https://colab.research.google.com) (with GPU support!) click on
+the button next to the notebook name.
 
 | Notebook                                                                                                              | Description                                                                                                                                                                                       |
 | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [`intro_to_thinc`][intro_to_thinc]<br />[![Open in Colab][colab]][intro_to_thinc_colab]                               | Everything you need to know to get started. Composing and training a model on the MNIST data, using config files, registering custom functions and wrapping PyTorch, TensorFlow and MXNet models. |
 | [`transformers_tagger_bert`][transformers_tagger_bert]<br />[![Open in Colab][colab]][transformers_tagger_bert_colab] | How to use Thinc, `transformers` and PyTorch to train a part-of-speech tagger. From model definition and config to the training loop.                                                             |
 | [`pos_tagger_basic_cnn`][pos_tagger_basic_cnn]<br />[![Open in Colab][colab]][pos_tagger_basic_cnn_colab]             | Implementing and training a basic CNN for part-of-speech tagging model without external dependencies and using different levels of Thinc's config system.                                         |
 | [`parallel_training_ray`][parallel_training_ray]<br />[![Open in Colab][colab]][parallel_training_ray_colab]          | How to set up synchronous and asynchronous parameter server training with Thinc and [Ray](https://ray.readthedocs.io/en/latest/).                                                                 |
 
 **[View more &rarr;](examples)**
 
-[colab]: https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
+[colab]:
+  https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
 [intro_to_thinc]: examples/00_intro_to_thinc.ipynb
-[intro_to_thinc_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
+[intro_to_thinc_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
 [transformers_tagger_bert]: examples/02_transformers_tagger_bert.ipynb
-[transformers_tagger_bert_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
+[transformers_tagger_bert_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
 [pos_tagger_basic_cnn]: examples/03_pos_tagger_basic_cnn.ipynb
-[pos_tagger_basic_cnn_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
+[pos_tagger_basic_cnn_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
 [parallel_training_ray]: examples/04_parallel_training_ray.ipynb
-[parallel_training_ray_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
+[parallel_training_ray_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
 
 ### 📖 Documentation & usage guides
 
 | Documentation                                                                     | Description                                           |
 | --------------------------------------------------------------------------------- | ----------------------------------------------------- |
 | [Introduction](https://thinc.ai/docs)                                             | Everything you need to know.                          |
 | [Concept & Design](https://thinc.ai/docs/concept)                                 | Thinc's conceptual model and how it works.            |
@@ -99,15 +115,20 @@
 | [`thinc.schedules`](thinc/schedules.py)   | Generators for different rates, schedules, decays or series.                      |
 | [`thinc.backends`](thinc/backends)        | Backends for `numpy` and `cupy`.                                                  |
 | [`thinc.config`](thinc/config.py)         | Config parsing and validation and function registry system.                       |
 | [`thinc.util`](thinc/util.py)             | Utilities and helper functions.                                                   |
 
 ## 🐍 Development notes
 
-Thinc uses [`black`](https://github.com/psf/black) for auto-formatting, [`flake8`](http://flake8.pycqa.org/en/latest/) for linting and [`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is written compatible with **Python 3.6+**, with type hints wherever possible. See the [type reference](https://thinc.ai/docs/api-types) for more details on Thinc's custom types.
+Thinc uses [`black`](https://github.com/psf/black) for auto-formatting,
+[`flake8`](http://flake8.pycqa.org/en/latest/) for linting and
+[`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is
+written compatible with **Python 3.6+**, with type hints wherever possible. See
+the [type reference](https://thinc.ai/docs/api-types) for more details on
+Thinc's custom types.
 
 ### 👷‍♀️ Building Thinc from source
 
 Building Thinc from source requires the full dependencies listed in
 [`requirements.txt`](requirements.txt) to be installed. You'll also need a
 compiler to build the C extensions.
 
@@ -134,16 +155,20 @@
 export PYTHONPATH=`pwd`
 pip install -r requirements.txt
 python setup.py build_ext --inplace
 ```
 
 ### 🚦 Running tests
 
-Thinc comes with an [extensive test suite](thinc/tests). The following should all pass and not report any warnings or errors:
+Thinc comes with an [extensive test suite](thinc/tests). The following should
+all pass and not report any warnings or errors:
 
 ```bash
 python -m pytest thinc    # test suite
 python -m mypy thinc      # type checks
 python -m flake8 thinc    # linting
 ```
 
-To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim for a 100% test coverage. This doesn't mean that we meticulously write tests for every single line – we ignore blocks that are not relevant or difficult to test and make sure that the tests execute all code paths.
+To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim
+for a 100% test coverage. This doesn't mean that we meticulously write tests for
+every single line – we ignore blocks that are not relevant or difficult to test
+and make sure that the tests execute all code paths.
```

#### html2text {}

```diff
@@ -5,21 +5,21 @@
 type-checked, functional-programming API for **composing models**, with support
 for layers defined in other frameworks such as **PyTorch, TensorFlow and
 MXNet**. You can use Thinc as an interface layer, a standalone toolkit or a
 flexible way to develop new models. Previous versions of Thinc have been
 running quietly in production in thousands of companies, via both [spaCy]
 (https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the new version to
 let users **compose, configure and deploy custom models** built with their
-favorite framework. [![Azure Pipelines](https://img.shields.io/azure-devops/
-build/explosion-ai/public/7/master.svg?logo=azure-pipelines&style=flat-square)]
-(https://dev.azure.com/explosion-ai/public/_build?definitionId=7) [![Current
-Release Version](https://img.shields.io/github/v/release/explosion/
-thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)]
-(https://github.com/explosion/thinc/releases) [![PyPi Version](https://
-img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-
+favorite framework. [![tests](https://github.com/explosion/thinc/actions/
+workflows/tests.yml/badge.svg)](https://github.com/explosion/thinc/actions/
+workflows/tests.yml) [![Current Release Version](https://img.shields.io/github/
+v/release/explosion/thinc.svg?include_prereleases&sort=semver&style=flat-
+square&logo=github)](https://github.com/explosion/thinc/releases) [![PyPi
+Version](https://img.shields.io/pypi/v/
+thinc.svg?include_prereleases&sort=semver&style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc) [![conda
 Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-
 square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
 thinc) [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
 4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
 github.com/explosion/wheelwright/releases) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
@@ -38,19 +38,19 @@
 `setuptools` and `wheel` are up to date. For the most recent releases, pip 19.3
 or newer is recommended. ```bash pip install -U pip setuptools wheel pip
 install thinc ``` See the [extended installation docs](https://thinc.ai/docs/
 install#extended) for details on optional dependencies for different backends
 and GPU. You might also want to [set up static type checking](https://thinc.ai/
 docs/install#type-checking) to take advantage of Thinc's type system. > â ï¸
 If you have installed PyTorch and you are using Python 3.7+, uninstall the >
-package `dataclasses` with `pip uninstall dataclasses`, since it may have >
-been installed by PyTorch and is incompatible with Python 3.7+. ### ð
-Selected examples and notebooks Also see the [`/examples`](examples) directory
-and [usage documentation](https://thinc.ai/docs) for more examples. Most
-examples are Jupyter notebooks â to launch them on [Google Colab](https://
+package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+. ### ð Selected
+examples and notebooks Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks â to launch them on [Google Colab](https://
 colab.research.google.com) (with GPU support!) click on the button next to the
 notebook name. | Notebook | Description | | -----------------------------------
 -------------------------------------------------------------------------------
 --- | -------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------- | | [`intro_to_thinc`]
 [intro_to_thinc]
```

### Comparing `thinc-9.0.0.dev3/setup.cfg` & `thinc-9.0.0.dev4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 setup_requires = 
@@ -42,16 +43,17 @@
 	cymem>=2.0.2,<2.1.0
 	preshed>=3.0.2,<3.1.0
 	wasabi>=0.8.1,<1.2.0
 	srsly>=2.4.0,<3.0.0
 	catalogue>=2.0.4,<2.1.0
 	confection>=0.0.1,<1.0.0
 	setuptools
-	numpy>=1.15.0
-	pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
+	numpy>=1.15.0; python_version < "3.9"
+	numpy>=1.19.0; python_version >= "3.9"
+	pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0
 	packaging>=20.0
 	dataclasses>=0.6,<1.0; python_version < "3.7"
 	typing_extensions>=3.7.4.1,<4.5.0; python_version < "3.8"
 	contextvars>=2.4,<3; python_version < "3.7"
 
 [options.entry_points]
 pytest_randomly.random_seeder = 
@@ -88,14 +90,16 @@
 	cupy-cuda115>=5.0.0b4
 cuda116 = 
 	cupy-cuda116>=5.0.0b4
 cuda117 = 
 	cupy-cuda117>=5.0.0b4
 cuda11x = 
 	cupy-cuda11x>=11.0.0
+cuda12x = 
+	cupy-cuda12x>=11.5.0
 cuda-autodetect = 
 	cupy-wheel>=11.0.0
 datasets = 
 	ml_datasets>=0.2.0,<0.3.0
 torch = 
 	torch>=1.6.0
 tensorflow =
```

### Comparing `thinc-9.0.0.dev3/setup.py` & `thinc-9.0.0.dev4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 import sys
-import distutils.util
-from distutils.command.build_ext import build_ext
-from distutils.sysconfig import get_python_inc
+from setuptools.command.build_ext import build_ext
+from sysconfig import get_path
 from setuptools import Extension, setup, find_packages
 from pathlib import Path
 import numpy
 from Cython.Build import cythonize
 from Cython.Compiler import Options
 
 
@@ -16,52 +15,29 @@
 
 
 PACKAGES = find_packages()
 MOD_NAMES = [
     "thinc.backends.cblas",
     "thinc.backends.numpy_ops",
     "thinc.layers.sparselinear",
-    "thinc.layers.premap_ids"
+    "thinc.layers.premap_ids",
 ]
 COMPILE_OPTIONS = {
     "msvc": ["/Ox", "/EHsc"],
     "other": ["-O3", "-Wno-strict-prototypes", "-Wno-unused-function", "-std=c++11"],
 }
 COMPILER_DIRECTIVES = {
     "language_level": 3,
     "embedsignature": True,
     "annotation_typing": False,
+    "profile": sys.version_info < (3, 12),
 }
 LINK_OPTIONS = {"msvc": [], "other": []}
 
 
-def is_new_osx():
-    """Check whether we're on OSX >= 10.10"""
-    name = distutils.util.get_platform()
-    if sys.platform != "darwin":
-        return False
-    elif name.startswith("macosx-10"):
-        minor_version = int(name.split("-")[1].split(".")[1])
-        if minor_version >= 7:
-            return True
-        else:
-            return False
-    else:
-        return False
-
-
-if is_new_osx():
-    # On Mac, use libc++ because Apple deprecated use of libstdc
-    COMPILE_OPTIONS["other"].append("-stdlib=libc++")
-    LINK_OPTIONS["other"].append("-lc++")
-    # g++ (used by unix compiler on mac) links to libstdc++ as a default lib.
-    # See: https://stackoverflow.com/questions/1653047/avoid-linking-to-libstdc
-    LINK_OPTIONS["other"].append("-nodefaultlibs")
-
-
 # By subclassing build_extensions we have the actual compiler that will be used
 # which is really known only after finalize_options
 # http://stackoverflow.com/questions/724664/python-distutils-how-to-get-a-compiler-that-is-going-to-be-used
 class build_ext_options:
     def build_options(self):
         if hasattr(self.compiler, "initialize"):
             self.compiler.initialize()
@@ -94,15 +70,15 @@
     if len(sys.argv) > 1 and sys.argv[1] == "clean":
         return clean(root / "thinc")
 
     with (root / "thinc" / "about.py").open("r") as f:
         about = {}
         exec(f.read(), about)
 
-    include_dirs = [numpy.get_include(), get_python_inc(plat_specific=True)]
+    include_dirs = [numpy.get_include(), get_path("include")]
     ext_modules = []
     for name in MOD_NAMES:
         mod_path = name.replace(".", "/") + ".pyx"
         ext = Extension(name, [mod_path], language="c++", include_dirs=include_dirs)
         ext_modules.append(ext)
     print("Cythonizing sources")
     ext_modules = cythonize(
```

### Comparing `thinc-9.0.0.dev3/thinc/api.py` & `thinc-9.0.0.dev4/thinc/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,170 @@
-from .config import Config, registry, ConfigValidationError
-from .initializers import normal_init, uniform_init, glorot_uniform_init, zero_init
-from .initializers import configure_normal_init
-from .loss import CategoricalCrossentropy, L2Distance, CosineDistance
-from .loss import SequenceCategoricalCrossentropy
-from .model import Model, serialize_attr, deserialize_attr
-from .model import set_dropout_rate, change_attr_values, wrap_model_recursive
-from .shims import Shim, PyTorchGradScaler, PyTorchShim, TensorFlowShim, keras_model_fns
-from .shims import MXNetShim, TorchScriptShim, maybe_handshake_model
-from .optimizers import Adam, RAdam, SGD, Optimizer
-from .schedules import Schedule, cyclic_triangular, warmup_linear, constant
-from .schedules import constant_then, decaying, slanted_triangular, compounding
-from .schedules import plateau
-from .types import Ragged, Padded, ArgsKwargs, Unserializable
-from .util import fix_random_seed, is_cupy_array, set_active_gpu
-from .util import prefer_gpu, require_gpu, require_cpu
-from .util import DataValidationError, data_validation
-from .util import to_categorical, get_width, get_array_module, to_numpy
-from .util import torch2xp, xp2torch, tensorflow2xp, xp2tensorflow, mxnet2xp, xp2mxnet
-from .util import get_torch_default_device
-from .compat import has_cupy
-from .backends import get_ops, set_current_ops, get_current_ops, use_ops
-from .backends import Ops, CupyOps, MPSOps, NumpyOps, set_gpu_allocator
-from .backends import use_pytorch_for_gpu_memory, use_tensorflow_for_gpu_memory
-
-from .layers import Dropout, Embed, expand_window, HashEmbed, LayerNorm, Linear
-from .layers import Maxout, Mish, MultiSoftmax, Relu, softmax_activation, Softmax, LSTM
-from .layers import CauchySimilarity, ParametricAttention, Logistic
-from .layers import resizable, sigmoid_activation, Sigmoid, SparseLinear
-from .layers import SparseLinear_v2, ClippedLinear, ReluK, HardTanh, HardSigmoid
-from .layers import Dish, HardSwish, HardSwishMobilenet, Swish, Gelu
-from .layers import PyTorchWrapper, PyTorchRNNWrapper, PyTorchLSTM
-from .layers import TensorFlowWrapper, keras_subclass, MXNetWrapper
-from .layers import PyTorchWrapper_v2, Softmax_v2, PyTorchWrapper_v3
-from .layers import TorchScriptWrapper_v1, pytorch_to_torchscript_wrapper
-
-from .layers import add, bidirectional, chain, clone, concatenate, noop
-from .layers import residual, uniqued, siamese, list2ragged, ragged2list
-from .layers import map_list
-from .layers import with_array, with_array2d
-from .layers import with_padded, with_list, with_ragged, with_flatten
-from .layers import with_reshape, with_getitem, strings2arrays, list2array
-from .layers import list2ragged, ragged2list, list2padded, padded2list
-from .layers import remap_ids, remap_ids_v2, premap_ids
-from .layers import array_getitem, with_cpu, with_debug, with_nvtx_range
-from .layers import with_signpost_interval
-from .layers import tuplify, with_flatten_v2
-
-from .layers import reduce_first, reduce_last, reduce_max, reduce_mean, reduce_sum
-
+from .backends import (
+    CupyOps,
+    MPSOps,
+    NumpyOps,
+    Ops,
+    get_current_ops,
+    get_ops,
+    set_current_ops,
+    set_gpu_allocator,
+    use_ops,
+    use_pytorch_for_gpu_memory,
+    use_tensorflow_for_gpu_memory,
+)
+from .compat import enable_mxnet, enable_tensorflow, has_cupy
+from .config import Config, ConfigValidationError, registry
+from .initializers import (
+    configure_normal_init,
+    glorot_uniform_init,
+    normal_init,
+    uniform_init,
+    zero_init,
+)
+from .layers import (
+    LSTM,
+    CauchySimilarity,
+    ClippedLinear,
+    Dish,
+    Dropout,
+    Embed,
+    Gelu,
+    HardSigmoid,
+    HardSwish,
+    HardSwishMobilenet,
+    HardTanh,
+    HashEmbed,
+    LayerNorm,
+    Linear,
+    Logistic,
+    Maxout,
+    Mish,
+    MultiSoftmax,
+    MXNetWrapper,
+    ParametricAttention,
+    ParametricAttention_v2,
+    PyTorchLSTM,
+    PyTorchRNNWrapper,
+    PyTorchWrapper,
+    PyTorchWrapper_v2,
+    PyTorchWrapper_v3,
+    Relu,
+    ReluK,
+    Sigmoid,
+    Softmax,
+    Softmax_v2,
+    SparseLinear,
+    SparseLinear_v2,
+    Swish,
+    TensorFlowWrapper,
+    TorchScriptWrapper_v1,
+    add,
+    array_getitem,
+    bidirectional,
+    chain,
+    clone,
+    concatenate,
+    expand_window,
+    keras_subclass,
+    list2array,
+    list2padded,
+    list2ragged,
+    map_list,
+    noop,
+    padded2list,
+    premap_ids,
+    pytorch_to_torchscript_wrapper,
+    ragged2list,
+    reduce_first,
+    reduce_last,
+    reduce_max,
+    reduce_mean,
+    reduce_sum,
+    remap_ids,
+    remap_ids_v2,
+    residual,
+    resizable,
+    siamese,
+    sigmoid_activation,
+    softmax_activation,
+    strings2arrays,
+    tuplify,
+    uniqued,
+    with_array,
+    with_array2d,
+    with_cpu,
+    with_debug,
+    with_flatten,
+    with_flatten_v2,
+    with_getitem,
+    with_list,
+    with_nvtx_range,
+    with_padded,
+    with_ragged,
+    with_reshape,
+    with_signpost_interval,
+)
+from .loss import (
+    CategoricalCrossentropy,
+    CosineDistance,
+    L2Distance,
+    SequenceCategoricalCrossentropy,
+)
+from .model import (
+    Model,
+    change_attr_values,
+    deserialize_attr,
+    serialize_attr,
+    set_dropout_rate,
+    wrap_model_recursive,
+)
+from .optimizers import SGD, Adam, Optimizer, RAdam
+from .schedules import (
+    Schedule,
+    compounding,
+    constant,
+    constant_then,
+    cyclic_triangular,
+    decaying,
+    plateau,
+    slanted_triangular,
+    warmup_linear,
+)
+from .shims import (
+    MXNetShim,
+    PyTorchGradScaler,
+    PyTorchShim,
+    Shim,
+    TensorFlowShim,
+    TorchScriptShim,
+    keras_model_fns,
+    maybe_handshake_model,
+)
+from .types import ArgsKwargs, Padded, Ragged, Unserializable
+from .util import (
+    DataValidationError,
+    data_validation,
+    fix_random_seed,
+    get_array_module,
+    get_torch_default_device,
+    get_width,
+    is_cupy_array,
+    mxnet2xp,
+    prefer_gpu,
+    require_cpu,
+    require_gpu,
+    set_active_gpu,
+    tensorflow2xp,
+    to_categorical,
+    to_numpy,
+    torch2xp,
+    xp2mxnet,
+    xp2tensorflow,
+    xp2torch,
+)
 
 # fmt: off
 __all__ = [
     # .config
     "Config", "registry", "ConfigValidationError",
     # .initializers
     "normal_init", "uniform_init", "glorot_uniform_init", "zero_init",
@@ -76,14 +189,16 @@
     "fix_random_seed", "is_cupy_array", "set_active_gpu",
     "prefer_gpu", "require_gpu", "require_cpu",
     "DataValidationError", "data_validation",
     "to_categorical", "get_width", "get_array_module", "to_numpy",
     "torch2xp", "xp2torch", "tensorflow2xp", "xp2tensorflow", "mxnet2xp", "xp2mxnet",
     "get_torch_default_device",
     # .compat
+    "enable_mxnet",
+    "enable_tensorflow",
     "has_cupy",
     # .backends
     "get_ops", "set_current_ops", "get_current_ops", "use_ops",
     "Ops", "CupyOps", "MPSOps", "NumpyOps", "set_gpu_allocator",
     "use_pytorch_for_gpu_memory", "use_tensorflow_for_gpu_memory",
     # .layers
     "Dropout", "Embed", "expand_window", "HashEmbed", "LayerNorm", "Linear",
@@ -91,15 +206,15 @@
     "CauchySimilarity", "ParametricAttention", "Logistic",
     "resizable", "sigmoid_activation", "Sigmoid", "SparseLinear",
     "ClippedLinear", "ReluK", "HardTanh", "HardSigmoid",
     "Dish", "HardSwish", "HardSwishMobilenet", "Swish", "Gelu",
     "PyTorchWrapper", "PyTorchRNNWrapper", "PyTorchLSTM",
     "TensorFlowWrapper", "keras_subclass", "MXNetWrapper",
     "PyTorchWrapper_v2", "Softmax_v2", "PyTorchWrapper_v3",
-    "SparseLinear_v2", "TorchScriptWrapper_v1",
+    "SparseLinear_v2", "TorchScriptWrapper_v1", "ParametricAttention_v2",
 
     "add", "bidirectional", "chain", "clone", "concatenate", "noop",
     "residual", "uniqued", "siamese", "list2ragged", "ragged2list",
     "map_list",
     "with_array", "with_array2d",
     "with_padded", "with_list", "with_ragged", "with_flatten",
     "with_reshape", "with_getitem", "strings2arrays", "list2array",
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/__init__.py` & `thinc-9.0.0.dev4/thinc/backends/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import contextlib
-from typing import Type, Dict, Any, Callable, Optional, cast
-
-from contextvars import ContextVar
 import threading
+from contextvars import ContextVar
+from typing import Any, Callable, Dict, Optional, Type, cast
 
-from .ops import Ops
-from .cupy_ops import CupyOps
-from .numpy_ops import NumpyOps
-from .mps_ops import MPSOps
-from ._cupy_allocators import cupy_tensorflow_allocator, cupy_pytorch_allocator
-from ._param_server import ParamServer
-from ..util import assert_tensorflow_installed, assert_pytorch_installed
-from ..util import get_torch_default_device, is_cupy_array, require_cpu
 from .. import registry
 from ..compat import cupy, has_cupy
-
+from ..util import (
+    assert_pytorch_installed,
+    assert_tensorflow_installed,
+    get_torch_default_device,
+    is_cupy_array,
+    require_cpu,
+)
+from ._cupy_allocators import cupy_pytorch_allocator, cupy_tensorflow_allocator
+from ._param_server import ParamServer
+from .cupy_ops import CupyOps
+from .mps_ops import MPSOps
+from .numpy_ops import NumpyOps
+from .ops import Ops
 
 context_ops: ContextVar[Optional[Ops]] = ContextVar("context_ops", default=None)
 context_pools: ContextVar[dict] = ContextVar("context_pools", default={})
 
 # Internal use of thread-local storage only for detecting cases where a Jupyter
 # notebook might not have preserved contextvars across cells.
 _GLOBAL_STATE = {"ops": None}
 
+# Thread-local state.
+_LOCAL_STATE = threading.local()
+
 
 def set_gpu_allocator(allocator: str) -> None:  # pragma: no cover
     """Route GPU memory allocation via PyTorch or tensorflow.
     Raise an error if the given argument does not match either of the two.
     """
     if allocator == "pytorch":
         use_pytorch_for_gpu_memory()
@@ -145,30 +151,22 @@
     current_ops = context_ops.get()
     thread_ops = _get_thread_state().ops
     if type(current_ops) == type(thread_ops):
         return True
     return False
 
 
-def _get_thread_state():
+def _get_thread_state() -> threading.local:
     """Get a thread-specific state variable that inherits from a global
     state when it's created."""
-    thread: threading.Thread = threading.current_thread()
-    if not hasattr(thread, "__local"):
-        thread.__local = _create_thread_local(_GLOBAL_STATE)
-    return thread.__local
-
-
-def _create_thread_local(
-    attrs: Dict[str, Any], local_class: Type[threading.local] = threading.local
-):
-    obj = local_class()
-    for name, value in attrs.items():
-        setattr(obj, name, value)
-    return obj
+    if not hasattr(_LOCAL_STATE, "initialized") or not _LOCAL_STATE.initialized:
+        for name, value in _GLOBAL_STATE.items():
+            setattr(_LOCAL_STATE, name, value)
+        _LOCAL_STATE.initialized = True
+    return _LOCAL_STATE
 
 
 __all__ = [
     "set_current_ops",
     "get_current_ops",
     "use_ops",
     "ParamServer",
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/_cupy_allocators.py` & `thinc-9.0.0.dev4/thinc/backends/_cupy_allocators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import cast
 
+from ..compat import cupy, tensorflow, torch
 from ..types import ArrayXd
 from ..util import get_torch_default_device, tensorflow2xp
-from ..compat import torch, cupy, tensorflow
 
 
 def cupy_tensorflow_allocator(size_in_bytes: int):
     """Function that can be passed into cupy.cuda.set_allocator, to have cupy
     allocate memory via TensorFlow. This is important when using the two libraries
     together, as otherwise OOM errors can occur when there's available memory
     sitting in the other library's pool.
     """
     size_in_bytes = max(1024, size_in_bytes)
-    tensor = tensorflow.zeros((size_in_bytes // 4,), dtype=tensorflow.dtypes.float32)
+    tensor = tensorflow.zeros((size_in_bytes // 4,), dtype=tensorflow.dtypes.float32)  # type: ignore
     # We convert to cupy via dlpack, so that we can get a memory pointer.
     cupy_array = cast(ArrayXd, tensorflow2xp(tensor))
     address = int(cupy_array.data)
     # cupy has a neat class to help us here. Otherwise it will try to free.
     memory = cupy.cuda.memory.UnownedMemory(address, size_in_bytes, cupy_array)
     # Now return a new memory pointer.
     return cupy.cuda.memory.MemoryPointer(memory, 0)
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/_custom_kernels.cu` & `thinc-9.0.0.dev4/thinc/backends/_custom_kernels.cu`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,33 @@
                 X[(x_start * I) + i];
         }
     }
 }
 
 
 template <typename T>
+__global__ void pad(T* out, T const **seqs, int const *lengths, int stride, int N, int L)
+{
+    int _loop_start = blockIdx.x * blockDim.x + threadIdx.x;
+    int _loop_stride = blockDim.x * gridDim.x;
+
+    for (int i = _loop_start; i < L * stride; i += _loop_stride) {
+        for (int j = 0; j < N; ++j) {
+            T const *seq = seqs[j];
+            if (i < lengths[j] * stride) {
+                out[j * L * stride + i] = seq[i];
+            } else {
+                out[j * L * stride + i] = T();
+            }
+        }
+    }
+}
+
+
+template <typename T>
 __global__ void maxout(T* best, int* which, const T* cands, int B, int O, int P)
 {
     int _loop_start = blockIdx.x * blockDim.x + threadIdx.x;
     int _loop_stride = blockDim.x * gridDim.x;
     for (int bo = _loop_start; bo < B * O; bo += _loop_stride)
     {
         // Go to the candidates at the output we're working on
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/_custom_kernels.py` & `thinc-9.0.0.dev4/thinc/backends/_custom_kernels.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from typing import Optional, Tuple
+import operator
 import re
-from pathlib import Path
 from collections import defaultdict
-from ..compat import cupy, has_cupy_gpu
+from functools import reduce
+from pathlib import Path
+from typing import Callable, Optional, Tuple
 
+import numpy
+
+from ..compat import cupy, has_cupy_gpu
 
 PWD = Path(__file__).parent
 KERNELS_SRC = (PWD / "_custom_kernels.cu").read_text(encoding="utf8")
 KERNELS_LIST = [
     "backprop_clipped_linear<double>",
     "backprop_clipped_linear<float>",
     "backprop_dish<double>",
@@ -40,14 +44,18 @@
     "gather_add<float>",
     "gelu<double>",
     "gelu<float>",
     "maxout<double>",
     "maxout<float>",
     "mish<double>",
     "mish<float>",
+    "pad<double>",
+    "pad<float>",
+    "pad<int>",
+    "pad<long long>",
     "reduce_max<double>",
     "reduce_max<float>",
     "reduce_sum<double>",
     "reduce_sum<float>",
     "seq2col<double>",
     "seq2col<float>",
     "swish<double>",
@@ -58,82 +66,114 @@
         code=KERNELS_SRC, options=("--std=c++11",), name_expressions=KERNELS_LIST
     )
     if has_cupy_gpu
     else None
 )
 
 
-def _get_kernel(name):
-    """A small wrapper around KERNELS.get_function that verifies first that
-    compiler kernels are available (cupy is installed)."""
-    if KERNELS is None:
-        return None
-    else:
-        return KERNELS.get_function(name)
+class LazyKernel:
+    """Wraps around `cupy.RawModule` and `cupy.RawKernel` to verify CuPy availability
+    and lazily compile the latter on first invocation.
+
+    The default CuPy behaviour triggers the compilation as soon as the `cupy.RawKernel` object
+    is accessed."""
+
+    name: str
+    _kernel: Optional["cupy.RawKernel"]
+    _compile_callback: Optional[Callable[[], "cupy.RawKernel"]]
+
+    __slots__ = ["name", "_kernel", "_compile_callback"]
+
+    def __init__(
+        self,
+        name: str,
+        *,
+        compile_callback: Optional[Callable[[], "cupy.RawKernel"]] = None,
+    ) -> None:
+        self.name = name
+        self._kernel = None
+        self._compile_callback = compile_callback
+
+    def __call__(self, *args, **kwargs):
+        self._compile_kernel()
+        self._kernel(*args, **kwargs)
+
+    def _compile_kernel(self):
+        if self._kernel is not None:
+            return
+
+        if self._compile_callback is not None:
+            self._kernel = self._compile_callback()
+        elif KERNELS is not None:
+            self._kernel = KERNELS.get_function(self.name)
+
+        if self._kernel is None:
+            raise ValueError(f"couldn't compile Cupy kernel '{self.name}'")
 
 
-def compile_mmh(src):
+def compile_mmh():
     if not has_cupy_gpu:
         return None
-    return cupy.RawKernel(src, "hash_data")
-
-
-MMH_SRC = (PWD / "_murmur3.cu").read_text(encoding="utf8")
+    return cupy.RawKernel((PWD / "_murmur3.cu").read_text(encoding="utf8"), "hash_data")
 
 
-clipped_linear_kernel_float = _get_kernel("clipped_linear<float>")
-clipped_linear_kernel_double = _get_kernel("clipped_linear<double>")
-dish_kernel_float = _get_kernel("dish<float>")
-dish_kernel_double = _get_kernel("dish<double>")
-gather_add_kernel_float = _get_kernel("gather_add<float>")
-gather_add_kernel_double = _get_kernel("gather_add<double>")
-gelu_kernel_float = _get_kernel("gelu<float>")
-gelu_kernel_double = _get_kernel("gelu<double>")
-hash_data_kernel = compile_mmh(MMH_SRC)
-maxout_kernel_float = _get_kernel("maxout<float>")
-maxout_kernel_double = _get_kernel("maxout<double>")
-mish_kernel_float = _get_kernel("mish<float>")
-mish_kernel_double = _get_kernel("mish<double>")
-reduce_max_kernel_float = _get_kernel("reduce_max<float>")
-reduce_max_kernel_double = _get_kernel("reduce_max<double>")
-reduce_sum_kernel_float = _get_kernel("reduce_sum<float>")
-reduce_sum_kernel_double = _get_kernel("reduce_sum<double>")
-seq2col_kernel_float = _get_kernel("seq2col<float>")
-seq2col_kernel_double = _get_kernel("seq2col<double>")
-swish_kernel_float = _get_kernel("swish<float>")
-swish_kernel_double = _get_kernel("swish<double>")
-
-backprop_clipped_linear_kernel_double = _get_kernel("backprop_clipped_linear<double>")
-backprop_clipped_linear_kernel_float = _get_kernel("backprop_clipped_linear<float>")
-backprop_dish_kernel_double = _get_kernel("backprop_dish<double>")
-backprop_dish_kernel_float = _get_kernel("backprop_dish<float>")
-backprop_gelu_kernel_double = _get_kernel("backprop_gelu<double>")
-backprop_gelu_kernel_float = _get_kernel("backprop_gelu<float>")
-backprop_hard_swish_kernel_double = _get_kernel("backprop_hard_swish<double>")
-backprop_hard_swish_kernel_float = _get_kernel("backprop_hard_swish<float>")
-backprop_hard_swish_mobilenet_kernel_double = _get_kernel(
+clipped_linear_kernel_float = LazyKernel("clipped_linear<float>")
+clipped_linear_kernel_double = LazyKernel("clipped_linear<double>")
+dish_kernel_float = LazyKernel("dish<float>")
+dish_kernel_double = LazyKernel("dish<double>")
+gather_add_kernel_float = LazyKernel("gather_add<float>")
+gather_add_kernel_double = LazyKernel("gather_add<double>")
+gelu_kernel_float = LazyKernel("gelu<float>")
+gelu_kernel_double = LazyKernel("gelu<double>")
+hash_data_kernel = LazyKernel("hash_data", compile_callback=compile_mmh)
+maxout_kernel_float = LazyKernel("maxout<float>")
+maxout_kernel_double = LazyKernel("maxout<double>")
+mish_kernel_float = LazyKernel("mish<float>")
+mish_kernel_double = LazyKernel("mish<double>")
+pad_kernel_float = LazyKernel("pad<float>")
+pad_kernel_double = LazyKernel("pad<double>")
+pad_kernel_int32 = LazyKernel("pad<int>")
+pad_kernel_int64 = LazyKernel("pad<long long>")
+reduce_max_kernel_float = LazyKernel("reduce_max<float>")
+reduce_max_kernel_double = LazyKernel("reduce_max<double>")
+reduce_sum_kernel_float = LazyKernel("reduce_sum<float>")
+reduce_sum_kernel_double = LazyKernel("reduce_sum<double>")
+seq2col_kernel_float = LazyKernel("seq2col<float>")
+seq2col_kernel_double = LazyKernel("seq2col<double>")
+swish_kernel_float = LazyKernel("swish<float>")
+swish_kernel_double = LazyKernel("swish<double>")
+
+backprop_clipped_linear_kernel_double = LazyKernel("backprop_clipped_linear<double>")
+backprop_clipped_linear_kernel_float = LazyKernel("backprop_clipped_linear<float>")
+backprop_dish_kernel_double = LazyKernel("backprop_dish<double>")
+backprop_dish_kernel_float = LazyKernel("backprop_dish<float>")
+backprop_gelu_kernel_double = LazyKernel("backprop_gelu<double>")
+backprop_gelu_kernel_float = LazyKernel("backprop_gelu<float>")
+backprop_hard_swish_kernel_double = LazyKernel("backprop_hard_swish<double>")
+backprop_hard_swish_kernel_float = LazyKernel("backprop_hard_swish<float>")
+backprop_hard_swish_mobilenet_kernel_double = LazyKernel(
     "backprop_hard_swish_mobilenet<double>"
 )
-backprop_hard_swish_mobilenet_kernel_float = _get_kernel(
+backprop_hard_swish_mobilenet_kernel_float = LazyKernel(
     "backprop_hard_swish_mobilenet<float>"
 )
-backprop_maxout_kernel_double = _get_kernel("backprop_maxout<double>")
-backprop_maxout_kernel_float = _get_kernel("backprop_maxout<float>")
-backprop_mish_kernel_double = _get_kernel("backprop_mish<double>")
-backprop_mish_kernel_float = _get_kernel("backprop_mish<float>")
-backprop_reduce_max_kernel_double = _get_kernel("backprop_reduce_max<double>")
-backprop_reduce_max_kernel_float = _get_kernel("backprop_reduce_max<float>")
-backprop_reduce_mean_kernel_double = _get_kernel("backprop_reduce_mean<double>")
-backprop_reduce_mean_kernel_float = _get_kernel("backprop_reduce_mean<float>")
-backprop_reduce_sum_kernel_double = _get_kernel("backprop_reduce_sum<double>")
-backprop_reduce_sum_kernel_float = _get_kernel("backprop_reduce_sum<float>")
-backprop_seq2col_kernel_double = _get_kernel("backprop_seq2col<double>")
-backprop_seq2col_kernel_float = _get_kernel("backprop_seq2col<float>")
-backprop_swish_kernel_double = _get_kernel("backprop_swish<double>")
-backprop_swish_kernel_float = _get_kernel("backprop_swish<float>")
+backprop_maxout_kernel_double = LazyKernel("backprop_maxout<double>")
+backprop_maxout_kernel_float = LazyKernel("backprop_maxout<float>")
+backprop_mish_kernel_double = LazyKernel("backprop_mish<double>")
+backprop_mish_kernel_float = LazyKernel("backprop_mish<float>")
+backprop_reduce_max_kernel_double = LazyKernel("backprop_reduce_max<double>")
+backprop_reduce_max_kernel_float = LazyKernel("backprop_reduce_max<float>")
+backprop_reduce_mean_kernel_double = LazyKernel("backprop_reduce_mean<double>")
+backprop_reduce_mean_kernel_float = LazyKernel("backprop_reduce_mean<float>")
+backprop_reduce_sum_kernel_double = LazyKernel("backprop_reduce_sum<double>")
+backprop_reduce_sum_kernel_float = LazyKernel("backprop_reduce_sum<float>")
+backprop_seq2col_kernel_double = LazyKernel("backprop_seq2col<double>")
+backprop_seq2col_kernel_float = LazyKernel("backprop_seq2col<float>")
+backprop_swish_kernel_double = LazyKernel("backprop_swish<double>")
+backprop_swish_kernel_float = LazyKernel("backprop_swish<float>")
 
 
 def _alloc(shape, dtype, *, zeros: bool = True):
     if zeros:
         return cupy.zeros(shape, dtype)
     else:
         return cupy.empty(shape, dtype)
@@ -142,14 +182,73 @@
 def _alloc_like(array, zeros: bool = True):
     if zeros:
         return cupy.zeros_like(array)
     else:
         return cupy.empty_like(array)
 
 
+def pad(seqs, round_to=1, *, threads_per_block=128, num_blocks=128):
+    if round_to < 1:
+        raise ValueError(f"Rounding for padding must at least be 1, was: {round_to}")
+    for seq in seqs:
+        _is_float_or_int_array(seq)
+
+    seq_lens = [len(seq) for seq in seqs]
+    max_seq_len = max(seq_lens)
+    # Round the length to nearest bucket -- helps on GPU, to make similar
+    # array sizes.
+    max_seq_len += -max_seq_len % round_to
+    seq_lens = cupy.array(seq_lens, dtype="int32")
+    final_shape = (len(seqs), max_seq_len) + seqs[0].shape[1:]
+    out = cupy.empty(final_shape, dtype=seqs[0].dtype)
+
+    # Extract pointers from CuPy arrays, so that we can address
+    # them in the CUDA kernel.
+    ptrs = numpy.empty(
+        (
+            len(
+                seqs,
+            )
+        ),
+        "int64",
+    )
+    for idx, seq in enumerate(seqs):
+        ptrs[idx] = seq.data.ptr
+    ptrs = cupy.array(ptrs)
+
+    stride = reduce(operator.mul, seqs[0].shape[1:], 1)
+
+    if out.dtype == "float32":
+        pad_kernel_float(
+            (num_blocks,),
+            (threads_per_block,),
+            (out, ptrs, seq_lens, stride, len(seqs), max_seq_len),
+        )
+    elif out.dtype == "float64":
+        pad_kernel_double(
+            (num_blocks,),
+            (threads_per_block,),
+            (out, ptrs, seq_lens, stride, len(seqs), max_seq_len),
+        )
+    elif out.dtype == "int32":
+        pad_kernel_int32(
+            (num_blocks,),
+            (threads_per_block,),
+            (out, ptrs, seq_lens, stride, len(seqs), max_seq_len),
+        )
+    elif out.dtype == "int64":
+        pad_kernel_int64(
+            (num_blocks,),
+            (threads_per_block,),
+            (out, ptrs, seq_lens, stride, len(seqs), max_seq_len),
+        )
+
+    return out
+
+
 def clipped_linear(
     X,
     *,
     inplace=False,
     slope=1.0,
     offset=0.0,
     min_val=0.0,
@@ -717,14 +816,26 @@
         "float64",
     ), "CUDA kernel can only handle float32 and float64"
     if shape is not None and out.shape != shape:
         msg = f"array has incorrect shape, expected: {shape}, was: {out.shape}"
         raise ValueError(msg)
 
 
+def _is_float_or_int_array(out, *, shape: Optional[Tuple] = None):
+    assert out.dtype in (
+        "float32",
+        "float64",
+        "int32",
+        "int64",
+    ), "CUDA kernel can only handle float32, float64, int32 and int64"
+    if shape is not None and out.shape != shape:
+        msg = f"array has incorrect shape, expected: {shape}, was: {out.shape}"
+        raise ValueError(msg)
+
+
 def _check_lengths(lengths, n_elems: int, *, min_length=0):
     assert lengths.dtype == "int32", "lengths should be encoded as 32-bit integers"
     if not cupy.all(lengths >= min_length):
         raise ValueError(f"all sequence lengths must be >= {min_length}")
     if cupy.sum(lengths) != n_elems:
         raise IndexError("lengths must sum up to the batch size")
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/_murmur3.cu` & `thinc-9.0.0.dev4/thinc/backends/_murmur3.cu`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/backends/_param_server.py` & `thinc-9.0.0.dev4/thinc/backends/_param_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Dict, Tuple, Optional, Any
+from typing import Any, Dict, Optional, Tuple
 
 from ..types import FloatsXd
 from ..util import get_array_module
 
-
 KeyT = Tuple[int, str]
 
 
 class ParamServer:
     """Serve parameters for a single process."""
 
     _params: Dict[KeyT, FloatsXd] = {}
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/cblas.pxd` & `thinc-9.0.0.dev4/thinc/backends/cblas.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from libcpp.memory cimport shared_ptr
 
-
 ctypedef void (*sgemm_ptr)(bint transA, bint transB, int M, int N, int K,
                            float alpha, const float* A, int lda, const float* B,
                            int ldb, float beta, float* C, int ldc) nogil
 ctypedef void (*dgemm_ptr)(bint transA, bint transB, int M, int N, int K,
                            double alpha, const double* A, int lda, const double* B,
                            int ldb, double beta, double* C, int ldc) nogil
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/cblas.pyx` & `thinc-9.0.0.dev4/thinc/backends/cblas.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# cython: profile=False
 cimport blis.cy
 from cython.operator cimport dereference as deref
 from libcpp.memory cimport make_shared
 
 
 # Single- and double-precision wrappers for `blis.cy.scalv`
 cdef void blis_sscal(int N, float alpha, float* X, int incX) nogil:
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/cpu_kernels.hh` & `thinc-9.0.0.dev4/thinc/backends/cpu_kernels.hh`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/backends/cupy_ops.py` & `thinc-9.0.0.dev4/thinc/backends/cupy_ops.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import numpy
+
 from .. import registry
-from .ops import Ops
-from .numpy_ops import NumpyOps
-from . import _custom_kernels
-from ..types import DeviceTypes
-from ..util import torch2xp, tensorflow2xp, mxnet2xp
-from ..util import is_cupy_array
-from ..util import is_torch_cuda_array, is_tensorflow_gpu_array, is_mxnet_gpu_array
 from ..compat import cupy, cupyx
+from ..types import DeviceTypes
+from ..util import (
+    is_cupy_array,
+    is_mxnet_gpu_array,
+    is_tensorflow_gpu_array,
+    is_torch_cuda_array,
+    mxnet2xp,
+    tensorflow2xp,
+    torch2xp,
+)
+from . import _custom_kernels
+from .numpy_ops import NumpyOps
+from .ops import Ops
 
 
 @registry.ops("CupyOps")
 class CupyOps(Ops):
     name = "cupy"
     xp = cupy
     _xp2 = cupyx
@@ -83,21 +90,47 @@
         elif is_torch_cuda_array(data):
             array = torch2xp(data)
         elif is_tensorflow_gpu_array(data):
             array = tensorflow2xp(data)
         elif is_mxnet_gpu_array(data):
             array = mxnet2xp(data)
         else:
-            array = self.xp.array(data)
+            array = self.xp.array(data, dtype=dtype)
 
         if dtype is not None:
             array = array.astype(dtype=dtype, copy=False)
 
         return array
 
+    def pad(self, seqs, round_to=1):
+        """Perform padding on a list of arrays so that they each have the same
+        length, by taking the maximum dimension across each axis. This only
+        works on non-empty sequences with the same `ndim` and `dtype`.
+        """
+        # TODO: This should be generalized to handle different ranks
+        if not seqs:
+            raise ValueError("Cannot pad empty sequence")
+        if len(set(seq.ndim for seq in seqs)) != 1:
+            raise ValueError("Cannot pad sequences with different ndims")
+        if len(set(seq.dtype for seq in seqs)) != 1:
+            raise ValueError("Cannot pad sequences with different dtypes")
+        if len(set(seq.shape[1:] for seq in seqs)) != 1:
+            raise ValueError("Cannot pad sequences that differ on other dimensions")
+
+        # Our CUDA kernel can currently only handle C contiguous arrays.
+        if not all(seq.flags["C_CONTIGUOUS"] for seq in seqs) or seqs[0].dtype not in (
+            "float32",
+            "float64",
+            "int32",
+            "int64",
+        ):
+            return super().pad(seqs, round_to)
+
+        return _custom_kernels.pad(seqs, round_to)
+
     def maxout(self, X):
         if X.dtype in ("float32", "float64"):
             return _custom_kernels.maxout(X)
         else:
             return super().maxout(X)
 
     def backprop_maxout(self, dY, which, P):
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/mps_ops.py` & `thinc-9.0.0.dev4/thinc/backends/mps_ops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import TYPE_CHECKING
+
 import numpy
 
 from .. import registry
-from . import NumpyOps, Ops
+from .numpy_ops import NumpyOps
+from .ops import Ops
 
 if TYPE_CHECKING:
     # Type checking does not work with dynamic base classes, since MyPy cannot
     # determine against which base class to check. So, always derive from Ops
     # during type checking.
     _Ops = Ops
 else:
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/numpy_ops.pxd` & `thinc-9.0.0.dev4/thinc/backends/numpy_ops.pxd`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/backends/numpy_ops.pyx` & `thinc-9.0.0.dev4/thinc/backends/numpy_ops.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # cython: cdivision=True
 # cython: infer_types=True
-# cython: profile=True
-from typing import Optional
 from collections.abc import Sized
+from typing import Optional
+
 import numpy
 
 cimport cython
-from libc.string cimport memcpy, memset
-from libc.stdlib cimport calloc, malloc, free
-from libc.stdint cimport uint32_t, uint64_t
-from libc.string cimport memcpy
-from libc.math cimport isnan
+cimport numpy as np
 from cymem.cymem cimport Pool
-from preshed.maps cimport PreshMap
+from libc.math cimport isnan
+from libc.stdint cimport uint32_t, uint64_t
+from libc.stdlib cimport calloc, free, malloc
+from libc.string cimport memcpy, memset
 from murmurhash.mrmr cimport hash64
-cimport numpy as np
+from preshed.maps cimport PreshMap
 
 from .. import registry
+from ..types import ArrayXd, DeviceTypes, DTypes, Shape
 from ..util import copy_array, get_array_module
-from ..types import DeviceTypes, DTypes, Shape, ArrayXd
-from .cblas cimport CBlas, daxpy, saxpy, sgemm, dgemm, sscal
-from .ops import Ops, _split_weights, _transpose_weights, _untranspose_unsplit_weights
+
+from .cblas cimport CBlas, daxpy, dgemm, saxpy, sgemm, sscal
+
 from ..compat import has_blis
+from .ops import Ops, _split_weights, _transpose_weights, _untranspose_unsplit_weights
 
 
 cdef extern from "math.h":
     float logf(float x) nogil
     float sqrtf(float x) nogil
     float expf(float x) nogil
     float tanhf(float x) nogil
@@ -56,15 +57,15 @@
             array = data
         elif hasattr(data, 'numpy'):
             # Handles PyTorch Tensor
             array = data.numpy()
         elif hasattr(data, "get"):
             array = data.get()
         else:
-            array = self.xp.array(data)
+            array = self.xp.array(data, dtype=dtype)
 
         if dtype is not None:
             array = array.astype(dtype=dtype, copy=False)
 
         return array
 
 
@@ -335,16 +336,19 @@
         return keys
 
     def reduce_mean(self, reals2d_ft X, int[::1] lengths):
         cdef int B = lengths.shape[0]
         cdef int O = X.shape[1]
         cdef int T = X.shape[0]
 
-        assert B != 0
-        assert O != 0
+        if B == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(B, O), dtype="float32")
+            else:
+                return numpy.zeros(shape=(B, O), dtype="float64")
 
         cdef np.ndarray means
         if reals2d_ft is float2d_t:
             means = numpy.zeros(shape=(B, O), dtype="float32")
             cpu_reduce_mean(<float *>means.data, &X[0, 0], &lengths[0], B, T, O)
         else:
             means = numpy.zeros(shape=(B, O), dtype="float64")
@@ -358,16 +362,19 @@
         cdef int T = 0
 
         for length in lengths[:B]:
             if length < 0:
                 raise ValueError(f"all sequence lengths must be >= 0, got {length}")
             T += length
 
-        assert T != 0
-        assert O != 0
+        if T == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(T, O), dtype="float32")
+            else:
+                return numpy.zeros(shape=(T, O), dtype="float64")
 
         cdef np.ndarray dX
         if reals2d_ft is float2d_t:
             dX = numpy.zeros((T, O), dtype="float32")
             cpu_backprop_reduce_mean(<float *>dX.data, &d_means[0,0], &lengths[0], B, T, O)
         else:
             dX = numpy.zeros((T, O), dtype="float64")
@@ -376,16 +383,19 @@
         return dX
 
     def reduce_sum(self, reals2d_ft X, int[::1] lengths):
         cdef int B = lengths.shape[0]
         cdef int O = X.shape[1]
         cdef int T = X.shape[0]
 
-        assert B != 0
-        assert O != 0
+        if B == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(B, O), dtype="float32")
+            else:
+                return numpy.zeros(shape=(B, O), dtype="float64")
 
         cdef np.ndarray sums
         if reals2d_ft is float2d_t:
             sums = numpy.zeros(shape=(B, O), dtype="float32")
             cpu_reduce_sum(<float *>sums.data, &X[0, 0], &lengths[0], B, T, O)
         else:
             sums = numpy.zeros(shape=(B, O), dtype="float64")
@@ -399,16 +409,19 @@
         cdef int T = 0
 
         for length in lengths[:B]:
             if length < 0:
                 raise ValueError(f"all sequence lengths must be >= 0, got {length}")
             T += length
 
-        assert T != 0
-        assert O != 0
+        if T == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(T, O), dtype="float32")
+            else:
+                return numpy.zeros(shape=(T, O), dtype="float64")
 
         cdef np.ndarray dX
         if reals2d_ft is float2d_t:
             dX = numpy.zeros((T, O), dtype="float32")
             cpu_backprop_reduce_sum(<float *>dX.data, &d_sums[0,0], &lengths[0], B, T, O)
         else:
             dX = numpy.zeros((T, O), dtype="float64")
@@ -417,20 +430,24 @@
         return dX
 
     def reduce_max(self, reals2d_ft X, int[::1] lengths):
         cdef int B = lengths.shape[0]
         cdef int O = X.shape[1]
         cdef int T = X.shape[0]
 
-        assert B != 0
-        assert O != 0
-
-        cdef np.ndarray maxes
         # Needs to be zero-initialized as we start by assuming that the first element is the max value.
         cdef np.ndarray which = self.alloc(shape=(B, O), dtype="i", zeros=True)
+
+        if B == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(B, O), dtype="float32"), which
+            else:
+                return numpy.zeros(shape=(B, O), dtype="float64"), which
+
+        cdef np.ndarray maxes
         if reals2d_ft is float2d_t:
             maxes = self.alloc(shape=(B, O), dtype="float32", zeros=False)
             cpu_reduce_max(<float*>maxes.data, <int*>which.data, &X[0, 0], &lengths[0], B, T, O)
         else:
             maxes = self.alloc(shape=(B, O), dtype="float64", zeros=False)
             cpu_reduce_max(<double*>maxes.data, <int*>which.data, &X[0, 0], &lengths[0], B, T, O)
 
@@ -442,16 +459,19 @@
         cdef int T = 0
 
         for length in lengths[:B]:
             if length <= 0:
                 raise ValueError(f"all sequence lengths must be > 0, got {length}")
             T += length
 
-        assert T != 0
-        assert O != 0
+        if T == 0 or O == 0:
+            if reals2d_ft is float2d_t:
+                return numpy.zeros(shape=(T, O), dtype="float32")
+            else:
+                return numpy.zeros(shape=(T, O), dtype="float64")
 
         cdef np.ndarray dX
         if reals2d_ft is float2d_t:
             dX = numpy.zeros((T, O), dtype="float32")
             cpu_backprop_reduce_max(<float *>dX.data, &d_maxes[0,0], &which[0, 0],
                 &lengths[0], B, T, O)
         else:
```

### Comparing `thinc-9.0.0.dev3/thinc/backends/ops.py` & `thinc-9.0.0.dev4/thinc/backends/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,57 @@
+import itertools
 import math
+from typing import (
+    Any,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
 
-from typing import Optional, List, Tuple, Sequence, Type, Union, cast, TypeVar
-from typing import Iterator, overload, Any
 import numpy
-import itertools
 
-from ..types import Xp, Shape, DTypes, DTypesInt, DTypesFloat, List2d, ArrayXd
-from ..types import Floats1d, Floats2d, Floats3d, Floats4d
-from ..types import Array1d, Array2d, Array3d, Array4d, ListXd
-from ..types import FloatsXd, Ints1d, Ints2d, Ints3d, Ints4d, IntsXd, _Floats
-from ..types import FloatsXdT
-from ..types import DeviceTypes, Generator, Padded, Batchable, SizedGenerator
+from ..types import (
+    Array1d,
+    Array2d,
+    Array3d,
+    Array4d,
+    ArrayXd,
+    Batchable,
+    DeviceTypes,
+    DTypes,
+    DTypesFloat,
+    DTypesInt,
+    Floats1d,
+    Floats2d,
+    Floats3d,
+    Floats4d,
+    FloatsXd,
+    FloatsXdT,
+    Generator,
+    Ints1d,
+    Ints2d,
+    Ints3d,
+    Ints4d,
+    IntsXd,
+    List2d,
+    ListXd,
+    Padded,
+    Shape,
+    SizedGenerator,
+    Xp,
+    _Floats,
+)
 from ..util import get_array_module, is_xp_array, to_numpy
-
 from .cblas import CBlas
 
 ArrayT = TypeVar("ArrayT", bound=ArrayXd)
 FloatsT = TypeVar("FloatsT", bound=_Floats)
 SQRT2PI = math.sqrt(2.0 / math.pi)
 INV_SQRT2 = 1.0 / math.sqrt(2.0)
 INV_SQRT_2PI = 1.0 / math.sqrt(2.0 * math.pi)
@@ -354,29 +389,34 @@
     def pad(  # noqa: F811
         self, seqs: Union[List[Ints2d], List[Floats2d]], round_to=1
     ) -> Array3d:
         """Perform padding on a list of arrays so that they each have the same
         length, by taking the maximum dimension across each axis. This only
         works on non-empty sequences with the same `ndim` and `dtype`.
         """
+        if round_to < 1:
+            raise ValueError(
+                f"Rounding for padding must at least be 1, was: {round_to}"
+            )
+
         # TODO: This should be generalized to handle different ranks
         if not seqs:
             raise ValueError("Cannot pad empty sequence")
         if len(set(seq.ndim for seq in seqs)) != 1:
             raise ValueError("Cannot pad sequences with different ndims")
         if len(set(seq.dtype for seq in seqs)) != 1:
             raise ValueError("Cannot pad sequences with different dtypes")
         if len(set(seq.shape[1:] for seq in seqs)) != 1:
             raise ValueError("Cannot pad sequences that differ on other dimensions")
         # Find the maximum dimension along each axis. That's what we'll pad to.
-        length = max(len(seq) for seq in seqs)
+        max_seq_len = max(len(seq) for seq in seqs)
         # Round the length to nearest bucket -- helps on GPU, to make similar
         # array sizes.
-        length = (length + (round_to - 1)) // round_to * round_to
-        final_shape = (len(seqs), length) + seqs[0].shape[1:]
+        max_seq_len += -max_seq_len % round_to
+        final_shape = (len(seqs), max_seq_len) + seqs[0].shape[1:]
         output: Array3d = cast(Array3d, self.alloc(final_shape, dtype=seqs[0].dtype))
         for i, arr in enumerate(seqs):
             # It's difficult to convince this that the dtypes will match.
             output[i, : arr.shape[0]] = arr  # type: ignore[assignment, call-overload]
         return output
 
     def unpad(self, padded: Array3d, lengths: List[int]) -> List2d:
@@ -1245,25 +1285,27 @@
                 Y[i] = X[start : start + length].max(axis=0)
             start += length
         return Y, which
 
     def backprop_reduce_first(
         self, d_firsts: Floats2d, starts_ends: Ints1d
     ) -> Floats2d:
-        if starts_ends.size < 2:
-            raise ValueError(f"starts_ends should least have size 2")
+        if starts_ends.size == 0:
+            return self.alloc2f(0, d_firsts.shape[1], dtype=d_firsts.dtype, zeros=True)
+        elif starts_ends.size == 1:
+            raise ValueError(f"starts_ends must not have size 1")
         dX = self.alloc2f(
             int(starts_ends[-1]), d_firsts.shape[1], dtype=d_firsts.dtype, zeros=True
         )
         dX[starts_ends[:-1]] = d_firsts
         return dX
 
     def backprop_reduce_last(self, d_lasts: Floats2d, lasts: Ints1d) -> Floats2d:
-        if lasts.size < 1:
-            raise ValueError(f"lasts should least have size 2")
+        if lasts.size == 0:
+            return self.alloc2f(0, d_lasts.shape[1], dtype=d_lasts.dtype, zeros=True)
         dX = self.alloc2f(
             int(lasts[-1]) + 1, d_lasts.shape[1], dtype=d_lasts.dtype, zeros=True
         )
         dX[lasts] = d_lasts
         return dX
 
     def backprop_reduce_sum(self, d_sums: Floats2d, lengths: Ints1d) -> Floats2d:
```

### Comparing `thinc-9.0.0.dev3/thinc/config.py` & `thinc-9.0.0.dev4/thinc/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import catalogue
 import confection
-from confection import Config, ConfigValidationError, Promise, VARIABLE_RE
+from confection import VARIABLE_RE, Config, ConfigValidationError, Promise
+
 from .types import Decorator
 
 
 class registry(confection.registry):
     # fmt: off
     optimizers: Decorator = catalogue.create("thinc", "optimizers", entry_points=True)
     schedules: Decorator = catalogue.create("thinc", "schedules", entry_points=True)
```

### Comparing `thinc-9.0.0.dev3/thinc/initializers.py` & `thinc-9.0.0.dev4/thinc/initializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Callable, cast
+
 import numpy
 
 from .backends import Ops
 from .config import registry
 from .types import FloatsXd, Shape
 from .util import partial
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/__init__.py` & `thinc-9.0.0.dev4/thinc/layers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 # Weights layers
+# Combinators
+from .add import add
+
+# Array manipulation
+from .array_getitem import array_getitem
+from .bidirectional import bidirectional
 from .cauchysimilarity import CauchySimilarity
+from .chain import chain
+from .clipped_linear import ClippedLinear, HardSigmoid, HardTanh, ReluK
+from .clone import clone
+from .concatenate import concatenate
 from .dish import Dish
 from .dropout import Dropout
 from .embed import Embed
 from .expand_window import expand_window
+from .gelu import Gelu
+from .hard_swish import HardSwish
+from .hard_swish_mobilenet import HardSwishMobilenet
 from .hashembed import HashEmbed
 from .layernorm import LayerNorm
 from .linear import Linear
-from .lstm import LSTM, PyTorchLSTM
+
+# Data-type transfers
+from .list2array import list2array
+from .list2padded import list2padded
+from .list2ragged import list2ragged
 from .logistic import Logistic
+from .lstm import LSTM, PyTorchLSTM
+from .map_list import map_list
 from .maxout import Maxout
 from .mish import Mish
 from .multisoftmax import MultiSoftmax
-from .parametricattention import ParametricAttention
-from .pytorchwrapper import PyTorchWrapper, PyTorchWrapper_v2, PyTorchWrapper_v3
-from .pytorchwrapper import PyTorchRNNWrapper
-from .relu import Relu
-from .clipped_linear import ClippedLinear, ReluK, HardSigmoid, HardTanh
-from .hard_swish import HardSwish
-from .hard_swish_mobilenet import HardSwishMobilenet
-from .swish import Swish
-from .gelu import Gelu
-from .resizable import resizable
-from .sigmoid_activation import sigmoid_activation
-from .sigmoid import Sigmoid
-from .softmax_activation import softmax_activation
-from .softmax import Softmax, Softmax_v2
-from .sparselinear import SparseLinear, SparseLinear_v2
-from .tensorflowwrapper import TensorFlowWrapper, keras_subclass
-from .torchscriptwrapper import TorchScriptWrapper_v1, pytorch_to_torchscript_wrapper
 from .mxnetwrapper import MXNetWrapper
-
-# Combinators
-from .add import add
-from .bidirectional import bidirectional
-from .chain import chain
-from .clone import clone
-from .concatenate import concatenate
-from .map_list import map_list
 from .noop import noop
-from .residual import residual
-from .uniqued import uniqued
-from .siamese import siamese
-from .tuplify import tuplify
+from .padded2list import padded2list
+from .parametricattention import ParametricAttention
+from .parametricattention_v2 import ParametricAttention_v2
+from .premap_ids import premap_ids
+from .pytorchwrapper import (
+    PyTorchRNNWrapper,
+    PyTorchWrapper,
+    PyTorchWrapper_v2,
+    PyTorchWrapper_v3,
+)
+from .ragged2list import ragged2list
 
 # Pooling
 from .reduce_first import reduce_first
 from .reduce_last import reduce_last
 from .reduce_max import reduce_max
 from .reduce_mean import reduce_mean
 from .reduce_sum import reduce_sum
-
-# Array manipulation
-from .array_getitem import array_getitem
-
-# Data-type transfers
-from .list2array import list2array
-from .list2ragged import list2ragged
-from .list2padded import list2padded
-from .ragged2list import ragged2list
-from .padded2list import padded2list
+from .relu import Relu
 from .remap_ids import remap_ids, remap_ids_v2
-from .premap_ids import premap_ids
+from .residual import residual
+from .resizable import resizable
+from .siamese import siamese
+from .sigmoid import Sigmoid
+from .sigmoid_activation import sigmoid_activation
+from .softmax import Softmax, Softmax_v2
+from .softmax_activation import softmax_activation
+from .sparselinear import SparseLinear, SparseLinear_v2
 from .strings2arrays import strings2arrays
+from .swish import Swish
+from .tensorflowwrapper import TensorFlowWrapper, keras_subclass
+from .torchscriptwrapper import TorchScriptWrapper_v1, pytorch_to_torchscript_wrapper
+from .tuplify import tuplify
+from .uniqued import uniqued
 from .with_array import with_array
 from .with_array2d import with_array2d
 from .with_cpu import with_cpu
+from .with_debug import with_debug
 from .with_flatten import with_flatten
 from .with_flatten_v2 import with_flatten_v2
-from .with_padded import with_padded
+from .with_getitem import with_getitem
 from .with_list import with_list
+from .with_nvtx_range import with_nvtx_range
+from .with_padded import with_padded
 from .with_ragged import with_ragged
 from .with_reshape import with_reshape
-from .with_getitem import with_getitem
-from .with_debug import with_debug
-from .with_nvtx_range import with_nvtx_range
 from .with_signpost_interval import with_signpost_interval
 
-
 # fmt: off
 __all__ = [
     "CauchySimilarity",
     "Linear",
     "Dropout",
     "Embed",
     "expand_window",
     "HashEmbed",
     "LayerNorm",
     "LSTM",
     "Maxout",
     "Mish",
     "MultiSoftmax",
     "ParametricAttention",
+    "ParametricAttention_v2",
     "PyTorchLSTM",
     "PyTorchWrapper",
     "PyTorchWrapper_v2",
     "PyTorchWrapper_v3",
     "PyTorchRNNWrapper",
     "Relu",
     "sigmoid_activation",
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/add.py` & `thinc-9.0.0.dev4/thinc/layers/add.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Any, Tuple, Callable, Optional, TypeVar, Dict
+from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import ArrayXd, XY_XY_OutT
 from ..util import get_width
 
-
 InT = TypeVar("InT", bound=Any)
 OutT = TypeVar("OutT", bound=ArrayXd)
 
 
 @registry.layers("add.v1")
 def add(
     layer1: Model[InT, OutT], layer2: Model[InT, OutT], *layers: Model
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/array_getitem.py` & `thinc-9.0.0.dev4/thinc/layers/array_getitem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Union, Sequence, Tuple, TypeVar
-from ..types import ArrayXd, FloatsXd, IntsXd
-from ..model import Model
+from typing import Sequence, Tuple, TypeVar, Union
 
+from ..model import Model
+from ..types import ArrayXd, FloatsXd, IntsXd
 
 AxisIndex = Union[int, slice, Sequence[int]]
 Index = Union[AxisIndex, Tuple[AxisIndex, ...]]
 ArrayTXd = TypeVar("ArrayTXd", bound=ArrayXd)
 
 
 def array_getitem(index: Index) -> Model[ArrayTXd, ArrayTXd]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/bidirectional.py` & `thinc-9.0.0.dev4/thinc/layers/bidirectional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Optional, Tuple, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..backends import Ops
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Padded
 
-
 InT = Padded
 OutT = Padded
 
 
 @registry.layers("bidirectional.v1")
 def bidirectional(
     l2r: Model[InT, OutT], r2l: Optional[Model[InT, OutT]] = None
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/cauchysimilarity.py` & `thinc-9.0.0.dev4/thinc/layers/cauchysimilarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats1d, Floats2d
 from ..util import get_width
 
-
 InT = Tuple[Floats2d, Floats2d]
 OutT = Floats1d
 
 
 @registry.layers("CauchySimilarity.v1")
 def CauchySimilarity(nI: Optional[int] = None) -> Model[InT, OutT]:
     """Compare input vectors according to the Cauchy similarity function proposed by
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/chain.py` & `thinc-9.0.0.dev4/thinc/layers/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, Callable, Optional, TypeVar, Any, Dict, List, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
-from ..util import get_width
+from ..model import Model
 from ..types import XY_YZ_OutT
-
+from ..util import get_width
 
 InT = TypeVar("InT")
 MidT = TypeVar("MidT")
 OutT = TypeVar("OutT")
 
 # Keep this function so we can provide variable arguments via the config
 @registry.layers("chain.v1")
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/clipped_linear.py` & `thinc-9.0.0.dev4/thinc/layers/clipped_linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import glorot_uniform_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import glorot_uniform_init, zero_init
+from .layernorm import LayerNorm
 
 
 @registry.layers("ClippedLinear.v1")
 def ClippedLinear(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/clone.py` & `thinc-9.0.0.dev4/thinc/layers/clone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import TypeVar, cast, List
+from typing import List, TypeVar, cast
 
-from .noop import noop
-from .chain import chain
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
+from .chain import chain
+from .noop import noop
 
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
 
 
 @registry.layers("clone.v1")
 def clone(orig: Model[InT, OutT], n: int) -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/concatenate.py` & `thinc-9.0.0.dev4/thinc/layers/concatenate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-from typing import Any, List, Tuple, Callable, Optional
-from typing import TypeVar, cast, Dict, Union, Sequence
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
 from ..backends import NumpyOps
-from ..model import Model
 from ..config import registry
-from ..types import Array2d, Ragged
+from ..model import Model
+from ..types import Array2d, Ragged, XY_XY_OutT
 from ..util import get_width
 from .noop import noop
-from ..types import XY_XY_OutT
-
 
 NUMPY_OPS = NumpyOps()
 
 
 InT = TypeVar("InT", bound=Any)
 OutT = TypeVar("OutT", bound=Union[Array2d, Sequence[Array2d], Ragged])
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/dish.py` & `thinc-9.0.0.dev4/thinc/layers/swish.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import he_normal_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import he_normal_init, zero_init
+from .layernorm import LayerNorm
 
 
-@registry.layers("Dish.v1")
-def Dish(
+@registry.layers("Swish.v1")
+def Swish(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
     dropout: Optional[float] = None,
     normalize: bool = False,
 ) -> Model[Floats2d, Floats2d]:
     if init_W is None:
         init_W = he_normal_init
     if init_b is None:
         init_b = zero_init
     model: Model[Floats2d, Floats2d] = Model(
-        "dish",
+        "swish",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
     if normalize:
         model = chain(model, LayerNorm(nI=nO))
@@ -40,18 +40,18 @@
 
 def forward(
     model: Model[Floats2d, Floats2d], X: Floats2d, is_train: bool
 ) -> Tuple[Floats2d, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
     Y_preact = model.ops.affine(X, W, b)
-    Y = model.ops.dish(Y_preact)
+    Y = model.ops.swish(Y_preact)
 
     def backprop(dY: Floats2d) -> Floats2d:
-        dY = model.ops.backprop_dish(dY, X, inplace=False)
+        dY = model.ops.backprop_swish(dY, Y_preact, Y, inplace=False)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/dropout.py` & `thinc-9.0.0.dev4/thinc/layers/dropout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, Callable, List, TypeVar, cast, Union, Sequence
+from typing import Callable, List, Sequence, Tuple, TypeVar, Union, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import ArrayXd, Ragged, Padded
-
+from ..model import Model
+from ..types import ArrayXd, Padded, Ragged
 
 InT = TypeVar("InT", bound=Union[ArrayXd, Sequence[ArrayXd], Ragged, Padded])
 
 
 @registry.layers("Dropout.v1")
 def Dropout(rate: float = 0.0) -> Model[InT, InT]:
     """Help prevent overfitting by adding a random distortion to the input data
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/embed.py` & `thinc-9.0.0.dev4/thinc/layers/embed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Dict, Callable, Tuple, Optional, Union, cast, TypeVar
+from typing import Callable, Dict, Optional, Tuple, TypeVar, Union, cast
 
-from .chain import chain
-from .array_getitem import ints_getitem
-from ..model import Model
 from ..config import registry
-from ..types import Ints1d, Ints2d, Floats1d, Floats2d
 from ..initializers import uniform_init
+from ..model import Model
+from ..types import Floats1d, Floats2d, Ints1d, Ints2d
 from ..util import get_width, partial
-
+from .array_getitem import ints_getitem
+from .chain import chain
 
 InT = TypeVar("InT", bound=Union[Ints1d, Ints2d])
 OutT = Floats2d
 
 
 @registry.layers("Embed.v1")
 def Embed(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/expand_window.py` & `thinc-9.0.0.dev4/thinc/layers/expand_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, TypeVar, Callable, Union, cast
+from typing import Callable, Tuple, TypeVar, Union, cast
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d, Ragged
 
-
 InT = TypeVar("InT", Floats2d, Ragged)
 
 
 @registry.layers("expand_window.v1")
 def expand_window(window_size: int = 1) -> Model[InT, InT]:
     """For each vector in an input, construct an output vector that contains the
     input and a window of surrounding vectors. This is one step in a convolution.
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/gelu.py` & `thinc-9.0.0.dev4/thinc/layers/gelu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import he_normal_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import he_normal_init, zero_init
+from .layernorm import LayerNorm
 
 
 @registry.layers("Gelu.v1")
 def Gelu(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/hard_swish.py` & `thinc-9.0.0.dev4/thinc/layers/dish.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import he_normal_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import he_normal_init, zero_init
+from .layernorm import LayerNorm
 
 
-@registry.layers("HardSwish.v1")
-def HardSwish(
+@registry.layers("Dish.v1")
+def Dish(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
     dropout: Optional[float] = None,
     normalize: bool = False,
 ) -> Model[Floats2d, Floats2d]:
     if init_W is None:
         init_W = he_normal_init
     if init_b is None:
         init_b = zero_init
     model: Model[Floats2d, Floats2d] = Model(
-        "hardswish",
+        "dish",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
     if normalize:
         model = chain(model, LayerNorm(nI=nO))
@@ -40,18 +40,18 @@
 
 def forward(
     model: Model[Floats2d, Floats2d], X: Floats2d, is_train: bool
 ) -> Tuple[Floats2d, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
     Y_preact = model.ops.affine(X, W, b)
-    Y = model.ops.hard_swish(Y_preact)
+    Y = model.ops.dish(Y_preact)
 
     def backprop(dY: Floats2d) -> Floats2d:
-        dY = model.ops.backprop_hard_swish(dY, Y_preact, inplace=False)
+        dY = model.ops.backprop_dish(dY, X, inplace=False)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/hard_swish_mobilenet.py` & `thinc-9.0.0.dev4/thinc/layers/hard_swish.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import he_normal_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import he_normal_init, zero_init
+from .layernorm import LayerNorm
 
 
-@registry.layers("HardSwishMobilenet.v1")
-def HardSwishMobilenet(
+@registry.layers("HardSwish.v1")
+def HardSwish(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
     dropout: Optional[float] = None,
     normalize: bool = False,
 ) -> Model[Floats2d, Floats2d]:
     if init_W is None:
         init_W = he_normal_init
     if init_b is None:
         init_b = zero_init
     model: Model[Floats2d, Floats2d] = Model(
-        "hardswishmobilenet",
+        "hardswish",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
     if normalize:
         model = chain(model, LayerNorm(nI=nO))
@@ -40,18 +40,18 @@
 
 def forward(
     model: Model[Floats2d, Floats2d], X: Floats2d, is_train: bool
 ) -> Tuple[Floats2d, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
     Y_preact = model.ops.affine(X, W, b)
-    Y = model.ops.hard_swish_mobilenet(Y_preact)
+    Y = model.ops.hard_swish(Y_preact)
 
     def backprop(dY: Floats2d) -> Floats2d:
-        dY = model.ops.backprop_hard_swish_mobilenet(dY, Y_preact, inplace=False)
+        dY = model.ops.backprop_hard_swish(dY, Y_preact, inplace=False)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/hashembed.py` & `thinc-9.0.0.dev4/thinc/layers/hashembed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Callable, Dict, Tuple, Optional, Any, Union, cast, TypeVar
+from typing import Any, Callable, Dict, Optional, Tuple, TypeVar, Union, cast
 
-from .chain import chain
-from .array_getitem import ints_getitem
-from ..model import Model
 from ..config import registry
-from ..types import Floats1d, Floats2d, Ints2d, Ints1d
 from ..initializers import uniform_init
+from ..model import Model
+from ..types import Floats1d, Floats2d, Ints1d, Ints2d
 from ..util import partial
-
+from .array_getitem import ints_getitem
+from .chain import chain
 
 InT = TypeVar("InT", bound=Union[Ints1d, Ints2d])
 OutT = Floats2d
 
 
 @registry.layers("HashEmbed.v1")
 def HashEmbed(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/layernorm.py` & `thinc-9.0.0.dev4/thinc/layers/layernorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
+from ..backends import Ops
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d
-from ..backends import Ops
 from ..util import get_width
 
-
 InT = Floats2d
 
 
 @registry.layers("LayerNorm.v1")
 def LayerNorm(nI: Optional[int] = None) -> Model[InT, InT]:
     return Model(
         "layernorm",
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/linear.py` & `thinc-9.0.0.dev4/thinc/layers/relu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,58 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Floats1d, Floats2d
 from ..initializers import glorot_uniform_init, zero_init
+from ..model import Model
+from ..types import Floats1d, Floats2d
 from ..util import get_width, partial
-
+from .chain import chain
+from .dropout import Dropout
+from .layernorm import LayerNorm
 
 InT = Floats2d
 OutT = Floats2d
 
 
-@registry.layers("Linear.v1")
-def Linear(
+@registry.layers("Relu.v1")
+def Relu(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
+    dropout: Optional[float] = None,
+    normalize: bool = False,
 ) -> Model[InT, OutT]:
-    """Multiply inputs by a weights matrix and adds a bias vector."""
     if init_W is None:
         init_W = glorot_uniform_init
     if init_b is None:
         init_b = zero_init
-    return Model(
-        "linear",
+    model: Model[InT, OutT] = Model(
+        "relu",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
+    if normalize:
+        model = chain(model, LayerNorm(nI=nO))
+    if dropout is not None:
+        model = chain(model, cast(Model[Floats2d, Floats2d], Dropout(dropout)))
+    return model
 
 
 def forward(model: Model[InT, OutT], X: InT, is_train: bool) -> Tuple[OutT, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
-    Y = model.ops.gemm(X, W, trans2=True)
-    Y += b
+    Y = model.ops.affine(X, W, b)
+    Y = model.ops.relu(Y)
 
     def backprop(dY: OutT) -> InT:
+        dY = model.ops.backprop_relu(dY, Y)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/list2array.py` & `thinc-9.0.0.dev4/thinc/layers/list2array.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, TypeVar, List
+from typing import Callable, List, Tuple, TypeVar
 
 from ..backends import NumpyOps
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Array2d
 
-
 NUMPY_OPS = NumpyOps()
 
 
 OutT = TypeVar("OutT", bound=Array2d)
 InT = List[OutT]
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/list2padded.py` & `thinc-9.0.0.dev4/thinc/layers/list2padded.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, Callable, TypeVar, cast
+from typing import Callable, Tuple, TypeVar, cast
 
-from ..types import Padded, List2d
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
+from ..types import List2d, Padded
 
 InT = TypeVar("InT", bound=List2d)
 OutT = Padded
 
 
 @registry.layers("list2padded.v1")
 def list2padded() -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/list2ragged.py` & `thinc-9.0.0.dev4/thinc/layers/list2ragged.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, List, Callable, cast, TypeVar
+from typing import Callable, List, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import ListXd, ArrayXd, Ragged
-
+from ..model import Model
+from ..types import ArrayXd, ListXd, Ragged
 
 InT = TypeVar("InT", bound=ListXd)
 OutT = Ragged
 
 
 @registry.layers("list2ragged.v1")
 def list2ragged() -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/logistic.py` & `thinc-9.0.0.dev4/thinc/layers/logistic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, Callable
+from typing import Callable, Tuple
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d
 
-
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("Logistic.v1")
 def Logistic() -> Model[InT, OutT]:
     """Deprecated in favor of `sigmoid_activation` layer, for more consistent
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/lstm.py` & `thinc-9.0.0.dev4/thinc/layers/lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Tuple, Callable, cast
 from functools import partial
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
+from ..backends import Ops
 from ..config import registry
-from ..util import get_width
+from ..initializers import glorot_uniform_init, zero_init
+from ..model import Model
 from ..types import Floats1d, Floats2d, Floats4d, Padded, Ragged
+from ..util import get_width
 from .noop import noop
-from ..initializers import glorot_uniform_init, zero_init
-from ..backends import Ops
 
 
 @registry.layers("LSTM.v1")
 def LSTM(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
@@ -41,16 +41,17 @@
 
 
 @registry.layers("PyTorchLSTM.v1")
 def PyTorchLSTM(
     nO: int, nI: int, *, bi: bool = False, depth: int = 1, dropout: float = 0.0
 ) -> Model[Padded, Padded]:
     import torch.nn
-    from .with_padded import with_padded
+
     from .pytorchwrapper import PyTorchRNNWrapper
+    from .with_padded import with_padded
 
     if depth == 0:
         return noop()  # type: ignore[misc]
     nH = nO
     if bi:
         nH = nO // 2
     pytorch_rnn = PyTorchRNNWrapper(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/map_list.py` & `thinc-9.0.0.dev4/thinc/layers/map_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Callable, TypeVar, List, Tuple, Optional
-from ..model import Model
+from typing import Callable, List, Optional, Tuple, TypeVar
 
+from ..model import Model
 
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
 
 
 def map_list(layer: Model[InT, OutT]) -> Model[List[InT], List[OutT]]:
     """Create a model that maps a child layer across list inputs."""
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/maxout.py` & `thinc-9.0.0.dev4/thinc/layers/maxout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
 from ..config import registry
 from ..initializers import glorot_uniform_init, zero_init
+from ..model import Model
 from ..types import Floats2d
 from ..util import get_width, partial
+from .chain import chain
 from .dropout import Dropout
 from .layernorm import LayerNorm
-from .chain import chain
-
 
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("Maxout.v1")
 def Maxout(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/mish.py` & `thinc-9.0.0.dev4/thinc/layers/mish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
-from ..initializers import glorot_uniform_init, zero_init
 from ..config import registry
+from ..initializers import glorot_uniform_init, zero_init
+from ..model import Model
 from ..types import Floats1d, Floats2d
 from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-
+from .layernorm import LayerNorm
 
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("Mish.v1")
 def Mish(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/multisoftmax.py` & `thinc-9.0.0.dev4/thinc/layers/multisoftmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Optional, Tuple, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..types import Floats2d, Floats1d
-from ..model import Model
 from ..config import registry
+from ..model import Model
+from ..types import Floats1d, Floats2d
 from ..util import get_width
 
-
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("MultiSoftmax.v1")
 def MultiSoftmax(nOs: Tuple[int, ...], nI: Optional[int] = None) -> Model[InT, OutT]:
     """Neural network layer that predicts several multi-class attributes at once.
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/mxnetwrapper.py` & `thinc-9.0.0.dev4/thinc/layers/mxnetwrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Callable, Tuple, Optional, Any, Type
+from typing import Any, Callable, Optional, Tuple, Type
 
+from ..config import registry
 from ..model import Model
 from ..shims import MXNetShim
-from ..config import registry
-from ..util import is_xp_array, is_mxnet_array
-from ..util import mxnet2xp, xp2mxnet, convert_recursive
 from ..types import ArgsKwargs
+from ..util import convert_recursive, is_mxnet_array, is_xp_array, mxnet2xp, xp2mxnet
 
 
 @registry.layers("MXNetWrapper.v1")
 def MXNetWrapper(
     mxnet_model,
     convert_inputs: Optional[Callable] = None,
     convert_outputs: Optional[Callable] = None,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/padded2list.py` & `thinc-9.0.0.dev4/thinc/layers/padded2list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, Callable, TypeVar, cast
+from typing import Callable, Tuple, TypeVar, cast
 
-from ..types import Padded, List2d
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
+from ..types import List2d, Padded
 
 InT = Padded
 OutT = TypeVar("OutT", bound=List2d)
 
 
 @registry.layers("padded2list.v1")
 def padded2list() -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/parametricattention.py` & `thinc-9.0.0.dev4/thinc/layers/parametricattention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional
+from typing import Callable, Optional, Tuple
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Ragged
 from ..util import get_width
 
-
 InT = Ragged
 OutT = Ragged
 
 
 @registry.layers("ParametricAttention.v1")
 def ParametricAttention(nO: Optional[int] = None) -> Model[InT, OutT]:
     """Weight inputs by similarity to a learned vector"""
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/premap_ids.pyx` & `thinc-9.0.0.dev4/thinc/layers/premap_ids.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# cython: binding=True, infer_types=True
+# cython: binding=True, infer_types=True, profile=False
 import numpy
+
 from preshed.maps cimport PreshMap
-from typing import Dict, Union, Optional, cast, Callable, Tuple, Mapping
-from ..types import Ints1d, Ints2d
+
+from typing import Callable, Dict, Mapping, Optional, Tuple, Union, cast
+
 from ..config import registry
 from ..model import Model
+from ..types import Ints1d, Ints2d
 from ..util import to_numpy
 
-
 InT = Union[Ints1d, Ints2d]
 OutT = Ints2d
 
 
 cdef lookup(PreshMap mapping, long[:] keys, long default):
     """
     Faster dict.get(keys, default) for the case when
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/pytorchwrapper.py` & `thinc-9.0.0.dev4/thinc/layers/pytorchwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Callable, Dict, Tuple, Optional, Any, cast
+from typing import Any, Callable, Dict, Optional, Tuple, cast
 
 from ..compat import torch
+from ..config import registry
 from ..model import Model
 from ..shims import PyTorchGradScaler, PyTorchShim
-from ..config import registry
-from ..util import is_xp_array, is_torch_array, partial
-from ..util import xp2torch, torch2xp, convert_recursive
-from ..types import Floats3d, ArgsKwargs, Padded
+from ..types import ArgsKwargs, Floats3d, Padded
+from ..util import (
+    convert_recursive,
+    is_torch_array,
+    is_xp_array,
+    partial,
+    torch2xp,
+    xp2torch,
+)
 
 
 @registry.layers("PyTorchRNNWrapper.v1")
 def PyTorchRNNWrapper(
     pytorch_model: Any,
     convert_inputs: Optional[Callable] = None,
     convert_outputs: Optional[Callable] = None,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/ragged2list.py` & `thinc-9.0.0.dev4/thinc/layers/ragged2list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, Callable, TypeVar, cast
+from typing import Callable, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Ragged, ListXd
-
+from ..model import Model
+from ..types import ListXd, Ragged
 
 InT = Ragged
 OutT = TypeVar("OutT", bound=ListXd)
 
 
 @registry.layers("ragged2list.v1")
 def ragged2list() -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/reduce_first.py` & `thinc-9.0.0.dev4/thinc/layers/reduce_first.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Callable, Tuple, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Ragged, Floats2d
+from ..model import Model
+from ..types import Floats2d, Ragged
 from ..util import ArrayInfo
 
-
 InT = Ragged
 OutT = Floats2d
 
 
 @registry.layers("reduce_first.v1")
 def reduce_first() -> Model[InT, OutT]:
     """Reduce ragged-formatted sequences to their first element."""
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/reduce_last.py` & `thinc-9.0.0.dev4/thinc/layers/reduce_last.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Tuple, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Ragged, Floats2d
+from ..model import Model
+from ..types import Floats2d, Ragged
 from ..util import ArrayInfo
 
 InT = Ragged
 OutT = Floats2d
 
 
 @registry.layers("reduce_last.v1")
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/reduce_max.py` & `thinc-9.0.0.dev4/thinc/layers/reduce_max.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, cast
+from typing import Callable, Tuple, cast
 
-from ..types import Floats2d, Ragged
-from ..model import Model
 from ..config import registry
+from ..model import Model
+from ..types import Floats2d, Ragged
 from ..util import ArrayInfo
 
-
 InT = Ragged
 OutT = Floats2d
 
 
 @registry.layers("reduce_max.v1")
 def reduce_max() -> Model[InT, OutT]:
     return Model("reduce_max", forward)
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/reduce_mean.py` & `thinc-9.0.0.dev4/thinc/layers/reduce_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, cast
+from typing import Callable, Tuple, cast
 
-from ..types import Floats2d, Ragged
-from ..model import Model
 from ..config import registry
+from ..model import Model
+from ..types import Floats2d, Ragged
 from ..util import ArrayInfo
 
-
 InT = Ragged
 OutT = Floats2d
 
 
 @registry.layers("reduce_mean.v1")
 def reduce_mean() -> Model[InT, OutT]:
     return Model("reduce_mean", forward)
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/reduce_sum.py` & `thinc-9.0.0.dev4/thinc/layers/reduce_sum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Callable, Tuple, cast
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d, Ragged
 from ..util import ArrayInfo
 
-
 InT = Ragged
 OutT = Floats2d
 
 
 @registry.layers("reduce_sum.v1")
 def reduce_sum() -> Model[InT, OutT]:
     return Model("reduce_sum", forward)
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/relu.py` & `thinc-9.0.0.dev4/thinc/layers/sigmoid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,65 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
-from ..initializers import glorot_uniform_init, zero_init
 from ..config import registry
-from ..types import Floats2d, Floats1d
+from ..initializers import zero_init
+from ..model import Model
+from ..types import Floats1d, Floats2d
 from ..util import get_width, partial
-from .chain import chain
-from .layernorm import LayerNorm
-from .dropout import Dropout
-
 
 InT = Floats2d
 OutT = Floats2d
 
 
-@registry.layers("Relu.v1")
-def Relu(
+@registry.layers("Sigmoid.v1")
+def Sigmoid(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
-    dropout: Optional[float] = None,
-    normalize: bool = False,
 ) -> Model[InT, OutT]:
+    """A dense layer, followed by a sigmoid (logistic) activation function. This
+    is usually used instead of the Softmax layer as an output for multi-label
+    classification.
+    """
     if init_W is None:
-        init_W = glorot_uniform_init
+        init_W = zero_init
     if init_b is None:
         init_b = zero_init
-    model: Model[InT, OutT] = Model(
-        "relu",
+    return Model(
+        "sigmoid",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
-    if normalize:
-        model = chain(model, LayerNorm(nI=nO))
-    if dropout is not None:
-        model = chain(model, cast(Model[Floats2d, Floats2d], Dropout(dropout)))
-    return model
 
 
 def forward(model: Model[InT, OutT], X: InT, is_train: bool) -> Tuple[OutT, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
     Y = model.ops.affine(X, W, b)
-    Y = model.ops.relu(Y)
+    Y = model.ops.sigmoid(Y)
 
-    def backprop(dY: OutT) -> InT:
-        dY = model.ops.backprop_relu(dY, Y)
+    def backprop(dY: InT) -> OutT:
+        dY = model.ops.backprop_sigmoid(dY, Y, inplace=False)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
 
 
 def init(
     init_W: Callable,
     init_b: Callable,
     model: Model[InT, OutT],
     X: Optional[InT] = None,
     Y: Optional[OutT] = None,
 ) -> None:
-    if X is not None:
+    if X is not None and model.has_dim("nI") is None:
         model.set_dim("nI", get_width(X))
-    if Y is not None:
+    if Y is not None and model.has_dim("nO") is None:
         model.set_dim("nO", get_width(Y))
     model.set_param("W", init_W(model.ops, (model.get_dim("nO"), model.get_dim("nI"))))
     model.set_param("b", init_b(model.ops, (model.get_dim("nO"),)))
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/remap_ids.py` & `thinc-9.0.0.dev4/thinc/layers/remap_ids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from typing import Tuple, Callable, Sequence, cast
-from typing import Dict, Union, Optional, Hashable, Any
+from typing import Any, Callable, Dict, Hashable, Optional, Sequence, Tuple, Union, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Ints1d, Ints2d, DTypes
+from ..model import Model
+from ..types import DTypes, Ints1d, Ints2d
 from ..util import is_xp_array, to_numpy
 
-
 InT = Union[Sequence[Hashable], Ints1d, Ints2d]
 OutT = Ints2d
 
 InT_v1 = Sequence[Any]
 OutT_v1 = Ints2d
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/residual.py` & `thinc-9.0.0.dev4/thinc/layers/residual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Tuple, Callable, Optional, List, TypeVar
+from typing import Callable, List, Optional, Tuple, TypeVar
 
-from ..model import Model
 from ..config import registry
-from ..types import Floats1d, Floats2d, Floats3d, Floats4d, FloatsXd, Ragged, Padded
+from ..model import Model
+from ..types import Floats1d, Floats2d, Floats3d, Floats4d, FloatsXd, Padded, Ragged
 
 # fmt: off
 InT = TypeVar(  
     "InT", List[Floats1d], List[Floats2d], List[Floats3d], List[Floats4d], 
     Ragged, Padded, FloatsXd, Floats1d, Floats2d, Floats3d, Floats4d)
 # fmt: on
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/resizable.py` & `thinc-9.0.0.dev4/thinc/layers/resizable.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, Optional, TypeVar
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d
 
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
 
 
 @registry.layers("resizable.v1")
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/siamese.py` & `thinc-9.0.0.dev4/thinc/layers/siamese.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional, TypeVar
+from typing import Callable, Optional, Tuple, TypeVar
 
+from ..config import registry
 from ..model import Model
 from ..types import ArrayXd
-from ..config import registry
 from ..util import get_width
 
-
 LayerT = TypeVar("LayerT")
 SimT = TypeVar("SimT")
 InT = Tuple[LayerT, LayerT]
 OutT = TypeVar("OutT", bound=ArrayXd)
 
 
 @registry.layers("siamese.v1")
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/softmax.py` & `thinc-9.0.0.dev4/thinc/layers/softmax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional, cast
+from typing import Callable, Optional, Tuple, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Floats2d, Floats1d
 from ..initializers import zero_init
-from ..util import get_width, partial, ArrayInfo
-
+from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import ArrayInfo, get_width, partial
 
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("Softmax.v1")
 def Softmax(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/softmax_activation.py` & `thinc-9.0.0.dev4/thinc/layers/softmax_activation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, Callable
+from typing import Callable, Tuple
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Floats2d
 
-
 InT = Floats2d
 OutT = Floats2d
 
 
 @registry.layers("softmax_activation.v1")
 def softmax_activation() -> Model[InT, OutT]:
     return Model("softmax_activation", forward)
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/sparselinear.pyx` & `thinc-9.0.0.dev4/thinc/layers/sparselinear.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# cython: infer_types=True, cdivision=True, bounds_check=False, wraparound=False
-cimport numpy as np
-from libc.stdint cimport uint64_t, int32_t, uint32_t
+# cython: infer_types=True, cdivision=True, bounds_check=False, wraparound=False, profile=False
 cimport cython
+cimport numpy as np
+from libc.stdint cimport int32_t, uint32_t, uint64_t
 
-from typing import Tuple, Callable, Optional
+from typing import Callable, Optional, Tuple
 
-from ..types import ArrayXd
-from ..model import Model
+from ..backends import CupyOps, NumpyOps
 from ..config import registry
-from ..util import get_width, is_cupy_array, is_numpy_array, get_array_module
-from ..backends import NumpyOps, CupyOps
-
+from ..model import Model
+from ..types import ArrayXd
+from ..util import get_array_module, get_width, is_cupy_array, is_numpy_array
 
 InT = Tuple[ArrayXd, ArrayXd, ArrayXd]
 OutT = ArrayXd
 
 
 @cython.binding(True)
 @registry.layers("SparseLinear.v1")
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/strings2arrays.py` & `thinc-9.0.0.dev4/thinc/layers/strings2arrays.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Tuple, List, Callable, Sequence
+from ctypes import c_uint64
+from typing import Callable, List, Sequence, Tuple
+
 from murmurhash import hash_unicode
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Ints2d
 
-
 InT = Sequence[Sequence[str]]
 OutT = List[Ints2d]
 
 
 @registry.layers("strings2arrays.v1")
 def strings2arrays() -> Model[InT, OutT]:
     """Transform a sequence of string sequences to a list of arrays."""
     return Model("strings2arrays", forward)
 
 
 def forward(model: Model[InT, OutT], Xs: InT, is_train: bool) -> Tuple[OutT, Callable]:
-    hashes = [[hash_unicode(word) for word in X] for X in Xs]
-    hash_arrays = [model.ops.asarray2i(h, dtype="uint64") for h in hashes]
+    # Cast 32-bit (signed) integer to 64-bit unsigned, since such casting
+    # is deprecated in NumPy.
+    hashes = [[c_uint64(hash_unicode(word)).value for word in X] for X in Xs]
+    hash_arrays = [model.ops.asarray1i(h, dtype="uint64") for h in hashes]
     arrays = [model.ops.reshape2i(array, -1, 1) for array in hash_arrays]
 
     def backprop(dX: OutT) -> InT:
         return []
 
     return arrays, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/swish.py` & `thinc-9.0.0.dev4/thinc/layers/hard_swish_mobilenet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Tuple, Optional, Callable, cast
+from typing import Callable, Optional, Tuple, cast
 
 from ..config import registry
+from ..initializers import he_normal_init, zero_init
 from ..model import Model
+from ..types import Floats1d, Floats2d
+from ..util import get_width, partial
 from .chain import chain
-from .layernorm import LayerNorm
 from .dropout import Dropout
-from ..types import Floats1d, Floats2d
-from ..util import partial, get_width
-from ..initializers import he_normal_init, zero_init
+from .layernorm import LayerNorm
 
 
-@registry.layers("Swish.v1")
-def Swish(
+@registry.layers("HardSwishMobilenet.v1")
+def HardSwishMobilenet(
     nO: Optional[int] = None,
     nI: Optional[int] = None,
     *,
     init_W: Optional[Callable] = None,
     init_b: Optional[Callable] = None,
     dropout: Optional[float] = None,
     normalize: bool = False,
 ) -> Model[Floats2d, Floats2d]:
     if init_W is None:
         init_W = he_normal_init
     if init_b is None:
         init_b = zero_init
     model: Model[Floats2d, Floats2d] = Model(
-        "swish",
+        "hardswishmobilenet",
         forward,
         init=partial(init, init_W, init_b),
         dims={"nO": nO, "nI": nI},
         params={"W": None, "b": None},
     )
     if normalize:
         model = chain(model, LayerNorm(nI=nO))
@@ -40,18 +40,18 @@
 
 def forward(
     model: Model[Floats2d, Floats2d], X: Floats2d, is_train: bool
 ) -> Tuple[Floats2d, Callable]:
     W = cast(Floats2d, model.get_param("W"))
     b = cast(Floats1d, model.get_param("b"))
     Y_preact = model.ops.affine(X, W, b)
-    Y = model.ops.swish(Y_preact)
+    Y = model.ops.hard_swish_mobilenet(Y_preact)
 
     def backprop(dY: Floats2d) -> Floats2d:
-        dY = model.ops.backprop_swish(dY, Y_preact, Y, inplace=False)
+        dY = model.ops.backprop_hard_swish_mobilenet(dY, Y_preact, inplace=False)
         model.inc_grad("b", dY.sum(axis=0))
         model.inc_grad("W", model.ops.gemm(dY, X, trans1=True))
         return model.ops.gemm(dY, W)
 
     return Y, backprop
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/tensorflowwrapper.py` & `thinc-9.0.0.dev4/thinc/layers/tensorflowwrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+# mypy: ignore-errors
 from typing import Any, Callable, Dict, Optional, Tuple, Type, TypeVar
 
 import srsly
 
+from ..compat import tensorflow as tf
 from ..model import Model
 from ..shims import TensorFlowShim, keras_model_fns, maybe_handshake_model
-from ..util import xp2tensorflow, tensorflow2xp, assert_tensorflow_installed
-from ..util import is_tensorflow_array, convert_recursive, is_xp_array
-from ..types import ArrayXd, ArgsKwargs
-from ..compat import tensorflow as tf
+from ..types import ArgsKwargs, ArrayXd
+from ..util import (
+    assert_tensorflow_installed,
+    convert_recursive,
+    is_tensorflow_array,
+    is_xp_array,
+    tensorflow2xp,
+    xp2tensorflow,
+)
 
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
 InFunc = TypeVar("InFunc")
 XType = TypeVar("XType", bound=ArrayXd)
 YType = TypeVar("YType", bound=ArrayXd)
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/torchscriptwrapper.py` & `thinc-9.0.0.dev4/thinc/layers/torchscriptwrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Any, Callable, Optional
 
 from ..compat import torch
 from ..model import Model
 from ..shims import PyTorchGradScaler, PyTorchShim, TorchScriptShim
-from .pytorchwrapper import forward, convert_pytorch_default_inputs
-from .pytorchwrapper import convert_pytorch_default_outputs
+from .pytorchwrapper import (
+    convert_pytorch_default_inputs,
+    convert_pytorch_default_outputs,
+    forward,
+)
 
 
 def TorchScriptWrapper_v1(
     torchscript_model: Optional["torch.jit.ScriptModule"] = None,
     convert_inputs: Optional[Callable] = None,
     convert_outputs: Optional[Callable] = None,
     mixed_precision: bool = False,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/tuplify.py` & `thinc-9.0.0.dev4/thinc/layers/tuplify.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Optional, Tuple, Any, TypeVar
+from typing import Any, Optional, Tuple, TypeVar
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 
 InT = TypeVar("InT")
 OutT = Tuple
 
 
 @registry.layers("tuplify.v1")
 def tuplify(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/uniqued.py` & `thinc-9.0.0.dev4/thinc/layers/uniqued.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Tuple, Callable, Optional
+from typing import Callable, Optional, Tuple
+
 import numpy
 
-from ..model import Model
 from ..config import registry
-from ..types import Ints2d, Floats2d
-
+from ..model import Model
+from ..types import Floats2d, Ints2d
 
 InT = Ints2d
 OutT = Floats2d
 
 
 @registry.layers("uniqued.v1")
 def uniqued(layer: Model, *, column: int = 0) -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_array.py` & `thinc-9.0.0.dev4/thinc/layers/with_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, Callable, Optional, TypeVar, Union, cast
+from typing import Callable, Optional, Tuple, TypeVar, Union, cast
 
 from ..backends import NumpyOps
-from ..model import Model
 from ..config import registry
-from ..types import Padded, Ragged, ArrayXd, Array3d, ListXd
-
+from ..model import Model
+from ..types import Array3d, ArrayXd, ListXd, Padded, Ragged
 
 NUMPY_OPS = NumpyOps()
 
 
 ArrayTXd = TypeVar("ArrayTXd", bound=ArrayXd)
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, ListXd, ArrayXd])
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_array2d.py` & `thinc-9.0.0.dev4/thinc/layers/with_array2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional, TypeVar, cast, List, Union
+from typing import Callable, List, Optional, Tuple, TypeVar, Union, cast
 
 from ..backends import NumpyOps
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import Array2d, Floats2d, List2d, Padded, Ragged
 
-
 NUMPY_OPS = NumpyOps()
 
 
 ValT = TypeVar("ValT", bound=Array2d)
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, List2d, Array2d])
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_cpu.py` & `thinc-9.0.0.dev4/thinc/layers/with_cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Tuple, Callable, Any
+from typing import Any, Callable, Tuple
 
 import numpy
+
 from thinc.backends import Ops
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 
 
 @registry.layers("with_cpu.v1")
 def with_cpu(layer: Model, ops: Ops) -> Model:
     layer.to_cpu()
     return Model(
         f"with_cpu({layer.name})",
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_debug.py` & `thinc-9.0.0.dev4/thinc/layers/with_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable, Any, Tuple, TypeVar
+from typing import Any, Callable, Optional, Tuple, TypeVar
 
 from ..model import Model
 
 _ModelT = TypeVar("_ModelT", bound=Model)
 
 do_nothing = lambda *args, **kwargs: None
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_flatten.py` & `thinc-9.0.0.dev4/thinc/layers/with_flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Tuple, Callable, Sequence, Any, cast, TypeVar, Optional, List
+from typing import Any, Callable, List, Optional, Sequence, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
+from ..model import Model
 from ..types import ArrayXd, ListXd
 
 ItemT = TypeVar("ItemT")
 InT = Sequence[Sequence[ItemT]]
 OutT = ListXd
 InnerInT = Sequence[ItemT]
 InnerOutT = ArrayXd
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_flatten_v2.py` & `thinc-9.0.0.dev4/thinc/layers/with_flatten_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Tuple, Callable, Sequence, Any, cast, TypeVar, Optional, List
+from typing import Any, Callable, List, Optional, Sequence, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
 
 InItemT = TypeVar("InItemT")
 OutItemT = TypeVar("OutItemT")
 ItemT = TypeVar("ItemT")
 
 NestedT = List[List[ItemT]]
 FlatT = List[ItemT]
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_getitem.py` & `thinc-9.0.0.dev4/thinc/layers/with_getitem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Callable, Optional, Tuple, Any
+from typing import Any, Callable, Optional, Tuple
 
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
 
 InT = Tuple[Any, ...]
 OutT = Tuple[Any, ...]
 
 
 @registry.layers("with_getitem.v1")
 def with_getitem(idx: int, layer: Model) -> Model[InT, OutT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_list.py` & `thinc-9.0.0.dev4/thinc/layers/with_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Tuple, Callable, List, Optional, TypeVar, Union, cast
+from typing import Callable, List, Optional, Tuple, TypeVar, Union, cast
 
-from ..types import Padded, Ragged, Array2d, List2d, Floats2d, Ints2d
-from ..model import Model
 from ..config import registry
+from ..model import Model
+from ..types import Array2d, Floats2d, Ints2d, List2d, Padded, Ragged
 
 SeqT = TypeVar("SeqT", Padded, Ragged, List2d, List[Floats2d], List[Ints2d])
 
 
 @registry.layers("with_list.v1")
 def with_list(layer: Model[List2d, List2d]) -> Model[SeqT, SeqT]:
     return Model(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_nvtx_range.py` & `thinc-9.0.0.dev4/thinc/layers/with_nvtx_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Optional, Callable, Any, Tuple, TypeVar
+from typing import Any, Callable, Optional, Tuple, TypeVar
 
 from ..model import Model
 from ..util import use_nvtx_range
 
-
 _ModelT = TypeVar("_ModelT", bound=Model)
 
 
 def with_nvtx_range(
     layer: _ModelT,
     name: Optional[str] = None,
     *,
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_padded.py` & `thinc-9.0.0.dev4/thinc/layers/with_padded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Tuple, Callable, Optional, TypeVar, Union, cast, List
+from typing import Callable, List, Optional, Tuple, TypeVar, Union, cast
 
-from ..types import Padded, Ragged, Floats3d, Ints1d, List2d, Array2d
-from ..model import Model
 from ..config import registry
+from ..model import Model
+from ..types import Array2d, Floats3d, Ints1d, List2d, Padded, Ragged
 from ..util import is_xp_array
 
-
 PaddedData = Tuple[Floats3d, Ints1d, Ints1d, Ints1d]
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, List2d, Floats3d, PaddedData])
 
 
 @registry.layers("with_padded.v1")
 def with_padded(layer: Model[Padded, Padded]) -> Model[SeqT, SeqT]:
     return Model(
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_ragged.py` & `thinc-9.0.0.dev4/thinc/layers/with_ragged.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Tuple, Callable, Optional, TypeVar, cast, List, Union
+from typing import Callable, List, Optional, Tuple, TypeVar, Union, cast
 
 from ..backends import NumpyOps
-from ..types import Padded, Ragged, Array2d, ListXd, List2d, Ints1d
-from ..model import Model
 from ..config import registry
-
+from ..model import Model
+from ..types import Array2d, Ints1d, List2d, ListXd, Padded, Ragged
 
 NUMPY_OPS = NumpyOps()
 
 
 RaggedData = Tuple[Array2d, Ints1d]
 SeqT = TypeVar("SeqT", bound=Union[Padded, Ragged, ListXd, RaggedData])
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_reshape.py` & `thinc-9.0.0.dev4/thinc/layers/with_reshape.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Tuple, Callable, Optional, cast, TypeVar, List
+from typing import Callable, List, Optional, Tuple, TypeVar, cast
 
-from ..model import Model
 from ..config import registry
-from ..types import Array3d, Array2d
-
+from ..model import Model
+from ..types import Array2d, Array3d
 
 InT = TypeVar("InT", bound=Array3d)
 OutT = TypeVar("OutT", bound=Array2d)
 
 
 @registry.layers("with_reshape.v1")
 def with_reshape(layer: Model[OutT, OutT]) -> Model[InT, InT]:
```

### Comparing `thinc-9.0.0.dev3/thinc/layers/with_signpost_interval.py` & `thinc-9.0.0.dev4/thinc/layers/with_signpost_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Optional, Callable, Any, Tuple, TypeVar
+from typing import Any, Callable, Optional, Tuple, TypeVar
 
 from ..compat import has_os_signpost, os_signpost
 from ..model import Model
 
-
 _ModelT = TypeVar("_ModelT", bound=Model)
 
 
 def with_signpost_interval(
     layer: _ModelT,
     signposter: "os_signpost.Signposter",
     name: Optional[str] = None,
```

### Comparing `thinc-9.0.0.dev3/thinc/legacy/loss.py` & `thinc-9.0.0.dev4/thinc/loss.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,56 @@
-from typing import Optional, Sequence, Dict, Union, Tuple
-from typing import cast, List
-from ..types import Floats2d, Ints1d
-from ..config import registry
-from ..util import to_categorical, get_array_module
-from ..loss import IntsOrFloatsOrStrs, Loss
-from ..loss import _make_mask, _make_mask_by_value
+from abc import abstractmethod
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
+
+from .config import registry
+from .types import Floats2d, Ints1d
+from .util import get_array_module, to_categorical
+
+LossT = TypeVar("LossT")
+GradT = TypeVar("GradT")
+GuessT = TypeVar("GuessT")
+TruthT = TypeVar("TruthT")
+IntsOrFloats = Union[Ints1d, Floats2d]
+IntsOrFloatsOrStrs = Union[Ints1d, Floats2d, Sequence[int], Sequence[str]]
+
+
+class Loss(Generic[GuessT, TruthT, GradT, LossT]):  # pragma: no cover
+    """Base class for classes computing the loss / gradient. The class can
+    be initialized with settings if needed. It provides get_loss and
+    get_grad as separate methods to allow calculating them separately. It
+    also provides a __call__ method that returns a tuple of both.
+    """
+
+    def __init__(self, **kwargs: Any) -> None:
+        ...
+
+    def __call__(self, guesses: GuessT, truths: TruthT) -> Tuple[GradT, LossT]:
+        return self.get_grad(guesses, truths), self.get_loss(guesses, truths)
+
+    @abstractmethod
+    def get_grad(self, guesses: GuessT, truths: TruthT) -> GradT:
+        ...
+
+    @abstractmethod
+    def get_loss(self, guesses: GuessT, truths: TruthT) -> LossT:
+        ...
 
 
-TruthsT = Union[List[Optional[str]], List[int], Ints1d, Floats2d]
-
-
-class LegacyCategoricalCrossentropy(Loss):
+class CategoricalCrossentropy(Loss):
     names: Optional[Sequence[str]]
     missing_value: Optional[Union[str, int]]
     _name_to_i: Dict[str, int]
 
     def __init__(
         self,
         *,
@@ -30,256 +66,374 @@
         self.neg_prefix = neg_prefix
         self.label_smoothing = label_smoothing
         if names is not None:
             self._name_to_i = {name: i for i, name in enumerate(names)}
         else:
             self._name_to_i = {}
 
-    def convert_truths(
-        self, truths: TruthsT, guesses: Floats2d
-    ) -> Tuple[Floats2d, Floats2d]:
+    def convert_truths(self, truths, guesses: Floats2d) -> Tuple[Floats2d, Floats2d]:
         xp = get_array_module(guesses)
         missing = []
         negatives_mask = None
         if self.names:
             negatives_mask = xp.ones((len(truths), len(self.names)), dtype="f")
         missing_value = self.missing_value
         # Convert list of ints or list of strings
         if isinstance(truths, list):
+            truths = list(truths)
             if len(truths):
                 if isinstance(truths[0], int):
                     for i, value in enumerate(truths):
-                        if not isinstance(value, int):
-                            raise ValueError(
-                                "All values in the truths list have to "
-                                "have the same type. The first value was "
-                                f"detected to be integer, but found {type(value)}."
-                            )
                         if value == missing_value:
                             missing.append(i)
                 else:
-                    truths = cast(List[Optional[str]], truths)
                     if self.names is None:
                         msg = (
                             "Cannot calculate loss from list of strings without names. "
                             "You can pass the names as a keyword argument when you "
                             "create the loss object, "
                             "e.g. CategoricalCrossentropy(names=['dog', 'cat'])"
                         )
                         raise ValueError(msg)
                     for i, value in enumerate(truths):
-                        if not (isinstance(value, str) or value == missing_value):
-                            raise ValueError(
-                                "All values in the truths list have to "
-                                "have the same type. The first value was "
-                                f"detected to be string, but found {type(value)}."
-                            )
                         if value == missing_value:
                             truths[i] = self.names[0]
                             missing.append(i)
                         elif (
                             value
                             and self.neg_prefix
                             and value.startswith(self.neg_prefix)
                         ):
-                            neg_value = value[len(self.neg_prefix) :]
-                            truths[i] = neg_value
-                            neg_index = self._name_to_i[neg_value]
+                            truths[i] = value[len(self.neg_prefix) :]
+                            neg_index = self._name_to_i[truths[i]]
                             negatives_mask[i] = 0  # type: ignore
                             negatives_mask[i][neg_index] = -1  # type: ignore
-                    # In the loop above, we have ensured that `truths` doesn't
-                    # contain `None` (anymore). However, mypy can't infer this
-                    # and doesn't like the shadowing.
-                    truths_str = cast(List[str], truths)
-                    truths = [self._name_to_i[name] for name in truths_str]
+                    truths = [self._name_to_i[name] for name in truths]
             truths = xp.asarray(truths, dtype="i")
             mask = _make_mask(guesses, missing)
         else:
             mask = _make_mask_by_value(truths, guesses, missing_value)
-        truths = cast(Union[Ints1d, Floats2d], truths)
         if truths.ndim != guesses.ndim:
             # transform categorical values to one-hot encoding
-            truths_2d = to_categorical(
-                truths,
+            truths = to_categorical(
+                cast(Ints1d, truths),
                 n_classes=guesses.shape[-1],
                 label_smoothing=self.label_smoothing,
             )
         else:
             if self.label_smoothing:
                 raise ValueError(
                     "Label smoothing is only applied, when truths have type "
                     "List[str], List[int] or Ints1d, but it seems like Floats2d "
                     "was provided."
                 )
-            truths_2d = cast(Floats2d, truths)
         # Transform negative annotations to a 0 for the negated value
         # + mask all other values for that row
         if negatives_mask is not None:
-            truths_2d *= negatives_mask
-            truths_2d[truths_2d == -1] = 0
+            truths *= negatives_mask
+            truths[truths == -1] = 0
             negatives_mask[negatives_mask == -1] = 1
             mask *= negatives_mask
-        return cast(Floats2d, truths_2d), mask
+        return truths, mask
 
-    def __call__(self, guesses: Floats2d, truths: TruthsT) -> Tuple[Floats2d, float]:
+    def __call__(
+        self, guesses: Floats2d, truths: IntsOrFloatsOrStrs
+    ) -> Tuple[Floats2d, float]:
         d_truth = self.get_grad(guesses, truths)
         return (d_truth, self._get_loss_from_grad(d_truth))
 
-    def get_grad(self, guesses: Floats2d, truths: TruthsT) -> Floats2d:
+    def get_grad(self, guesses: Floats2d, truths: IntsOrFloatsOrStrs) -> Floats2d:
         target, mask = self.convert_truths(truths, guesses)
         xp = get_array_module(target)
         if guesses.shape != target.shape:  # pragma: no cover
             err = f"Cannot calculate CategoricalCrossentropy loss: mismatched shapes: {guesses.shape} vs {target.shape}."
             raise ValueError(err)
-        elif xp.any(guesses > 1) or xp.any(guesses < 0):  # pragma: no cover
+        if xp.any(guesses > 1) or xp.any(guesses < 0):  # pragma: no cover
             err = f"Cannot calculate CategoricalCrossentropy loss with guesses outside the [0,1] interval."
             raise ValueError(err)
-        elif xp.any(target > 1) or xp.any(target < 0):  # pragma: no cover
+        if xp.any(target > 1) or xp.any(target < 0):  # pragma: no cover
             err = f"Cannot calculate CategoricalCrossentropy loss with truth values outside the [0,1] interval."
             raise ValueError(err)
         difference = guesses - target
         difference *= mask
         if self.normalize:
             difference = difference / guesses.shape[0]
         return difference
 
-    def get_loss(self, guesses: Floats2d, truths: TruthsT) -> float:
+    def get_loss(self, guesses: Floats2d, truths: IntsOrFloatsOrStrs) -> float:
         d_truth = self.get_grad(guesses, truths)
         return self._get_loss_from_grad(d_truth)
 
     def _get_loss_from_grad(self, d_truth: Floats2d) -> float:
         # TODO: Add overload for axis=None case to sum
         return (d_truth**2).sum()  # type: ignore
 
 
-class LegacySequenceCategoricalCrossentropy(Loss):
+@registry.losses("CategoricalCrossentropy.v1")
+def configure_CategoricalCrossentropy_v1(
+    *,
+    normalize: bool = True,
+    names: Optional[Sequence[str]] = None,
+    missing_value: Optional[Union[str, int]] = None,
+) -> CategoricalCrossentropy:
+    return CategoricalCrossentropy(
+        normalize=normalize, names=names, missing_value=missing_value
+    )
+
+
+@registry.losses("CategoricalCrossentropy.v2")
+def configure_CategoricalCrossentropy_v2(
+    *,
+    normalize: bool = True,
+    names: Optional[Sequence[str]] = None,
+    missing_value: Optional[Union[str, int]] = None,
+    neg_prefix: Optional[str] = None,
+) -> CategoricalCrossentropy:
+    return CategoricalCrossentropy(
+        normalize=normalize,
+        names=names,
+        missing_value=missing_value,
+        neg_prefix=neg_prefix,
+    )
+
+
+@registry.losses("CategoricalCrossentropy.v3")
+def configure_CategoricalCrossentropy_v3(
+    *,
+    normalize: bool = True,
+    names: Optional[Sequence[str]] = None,
+    missing_value: Optional[Union[str, int]] = None,
+    neg_prefix: Optional[str] = None,
+    label_smoothing: float = 0.0,
+) -> CategoricalCrossentropy:
+    return CategoricalCrossentropy(
+        normalize=normalize,
+        names=names,
+        missing_value=missing_value,
+        neg_prefix=neg_prefix,
+        label_smoothing=label_smoothing,
+    )
+
+
+class SequenceCategoricalCrossentropy(Loss):
     def __init__(
         self,
         *,
         normalize: bool = True,
         names: Optional[Sequence[str]] = None,
         missing_value: Optional[Union[str, int]] = None,
         neg_prefix: Optional[str] = None,
         label_smoothing: float = 0.0,
     ):
-        self.cc = LegacyCategoricalCrossentropy(
+        self.cc = CategoricalCrossentropy(
             normalize=False,
             names=names,
             missing_value=missing_value,
             neg_prefix=neg_prefix,
             label_smoothing=label_smoothing,
         )
         self.normalize = normalize
 
     def __call__(
-        self, guesses: Sequence[Floats2d], truths: Sequence[TruthsT]
+        self, guesses: Sequence[Floats2d], truths: Sequence[IntsOrFloatsOrStrs]
     ) -> Tuple[List[Floats2d], float]:
         grads = self.get_grad(guesses, truths)
         loss = self._get_loss_from_grad(grads)
         return grads, loss
 
     def get_grad(
-        self, guesses: Sequence[Floats2d], truths: Sequence[TruthsT]
+        self, guesses: Sequence[Floats2d], truths: Sequence[IntsOrFloatsOrStrs]
     ) -> List[Floats2d]:
+        err = "Cannot calculate SequenceCategoricalCrossentropy loss: guesses and truths must be same length"
         if len(guesses) != len(truths):  # pragma: no cover
-            err = "Cannot calculate SequenceCategoricalCrossentropy loss: guesses and truths must be same length"
             raise ValueError(err)
         n = len(guesses)
         d_scores = []
         for yh, y in zip(guesses, truths):
             d_yh = self.cc.get_grad(yh, y)
             if self.normalize:
                 d_yh /= n
             d_scores.append(d_yh)
         return d_scores
 
-    def get_loss(self, guesses: Sequence[Floats2d], truths: Sequence[TruthsT]) -> float:
+    def get_loss(
+        self, guesses: Sequence[Floats2d], truths: Sequence[IntsOrFloatsOrStrs]
+    ) -> float:
         return self._get_loss_from_grad(self.get_grad(guesses, truths))
 
     def _get_loss_from_grad(self, grads: Sequence[Floats2d]) -> float:
         loss = 0.0
         for grad in grads:
-            loss += self.cc._get_loss_from_grad(grad)  # type: ignore
+            loss += self.cc._get_loss_from_grad(grad)
         return loss
 
 
-@registry.losses("CategoricalCrossentropy.v1")
-def configure_CategoricalCrossentropy_v1(
-    *,
-    normalize: bool = True,
-    names: Optional[Sequence[str]] = None,
-    missing_value: Optional[Union[str, int]] = None,
-) -> LegacyCategoricalCrossentropy:
-    return LegacyCategoricalCrossentropy(
-        normalize=normalize, names=names, missing_value=missing_value
-    )
-
-
-@registry.losses("CategoricalCrossentropy.v2")
-def configure_CategoricalCrossentropy_v2(
-    *,
-    normalize: bool = True,
-    names: Optional[Sequence[str]] = None,
-    missing_value: Optional[Union[str, int]] = None,
-    neg_prefix: Optional[str] = None,
-) -> LegacyCategoricalCrossentropy:
-    return LegacyCategoricalCrossentropy(
-        normalize=normalize,
-        names=names,
-        missing_value=missing_value,
-        neg_prefix=neg_prefix,
-    )
-
-
-@registry.losses("CategoricalCrossentropy.v3")
-def configure_CategoricalCrossentropy_v3(
-    *,
-    normalize: bool = True,
-    names: Optional[Sequence[str]] = None,
-    missing_value: Optional[Union[str, int]] = None,
-    neg_prefix: Optional[str] = None,
-    label_smoothing: float = 0.0,
-) -> LegacyCategoricalCrossentropy:
-    return LegacyCategoricalCrossentropy(
-        normalize=normalize,
-        names=names,
-        missing_value=missing_value,
-        neg_prefix=neg_prefix,
-        label_smoothing=label_smoothing,
-    )
-
-
 @registry.losses("SequenceCategoricalCrossentropy.v1")
 def configure_SequenceCategoricalCrossentropy_v1(
     *, normalize: bool = True, names: Optional[Sequence[str]] = None
-) -> LegacySequenceCategoricalCrossentropy:
-    return LegacySequenceCategoricalCrossentropy(normalize=normalize, names=names)
+) -> SequenceCategoricalCrossentropy:
+    return SequenceCategoricalCrossentropy(normalize=normalize, names=names)
 
 
 @registry.losses("SequenceCategoricalCrossentropy.v2")
 def configure_SequenceCategoricalCrossentropy_v2(
     *,
     normalize: bool = True,
     names: Optional[Sequence[str]] = None,
     neg_prefix: Optional[str] = None,
-) -> LegacySequenceCategoricalCrossentropy:
-    return LegacySequenceCategoricalCrossentropy(
+) -> SequenceCategoricalCrossentropy:
+    return SequenceCategoricalCrossentropy(
         normalize=normalize, names=names, neg_prefix=neg_prefix
     )
 
 
 @registry.losses("SequenceCategoricalCrossentropy.v3")
 def configure_SequenceCategoricalCrossentropy_v3(
     *,
     normalize: bool = True,
     names: Optional[Sequence[str]] = None,
     missing_value: Optional[Union[str, int]] = None,
     neg_prefix: Optional[str] = None,
     label_smoothing: float = 0.0,
-) -> LegacySequenceCategoricalCrossentropy:
-    return LegacySequenceCategoricalCrossentropy(
+) -> SequenceCategoricalCrossentropy:
+    return SequenceCategoricalCrossentropy(
         normalize=normalize,
         names=names,
-        neg_prefix=neg_prefix,
         missing_value=missing_value,
+        neg_prefix=neg_prefix,
         label_smoothing=label_smoothing,
     )
+
+
+class L2Distance(Loss):
+    def __init__(self, *, normalize: bool = True):
+        self.normalize = normalize
+
+    def __call__(self, guesses: Floats2d, truths: Floats2d) -> Tuple[Floats2d, float]:
+        return self.get_grad(guesses, truths), self.get_loss(guesses, truths)
+
+    def get_grad(self, guesses: Floats2d, truths: Floats2d) -> Floats2d:
+        if guesses.shape != truths.shape:  # pragma: no cover
+            err = f"Cannot calculate L2 distance: mismatched shapes: {guesses.shape} vs {truths.shape}."
+            raise ValueError(err)
+        difference = guesses - truths
+        if self.normalize:
+            difference = difference / guesses.shape[0]
+        return difference
+
+    def get_loss(self, guesses: Floats2d, truths: Floats2d) -> float:
+        if guesses.shape != truths.shape:  # pragma: no cover
+            err = f"Cannot calculate L2 distance: mismatched shapes: {guesses.shape} vs {truths.shape}."
+            raise ValueError(err)
+        d_truth = self.get_grad(guesses, truths)
+        # TODO: Add overload for axis=None case to sum
+        return (d_truth**2).sum()  # type: ignore
+
+
+@registry.losses("L2Distance.v1")
+def configure_L2Distance(*, normalize: bool = True) -> L2Distance:
+    return L2Distance(normalize=normalize)
+
+
+class CosineDistance(Loss):
+    def __init__(self, *, normalize: bool = True, ignore_zeros: bool = False):
+        self.normalize = normalize
+        self.ignore_zeros = ignore_zeros
+
+    def __call__(self, guesses: Floats2d, truths: Floats2d) -> Tuple[Floats2d, float]:
+        return self.get_grad(guesses, truths), self.get_loss(guesses, truths)
+
+    def get_similarity(self, guesses: Floats2d, truths: Floats2d) -> float:
+        if guesses.shape != truths.shape:  # pragma: no cover
+            err = f"Cannot calculate cosine similarity: mismatched shapes: {guesses.shape} vs {truths.shape}."
+            raise ValueError(err)
+
+        xp = get_array_module(guesses)
+        # Add a small constant to avoid 0 vectors
+        yh = guesses + 1e-8
+        y = truths + 1e-8
+        norm_yh = xp.linalg.norm(yh, axis=1, keepdims=True)
+        norm_y = xp.linalg.norm(y, axis=1, keepdims=True)
+        mul_norms = norm_yh * norm_y
+        cosine = (yh * y).sum(axis=1, keepdims=True) / mul_norms
+        return cosine
+
+    def get_grad(self, guesses: Floats2d, truths: Floats2d) -> Floats2d:
+        if guesses.shape != truths.shape:  # pragma: no cover
+            err = f"Cannot calculate cosine similarity: mismatched shapes: {guesses.shape} vs {truths.shape}."
+            raise ValueError(err)
+
+        # Note: not using get_distance() here to avoid duplicating certain calculations
+        xp = get_array_module(guesses)
+        # Find the zero vectors
+        if self.ignore_zeros:
+            zero_indices = xp.abs(truths).sum(axis=1) == 0
+        # Add a small constant to avoid 0 vectors
+        yh = guesses + 1e-8
+        y = truths + 1e-8
+        # https://math.stackexchange.com/questions/1923613/partial-derivative-of-cosinesimilarity
+        norm_yh = xp.linalg.norm(yh, axis=1, keepdims=True)
+        norm_y = xp.linalg.norm(y, axis=1, keepdims=True)
+        mul_norms = norm_yh * norm_y
+        cosine = (yh * y).sum(axis=1, keepdims=True) / mul_norms
+        d_yh = (y / mul_norms) - (cosine * (yh / norm_yh**2))
+        if self.ignore_zeros:
+            # If the target was a zero vector, don't count it in the loss.
+            d_yh[zero_indices] = 0
+        if self.normalize:
+            d_yh = d_yh / guesses.shape[0]
+        return -d_yh
+
+    def get_loss(self, guesses: Floats2d, truths: Floats2d) -> float:
+        if guesses.shape != truths.shape:  # pragma: no cover
+            err = f"Cannot calculate cosine similarity: mismatched shapes: {guesses.shape} vs {truths.shape}."
+            raise ValueError(err)
+
+        xp = get_array_module(guesses)
+        cosine = self.get_similarity(guesses, truths)
+        losses = xp.abs(cosine - 1)
+        if self.ignore_zeros:
+            # If the target was a zero vector, don't count it in the loss.
+            zero_indices = xp.abs(truths).sum(axis=1) == 0
+            losses[zero_indices] = 0
+        if self.normalize:
+            losses = losses / guesses.shape[0]
+        loss = losses.sum()
+        return loss
+
+
+@registry.losses("CosineDistance.v1")
+def configure_CosineDistance(
+    *, normalize: bool = True, ignore_zeros: bool = False
+) -> CosineDistance:
+    return CosineDistance(normalize=normalize, ignore_zeros=ignore_zeros)
+
+
+def _make_mask(guesses, missing) -> Floats2d:
+    xp = get_array_module(guesses)
+    mask = xp.ones(guesses.shape, dtype="f")
+    mask[missing] = 0
+    return mask
+
+
+def _make_mask_by_value(truths, guesses, missing_value) -> Floats2d:
+    xp = get_array_module(guesses)
+    mask = xp.ones(guesses.shape, dtype="f")
+
+    if missing_value is not None:
+        if truths.ndim == 1:
+            mask[truths == missing_value] = 0.0
+        else:
+            # In 2D truths, labels are encoded as one-hot vectors, so we can get
+            # the label indices using argmax.
+            labels = xp.argmax(truths, axis=-1)
+            mask[labels == missing_value] = 0.0
+
+    return mask
+
+
+__all__ = [
+    "SequenceCategoricalCrossentropy",
+    "CategoricalCrossentropy",
+    "L2Distance",
+    "CosineDistance",
+]
```

### Comparing `thinc-9.0.0.dev3/thinc/model.py` & `thinc-9.0.0.dev4/thinc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,43 @@
-from typing import Dict, List, Callable, Optional, Any, Union, Iterable, Set, cast
-from typing import Generic, Sequence, Tuple, TypeVar, Iterator
 import contextlib
-from contextvars import ContextVar
-import srsly
-from pathlib import Path
 import copy
 import functools
 import threading
+from contextvars import ContextVar
+from pathlib import Path
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import srsly
 
-from .backends import ParamServer, Ops, NumpyOps, CupyOps, get_current_ops
+from .backends import CupyOps, NumpyOps, Ops, ParamServer, get_current_ops
 from .optimizers import Optimizer  # noqa: F401
 from .shims import Shim
-from .util import convert_recursive, is_xp_array, DATA_VALIDATION
-from .util import partial, validate_fwd_input_output
 from .types import FloatsXd
-
+from .util import (
+    DATA_VALIDATION,
+    convert_recursive,
+    is_xp_array,
+    partial,
+    validate_fwd_input_output,
+)
 
 InT = TypeVar("InT")
 OutT = TypeVar("OutT")
 SelfT = TypeVar("SelfT", bound="Model")
 
 context_operators: ContextVar[dict] = ContextVar("context_operators", default={})
```

### Comparing `thinc-9.0.0.dev3/thinc/mypy.py` & `thinc-9.0.0.dev4/thinc/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Dict, List
 import itertools
-from mypy.errors import Errors
+from typing import Dict, List
+
+from mypy.checker import TypeChecker
 from mypy.errorcodes import ErrorCode
+from mypy.errors import Errors
+from mypy.nodes import CallExpr, Decorator, Expression, FuncDef, MypyFile, NameExpr
 from mypy.options import Options
-from mypy.plugin import FunctionContext, Plugin, CheckerPluginInterface
-from mypy.types import Instance, Type, CallableType, TypeVarType
-from mypy.nodes import Expression, CallExpr, NameExpr, FuncDef, Decorator, MypyFile
-from mypy.checker import TypeChecker
+from mypy.plugin import CheckerPluginInterface, FunctionContext, Plugin
 from mypy.subtypes import is_subtype
+from mypy.types import CallableType, Instance, Type, TypeVarType
 
 thinc_model_fullname = "thinc.model.Model"
 chained_out_fullname = "thinc.types.XY_YZ_OutT"
 intoin_outtoout_out_fullname = "thinc.types.XY_XY_OutT"
 
 
 def plugin(version: str):
```

### Comparing `thinc-9.0.0.dev3/thinc/optimizers.py` & `thinc-9.0.0.dev4/thinc/optimizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Any, Dict, Optional, Union, Tuple, List, cast
-from collections import defaultdict
 import itertools
 import math
+from collections import defaultdict
 from types import GeneratorType
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from .backends import get_array_ops
-from .types import Generator, FloatsXd
 from .config import registry
-from .schedules import constant, Schedule
-
+from .schedules import Schedule, constant
+from .types import FloatsXd, Generator
 
 KeyT = Tuple[int, str]
 ScheduleT = Union[float, List[float], Generator, Schedule]
 
 SGD_DEFAULTS: Dict[str, Union[float, bool, int]] = {
     "L2": 0.0,
     "L2_is_weight_decay": True,
```

### Comparing `thinc-9.0.0.dev3/thinc/schedules.py` & `thinc-9.0.0.dev4/thinc/schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Generators that provide different rates, schedules, decays or series."""
-from typing import Any, Callable, Dict, Generator, Generic, Tuple, TypeVar
-from typing import Optional
-from dataclasses import dataclass
 import itertools
+from dataclasses import dataclass
+from typing import Any, Callable, Dict, Generator, Generic, Optional, Tuple, TypeVar
+
 import numpy
 
 from .config import registry
 
 OutT = TypeVar("OutT")
```

### Comparing `thinc-9.0.0.dev3/thinc/shims/mxnet.py` & `thinc-9.0.0.dev4/thinc/shims/mxnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
+# mypy: ignore-errors
+import copy
 from typing import Any, cast
+
 import srsly
-import copy
 
-from ..util import mxnet2xp, convert_recursive, make_tempfile, xp2mxnet
-from ..util import get_array_module
+from ..compat import mxnet as mx
 from ..optimizers import Optimizer
 from ..types import ArgsKwargs, FloatsXd
+from ..util import (
+    convert_recursive,
+    get_array_module,
+    make_tempfile,
+    mxnet2xp,
+    xp2mxnet,
+)
 from .shim import Shim
-from ..compat import mxnet as mx
 
 
 class MXNetShim(Shim):
     """Interface between a MXNet model and a Thinc Model. This container is
     *not* a Thinc Model subclass itself.
     """
```

### Comparing `thinc-9.0.0.dev3/thinc/shims/pytorch.py` & `thinc-9.0.0.dev4/thinc/shims/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-from typing import Any, Dict, Optional, cast, Callable
 import contextlib
-from io import BytesIO
 import itertools
+from io import BytesIO
+from typing import Any, Callable, Dict, Optional, cast
+
 import srsly
 
-from ..util import torch2xp, xp2torch, convert_recursive, iterate_recursive
-from ..util import get_torch_default_device
+from ..backends import CupyOps, context_pools, get_current_ops, set_gpu_allocator
 from ..compat import torch
-from ..backends import get_current_ops, context_pools, CupyOps
-from ..backends import set_gpu_allocator
 from ..optimizers import Optimizer
 from ..types import ArgsKwargs, FloatsXd
+from ..util import (
+    convert_recursive,
+    get_torch_default_device,
+    iterate_recursive,
+    torch2xp,
+    xp2torch,
+)
 from .pytorch_grad_scaler import PyTorchGradScaler
 from .shim import Shim
 
 
 class PyTorchShim(Shim):
     """Interface between a PyTorch model and a Thinc Model. This container is
     *not* a Thinc Model subclass itself.
```

### Comparing `thinc-9.0.0.dev3/thinc/shims/pytorch_grad_scaler.py` & `thinc-9.0.0.dev4/thinc/shims/pytorch_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/shims/shim.py` & `thinc-9.0.0.dev4/thinc/shims/shim.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Any, Optional, Tuple, Callable, Dict, Union
-import copy
 import contextlib
-from pathlib import Path
+import copy
 import threading
+from pathlib import Path
+from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 
 class Shim:  # pragma: no cover
     """Define a basic interface for external models. Users can create subclasses
     of 'shim' to wrap external libraries. We provide shims for PyTorch.
 
     The Thinc Model class treats Shim objects as a sort of special type of
```

### Comparing `thinc-9.0.0.dev3/thinc/shims/tensorflow.py` & `thinc-9.0.0.dev4/thinc/shims/tensorflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Any, Dict, List, Optional
-import catalogue
+# mypy: ignore-errors
 import contextlib
 import copy
 from io import BytesIO
+from typing import Any, Dict, List, Optional
+
+import catalogue
 import numpy
 
 from ..backends import Ops, get_current_ops
+from ..compat import cupy, h5py
+from ..compat import tensorflow as tf
 from ..optimizers import Optimizer
 from ..types import ArgsKwargs, ArrayXd
 from ..util import get_array_module
 from .shim import Shim
-from ..compat import tensorflow as tf
-from ..compat import cupy, h5py
 
 keras_model_fns = catalogue.create("thinc", "keras", entry_points=True)
 
 
 def maybe_handshake_model(keras_model):
     """Call the required predict/compile/build APIs to initialize a model if it
     is a subclass of tf.keras.Model. This is required to be able to call set_weights
```

### Comparing `thinc-9.0.0.dev3/thinc/shims/torchscript.py` & `thinc-9.0.0.dev4/thinc/shims/torchscript.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Any, Optional
 from io import BytesIO
+from typing import Any, Optional
+
 import srsly
 
 from ..compat import torch
 from ..util import get_torch_default_device
 from .pytorch import PyTorchShim
 from .pytorch_grad_scaler import PyTorchGradScaler
 
@@ -53,11 +54,14 @@
 
     def from_bytes(self, bytes_data):
         device = get_torch_default_device()
         msg = srsly.msgpack_loads(bytes_data)
         self.cfg = msg["config"]
         filelike = BytesIO(msg["model"])
         filelike.seek(0)
-        self._model = torch.jit.load(filelike, map_location=device)
+        # As of Torch 2.0.0, loading TorchScript models directly to
+        # an MPS device is not supported.
+        map_location = torch.device("cpu") if device.type == "mps" else device
+        self._model = torch.jit.load(filelike, map_location=map_location)
         self._model.to(device)
         self._grad_scaler.to_(device)
         return self
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/backends/test_ops.py` & `thinc-9.0.0.dev4/thinc/tests/backends/test_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,70 @@
+import inspect
+import platform
 from typing import Tuple, cast
 
-import pytest
 import numpy
-import platform
+import pytest
 from hypothesis import given, settings
 from hypothesis.strategies import composite, integers
 from numpy.testing import assert_allclose
 from packaging.version import Version
-from thinc.api import NumpyOps, CupyOps, Ops, get_ops
-from thinc.api import get_current_ops, use_ops
-from thinc.util import torch2xp, xp2torch
+
+from thinc.api import (
+    LSTM,
+    CupyOps,
+    NumpyOps,
+    Ops,
+    fix_random_seed,
+    get_current_ops,
+    get_ops,
+    use_ops,
+)
+from thinc.backends._custom_kernels import KERNELS, KERNELS_LIST, compile_mmh
 from thinc.compat import has_cupy_gpu, has_torch, torch_version
-from thinc.api import fix_random_seed
-from thinc.api import LSTM
 from thinc.types import Floats2d
-import inspect
+from thinc.util import torch2xp, xp2torch
 
 from .. import strategies
 from ..strategies import arrays_BI, ndarrays_of_shape
 
-
 MAX_EXAMPLES = 10
 
 VANILLA_OPS = Ops(numpy)  # type:ignore
 NUMPY_OPS = NumpyOps()
 BLIS_OPS = NumpyOps(use_blis=True)
 CPU_OPS = [NUMPY_OPS, VANILLA_OPS]
 XP_OPS = [NUMPY_OPS]
 if has_cupy_gpu:
     XP_OPS.append(CupyOps())
 ALL_OPS = XP_OPS + [VANILLA_OPS]
 
 FLOAT_TYPES = ["float32", "float64"]
+INT_TYPES = ["int32", "int64"]
+
+REDUCTIONS = ["reduce_first", "reduce_last", "reduce_max", "reduce_mean", "reduce_sum"]
+
+REDUCE_ZERO_LENGTH_RAISES = [
+    ("reduce_first", True),
+    ("reduce_last", True),
+    ("reduce_max", True),
+    # From a mathematical perspective we'd want mean reduction to raise for
+    # zero-length sequences, since floating point numbers are not a monoid
+    # under averaging. However, floret relies on reduce_mean to return a
+    # zero-vector in this case.
+    ("reduce_mean", False),
+    ("reduce_sum", False),
+]
 
 
 def create_pytorch_funcs():
-    import torch
     import math
 
+    import torch
+
     def torch_relu(x):
         return torch.nn.functional.relu(x)
 
     def torch_relu_k(x):
         return torch.nn.functional.relu6(x)
 
     def torch_hard_sigmoid(x):
@@ -129,14 +152,15 @@
             for i, (p1, p2) in enumerate(zip(annots, base_annots)):
                 if p1 != inspect.Parameter.empty and p2 != inspect.Parameter.empty:
                     # Need to check string value to handle TypeVars etc.
                     assert str(p1) == str(p2), attr
 
 
 @pytest.mark.parametrize("ops", ALL_OPS)
+@pytest.mark.filterwarnings("ignore::RuntimeWarning")
 def test_adam_incorrect_inputs(ops):
     one = ops.xp.zeros(1, dtype="f")
     two = ops.xp.zeros(2, dtype="f")
 
     ops.adam(one, one, one, one, 0.0, 0.0, 0.0, 0.0)
     with pytest.raises(ValueError):
         ops.adam(two, one, one, one, 0.0, 0.0, 0.0, 0.0)
@@ -787,14 +811,47 @@
     flat2 = cpu_ops.flatten([x for x in X], pad=1, dtype="f")
     assert len(flat2) > len(flat)
     unflat2 = cpu_ops.unflatten(flat2, [len(x) for x in X], pad=1)
     assert_allclose(X, unflat2)
 
 
 @pytest.mark.parametrize("ops", ALL_OPS)
+@pytest.mark.parametrize("dtype", FLOAT_TYPES + INT_TYPES)
+def test_pad(ops, dtype):
+    X = [ops.xp.arange(1, 3, dtype=dtype), ops.xp.arange(1, 5, dtype=dtype)]
+    ops.xp.testing.assert_allclose(ops.pad(X), [[1, 2, 0, 0], [1, 2, 3, 4]])
+    ops.xp.testing.assert_allclose(
+        ops.pad(X, round_to=8), [[1, 2, 0, 0, 0, 0, 0, 0], [1, 2, 3, 4, 0, 0, 0, 0]]
+    )
+
+    X = [
+        ops.xp.arange(1, 5, dtype=dtype).reshape(2, 2),
+        ops.xp.arange(1, 9, dtype=dtype).reshape(4, 2),
+    ]
+    ops.xp.testing.assert_allclose(
+        ops.pad(X),
+        [
+            [[1, 2], [3, 4], [0, 0], [0, 0]],
+            [[1, 2], [3, 4], [5, 6], [7, 8]],
+        ],
+    )
+
+    ops.xp.testing.assert_allclose(
+        ops.pad(X, round_to=5),
+        [
+            [[1, 2], [3, 4], [0, 0], [0, 0], [0, 0]],
+            [[1, 2], [3, 4], [5, 6], [7, 8], [0, 0]],
+        ],
+    )
+
+    with pytest.raises(ValueError, match=r"Rounding for padding must at least be 1"):
+        ops.pad(X, round_to=0)
+
+
+@pytest.mark.parametrize("ops", ALL_OPS)
 @pytest.mark.parametrize("dtype", FLOAT_TYPES)
 def test_reduce_sum(ops, dtype):
     X = ops.asarray2f(
         [[1.0, 2.0], [3.0, 4.0], [5.0, 6.0], [1.0, 2.0], [3.0, 4.0]], dtype=dtype
     )
     lengths = ops.asarray1i([3, 2])
     ops.xp.testing.assert_allclose(
@@ -1031,14 +1088,79 @@
         ops.backprop_reduce_mean(
             ops.xp.arange(1, 7, dtype=dtype).reshape(2, 3),
             ops.xp.array([-1, 2], dtype="int32"),
         )
 
 
 @pytest.mark.parametrize("ops", ALL_OPS)
+@pytest.mark.parametrize("dtype", FLOAT_TYPES)
+@pytest.mark.parametrize("reduction", REDUCTIONS)
+def test_reduce_empty_batch(ops, dtype, reduction):
+    func = getattr(ops, reduction)
+    backprop_func = getattr(ops, f"backprop_{reduction}")
+
+    lengths = ops.asarray1i([])
+    Y = func(ops.alloc((0, 10), dtype=dtype), lengths)
+
+    if reduction == "reduce_max":
+        Y, which = Y
+        dX = backprop_func(Y, which, lengths)
+    elif isinstance(Y, tuple):
+        Y, extra = Y
+        dX = backprop_func(Y, extra)
+    else:
+        dX = backprop_func(Y, lengths)
+
+    assert Y.shape == (0, 10)
+    assert dX.shape == (0, 10)
+
+
+@pytest.mark.parametrize("ops", ALL_OPS)
+@pytest.mark.parametrize("dtype", FLOAT_TYPES)
+@pytest.mark.parametrize("reduction", REDUCTIONS)
+def test_reduce_empty_hidden(ops, dtype, reduction):
+    func = getattr(ops, reduction)
+    backprop_func = getattr(ops, f"backprop_{reduction}")
+
+    lengths = ops.asarray1i([2, 3])
+    Y = func(ops.alloc((5, 0), dtype=dtype), lengths)
+
+    if reduction == "reduce_max":
+        Y, which = Y
+        dX = backprop_func(Y, which, lengths)
+    elif isinstance(Y, tuple):
+        Y, extra = Y
+        dX = backprop_func(Y, extra)
+    else:
+        dX = backprop_func(Y, lengths)
+
+    assert Y.shape == (2, 0)
+    assert dX.shape == (5, 0)
+
+
+@pytest.mark.parametrize("ops", ALL_OPS)
+@pytest.mark.parametrize("dtype", FLOAT_TYPES)
+@pytest.mark.parametrize("reduction_raises", REDUCE_ZERO_LENGTH_RAISES)
+def test_reduce_zero_seq_length(ops, dtype, reduction_raises):
+    reduction_str, raises = reduction_raises
+    reduction = getattr(ops, reduction_str)
+    X = ops.asarray2f(
+        [[1.0, 2.0], [3.0, 4.0], [5.0, 6.0], [1.0, 2.0], [3.0, 4.0]], dtype=dtype
+    )
+    lengths = ops.asarray1i([3, 0, 2])
+
+    if raises:
+        with pytest.raises(ValueError):
+            reduction(X, lengths)
+    else:
+        # All non-raising reductions have zero as their identity element.
+        ops.xp.testing.assert_allclose(reduction(X, lengths)[1], [0.0, 0.0])
+
+
+@pytest.mark.parametrize("ops", ALL_OPS)
 @settings(max_examples=MAX_EXAMPLES, deadline=None)
 @given(X=strategies.arrays_BI())
 def test_mish(ops, X):
     X = ops.asarray(X)
     Y = ops.mish(X)
     assert Y.shape == X.shape
     assert not ops.xp.isnan(Y).any()
@@ -1462,7 +1584,23 @@
     y = ops.to_numpy(x, byte_order=byte_order)
     assert numpy.array_equal(ops.to_numpy(x), ops.to_numpy(y))
     if byte_order in (">", "<"):
         # hack from: https://stackoverflow.com/a/49740663
         assert y.dtype.newbyteorder("S").newbyteorder("S").byteorder == byte_order
     else:
         assert x.dtype.byteorder == y.dtype.byteorder
+
+
+@pytest.mark.skipif(not has_cupy_gpu, reason="needs GPU/CuPy")
+def test_custom_kernel_compilation():
+    for kernel_name in KERNELS_LIST:
+        compiled_kernel = KERNELS.get_function(kernel_name)
+        assert compiled_kernel is not None
+
+    assert compile_mmh() is not None
+
+
+@pytest.mark.parametrize("ops", ALL_OPS)
+def test_asarray_from_list_uint64(ops):
+    # list contains int values both above and below int64.max
+    uint64_list = [16, 11648197037703959513]
+    assert uint64_list == list(ops.asarray(uint64_list, dtype="uint64"))
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/conftest.py` & `thinc-9.0.0.dev4/thinc/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,18 @@
         if opt in item.keywords and not getopt(opt):
             pytest.skip(f"need --{opt} option to run")
 
 
 @pytest.fixture()
 def pathy_fixture():
     pytest.importorskip("pathy")
-    import tempfile
     import shutil
-    from pathy import use_fs, Pathy
+    import tempfile
+
+    from pathy import Pathy, use_fs
 
     temp_folder = tempfile.mkdtemp(prefix="thinc-pathy")
     use_fs(temp_folder)
 
     root = Pathy("gs://test-bucket")
     root.mkdir(exist_ok=True)
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_basic_tagger.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_basic_tagger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,22 @@
-import pytest
 import random
-from thinc.api import Model, Relu, Softmax, HashEmbed, expand_window
-from thinc.api import chain, with_array, Adam, strings2arrays
+
+import pytest
+
+from thinc.api import (
+    Adam,
+    HashEmbed,
+    Model,
+    Relu,
+    Softmax,
+    chain,
+    expand_window,
+    strings2arrays,
+    with_array,
+)
 
 
 @pytest.fixture(scope="module")
 def ancora():
     pytest.importorskip("ml_datasets")
     import ml_datasets
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_combinators.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_combinators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-import pytest
 import numpy
+import pytest
 from numpy.testing import assert_allclose
-from thinc.api import clone, concatenate, noop, add, map_list
-from thinc.api import Linear, Dropout, Model, NumpyOps
+
+from thinc.api import (
+    Dropout,
+    Linear,
+    Model,
+    NumpyOps,
+    add,
+    clone,
+    concatenate,
+    map_list,
+    noop,
+)
 from thinc.layers import chain, tuplify
 
 
 @pytest.fixture(params=[1, 2, 9])
 def nB(request):
     return request.param
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_feed_forward.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_feed_forward.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import pytest
-import numpy
 from functools import partial
+
+import numpy
+import pytest
 from numpy.testing import assert_allclose
-from thinc.api import chain, Linear, Relu, NumpyOps
+
+from thinc.api import Linear, NumpyOps, Relu, chain
 
 
 @pytest.fixture(params=[1, 2, 9])
 def nB(request):
     return request.param
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_hash_embed.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_hash_embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy
+
 from thinc.api import HashEmbed
 
 
 def test_init():
     model = HashEmbed(64, 1000).initialize()
     assert model.get_dim("nV") == 1000
     assert model.get_dim("nO") == 64
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_layers_api.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_layers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import List, Optional
 
-from numpy.testing import assert_almost_equal
-from thinc.api import registry, with_padded, Dropout, NumpyOps, Model
-from thinc.backends import NumpyOps
-from thinc.util import data_validation, get_width
-from thinc.types import Ragged, Padded, Array2d, Floats2d, FloatsXd, Shape
-from thinc.compat import has_torch
 import numpy
 import pytest
 import srsly
+from numpy.testing import assert_almost_equal
+
+from thinc.api import Dropout, Model, NumpyOps, registry, with_padded
+from thinc.backends import NumpyOps
+from thinc.compat import has_torch
+from thinc.types import Array2d, Floats2d, FloatsXd, Padded, Ragged, Shape
+from thinc.util import data_validation, get_width
 
 OPS = NumpyOps()
 
 
 class NoDropoutOps(NumpyOps):
     def get_dropout_mask(self, shape: Shape, drop: Optional[float]) -> FloatsXd:
         if drop is None or drop <= 0:
@@ -124,14 +125,16 @@
     ("Embed.v1", {"nO": 4, "nV": int(array2dint.max() + 1), "column": 0, "dropout": 0.2}, array2dint, array2d),
     ("Embed.v1", {"nO": 4, "nV": int(array1dint.max() + 1)}, array1dint, array2d),
     ("HashEmbed.v1", {"nO": 1, "nV": int(array2dint.max()), "column": 0, "dropout": 0.2}, array2dint, array2d),
     ("HashEmbed.v1", {"nO": 1, "nV": 2}, array1dint, array2d),
     ("MultiSoftmax.v1", {"nOs": (1, 3)}, array2d, array2d),
     # ("CauchySimilarity.v1", {}, (array2d, array2d), array1d),
     ("ParametricAttention.v1", {}, ragged, ragged),
+    ("ParametricAttention.v2", {}, ragged, ragged),
+    ("ParametricAttention.v2", {"key_transform": {"@layers": "Gelu.v1"}}, ragged, ragged),
     ("SparseLinear.v1", {}, (numpy.asarray([1, 2, 3], dtype="uint64"), array1d, numpy.asarray([1, 1], dtype="i")), array2d),
     ("SparseLinear.v2", {}, (numpy.asarray([1, 2, 3], dtype="uint64"), array1d, numpy.asarray([1, 1], dtype="i")), array2d),
     ("remap_ids.v1", {"dtype": "f"}, ["a", 1, 5.0], array2dint),
     ("remap_ids.v2", {"mapping_table": {}, "column": 1}, numpy.array([[1, 2, 3], [4, 5, 6]]).T, array2dint),
     ("premap_ids.v1", {"mapping_table": {}, "column": 1}, numpy.array([[1, 2, 3], [4, 5, 6]]).T, array2dint),
     # fmt: on
 ]
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_linear.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import numpy
 import pytest
-from mock import MagicMock
 from hypothesis import given, settings
-import numpy
+from mock import MagicMock
 from numpy.testing import assert_allclose
-from thinc.api import Linear, chain, Dropout, SGD
+
+from thinc.api import SGD, Dropout, Linear, chain
 
 from ..strategies import arrays_OI_O_BI
 from ..util import get_model, get_shape
 
 
 @pytest.fixture
 def model():
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_lstm.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_lstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import numpy
 import timeit
-from thinc.api import NumpyOps, LSTM, PyTorchLSTM, with_padded, fix_random_seed
-from thinc.api import Ops
-from thinc.compat import has_torch
+
+import numpy
 import pytest
 
+from thinc.api import LSTM, NumpyOps, Ops, PyTorchLSTM, fix_random_seed, with_padded
+from thinc.compat import has_torch
+
 
 @pytest.fixture(params=[1, 6])
 def nI(request):
     return request.param
 
 
 @pytest.fixture(params=[1, 2, 7, 9])
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_mappers.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_mappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pytest
 import numpy
+import pytest
+
 from thinc.layers import premap_ids, remap_ids, remap_ids_v2
 
 
 @pytest.fixture
 def keys():
     return numpy.array([4, 2, 6, 1, 8, 7, 9, 3, 30])
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_mnist.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_mnist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import pytest
-from thinc.api import Relu, Softmax, chain, clone, Adam
-from thinc.api import PyTorchWrapper, TensorFlowWrapper
-from thinc.api import get_current_ops
-from thinc.compat import has_torch, has_tensorflow
+
+from thinc.api import (
+    Adam,
+    PyTorchWrapper,
+    Relu,
+    Softmax,
+    TensorFlowWrapper,
+    chain,
+    clone,
+    get_current_ops,
+)
+from thinc.compat import has_tensorflow, has_torch
 
 
 @pytest.fixture(scope="module")
 def mnist(limit=5000):
     pytest.importorskip("ml_datasets")
     import ml_datasets
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_mxnet_wrapper.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_mxnet_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from typing import cast
 
 import numpy
 import pytest
-from thinc.api import Adam, ArgsKwargs, Model, Ops, MXNetWrapper
-from thinc.api import get_current_ops, mxnet2xp, xp2mxnet
-from thinc.types import Array2d, Array1d, IntsXd
+
+from thinc.api import (
+    Adam,
+    ArgsKwargs,
+    Model,
+    MXNetWrapper,
+    Ops,
+    get_current_ops,
+    mxnet2xp,
+    xp2mxnet,
+)
 from thinc.compat import has_cupy_gpu, has_mxnet
+from thinc.types import Array1d, Array2d, IntsXd
 from thinc.util import to_categorical
 
 from ..util import check_input_converters, make_tempdir
 
 
 @pytest.fixture
 def n_hidden() -> int:
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_pytorch_wrapper.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_pytorch_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-from thinc.api import Linear, SGD, PyTorchWrapper, PyTorchWrapper_v2, PyTorchWrapper_v3
-from thinc.api import xp2torch, torch2xp, ArgsKwargs, use_ops
-from thinc.api import chain, get_current_ops, Relu
-from thinc.api import CupyOps, MPSOps, NumpyOps
+import numpy
+import pytest
+
+from thinc.api import (
+    SGD,
+    ArgsKwargs,
+    CupyOps,
+    Linear,
+    MPSOps,
+    NumpyOps,
+    PyTorchWrapper,
+    PyTorchWrapper_v2,
+    PyTorchWrapper_v3,
+    Relu,
+    chain,
+    get_current_ops,
+    torch2xp,
+    use_ops,
+    xp2torch,
+)
 from thinc.backends import context_pools
+from thinc.compat import has_cupy_gpu, has_torch, has_torch_amp, has_torch_mps_gpu
 from thinc.layers.pytorchwrapper import PyTorchWrapper_v3
+from thinc.shims.pytorch import (
+    default_deserialize_torch_model,
+    default_serialize_torch_model,
+)
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
-from thinc.shims.pytorch import default_deserialize_torch_model
-from thinc.shims.pytorch import default_serialize_torch_model
-from thinc.compat import has_torch, has_torch_amp
-from thinc.compat import has_cupy_gpu, has_torch_mps_gpu
-import numpy
-import pytest
 from thinc.util import get_torch_default_device
 
-from ..util import make_tempdir, check_input_converters
-
+from ..util import check_input_converters, make_tempdir
 
 XP_OPS = [NumpyOps()]
 if has_cupy_gpu:
     XP_OPS.append(CupyOps())
 if has_torch_mps_gpu:
     XP_OPS.append(MPSOps())
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_reduce.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import pytest
 import numpy
+import pytest
+
 from thinc.api import reduce_first, reduce_last, reduce_max, reduce_mean, reduce_sum
 from thinc.types import Ragged
 
 
 @pytest.fixture
 def Xs():
     seqs = [numpy.zeros((10, 8), dtype="f"), numpy.zeros((4, 8), dtype="f")]
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_resizable.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_resizable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import pytest
 from functools import partial
-from thinc.api import resizable, Linear
-from thinc.layers.resizable import resize_model, resize_linear_weighted
+
+import pytest
+
+from thinc.api import Linear, resizable
+from thinc.layers.resizable import resize_linear_weighted, resize_model
 
 
 @pytest.fixture
 def model():
     output_layer = Linear(nO=None, nI=None)
     fill_defaults = {"b": 0, "W": 0}
     model = resizable(
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_shim.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_shim.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import List
+
 from thinc.shims.shim import Shim
+
 from ..util import make_tempdir
 
 
 class MockShim(Shim):
     def __init__(self, data: List[int]):
         super().__init__(None, config=None, optimizer=None)
         self.data = data
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_softmax.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_softmax.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, cast
 
 import numpy
-from numpy.testing import assert_allclose
 import pytest
+from numpy.testing import assert_allclose
 
 from thinc.api import Model, NumpyOps, Softmax_v2
 from thinc.types import Floats2d, Ints1d
 from thinc.util import has_torch, torch2xp, xp2torch
 
 OPS = NumpyOps()
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_sparse_linear.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_sparse_linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import math
+
 import numpy
 import pytest
-from thinc.api import SGD, to_categorical, SparseLinear, SparseLinear_v2
+
+from thinc.api import SGD, SparseLinear, SparseLinear_v2, to_categorical
 
 
 @pytest.fixture
 def instances():
     lengths = numpy.asarray([5, 4], dtype="int32")
     keys = numpy.arange(9, dtype="uint64")
     values = numpy.ones(9, dtype="float32")
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_tensorflow_wrapper.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_tensorflow_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import numpy
 import pytest
-from thinc.api import Adam, ArgsKwargs, Linear, Model, TensorFlowWrapper
-from thinc.api import get_current_ops, keras_subclass, tensorflow2xp, xp2tensorflow
-from thinc.util import to_categorical
+
+from thinc.api import (
+    Adam,
+    ArgsKwargs,
+    Linear,
+    Model,
+    TensorFlowWrapper,
+    get_current_ops,
+    keras_subclass,
+    tensorflow2xp,
+    xp2tensorflow,
+)
 from thinc.compat import has_cupy_gpu, has_tensorflow
+from thinc.util import to_categorical
 
 from ..util import check_input_converters, make_tempdir
 
 
 @pytest.fixture
 def n_hidden():
     return 12
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_torchscriptwrapper.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_torchscriptwrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import pytest
 import numpy
+import pytest
 
-from thinc.api import PyTorchWrapper_v2, TorchScriptWrapper_v1
-from thinc.api import pytorch_to_torchscript_wrapper
+from thinc.api import (
+    PyTorchWrapper_v2,
+    TorchScriptWrapper_v1,
+    pytorch_to_torchscript_wrapper,
+)
 from thinc.compat import has_torch, torch
 
 
 @pytest.mark.skipif(not has_torch, reason="needs PyTorch")
 @pytest.mark.parametrize("nN,nI,nO", [(2, 3, 4)])
 def test_pytorch_script(nN, nI, nO):
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_transforms.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from thinc.api import strings2arrays, NumpyOps, Ragged, registry
 import numpy
 import pytest
 
+from thinc.api import NumpyOps, Ragged, registry, strings2arrays
+
 from ..util import get_data_checker
 
 
 @pytest.fixture(params=[[], [(10, 2)], [(5, 3), (1, 3)], [(2, 3), (0, 3), (1, 3)]])
 def shapes(request):
     return request.param
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_uniqued.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_uniqued.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import pytest
 import numpy
+import pytest
+from hypothesis import given, settings
+from hypothesis.strategies import composite, integers, lists
+from numpy.testing import assert_allclose
+
 from thinc.layers import Embed
 from thinc.layers.uniqued import uniqued
-from numpy.testing import assert_allclose
-from hypothesis import given, settings
-from hypothesis.strategies import integers, lists, composite
 
 ROWS = 10
 
 # This test uses a newer hypothesis feature than the skanky flatmap-style
 # I used previously. This is much nicer, although it still takes some getting
 # used to. The key feature is this composite decorator. It injects a function,
 # 'draw'.
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_with_debug.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_with_debug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from mock import MagicMock
-from thinc.api import with_debug, Linear
+
+from thinc.api import Linear, with_debug
 
 
 def test_with_debug():
     on_init = MagicMock()
     on_forward = MagicMock()
     on_backprop = MagicMock()
     model = with_debug(
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_with_flatten.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_with_flatten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+
 from thinc.api import Model, with_flatten_v2
 
 INPUT = [[1, 2, 3], [4, 5], [], [6, 7, 8]]
 INPUT_FLAT = [1, 2, 3, 4, 5, 6, 7, 8]
 OUTPUT = [[2, 3, 4], [5, 6], [], [7, 8, 9]]
 BACKPROP_OUTPUT = [[3, 4, 5], [6, 7], [], [8, 9, 10]]
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/layers/test_with_transforms.py` & `thinc-9.0.0.dev4/thinc/tests/layers/test_with_transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-import pytest
 import numpy
 import numpy.testing
-from thinc.api import NumpyOps, Model, Linear, noop
-from thinc.api import with_array2d, with_array, with_padded, with_list
-from thinc.api import with_ragged, with_getitem
-from thinc.types import Padded, Ragged
+import pytest
 
+from thinc.api import (
+    Linear,
+    Model,
+    NumpyOps,
+    noop,
+    with_array,
+    with_array2d,
+    with_getitem,
+    with_list,
+    with_padded,
+    with_ragged,
+)
+from thinc.types import Padded, Ragged
 
 from ..util import get_data_checker
 
 
 @pytest.fixture(params=[[], [(10, 2)], [(5, 3), (1, 3)], [(2, 3), (0, 3), (1, 3)]])
 def shapes(request):
     return request.param
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/model/test_model.py` & `thinc-9.0.0.dev4/thinc/tests/model/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,32 @@
-from collections import Counter
-import pytest
 import threading
 import time
-from thinc.api import Adam, CupyOps, Dropout, Linear, Model, Relu
-from thinc.api import Shim, Softmax, chain, change_attr_values
-from thinc.api import concatenate, set_dropout_rate
-from thinc.api import use_ops, with_debug, wrap_model_recursive
-from thinc.compat import has_cupy_gpu
+from collections import Counter
+
 import numpy
+import pytest
+
+from thinc.api import (
+    Adam,
+    CupyOps,
+    Dropout,
+    Linear,
+    Model,
+    Relu,
+    Shim,
+    Softmax,
+    chain,
+    change_attr_values,
+    concatenate,
+    set_dropout_rate,
+    use_ops,
+    with_debug,
+    wrap_model_recursive,
+)
+from thinc.compat import has_cupy_gpu
 
 from ..util import make_tempdir
 
 
 @pytest.fixture
 def model_with_no_args():
     return Linear()
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/model/test_validation.py` & `thinc-9.0.0.dev4/thinc/tests/model/test_validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 import pytest
-from thinc.api import chain, Relu, reduce_max, Softmax, with_ragged
-from thinc.api import ParametricAttention, list2ragged, reduce_sum
+
+from thinc.api import (
+    ParametricAttention,
+    Relu,
+    Softmax,
+    chain,
+    list2ragged,
+    reduce_max,
+    reduce_sum,
+    with_ragged,
+)
 from thinc.util import DataValidationError, data_validation
 
 
 def test_validation():
     model = chain(Relu(10), Relu(10), with_ragged(reduce_max()), Softmax())
     with data_validation(True):
         with pytest.raises(DataValidationError):
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/mypy/modules/fail_plugin.py` & `thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thinc.api import chain, Relu, reduce_max, Softmax, add, concatenate
+from thinc.api import Relu, Softmax, add, chain, concatenate, reduce_max
 
 bad_model = chain(Relu(10), reduce_max(), Softmax())
 
 bad_model2 = add(Relu(10), reduce_max(), Softmax())
 
 bad_model_only_plugin = chain(
     Relu(10), Relu(10), Relu(10), Relu(10), reduce_max(), Softmax()
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/mypy/modules/success_plugin.py` & `thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, TypeVar
 
-from thinc.api import chain, Relu, reduce_max, Softmax, add, Model
+from thinc.api import Model, Relu, Softmax, add, chain, reduce_max
 
 good_model = chain(Relu(10), Relu(10), Softmax())
 reveal_type(good_model)
 
 good_model2 = add(Relu(10), Relu(10), Softmax())
 reveal_type(good_model2)
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/mypy/outputs/fail-plugin.txt` & `thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/tests/mypy/outputs/success-no-plugin.txt` & `thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-no-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/tests/mypy/test_mypy.py` & `thinc-9.0.0.dev4/thinc/tests/mypy/test_mypy.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
-from pathlib import Path
 import shutil
 import sys
+from pathlib import Path
 
 import pytest
 
 mypy = pytest.importorskip("mypy")
 
 # You can change the following variable to True during development to overwrite expected output with generated output
 GENERATE = False
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/regression/issue519/test_issue519.py` & `thinc-9.0.0.dev4/thinc/tests/regression/issue519/test_issue519.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/tests/regression/test_issue564.py` & `thinc-9.0.0.dev4/thinc/tests/regression/test_issue564.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/tests/shims/test_pytorch_grad_scaler.py` & `thinc-9.0.0.dev4/thinc/tests/shims/test_pytorch_grad_scaler.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
-
 from hypothesis import given, settings
 from hypothesis.strategies import lists, one_of, tuples
+
+from thinc.api import PyTorchGradScaler
 from thinc.compat import has_torch, has_torch_amp, has_torch_cuda_gpu, torch
 from thinc.util import is_torch_array
-from thinc.api import PyTorchGradScaler
 
 from ..strategies import ndarrays
 
 
 def tensors():
     return ndarrays().map(lambda a: torch.tensor(a).cuda())
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/strategies.py` & `thinc-9.0.0.dev4/thinc/tests/strategies.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy
-from hypothesis.strategies import just, tuples, integers, floats
 from hypothesis.extra.numpy import arrays
-from thinc.api import NumpyOps, Linear
+from hypothesis.strategies import floats, integers, just, tuples
+
+from thinc.api import Linear, NumpyOps
 
 
 def get_ops():
     return NumpyOps()
 
 
 def get_model(W_values, b_values):
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_config.py` & `thinc-9.0.0.dev4/thinc/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-import pytest
-from typing import Iterable, Union, Optional, List, Callable, Dict, Any
+import inspect
+import pickle
 from types import GeneratorType
-from pydantic import BaseModel, StrictBool, StrictFloat, PositiveInt, constr
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+
 import catalogue
+import numpy
+import pytest
+
+try:
+    from pydantic.v1 import BaseModel, PositiveInt, StrictBool, StrictFloat, constr
+except ImportError:
+    from pydantic import BaseModel, PositiveInt, StrictBool, StrictFloat, constr  # type: ignore
+
 import thinc.config
+from thinc.api import Config, Model, NumpyOps, RAdam
 from thinc.config import ConfigValidationError
 from thinc.types import Generator, Ragged
-from thinc.api import Config, RAdam, Model, NumpyOps
 from thinc.util import partial
-import numpy
-import inspect
-import pickle
 
 from .util import make_tempdir
 
-
 EXAMPLE_CONFIG = """
 [optimizer]
 @optimizers = "Adam.v1"
 beta1 = 0.9
 beta2 = 0.999
 use_averages = true
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_examples.py` & `thinc-9.0.0.dev4/thinc/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_import__all__.py` & `thinc-9.0.0.dev4/thinc/tests/test_import__all__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
+import importlib
 from collections import namedtuple
-from typing import Tuple, List
+from typing import List, Tuple
 
 import pytest
-import importlib
 
 _Import = namedtuple("_Import", ["module", "name", "alias"])
 
 
 def get_imports(path: str) -> Tuple[_Import, ...]:
     """Parse Python file at path, retrieve import statements.
     Adapted from https://stackoverflow.com/a/9049549.
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_indexing.py` & `thinc-9.0.0.dev4/thinc/tests/test_indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pytest
 import numpy
+import pytest
 from numpy.testing import assert_allclose
-from thinc.types import Ragged, Pairs
+
+from thinc.types import Pairs, Ragged
 
 
 @pytest.fixture
 def ragged():
     data = numpy.zeros((20, 4), dtype="f")
     lengths = numpy.array([4, 2, 8, 1, 4], dtype="i")
     data[0] = 0
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_initializers.py` & `thinc-9.0.0.dev4/thinc/tests/test_initializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import numpy
 import pytest
-from thinc.api import glorot_uniform_init, zero_init, uniform_init, normal_init
-from thinc.api import NumpyOps
+
 from thinc import registry
-import numpy
+from thinc.api import (
+    NumpyOps,
+    glorot_uniform_init,
+    normal_init,
+    uniform_init,
+    zero_init,
+)
 
 
 @pytest.mark.parametrize(
     "init_func", [glorot_uniform_init, zero_init, uniform_init, normal_init]
 )
 def test_initializer_func_setup(init_func):
     ops = NumpyOps()
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_optimizers.py` & `thinc-9.0.0.dev4/thinc/tests/test_optimizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import pytest
-from thinc.api import registry, Optimizer
-from thinc.optimizers import KeyT, _wrap_generator
 import numpy
+import pytest
 
+from thinc.api import Optimizer, registry
+from thinc.optimizers import KeyT, _wrap_generator
 
 STUB_KEY: KeyT = (0, "")
 
 
 def _test_schedule_valid():
     while True:
         yield 0.456
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_schedules.py` & `thinc-9.0.0.dev4/thinc/tests/test_schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 from itertools import islice
+
 import pytest
-from thinc.api import decaying, compounding, slanted_triangular, constant_then
-from thinc.api import constant, warmup_linear, cyclic_triangular
-from thinc.optimizers import KeyT
+
+from thinc.api import (
+    compounding,
+    constant,
+    constant_then,
+    cyclic_triangular,
+    decaying,
+    slanted_triangular,
+    warmup_linear,
+)
 from thinc.schedules import plateau
 
 
 def test_decaying_rate():
     rates = decaying(0.001, 1e-4)
     rate = rates(step=0)
     assert rate == 0.001
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_serialize.py` & `thinc-9.0.0.dev4/thinc/tests/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 import pytest
 import srsly
-from thinc.api import with_array, Linear, Maxout, chain, Model, Shim
-from thinc.api import serialize_attr, deserialize_attr
+
+from thinc.api import (
+    Linear,
+    Maxout,
+    Model,
+    Shim,
+    chain,
+    deserialize_attr,
+    serialize_attr,
+    with_array,
+)
 
 
 @pytest.fixture
 def linear():
     return Linear(5, 3)
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_types.py` & `thinc-9.0.0.dev4/thinc/tests/test_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 import numpy
-from pydantic import create_model, ValidationError
-from thinc.types import Floats1d, Floats2d, Floats3d, Floats4d
-from thinc.types import Ints1d, Ints2d, Ints3d, Ints4d
 import pytest
 
+from thinc.types import (
+    Floats1d,
+    Floats2d,
+    Floats3d,
+    Floats4d,
+    Ints1d,
+    Ints2d,
+    Ints3d,
+    Ints4d,
+)
+
+try:
+    from pydantic.v1 import ValidationError, create_model
+except ImportError:
+    from pydantic import ValidationError, create_model  # type: ignore
+
+
+from thinc.types import (
+    Floats1d,
+    Floats2d,
+    Floats3d,
+    Floats4d,
+    Ints1d,
+    Ints2d,
+    Ints3d,
+    Ints4d,
+)
+
 
 @pytest.mark.parametrize(
     "arr,arr_type",
     [
         (numpy.zeros(0, dtype=numpy.float32), Floats1d),
         (numpy.zeros((0, 0), dtype=numpy.float32), Floats2d),
         (numpy.zeros((0, 0, 0), dtype=numpy.float32), Floats3d),
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/test_util.py` & `thinc-9.0.0.dev4/thinc/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-import pytest
 import numpy
+import pytest
 from hypothesis import given
-from thinc.api import get_width, Ragged, Padded
-from thinc.util import get_array_module, is_numpy_array, to_categorical
-from thinc.util import is_cupy_array
-from thinc.util import convert_recursive
-from thinc.util import smooth_one_hot
-from thinc.types import ArgsKwargs
 
+from thinc.api import Padded, Ragged, get_width
+from thinc.types import ArgsKwargs
+from thinc.util import (
+    convert_recursive,
+    get_array_module,
+    is_cupy_array,
+    is_numpy_array,
+    to_categorical,
+)
 
 from . import strategies
 
 ALL_XP = [numpy]
 try:
     import cupy
 
@@ -143,34 +146,14 @@
     with pytest.raises(ValueError, match=r"label_smoothing parameter"):
         to_categorical(numpy.asarray([0, 1, 2, 3, 4]), label_smoothing=0.8)
 
     with pytest.raises(ValueError, match=r"label_smoothing parameter"):
         to_categorical(numpy.asarray([0, 1, 2, 3, 4]), label_smoothing=0.88)
 
 
-@given(
-    n_classes=strategies.lengths(lo=2, hi=100),
-    n_samples=strategies.lengths(lo=1, hi=100),
-    label_smoothing=strategies.floats(min_value=0.0, max_value=1.0)
-)
-def test_smooth_one_hot(n_samples, n_classes, label_smoothing):
-    one_hot = numpy.zeros((n_samples, n_classes))
-    labels = numpy.random.randint(0, n_classes, (n_samples,))
-    one_hot[numpy.arange(n_samples), labels] = 1
-    max_smooth = (n_classes - 1) / n_classes
-    if label_smoothing >= max_smooth:
-        with pytest.raises(ValueError, match=r"label_smoothing parameter has to be less than"):
-            smooth_one_hot(one_hot, label_smoothing)
-    else:
-        smoothed = smooth_one_hot(one_hot, label_smoothing)
-        assert numpy.all(numpy.argmax(smoothed, axis=1) == labels)
-        assert smoothed.shape == one_hot.shape
-        assert numpy.allclose(smoothed.sum(1), 1.0)
-
-
 def test_convert_recursive():
     is_match = lambda obj: obj == "foo"
     convert_item = lambda obj: obj.upper()
     obj = {
         "a": {("b", "foo"): {"c": "foo", "d": ["foo", {"e": "foo", "f": (1, "foo")}]}}
     }
     result = convert_recursive(is_match, convert_item, obj)
```

### Comparing `thinc-9.0.0.dev3/thinc/tests/util.py` & `thinc-9.0.0.dev4/thinc/tests/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import contextlib
-from pathlib import Path
-import tempfile
 import shutil
-from thinc.api import Linear, Ragged, Padded, ArgsKwargs
+import tempfile
+from pathlib import Path
+
 import numpy
 import pytest
+
+from thinc.api import ArgsKwargs, Linear, Padded, Ragged
 from thinc.util import has_cupy, is_cupy_array, is_numpy_array
 
 
 @contextlib.contextmanager
 def make_tempdir():
     d = Path(tempfile.mkdtemp())
     yield d
```

### Comparing `thinc-9.0.0.dev3/thinc/types.py` & `thinc-9.0.0.dev4/thinc/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,43 @@
-from typing import Union, Tuple, Sized, Container, Any, TypeVar, Callable
-from typing import Iterable, Iterator, Sequence, Dict, Generic, cast
-from typing import Optional, List, overload
+import sys
 from abc import abstractmethod
 from dataclasses import dataclass
+from typing import (
+    Any,
+    Callable,
+    Container,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Sized,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
+
 import numpy
-import sys
-from .compat import has_cupy, cupy
+
+from .compat import cupy, has_cupy
 
 if has_cupy:
     get_array_module = cupy.get_array_module
 else:
     get_array_module = lambda obj: numpy
 
 # Use typing_extensions for Python versions < 3.8
 if sys.version_info < (3, 8):
-    from typing_extensions import Protocol, Literal
+    from typing_extensions import Literal, Protocol
 else:
-    from typing import Protocol, Literal  # noqa: F401
+    from typing import Literal, Protocol  # noqa: F401
 
 
 # fmt: off
 XY_YZ_OutT = TypeVar("XY_YZ_OutT")
 XY_XY_OutT = TypeVar("XY_XY_OutT")
 
 DeviceTypes = Literal["cpu", "gpu", "tpu"]
```

### Comparing `thinc-9.0.0.dev3/thinc/util.py` & `thinc-9.0.0.dev4/thinc/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,65 @@
-from typing import Any, Union, Sequence, cast, Dict, Optional, Callable, TypeVar
-from typing import List, Mapping
-from typing import TYPE_CHECKING
-
-import numpy
-import random
+import contextlib
 import functools
-from wasabi import table
-from pydantic import create_model, ValidationError
 import inspect
 import os
+import platform
+import random
 import tempfile
 import threading
-import contextlib
 from contextvars import ContextVar
 from dataclasses import dataclass
-from .compat import has_cupy, has_mxnet, has_torch, has_tensorflow
-from .compat import has_cupy_gpu, has_torch_cuda_gpu, has_gpu
-from .compat import torch, cupy, tensorflow as tf, mxnet as mx, cupy_from_dlpack
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import numpy
+from packaging.version import Version
+
+try:
+    from pydantic.v1 import ValidationError, create_model
+except ImportError:
+    from pydantic import ValidationError, create_model  # type: ignore
+
+import numpy
+from wasabi import table
 
-from .types import ArrayXd, ArgsKwargs, Ragged, Padded, FloatsXd, IntsXd, Floats2d  # noqa: E402
 from . import types  # noqa: E402
+from .compat import (
+    cupy,
+    cupy_from_dlpack,
+    has_cupy,
+    has_cupy_gpu,
+    has_gpu,
+    has_mxnet,
+    has_tensorflow,
+    has_torch,
+    has_torch_cuda_gpu,
+    has_torch_mps,
+)
+from .compat import mxnet as mx
+from .compat import tensorflow as tf
+from .compat import torch
+from .types import ArgsKwargs, ArrayXd, FloatsXd, IntsXd, Padded, Ragged  # noqa: E402
 
 if TYPE_CHECKING:
     from .api import Ops
 
+
 DATA_VALIDATION: ContextVar[bool] = ContextVar("DATA_VALIDATION", default=False)
 
 
 def get_torch_default_device() -> "torch.device":
     if torch is None:
         raise ValueError("Cannot get default Torch device when Torch is not available.")
 
@@ -120,28 +152,28 @@
 def is_torch_mps_array(obj: Any) -> bool:  # pragma: no cover
     return is_torch_array(obj) and hasattr(obj, "is_mps") and obj.is_mps
 
 
 def is_tensorflow_array(obj: Any) -> bool:  # pragma: no cover
     if not has_tensorflow:
         return False
-    elif isinstance(obj, tf.Tensor):
+    elif isinstance(obj, tf.Tensor):  # type: ignore
         return True
     else:
         return False
 
 
 def is_tensorflow_gpu_array(obj: Any) -> bool:  # pragma: no cover
     return is_tensorflow_array(obj) and "GPU:" in obj.device
 
 
 def is_mxnet_array(obj: Any) -> bool:  # pragma: no cover
     if not has_mxnet:
         return False
-    elif isinstance(obj, mx.nd.NDArray):
+    elif isinstance(obj, mx.nd.NDArray):  # type: ignore
         return True
     else:
         return False
 
 
 def is_mxnet_gpu_array(obj: Any) -> bool:  # pragma: no cover
     return is_mxnet_array(obj) and obj.context.device_type != "cpu"
@@ -168,15 +200,15 @@
         torch.cuda.set_device(gpu_id)
 
     return device
 
 
 def require_cpu() -> bool:  # pragma: no cover
     """Use CPU through best available backend."""
-    from .backends import set_current_ops, get_ops
+    from .backends import get_ops, set_current_ops
 
     ops = get_ops("cpu")
     set_current_ops(ops)
 
     return True
 
 
@@ -184,17 +216,23 @@
     """Use GPU if it's available. Returns True if so, False otherwise."""
     if has_gpu:
         require_gpu(gpu_id=gpu_id)
     return has_gpu
 
 
 def require_gpu(gpu_id: int = 0) -> bool:  # pragma: no cover
-    from .backends import set_current_ops, CupyOps, MPSOps
+    from .backends import CupyOps, MPSOps, set_current_ops
 
-    if not has_gpu:
+    if platform.system() == "Darwin" and not has_torch_mps:
+        if has_torch:
+            raise ValueError("Cannot use GPU, installed PyTorch does not support MPS")
+        raise ValueError("Cannot use GPU, PyTorch is not installed")
+    elif platform.system() != "Darwin" and not has_cupy:
+        raise ValueError("Cannot use GPU, CuPy is not installed")
+    elif not has_gpu:
         raise ValueError("No GPU devices detected")
 
     if has_cupy_gpu:
         set_current_ops(CupyOps())
         set_active_gpu(gpu_id)
     else:
         set_current_ops(MPSOps())
@@ -214,15 +252,14 @@
 
 def to_categorical(
     Y: IntsXd,
     n_classes: Optional[int] = None,
     *,
     label_smoothing: float = 0.0,
 ) -> FloatsXd:
-
     if n_classes is None:
         n_classes = int(numpy.max(Y) + 1)  # type: ignore
 
     if label_smoothing < 0.0:
         raise ValueError(
             "Label-smoothing parameter has to be greater than or equal to 0"
         )
@@ -249,40 +286,14 @@
 
     xp = get_array_module(Y)
     label_distr = xp.full((n_classes, n_classes), nongold_prob, dtype="float32")
     xp.fill_diagonal(label_distr, 1 - label_smoothing)
     return label_distr[Y]
 
 
-def smooth_one_hot(X: Floats2d, label_smoothing: float) -> Floats2d:
-    """
-    Apply label-smoothing to one-hot array.
-    """
-    n_classes = X.shape[1]
-    max_smooth = (n_classes - 1) / n_classes
-    if label_smoothing < 0.0:
-        raise ValueError(
-            "Label-smoothing parameter has to be greater than or equal to 0"
-        )
-    if not n_classes > 1:
-        raise ValueError(
-            "n_classes should be greater than 1 when label smoothing is enabled,"
-            f"but {n_classes} was provided."
-        )
-    if label_smoothing >= max_smooth:
-        raise ValueError(
-            f"For {n_classes} classes "
-            "label_smoothing parameter has to be less than "
-            f"{max_smooth}, but found {label_smoothing}."
-        )
-    X[X == 1] = 1 - label_smoothing
-    X[X == 0] = label_smoothing / (n_classes - 1)
-    return X
-
-
 def get_width(
     X: Union[ArrayXd, Ragged, Padded, Sequence[ArrayXd]], *, dim: int = -1
 ) -> int:
     """Infer the 'width' of a batch of data, which could be any of: Array,
     Ragged, Padded or Sequence of Arrays.
     """
     if isinstance(X, Ragged):
@@ -305,23 +316,25 @@
     else:
         err = "Cannot get width of object: has neither shape nor __getitem__"
         raise ValueError(err)
 
 
 def assert_tensorflow_installed() -> None:  # pragma: no cover
     """Raise an ImportError if TensorFlow is not installed."""
-    template = "TensorFlow support requires {pkg}: pip install thinc[tensorflow]"
+    template = "TensorFlow support requires {pkg}: pip install thinc[tensorflow]\n\nEnable TensorFlow support with thinc.api.enable_tensorflow()"
     if not has_tensorflow:
-        raise ImportError(template.format(pkg="tensorflow>=2.0.0"))
+        raise ImportError(template.format(pkg="tensorflow>=2.0.0,<2.6.0"))
 
 
 def assert_mxnet_installed() -> None:  # pragma: no cover
     """Raise an ImportError if MXNet is not installed."""
     if not has_mxnet:
-        raise ImportError("MXNet support requires mxnet: pip install thinc[mxnet]")
+        raise ImportError(
+            "MXNet support requires mxnet: pip install thinc[mxnet]\n\nEnable MXNet support with thinc.api.enable_mxnet()"
+        )
 
 
 def assert_pytorch_installed() -> None:  # pragma: no cover
     """Raise an ImportError if PyTorch is not installed."""
     if not has_torch:
         raise ImportError("PyTorch support requires torch: pip install thinc[torch]")
 
@@ -418,77 +431,77 @@
             return torch_tensor.detach().cpu().numpy()
         else:
             return cupy.asarray(torch_tensor)
 
 
 def xp2tensorflow(
     xp_tensor: ArrayXd, requires_grad: bool = False, as_variable: bool = False
-) -> "tf.Tensor":  # pragma: no cover
+) -> "tf.Tensor":  # type: ignore  # pragma: no cover
     """Convert a numpy or cupy tensor to a TensorFlow Tensor or Variable"""
     assert_tensorflow_installed()
     if hasattr(xp_tensor, "toDlpack"):
         dlpack_tensor = xp_tensor.toDlpack()  # type: ignore
-        tf_tensor = tf.experimental.dlpack.from_dlpack(dlpack_tensor)
+        tf_tensor = tf.experimental.dlpack.from_dlpack(dlpack_tensor)  # type: ignore
     elif hasattr(xp_tensor, "__dlpack__"):
         dlpack_tensor = xp_tensor.__dlpack__()  # type: ignore
-        tf_tensor = tf.experimental.dlpack.from_dlpack(dlpack_tensor)
+        tf_tensor = tf.experimental.dlpack.from_dlpack(dlpack_tensor)  # type: ignore
     else:
-        tf_tensor = tf.convert_to_tensor(xp_tensor)
+        tf_tensor = tf.convert_to_tensor(xp_tensor)  # type: ignore
     if as_variable:
         # tf.Variable() automatically puts in GPU if available.
         # So we need to control it using the context manager
-        with tf.device(tf_tensor.device):
-            tf_tensor = tf.Variable(tf_tensor, trainable=requires_grad)
+        with tf.device(tf_tensor.device):  # type: ignore
+            tf_tensor = tf.Variable(tf_tensor, trainable=requires_grad)  # type: ignore
     if requires_grad is False and as_variable is False:
         # tf.stop_gradient() automatically puts in GPU if available.
         # So we need to control it using the context manager
-        with tf.device(tf_tensor.device):
-            tf_tensor = tf.stop_gradient(tf_tensor)
+        with tf.device(tf_tensor.device):  # type: ignore
+            tf_tensor = tf.stop_gradient(tf_tensor)  # type: ignore
     return tf_tensor
 
 
 def tensorflow2xp(
-    tf_tensor: "tf.Tensor", *, ops: Optional["Ops"] = None
+    tf_tensor: "tf.Tensor", *, ops: Optional["Ops"] = None  # type: ignore
 ) -> ArrayXd:  # pragma: no cover
     """Convert a Tensorflow tensor to numpy or cupy tensor depending on the `ops` parameter.
     If `ops` is `None`, the type of the resultant tensor will be determined by the source tensor's device.
     """
     from .api import NumpyOps
 
     assert_tensorflow_installed()
     if is_tensorflow_gpu_array(tf_tensor):
         if isinstance(ops, NumpyOps):
             return tf_tensor.numpy()
         else:
-            dlpack_tensor = tf.experimental.dlpack.to_dlpack(tf_tensor)
+            dlpack_tensor = tf.experimental.dlpack.to_dlpack(tf_tensor)  # type: ignore
             return cupy_from_dlpack(dlpack_tensor)
     else:
         if isinstance(ops, NumpyOps) or ops is None:
             return tf_tensor.numpy()
         else:
             return cupy.asarray(tf_tensor.numpy())
 
 
 def xp2mxnet(
     xp_tensor: ArrayXd, requires_grad: bool = False
-) -> "mx.nd.NDArray":  # pragma: no cover
+) -> "mx.nd.NDArray":  # type: ignore  # pragma: no cover
     """Convert a numpy or cupy tensor to a MXNet tensor."""
     assert_mxnet_installed()
     if hasattr(xp_tensor, "toDlpack"):
         dlpack_tensor = xp_tensor.toDlpack()  # type: ignore
-        mx_tensor = mx.nd.from_dlpack(dlpack_tensor)
+        mx_tensor = mx.nd.from_dlpack(dlpack_tensor)  # type: ignore
     else:
-        mx_tensor = mx.nd.from_numpy(xp_tensor)
+        mx_tensor = mx.nd.from_numpy(xp_tensor)  # type: ignore
     if requires_grad:
         mx_tensor.attach_grad()
     return mx_tensor
 
 
 def mxnet2xp(
-    mx_tensor: "mx.nd.NDArray", *, ops: Optional["Ops"] = None
+    mx_tensor: "mx.nd.NDArray", *, ops: Optional["Ops"] = None  # type: ignore
 ) -> ArrayXd:  # pragma: no cover
     """Convert a MXNet tensor to a numpy or cupy tensor."""
     from .api import NumpyOps
 
     assert_mxnet_installed()
     if is_mxnet_gpu_array(mx_tensor):
         if isinstance(ops, NumpyOps):
@@ -638,15 +651,14 @@
     "is_cupy_array",
     "is_numpy_array",
     "set_active_gpu",
     "prefer_gpu",
     "require_gpu",
     "copy_array",
     "to_categorical",
-    "smooth_one_hot",
     "get_width",
     "xp2torch",
     "torch2xp",
     "tensorflow2xp",
     "xp2tensorflow",
     "validate_fwd_input_output",
     "DataValidationError",
```

### Comparing `thinc-9.0.0.dev3/thinc.egg-info/PKG-INFO` & `thinc-9.0.0.dev4/thinc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev3
+Version: 9.0.0.dev4
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,115 +18,172 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: blis<0.8.0,>=0.7.8
+Requires-Dist: murmurhash<1.1.0,>=1.0.2
+Requires-Dist: cymem<2.1.0,>=2.0.2
+Requires-Dist: preshed<3.1.0,>=3.0.2
+Requires-Dist: wasabi<1.2.0,>=0.8.1
+Requires-Dist: srsly<3.0.0,>=2.4.0
+Requires-Dist: catalogue<2.1.0,>=2.0.4
+Requires-Dist: confection<1.0.0,>=0.0.1
+Requires-Dist: setuptools
+Requires-Dist: numpy>=1.15.0; python_version < "3.9"
+Requires-Dist: numpy>=1.19.0; python_version >= "3.9"
+Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
+Requires-Dist: packaging>=20.0
+Requires-Dist: dataclasses<1.0,>=0.6; python_version < "3.7"
+Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1; python_version < "3.8"
+Requires-Dist: contextvars<3,>=2.4; python_version < "3.7"
 Provides-Extra: cuda
+Requires-Dist: cupy>=5.0.0b4; extra == "cuda"
 Provides-Extra: cuda80
+Requires-Dist: cupy-cuda80>=5.0.0b4; extra == "cuda80"
 Provides-Extra: cuda90
+Requires-Dist: cupy-cuda90>=5.0.0b4; extra == "cuda90"
 Provides-Extra: cuda91
+Requires-Dist: cupy-cuda91>=5.0.0b4; extra == "cuda91"
 Provides-Extra: cuda92
+Requires-Dist: cupy-cuda92>=5.0.0b4; extra == "cuda92"
 Provides-Extra: cuda100
+Requires-Dist: cupy-cuda100>=5.0.0b4; extra == "cuda100"
 Provides-Extra: cuda101
+Requires-Dist: cupy-cuda101>=5.0.0b4; extra == "cuda101"
 Provides-Extra: cuda102
+Requires-Dist: cupy-cuda102>=5.0.0b4; extra == "cuda102"
 Provides-Extra: cuda110
+Requires-Dist: cupy-cuda110>=5.0.0b4; extra == "cuda110"
 Provides-Extra: cuda111
+Requires-Dist: cupy-cuda111>=5.0.0b4; extra == "cuda111"
 Provides-Extra: cuda112
+Requires-Dist: cupy-cuda112>=5.0.0b4; extra == "cuda112"
 Provides-Extra: cuda113
+Requires-Dist: cupy-cuda113>=5.0.0b4; extra == "cuda113"
 Provides-Extra: cuda114
+Requires-Dist: cupy-cuda114>=5.0.0b4; extra == "cuda114"
 Provides-Extra: cuda115
+Requires-Dist: cupy-cuda115>=5.0.0b4; extra == "cuda115"
 Provides-Extra: cuda116
+Requires-Dist: cupy-cuda116>=5.0.0b4; extra == "cuda116"
 Provides-Extra: cuda117
+Requires-Dist: cupy-cuda117>=5.0.0b4; extra == "cuda117"
 Provides-Extra: cuda11x
+Requires-Dist: cupy-cuda11x>=11.0.0; extra == "cuda11x"
+Provides-Extra: cuda12x
+Requires-Dist: cupy-cuda12x>=11.5.0; extra == "cuda12x"
 Provides-Extra: cuda-autodetect
+Requires-Dist: cupy-wheel>=11.0.0; extra == "cuda-autodetect"
 Provides-Extra: datasets
+Requires-Dist: ml_datasets<0.3.0,>=0.2.0; extra == "datasets"
 Provides-Extra: torch
+Requires-Dist: torch>=1.6.0; extra == "torch"
 Provides-Extra: tensorflow
+Requires-Dist: tensorflow<2.6.0,>=2.0.0; extra == "tensorflow"
 Provides-Extra: mxnet
-License-File: LICENSE
+Requires-Dist: mxnet<1.6.0,>=1.5.1; extra == "mxnet"
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Thinc: A refreshing functional take on deep learning, compatible with your favorite libraries
 
 ### From the makers of [spaCy](https://spacy.io) and [Prodigy](https://prodi.gy)
 
-[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers an elegant,
-type-checked, functional-programming API for **composing models**, with support
-for layers defined in other frameworks such as **PyTorch, TensorFlow and MXNet**. You
-can use Thinc as an interface layer, a standalone toolkit or a flexible way to
-develop new models. Previous versions of Thinc have been running quietly in
-production in thousands of companies, via both [spaCy](https://spacy.io) and
-[Prodigy](https://prodi.gy). We wrote the new version to let users **compose,
-configure and deploy custom models** built with their favorite framework.
+[Thinc](https://thinc.ai) is a **lightweight deep learning library** that offers
+an elegant, type-checked, functional-programming API for **composing models**,
+with support for layers defined in other frameworks such as **PyTorch,
+TensorFlow and MXNet**. You can use Thinc as an interface layer, a standalone
+toolkit or a flexible way to develop new models. Previous versions of Thinc have
+been running quietly in production in thousands of companies, via both
+[spaCy](https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the new
+version to let users **compose, configure and deploy custom models** built with
+their favorite framework.
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/7/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=7)
+[![tests](https://github.com/explosion/thinc/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/thinc/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)](https://github.com/explosion/thinc/releases)
 [![PyPi Version](https://img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/thinc)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 [![Open demo in Colab][colab]][intro_to_thinc_colab]
 
 ## 🔥 Features
 
-- **Type-check** your model definitions with custom types and [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
+- **Type-check** your model definitions with custom types and
+  [`mypy`](https://mypy.readthedocs.io/en/latest/) plugin.
 - Wrap **PyTorch**, **TensorFlow** and **MXNet** models for use in your network.
-- Concise **functional-programming** approach to model definition, using composition rather than inheritance.
+- Concise **functional-programming** approach to model definition, using
+  composition rather than inheritance.
 - Optional custom infix notation via **operator overloading**.
 - Integrated **config system** to describe trees of objects and hyperparameters.
 - Choice of **extensible backends**.
 - **[Read more &rarr;](https://thinc.ai/docs)**
 
 ## 🚀 Quickstart
 
-Thinc is compatible with **Python 3.6+** and runs on **Linux**,
-**macOS** and **Windows**. The latest releases with binary wheels are available from
+Thinc is compatible with **Python 3.6+** and runs on **Linux**, **macOS** and
+**Windows**. The latest releases with binary wheels are available from
 [pip](https://pypi.python.org/pypi/thinc). Before you install Thinc and its
 dependencies, make sure that your `pip`, `setuptools` and `wheel` are up to
 date. For the most recent releases, pip 19.3 or newer is recommended.
 
 ```bash
 pip install -U pip setuptools wheel
 pip install thinc
 ```
 
-See the [extended installation docs](https://thinc.ai/docs/install#extended) for details on optional dependencies for different backends and GPU. You might also want to [set up static type checking](https://thinc.ai/docs/install#type-checking) to take advantage of Thinc's type system.
+See the [extended installation docs](https://thinc.ai/docs/install#extended) for
+details on optional dependencies for different backends and GPU. You might also
+want to
+[set up static type checking](https://thinc.ai/docs/install#type-checking) to
+take advantage of Thinc's type system.
 
 > ⚠️ If you have installed PyTorch and you are using Python 3.7+, uninstall the
-> package `dataclasses` with `pip uninstall dataclasses`, since it may have
-> been installed by PyTorch and is incompatible with Python 3.7+.
+> package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+.
 
 ### 📓 Selected examples and notebooks
 
-Also see the [`/examples`](examples) directory and [usage documentation](https://thinc.ai/docs) for more examples. Most examples are Jupyter notebooks – to launch them on [Google Colab](https://colab.research.google.com) (with GPU support!) click on the button next to the notebook name.
+Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks – to launch them on
+[Google Colab](https://colab.research.google.com) (with GPU support!) click on
+the button next to the notebook name.
 
 | Notebook                                                                                                              | Description                                                                                                                                                                                       |
 | --------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | [`intro_to_thinc`][intro_to_thinc]<br />[![Open in Colab][colab]][intro_to_thinc_colab]                               | Everything you need to know to get started. Composing and training a model on the MNIST data, using config files, registering custom functions and wrapping PyTorch, TensorFlow and MXNet models. |
 | [`transformers_tagger_bert`][transformers_tagger_bert]<br />[![Open in Colab][colab]][transformers_tagger_bert_colab] | How to use Thinc, `transformers` and PyTorch to train a part-of-speech tagger. From model definition and config to the training loop.                                                             |
 | [`pos_tagger_basic_cnn`][pos_tagger_basic_cnn]<br />[![Open in Colab][colab]][pos_tagger_basic_cnn_colab]             | Implementing and training a basic CNN for part-of-speech tagging model without external dependencies and using different levels of Thinc's config system.                                         |
 | [`parallel_training_ray`][parallel_training_ray]<br />[![Open in Colab][colab]][parallel_training_ray_colab]          | How to set up synchronous and asynchronous parameter server training with Thinc and [Ray](https://ray.readthedocs.io/en/latest/).                                                                 |
 
 **[View more &rarr;](examples)**
 
-[colab]: https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
+[colab]:
+  https://gistcdn.githack.com/ines/dcf354aa71a7665ae19871d7fd14a4e0/raw/461fc1f61a7bc5860f943cd4b6bcfabb8c8906e7/colab-badge.svg
 [intro_to_thinc]: examples/00_intro_to_thinc.ipynb
-[intro_to_thinc_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
+[intro_to_thinc_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/00_intro_to_thinc.ipynb
 [transformers_tagger_bert]: examples/02_transformers_tagger_bert.ipynb
-[transformers_tagger_bert_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
+[transformers_tagger_bert_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/02_transformers_tagger_bert.ipynb
 [pos_tagger_basic_cnn]: examples/03_pos_tagger_basic_cnn.ipynb
-[pos_tagger_basic_cnn_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
+[pos_tagger_basic_cnn_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/03_pos_tagger_basic_cnn.ipynb
 [parallel_training_ray]: examples/04_parallel_training_ray.ipynb
-[parallel_training_ray_colab]: https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
+[parallel_training_ray_colab]:
+  https://colab.research.google.com/github/explosion/thinc/blob/master/examples/04_parallel_training_ray.ipynb
 
 ### 📖 Documentation & usage guides
 
 | Documentation                                                                     | Description                                           |
 | --------------------------------------------------------------------------------- | ----------------------------------------------------- |
 | [Introduction](https://thinc.ai/docs)                                             | Everything you need to know.                          |
 | [Concept & Design](https://thinc.ai/docs/concept)                                 | Thinc's conceptual model and how it works.            |
@@ -150,15 +207,20 @@
 | [`thinc.schedules`](thinc/schedules.py)   | Generators for different rates, schedules, decays or series.                      |
 | [`thinc.backends`](thinc/backends)        | Backends for `numpy` and `cupy`.                                                  |
 | [`thinc.config`](thinc/config.py)         | Config parsing and validation and function registry system.                       |
 | [`thinc.util`](thinc/util.py)             | Utilities and helper functions.                                                   |
 
 ## 🐍 Development notes
 
-Thinc uses [`black`](https://github.com/psf/black) for auto-formatting, [`flake8`](http://flake8.pycqa.org/en/latest/) for linting and [`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is written compatible with **Python 3.6+**, with type hints wherever possible. See the [type reference](https://thinc.ai/docs/api-types) for more details on Thinc's custom types.
+Thinc uses [`black`](https://github.com/psf/black) for auto-formatting,
+[`flake8`](http://flake8.pycqa.org/en/latest/) for linting and
+[`mypy`](https://mypy.readthedocs.io/en/latest/) for type checking. All code is
+written compatible with **Python 3.6+**, with type hints wherever possible. See
+the [type reference](https://thinc.ai/docs/api-types) for more details on
+Thinc's custom types.
 
 ### 👷‍♀️ Building Thinc from source
 
 Building Thinc from source requires the full dependencies listed in
 [`requirements.txt`](requirements.txt) to be installed. You'll also need a
 compiler to build the C extensions.
 
@@ -185,16 +247,20 @@
 export PYTHONPATH=`pwd`
 pip install -r requirements.txt
 python setup.py build_ext --inplace
 ```
 
 ### 🚦 Running tests
 
-Thinc comes with an [extensive test suite](thinc/tests). The following should all pass and not report any warnings or errors:
+Thinc comes with an [extensive test suite](thinc/tests). The following should
+all pass and not report any warnings or errors:
 
 ```bash
 python -m pytest thinc    # test suite
 python -m mypy thinc      # type checks
 python -m flake8 thinc    # linting
 ```
 
-To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim for a 100% test coverage. This doesn't mean that we meticulously write tests for every single line – we ignore blocks that are not relevant or difficult to test and make sure that the tests execute all code paths.
+To view test coverage, you can run `python -m pytest thinc --cov=thinc`. We aim
+for a 100% test coverage. This doesn't mean that we meticulously write tests for
+every single line – we ignore blocks that are not relevant or difficult to test
+and make sure that the tests execute all code paths.
```

#### html2text {}

```diff
@@ -1,45 +1,72 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev3 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev4 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Programming Language ::
 Cython Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering Requires-Python: >=3.6 Description-Content-Type: text/
-markdown Provides-Extra: cuda Provides-Extra: cuda80 Provides-Extra: cuda90
-Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-Extra: cuda100 Provides-
-Extra: cuda101 Provides-Extra: cuda102 Provides-Extra: cuda110 Provides-Extra:
-cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113 Provides-Extra: cuda114
-Provides-Extra: cuda115 Provides-Extra: cuda116 Provides-Extra: cuda117
-Provides-Extra: cuda11x Provides-Extra: cuda-autodetect Provides-Extra:
-datasets Provides-Extra: torch Provides-Extra: tensorflow Provides-Extra: mxnet
-License-File: LICENSE _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# Thinc: A
-refreshing functional take on deep learning, compatible with your favorite
-libraries ### From the makers of [spaCy](https://spacy.io) and [Prodigy](https:
-//prodi.gy) [Thinc](https://thinc.ai) is a **lightweight deep learning
-library** that offers an elegant, type-checked, functional-programming API for
-**composing models**, with support for layers defined in other frameworks such
-as **PyTorch, TensorFlow and MXNet**. You can use Thinc as an interface layer,
-a standalone toolkit or a flexible way to develop new models. Previous versions
-of Thinc have been running quietly in production in thousands of companies, via
-both [spaCy](https://spacy.io) and [Prodigy](https://prodi.gy). We wrote the
-new version to let users **compose, configure and deploy custom models** built
-with their favorite framework. [![Azure Pipelines](https://img.shields.io/
-azure-devops/build/explosion-ai/public/7/master.svg?logo=azure-
-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/
-_build?definitionId=7) [![Current Release Version](https://img.shields.io/
-github/v/release/explosion/
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: blis<0.8.0,>=0.7.8 Requires-Dist:
+murmurhash<1.1.0,>=1.0.2 Requires-Dist: cymem<2.1.0,>=2.0.2 Requires-Dist:
+preshed<3.1.0,>=3.0.2 Requires-Dist: wasabi<1.2.0,>=0.8.1 Requires-Dist:
+srsly<3.0.0,>=2.4.0 Requires-Dist: catalogue<2.1.0,>=2.0.4 Requires-Dist:
+confection<1.0.0,>=0.0.1 Requires-Dist: setuptools Requires-Dist:
+numpy>=1.15.0; python_version < "3.9" Requires-Dist: numpy>=1.19.0;
+python_version >= "3.9" Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
+Requires-Dist: packaging>=20.0 Requires-Dist: dataclasses<1.0,>=0.6;
+python_version < "3.7" Requires-Dist: typing_extensions<4.5.0,>=3.7.4.1;
+python_version < "3.8" Requires-Dist: contextvars<3,>=2.4; python_version <
+"3.7" Provides-Extra: cuda Requires-Dist: cupy>=5.0.0b4; extra == "cuda"
+Provides-Extra: cuda80 Requires-Dist: cupy-cuda80>=5.0.0b4; extra == "cuda80"
+Provides-Extra: cuda90 Requires-Dist: cupy-cuda90>=5.0.0b4; extra == "cuda90"
+Provides-Extra: cuda91 Requires-Dist: cupy-cuda91>=5.0.0b4; extra == "cuda91"
+Provides-Extra: cuda92 Requires-Dist: cupy-cuda92>=5.0.0b4; extra == "cuda92"
+Provides-Extra: cuda100 Requires-Dist: cupy-cuda100>=5.0.0b4; extra ==
+"cuda100" Provides-Extra: cuda101 Requires-Dist: cupy-cuda101>=5.0.0b4; extra
+== "cuda101" Provides-Extra: cuda102 Requires-Dist: cupy-cuda102>=5.0.0b4;
+extra == "cuda102" Provides-Extra: cuda110 Requires-Dist: cupy-
+cuda110>=5.0.0b4; extra == "cuda110" Provides-Extra: cuda111 Requires-Dist:
+cupy-cuda111>=5.0.0b4; extra == "cuda111" Provides-Extra: cuda112 Requires-
+Dist: cupy-cuda112>=5.0.0b4; extra == "cuda112" Provides-Extra: cuda113
+Requires-Dist: cupy-cuda113>=5.0.0b4; extra == "cuda113" Provides-Extra:
+cuda114 Requires-Dist: cupy-cuda114>=5.0.0b4; extra == "cuda114" Provides-
+Extra: cuda115 Requires-Dist: cupy-cuda115>=5.0.0b4; extra == "cuda115"
+Provides-Extra: cuda116 Requires-Dist: cupy-cuda116>=5.0.0b4; extra ==
+"cuda116" Provides-Extra: cuda117 Requires-Dist: cupy-cuda117>=5.0.0b4; extra
+== "cuda117" Provides-Extra: cuda11x Requires-Dist: cupy-cuda11x>=11.0.0; extra
+== "cuda11x" Provides-Extra: cuda12x Requires-Dist: cupy-cuda12x>=11.5.0; extra
+== "cuda12x" Provides-Extra: cuda-autodetect Requires-Dist: cupy-wheel>=11.0.0;
+extra == "cuda-autodetect" Provides-Extra: datasets Requires-Dist:
+ml_datasets<0.3.0,>=0.2.0; extra == "datasets" Provides-Extra: torch Requires-
+Dist: torch>=1.6.0; extra == "torch" Provides-Extra: tensorflow Requires-Dist:
+tensorflow<2.6.0,>=2.0.0; extra == "tensorflow" Provides-Extra: mxnet Requires-
+Dist: mxnet<1.6.0,>=1.5.1; extra == "mxnet" _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
+_l_o_g_o_._s_v_g_]# Thinc: A refreshing functional take on deep learning, compatible
+with your favorite libraries ### From the makers of [spaCy](https://spacy.io)
+and [Prodigy](https://prodi.gy) [Thinc](https://thinc.ai) is a **lightweight
+deep learning library** that offers an elegant, type-checked, functional-
+programming API for **composing models**, with support for layers defined in
+other frameworks such as **PyTorch, TensorFlow and MXNet**. You can use Thinc
+as an interface layer, a standalone toolkit or a flexible way to develop new
+models. Previous versions of Thinc have been running quietly in production in
+thousands of companies, via both [spaCy](https://spacy.io) and [Prodigy](https:
+//prodi.gy). We wrote the new version to let users **compose, configure and
+deploy custom models** built with their favorite framework. [![tests](https://
+github.com/explosion/thinc/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/thinc/actions/workflows/tests.yml) [![Current Release
+Version](https://img.shields.io/github/v/release/explosion/
 thinc.svg?include_prereleases&sort=semver&style=flat-square&logo=github)]
 (https://github.com/explosion/thinc/releases) [![PyPi Version](https://
 img.shields.io/pypi/v/thinc.svg?include_prereleases&sort=semver&style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/thinc) [![conda
 Version](https://img.shields.io/conda/vn/conda-forge/thinc.svg?style=flat-
 square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
 thinc) [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
@@ -61,19 +88,19 @@
 `setuptools` and `wheel` are up to date. For the most recent releases, pip 19.3
 or newer is recommended. ```bash pip install -U pip setuptools wheel pip
 install thinc ``` See the [extended installation docs](https://thinc.ai/docs/
 install#extended) for details on optional dependencies for different backends
 and GPU. You might also want to [set up static type checking](https://thinc.ai/
 docs/install#type-checking) to take advantage of Thinc's type system. > â ï¸
 If you have installed PyTorch and you are using Python 3.7+, uninstall the >
-package `dataclasses` with `pip uninstall dataclasses`, since it may have >
-been installed by PyTorch and is incompatible with Python 3.7+. ### ð
-Selected examples and notebooks Also see the [`/examples`](examples) directory
-and [usage documentation](https://thinc.ai/docs) for more examples. Most
-examples are Jupyter notebooks â to launch them on [Google Colab](https://
+package `dataclasses` with `pip uninstall dataclasses`, since it may have been
+> installed by PyTorch and is incompatible with Python 3.7+. ### ð Selected
+examples and notebooks Also see the [`/examples`](examples) directory and
+[usage documentation](https://thinc.ai/docs) for more examples. Most examples
+are Jupyter notebooks â to launch them on [Google Colab](https://
 colab.research.google.com) (with GPU support!) click on the button next to the
 notebook name. | Notebook | Description | | -----------------------------------
 -------------------------------------------------------------------------------
 --- | -------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------- | | [`intro_to_thinc`]
 [intro_to_thinc]
```

### Comparing `thinc-9.0.0.dev3/thinc.egg-info/SOURCES.txt` & `thinc-9.0.0.dev4/thinc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 thinc/layers/maxout.py
 thinc/layers/mish.py
 thinc/layers/multisoftmax.py
 thinc/layers/mxnetwrapper.py
 thinc/layers/noop.py
 thinc/layers/padded2list.py
 thinc/layers/parametricattention.py
+thinc/layers/parametricattention_v2.py
 thinc/layers/premap_ids.pyx
 thinc/layers/pytorchwrapper.py
 thinc/layers/ragged2list.py
 thinc/layers/reduce_first.py
 thinc/layers/reduce_last.py
 thinc/layers/reduce_max.py
 thinc/layers/reduce_mean.py
@@ -106,25 +107,25 @@
 thinc/layers/with_getitem.py
 thinc/layers/with_list.py
 thinc/layers/with_nvtx_range.py
 thinc/layers/with_padded.py
 thinc/layers/with_ragged.py
 thinc/layers/with_reshape.py
 thinc/layers/with_signpost_interval.py
-thinc/legacy/__init__.py
-thinc/legacy/loss.py
 thinc/shims/__init__.py
 thinc/shims/mxnet.py
 thinc/shims/pytorch.py
 thinc/shims/pytorch_grad_scaler.py
 thinc/shims/shim.py
 thinc/shims/tensorflow.py
 thinc/shims/torchscript.py
 thinc/tests/__init__.py
 thinc/tests/conftest.py
+thinc/tests/enable_mxnet.py
+thinc/tests/enable_tensorflow.py
 thinc/tests/strategies.py
 thinc/tests/test_config.py
 thinc/tests/test_examples.py
 thinc/tests/test_import__all__.py
 thinc/tests/test_indexing.py
 thinc/tests/test_initializers.py
 thinc/tests/test_loss.py
@@ -144,14 +145,15 @@
 thinc/tests/layers/test_hash_embed.py
 thinc/tests/layers/test_layers_api.py
 thinc/tests/layers/test_linear.py
 thinc/tests/layers/test_lstm.py
 thinc/tests/layers/test_mappers.py
 thinc/tests/layers/test_mnist.py
 thinc/tests/layers/test_mxnet_wrapper.py
+thinc/tests/layers/test_parametric_attention_v2.py
 thinc/tests/layers/test_pytorch_wrapper.py
 thinc/tests/layers/test_reduce.py
 thinc/tests/layers/test_resizable.py
 thinc/tests/layers/test_shim.py
 thinc/tests/layers/test_softmax.py
 thinc/tests/layers/test_sparse_linear.py
 thinc/tests/layers/test_tensorflow_wrapper.py
```

### Comparing `thinc-9.0.0.dev3/thinc.egg-info/requires.txt` & `thinc-9.0.0.dev4/thinc.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 cymem<2.1.0,>=2.0.2
 preshed<3.1.0,>=3.0.2
 wasabi<1.2.0,>=0.8.1
 srsly<3.0.0,>=2.4.0
 catalogue<2.1.0,>=2.0.4
 confection<1.0.0,>=0.0.1
 setuptools
-numpy>=1.15.0
-pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4
+pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
 packaging>=20.0
 
 [:python_version < "3.7"]
 dataclasses<1.0,>=0.6
 contextvars<3,>=2.4
 
 [:python_version < "3.8"]
 typing_extensions<4.5.0,>=3.7.4.1
 
+[:python_version < "3.9"]
+numpy>=1.15.0
+
+[:python_version >= "3.9"]
+numpy>=1.19.0
+
 [cuda]
 cupy>=5.0.0b4
 
 [cuda-autodetect]
 cupy-wheel>=11.0.0
 
 [cuda100]
@@ -56,14 +61,17 @@
 
 [cuda117]
 cupy-cuda117>=5.0.0b4
 
 [cuda11x]
 cupy-cuda11x>=11.0.0
 
+[cuda12x]
+cupy-cuda12x>=11.5.0
+
 [cuda80]
 cupy-cuda80>=5.0.0b4
 
 [cuda90]
 cupy-cuda90>=5.0.0b4
 
 [cuda91]
```

