# Comparing `tmp/nvidia_dali_nightly_cuda110-1.37.0.dev20240322.tar.gz` & `tmp/nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda110-1.37.0.dev20240322.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda110-1.37.0.dev20240322.tar` & `nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.37.0.dev20240322
-Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: 86d973fe68efd2776a103b61eb3d782a07c9c3f0
+Version: 1.37.0.dev20240405
+Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: d28d6cbfc665781c5f3ab4ba28602374c48da31b
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
