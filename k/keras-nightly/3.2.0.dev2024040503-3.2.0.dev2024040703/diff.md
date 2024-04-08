# Comparing `tmp/keras-nightly-3.2.0.dev2024040503.tar.gz` & `tmp/keras-nightly-3.2.0.dev2024040703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nightly-3.2.0.dev2024040503.tar", last modified: Fri Apr  5 03:20:23 2024, max compression
+gzip compressed data, was "keras-nightly-3.2.0.dev2024040703.tar", last modified: Sun Apr  7 03:20:30 2024, max compression
```

## Comparing `keras-nightly-3.2.0.dev2024040503.tar` & `keras-nightly-3.2.0.dev2024040703.tar`

### file list

```diff
@@ -1,691 +1,691 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.584281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.588281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.592281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.596281 keras-nightly-3.2.0.dev2024040503/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.600281 keras-nightly-3.2.0.dev2024040503/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.604281 keras-nightly-3.2.0.dev2024040503/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.608281 keras-nightly-3.2.0.dev2024040503/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.608281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.608281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.612281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.612281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.616281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    35373 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.616281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.620281 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31619 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.624281 keras-nightly-3.2.0.dev2024040503/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.628281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.628281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.628281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.632281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.632281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    62696 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.632281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.636281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.636281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.640281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.644281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.644281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.648281 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.648281 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.648281 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.648281 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.648281 keras-nightly-3.2.0.dev2024040503/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.652281 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.652281 keras-nightly-3.2.0.dev2024040503/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32036 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.656281 keras-nightly-3.2.0.dev2024040503/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   189853 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.656281 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    36189 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.656281 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27055 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26085 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.660281 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.664281 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45199 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26523 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 03:20:17.000000 keras-nightly-3.2.0.dev2024040503/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-05 03:20:23.000000 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-05 03:20:23.000000 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:20:23.000000 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 03:20:23.000000 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 03:20:23.000000 keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:20:23.668281 keras-nightly-3.2.0.dev2024040503/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-05 03:20:21.000000 keras-nightly-3.2.0.dev2024040503/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.789181 keras-nightly-3.2.0.dev2024040703/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-07 03:20:30.789181 keras-nightly-3.2.0.dev2024040703/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.701181 keras-nightly-3.2.0.dev2024040703/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.705181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.709181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.713181 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.717181 keras-nightly-3.2.0.dev2024040703/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.721181 keras-nightly-3.2.0.dev2024040703/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.725181 keras-nightly-3.2.0.dev2024040703/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.725181 keras-nightly-3.2.0.dev2024040703/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.725181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.729181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.729181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36056 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.733181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.737181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35373 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.737181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.737181 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.741181 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.741181 keras-nightly-3.2.0.dev2024040703/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31619 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.745181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.749181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.749181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.753181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62696 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.753181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.753181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.757181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.761181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.761181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.765181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.765181 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.765181 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.769181 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.769181 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.769181 keras-nightly-3.2.0.dev2024040703/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.769181 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.773181 keras-nightly-3.2.0.dev2024040703/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32036 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.773181 keras-nightly-3.2.0.dev2024040703/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189853 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36189 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.777181 keras-nightly-3.2.0.dev2024040703/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.781181 keras-nightly-3.2.0.dev2024040703/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26646 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.781181 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.781181 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45199 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.785181 keras-nightly-3.2.0.dev2024040703/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26523 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-07 03:20:24.000000 keras-nightly-3.2.0.dev2024040703/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.785181 keras-nightly-3.2.0.dev2024040703/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.785181 keras-nightly-3.2.0.dev2024040703/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.785181 keras-nightly-3.2.0.dev2024040703/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:20:30.789181 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-07 03:20:30.000000 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-07 03:20:30.000000 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:20:30.000000 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 03:20:30.000000 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 03:20:30.000000 keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:20:30.789181 keras-nightly-3.2.0.dev2024040703/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-07 03:20:28.000000 keras-nightly-3.2.0.dev2024040703/setup.py
```

### Comparing `keras-nightly-3.2.0.dev2024040503/PKG-INFO` & `keras-nightly-3.2.0.dev2024040703/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024040503
+Version: 3.2.0.dev2024040703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024040503/README.md` & `keras-nightly-3.2.0.dev2024040703/README.md`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.2.0.dev2024040503"
+__version__ = "3.2.0.dev2024040703"
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/config/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/distribution/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/random/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/tree/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/_tf_keras/keras/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/applications/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/config/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/distribution/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/ops/nn/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/random/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/activations/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/activations/activations.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/api_export.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/convnext.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/densenet.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/efficientnet.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/efficientnet_v2.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/imagenet_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/inception_resnet_v2.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/inception_v3.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet_v2.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/mobilenet_v3.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/nasnet.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/resnet.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/resnet_v2.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/vgg16.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/vgg19.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/applications/xception.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/backend_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/dtypes.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/global_state.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/keras_tensor.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/name_scope.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/stateless_scope.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/common/variables.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/config.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/exports.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/core.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/linalg.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/math.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/nn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/numpy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/random.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/sparse.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/jax/trainer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/core.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/linalg.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/math.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/nn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/numpy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/random.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/numpy/trainer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/core.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,15 @@
     elif dtype is not None and not x.dtype == dtype:
         if isinstance(x, tf.SparseTensor):
             x_shape = x.shape
             x = tf.cast(x, dtype)
             x.set_shape(x_shape)
             return x
         return tf.cast(x, dtype=dtype)
-    else:
-        return x
+    return x
 
 
 def convert_to_numpy(x):
     if isinstance(x, tf.SparseTensor):
         x_shape = x.shape
         x = tf.sparse.to_dense(x)
         x.set_shape(x_shape)
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/linalg.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/math.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/nn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/numpy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/random.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/sparse.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/trackable.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/tensorflow/trainer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/core.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/linalg.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/math.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/nn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/numpy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/random.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/backend/torch/trainer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/backup_and_restore.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/callback.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/callback_list.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/csv_logger.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/early_stopping.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/history.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/lambda_callback.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/learning_rate_scheduler.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/model_checkpoint.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/progbar_logger.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/remote_monitor.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/swap_ema_weights.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/tensorboard.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/callbacks/terminate_on_nan.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/constraints/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/constraints/constraints.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/boston_housing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/california_housing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar10.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/cifar100.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/fashion_mnist.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/imdb.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/mnist.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/datasets/reuters.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/distribution/distribution_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/dtype_policies/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/dtype_policies/dtype_policy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/export/export_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/initializers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/initializers/constant_initializers.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/initializers/initializer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/initializers/random_initializers.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/activation.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/elu.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/leaky_relu.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/prelu.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/relu.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/activations/softmax.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/additive_attention.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/attention.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/grouped_query_attention.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/attention/multi_head_attention.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_conv.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/base_separable_conv.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/separable_conv1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/convolutional/separable_conv2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/dense.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/einsum_dense.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/embedding.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
 from keras.src import regularizers
@@ -16,15 +18,15 @@
     e.g. `[[4], [20]] -> [[0.25, 0.1], [0.6, -0.2]]`
 
     This layer can only be used on positive integer inputs of a fixed range.
 
     Example:
 
     >>> model = keras.Sequential()
-    >>> model.add(keras.layers.Embedding(1000, 64, input_length=10))
+    >>> model.add(keras.layers.Embedding(1000, 64))
     >>> # The model will take as input an integer matrix of size (batch,
     >>> # input_length), and the largest integer (i.e. word index) in the input
     >>> # should be no larger than 999 (vocabulary size).
     >>> # Now model.output_shape is (None, 10, 64), where `None` is the batch
     >>> # dimension.
     >>> input_array = np.random.randint(1000, size=(32, 10))
     >>> model.compile('rmsprop', 'mse')
@@ -75,14 +77,19 @@
         embeddings_initializer="uniform",
         embeddings_regularizer=None,
         embeddings_constraint=None,
         mask_zero=False,
         lora_rank=None,
         **kwargs,
     ):
+        input_length = kwargs.pop("input_length", None)
+        if input_length is not None:
+            warnings.warn(
+                "Argument `input_length` is deprecated. Just remove it."
+            )
         super().__init__(**kwargs)
         self.input_dim = input_dim
         self.output_dim = output_dim
         self.embeddings_initializer = initializers.get(embeddings_initializer)
         self.embeddings_regularizer = regularizers.get(embeddings_regularizer)
         self.embeddings_constraint = constraints.get(embeddings_constraint)
         self.mask_zero = mask_zero
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/identity.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/input_layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/lambda_layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/masking.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/core/wrapper.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/input_spec.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/add.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/average.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/base_merge.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/concatenate.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/dot.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/maximum.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/minimum.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/multiply.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/merging/subtract.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/batch_normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/group_normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/layer_normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/spectral_normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/normalization/unit_normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/average_pooling3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/base_global_pooling.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/base_pooling.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/pooling/max_pooling3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/category_encoding.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/center_crop.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/discretization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/feature_space.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/hashing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/index_lookup.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/integer_lookup.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/normalization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_brightness.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_contrast.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_crop.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_flip.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_rotation.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_translation.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/random_zoom.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/rescaling.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/resizing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/string_lookup.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/text_vectorization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/activity_regularization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/alpha_dropout.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/dropout.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/gaussian_dropout.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/gaussian_noise.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/regularization/spatial_dropout.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/cropping3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/flatten.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/permute.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/repeat_vector.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/reshape.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/up_sampling3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/reshaping/zero_padding3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/bidirectional.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm1d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm2d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/conv_lstm3d.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/gru.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/lstm.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/simple_rnn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/layers/rnn/time_distributed.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/backend.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/layers.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/losses.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/sequence.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/preprocessing/text.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/json_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/legacy_h5_format.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/saving_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/legacy/saving/serialization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/losses/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/losses/loss.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/losses/losses.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/accuracy_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/confusion_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/f_score_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/hinge_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/iou_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/metric.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         def result(self):
             return self.true_positives
     ```
     """
 
     def __init__(self, dtype=None, name=None):
         self.name = name or auto_name(self.__class__.__name__)
-        self._dtype = dtype
+        self._dtype = dtype or backend.floatx()
         self._metrics = []
         self._variables = []
         self._tracker = Tracker(
             {
                 "variables": (
                     lambda x: isinstance(x, backend.Variable),
                     self._variables,
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/metrics_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/probabilistic_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/reduction_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/reduction_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from keras.src import backend
 from keras.src import initializers
 from keras.src import losses
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.metrics.metric import Metric
 from keras.src.saving import serialization_lib
 
 
 def reduce_to_samplewise_values(values, sample_weight, reduce_fn, dtype):
+    dtype = dtype or backend.floatx()
     mask = getattr(values, "_keras_mask", None)
     values = ops.cast(values, dtype=dtype)
     if sample_weight is not None:
-        sample_weight = ops.cast(sample_weight, dtype=dtype)
+        sample_weight = ops.convert_to_tensor(sample_weight, dtype=dtype)
+
         if mask is not None:
             sample_weight = losses.loss.apply_mask(
                 sample_weight, mask, dtype=dtype, reduction="sum"
             )
         # Update dimensions of weights to match with values if possible.
         values, sample_weight = losses.loss.squeeze_or_expand_to_same_rank(
             values, sample_weight
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/metrics/regression_metrics.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/models/cloning.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/models/functional.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/models/model.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/models/sequential.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/models/variable_mapping.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/core.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/function.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/image.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/linalg.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/math.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/nn.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/node.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/numpy.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/operation.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/operation_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/ops/symbolic_arguments.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adadelta.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adafactor.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adagrad.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adam.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adamax.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/adamw.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/base_optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/ftrl.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/lion.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/loss_scale_optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/nadam.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/optimizer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/rmsprop.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/schedules/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/optimizers/sgd.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/quantizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/quantizers/quantizers.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/random/random.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/random/seed_generator.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/regularizers/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/regularizers/regularizers.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/saving/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/saving/object_registration.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/saving/saving_api.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/saving/saving_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/saving/saving_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
     elif filepath.endswith(".keras"):
         archive = zipfile.ZipFile(filepath, "r")
         weights_store = H5IOStore(
             _VARS_FNAME + ".h5", archive=archive, mode="r"
         )
 
     failed_trackables = set()
-    print("objects_to_skip", objects_to_skip)
     if objects_to_skip is not None:
         visited_trackables = set(id(o) for o in objects_to_skip)
     else:
         visited_trackables = set()
     error_msgs = {}
     _load_state(
         model,
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/saving/serialization_lib.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/testing/test_case.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/testing/test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 import tempfile
 import unittest
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import distribution
 from keras.src import ops
 from keras.src import utils
 from keras.src.backend.common import is_float_dtype
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.models import Model
@@ -544,14 +545,30 @@
                     dtype = standardize_dtype(tensor.dtype)
                     self.assertEqual(dtype, spec.dtype)
                 for weight in layer.weights:
                     dtype = standardize_dtype(weight.dtype)
                     if is_float_dtype(dtype):
                         self.assertEqual(dtype, "float32")
 
+    def _uses_gpu(self):
+        # Condition used to skip tests when using the GPU
+        devices = distribution.list_devices()
+        if any(d.startswith("gpu") for d in devices):
+            return True
+        return False
+
+    def _tensorflow_uses_gpu(self):
+        return backend.backend() == "tensorflow" and self._uses_gpu()
+
+    def _jax_uses_gpu(self):
+        return backend.backend() == "jax" and self._uses_gpu()
+
+    def _torch_uses_gpu(self):
+        return backend.backend() == "torch" and self._uses_gpu()
+
 
 def create_keras_tensors(input_shape, dtype, sparse):
     if isinstance(input_shape, dict):
         return {
             utils.removesuffix(k, "_shape"): KerasTensor(
                 v, dtype=dtype[k], sparse=sparse
             )
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/testing/test_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/compile_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/array_slicing.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/data_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/epoch_iterator.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/trainers/trainer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/argument_validation.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/audio_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/backend_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/code_stats.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/dataset_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/dtype_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/file_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/image_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/image_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/io_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/jax_layer.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/model_visualization.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/module_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/naming.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/numerical_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/progbar.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/python_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/rng_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/sequence_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/summary_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/text_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/tf_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/timeseries_dataset_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/torch_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/traceback_utils.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/tracking.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/src/utils/tree.py` & `keras-nightly-3.2.0.dev2024040703/keras/src/utils/tree.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/tree/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras/utils/__init__.py` & `keras-nightly-3.2.0.dev2024040703/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/PKG-INFO` & `keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024040503
+Version: 3.2.0.dev2024040703
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024040503/keras_nightly.egg-info/SOURCES.txt` & `keras-nightly-3.2.0.dev2024040703/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024040503/setup.py` & `keras-nightly-3.2.0.dev2024040703/setup.py`

 * *Files identical despite different names*
