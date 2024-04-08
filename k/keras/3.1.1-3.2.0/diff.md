# Comparing `tmp/keras-3.1.1.tar.gz` & `tmp/keras-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-3.1.1.tar", last modified: Tue Mar 19 18:22:24 2024, max compression
+gzip compressed data, was "keras-3.2.0.tar", last modified: Mon Apr  8 21:21:53 2024, max compression
```

## Comparing `keras-3.1.1.tar` & `keras-3.2.0.tar`

### file list

```diff
@@ -1,691 +1,691 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.453714 keras-3.1.1/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-03-19 18:22:24.453361 keras-3.1.1/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4673 2024-03-19 18:22:09.000000 keras-3.1.1/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.355722 keras-3.1.1/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2095 2024-03-19 18:22:21.000000 keras-3.1.1/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.356592 keras-3.1.1/keras/_tf_keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.356742 keras-3.1.1/keras/_tf_keras/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2248 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.356889 keras-3.1.1/keras/_tf_keras/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357035 keras-3.1.1/keras/_tf_keras/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357184 keras-3.1.1/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357326 keras-3.1.1/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357468 keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357616 keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357773 keras-3.1.1/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.357932 keras-3.1.1/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358082 keras-3.1.1/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358223 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358371 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358520 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358662 keras-3.1.1/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358810 keras-3.1.1/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.358953 keras-3.1.1/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359103 keras-3.1.1/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359253 keras-3.1.1/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359400 keras-3.1.1/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359542 keras-3.1.1/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359684 keras-3.1.1/keras/_tf_keras/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6809 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359828 keras-3.1.1/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.359979 keras-3.1.1/keras/_tf_keras/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.360120 keras-3.1.1/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.360270 keras-3.1.1/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.360416 keras-3.1.1/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.360565 keras-3.1.1/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.360857 keras-3.1.1/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.361104 keras-3.1.1/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.361292 keras-3.1.1/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.361477 keras-3.1.1/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.361822 keras-3.1.1/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362026 keras-3.1.1/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362203 keras-3.1.1/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362367 keras-3.1.1/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362524 keras-3.1.1/keras/_tf_keras/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362687 keras-3.1.1/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.362841 keras-3.1.1/keras/_tf_keras/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9984 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.363082 keras-3.1.1/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.363233 keras-3.1.1/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.363393 keras-3.1.1/keras/_tf_keras/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3183 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.363668 keras-3.1.1/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5156 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.363880 keras-3.1.1/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.364081 keras-3.1.1/keras/_tf_keras/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.364445 keras-3.1.1/keras/_tf_keras/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8626 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.364794 keras-3.1.1/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365023 keras-3.1.1/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365213 keras-3.1.1/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365407 keras-3.1.1/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5565 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365604 keras-3.1.1/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365792 keras-3.1.1/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.365990 keras-3.1.1/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.366435 keras-3.1.1/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      757 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.366629 keras-3.1.1/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1365 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.366798 keras-3.1.1/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      510 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.366953 keras-3.1.1/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367106 keras-3.1.1/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367253 keras-3.1.1/keras/_tf_keras/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367397 keras-3.1.1/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367570 keras-3.1.1/keras/_tf_keras/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367721 keras-3.1.1/keras/_tf_keras/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.367864 keras-3.1.1/keras/_tf_keras/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368009 keras-3.1.1/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-03-19 18:22:21.000000 keras-3.1.1/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368154 keras-3.1.1/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-03-19 18:22:21.000000 keras-3.1.1/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368295 keras-3.1.1/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368439 keras-3.1.1/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368577 keras-3.1.1/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368717 keras-3.1.1/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.368859 keras-3.1.1/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369002 keras-3.1.1/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369145 keras-3.1.1/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369288 keras-3.1.1/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369598 keras-3.1.1/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369739 keras-3.1.1/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.369876 keras-3.1.1/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370014 keras-3.1.1/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370149 keras-3.1.1/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370303 keras-3.1.1/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370447 keras-3.1.1/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370585 keras-3.1.1/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370729 keras-3.1.1/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.370870 keras-3.1.1/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-03-19 18:22:21.000000 keras-3.1.1/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371012 keras-3.1.1/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      884 2024-03-19 18:22:21.000000 keras-3.1.1/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371150 keras-3.1.1/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-03-19 18:22:21.000000 keras-3.1.1/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371291 keras-3.1.1/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-03-19 18:22:21.000000 keras-3.1.1/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371432 keras-3.1.1/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-03-19 18:22:21.000000 keras-3.1.1/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371572 keras-3.1.1/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371714 keras-3.1.1/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.371865 keras-3.1.1/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372011 keras-3.1.1/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372159 keras-3.1.1/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372307 keras-3.1.1/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372443 keras-3.1.1/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372585 keras-3.1.1/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372727 keras-3.1.1/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-03-19 18:22:21.000000 keras-3.1.1/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.372865 keras-3.1.1/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-03-19 18:22:21.000000 keras-3.1.1/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373009 keras-3.1.1/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-03-19 18:22:21.000000 keras-3.1.1/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373152 keras-3.1.1/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-03-19 18:22:21.000000 keras-3.1.1/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373292 keras-3.1.1/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-03-19 18:22:21.000000 keras-3.1.1/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373430 keras-3.1.1/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9662 2024-03-19 18:22:21.000000 keras-3.1.1/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373657 keras-3.1.1/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-03-19 18:22:21.000000 keras-3.1.1/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373796 keras-3.1.1/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-03-19 18:22:21.000000 keras-3.1.1/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.373931 keras-3.1.1/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-03-19 18:22:21.000000 keras-3.1.1/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.374071 keras-3.1.1/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4231 2024-03-19 18:22:21.000000 keras-3.1.1/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.374350 keras-3.1.1/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-03-19 18:22:21.000000 keras-3.1.1/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.374532 keras-3.1.1/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-03-19 18:22:21.000000 keras-3.1.1/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.374679 keras-3.1.1/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8626 2024-03-19 18:22:21.000000 keras-3.1.1/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.374914 keras-3.1.1/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-03-19 18:22:21.000000 keras-3.1.1/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.375063 keras-3.1.1/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-03-19 18:22:21.000000 keras-3.1.1/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.375206 keras-3.1.1/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-03-19 18:22:21.000000 keras-3.1.1/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.375357 keras-3.1.1/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5565 2024-03-19 18:22:21.000000 keras-3.1.1/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.375622 keras-3.1.1/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-03-19 18:22:21.000000 keras-3.1.1/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.375931 keras-3.1.1/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-03-19 18:22:21.000000 keras-3.1.1/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.376098 keras-3.1.1/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-03-19 18:22:21.000000 keras-3.1.1/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.376285 keras-3.1.1/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-03-19 18:22:21.000000 keras-3.1.1/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.376492 keras-3.1.1/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      380 2024-03-19 18:22:21.000000 keras-3.1.1/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.376732 keras-3.1.1/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      180 2024-03-19 18:22:21.000000 keras-3.1.1/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.376967 keras-3.1.1/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-03-19 18:22:21.000000 keras-3.1.1/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.377289 keras-3.1.1/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-03-19 18:22:21.000000 keras-3.1.1/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.377496 keras-3.1.1/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-03-19 18:22:21.000000 keras-3.1.1/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.377673 keras-3.1.1/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-03-19 18:22:21.000000 keras-3.1.1/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.378125 keras-3.1.1/keras/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      649 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.378428 keras-3.1.1/keras/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3541 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12453 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.381709 keras-3.1.1/keras/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24920 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16849 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25275 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40461 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16035 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14510 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15521 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17169 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17935 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23522 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30695 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19007 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6364 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9111 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9434 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12706 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.382322 keras-3.1.1/keras/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1972 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.383946 keras-3.1.1/keras/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      584 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9738 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8853 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/dtypes.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2936 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8981 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1948 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/name_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3660 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17737 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7140 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.386549 keras-3.1.1/keras/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12772 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9680 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5711 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       26 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1756 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8758 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17221 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27719 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3688 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3595 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7559 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13805 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35724 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.388433 keras-3.1.1/keras/src/backend/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1013 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6862 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6920 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       28 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1921 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10587 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17544 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27208 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3907 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7659 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10643 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.391407 keras-3.1.1/keras/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1459 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9517 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2427 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7676 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6112 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11446 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25155 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    62979 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6819 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5400 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34505 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32141 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1994 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33462 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.393496 keras-3.1.1/keras/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1893 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14581 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9756 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1279 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1755 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15074 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23842 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    44332 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.395378 keras-3.1.1/keras/src/backend/torch/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       79 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1673 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1890 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      151 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2422 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1804 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      791 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2054 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1176 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8246 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13711 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17359 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.398680 keras-3.1.1/keras/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6944 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9831 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5262 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3207 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8934 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1302 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2966 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18489 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3105 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5340 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2731 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6844 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26418 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      670 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.399009 keras-3.1.1/keras/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1716 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/constraints/constraints.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.400537 keras-3.1.1/keras/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      384 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2645 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3851 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3087 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2915 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2930 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7150 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2394 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7204 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.400834 keras-3.1.1/keras/src/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/distribution/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31208 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.401202 keras-3.1.1/keras/src/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1033 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9839 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.401601 keras-3.1.1/keras/src/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/export/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27799 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/export/export_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.402646 keras-3.1.1/keras/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3945 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4885 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2634 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23353 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.403347 keras-3.1.1/keras/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8786 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.404549 keras-3.1.1/keras/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      273 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1237 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      810 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1901 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3454 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2671 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2259 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.405480 keras-3.1.1/keras/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4331 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11890 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17953 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27410 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.408931 keras-3.1.1/keras/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12031 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10696 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11618 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12644 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7302 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5573 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5672 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5693 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5895 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5899 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6001 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6089 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6452 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6533 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.411112 keras-3.1.1/keras/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12243 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26151 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7657 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      824 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5108 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9050 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2630 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1536 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9834 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61715 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.412947 keras-3.1.1/keras/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2151 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9250 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6587 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12764 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2213 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2685 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.414187 keras-3.1.1/keras/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13538 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8535 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9773 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4307 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1832 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.416772 keras-3.1.1/keras/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3345 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4151 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3236 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1461 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2426 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3132 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2470 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2358 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2452 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2586 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4126 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3226 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.421089 keras-3.1.1/keras/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14573 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7124 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5199 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13189 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29620 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8336 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10937 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    41400 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18476 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13921 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6467 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3815 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6270 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3806 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9648 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10615 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10816 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2178 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4615 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17753 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27857 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2140 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.422154 keras-3.1.1/keras/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1199 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3596 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3005 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1975 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2021 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7301 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.427093 keras-3.1.1/keras/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2762 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9046 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11267 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3060 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2088 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1336 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2323 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1594 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6096 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4911 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2108 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4648 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5062 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.429438 keras-3.1.1/keras/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13212 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27249 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8295 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8380 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8288 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2123 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26600 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25446 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18875 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17538 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4951 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4798 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.430139 keras-3.1.1/keras/src/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    70242 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/backend.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8413 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/layers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      524 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.430985 keras-3.1.1/keras/src/legacy/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    65532 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11173 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11111 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.432083 keras-3.1.1/keras/src/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7297 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22744 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      486 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9282 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21809 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.432563 keras-3.1.1/keras/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5637 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5899 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    64915 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/losses/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.434828 keras-3.1.1/keras/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7190 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15658 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61676 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11744 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3282 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26920 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8102 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26612 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7131 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19892 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.435827 keras-3.1.1/keras/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      144 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11120 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31081 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23569 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12905 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/sequential.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2165 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.437980 keras-3.1.1/keras/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      645 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21538 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15379 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31460 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17411 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30619 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61621 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5585 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   186858 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10476 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13766 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1701 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.440587 keras-3.1.1/keras/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3932 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4568 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7444 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3727 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5718 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4892 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3593 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35951 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8908 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4778 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11554 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5735 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      839 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5809 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.440897 keras-3.1.1/keras/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      520 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35514 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4365 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.441221 keras-3.1.1/keras/src/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1580 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/quantizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3231 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.441705 keras-3.1.1/keras/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      421 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13439 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4660 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/random/seed_generator.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.442000 keras-3.1.1/keras/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11800 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.442897 keras-3.1.1/keras/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      615 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7359 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8899 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26137 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28701 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.443326 keras-3.1.1/keras/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       50 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26180 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6198 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/testing/test_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.443906 keras-3.1.1/keras/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25825 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.445331 keras-3.1.1/keras/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5424 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14330 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17068 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3102 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9742 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2870 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19413 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5231 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2650 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3924 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    43638 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/trainers/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.450786 keras-3.1.1/keras/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1415 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2868 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14203 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4142 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28536 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16372 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/file_utils.py
--rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16617 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16539 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3492 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      264 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/jax_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15071 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1195 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/module_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1777 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4572 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10350 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4004 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1678 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4715 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      722 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/shape_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14414 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10575 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4631 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/tf_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9843 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4989 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/torch_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9004 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7906 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/tracking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20185 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/utils/tree.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      190 2024-03-19 18:22:09.000000 keras-3.1.1/keras/src/version.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.450975 keras-3.1.1/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-03-19 18:22:21.000000 keras-3.1.1/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.451140 keras-3.1.1/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-03-19 18:22:21.000000 keras-3.1.1/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.451295 keras-3.1.1/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-03-19 18:22:21.000000 keras-3.1.1/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-03-19 18:22:24.452798 keras-3.1.1/keras.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-03-19 18:22:24.000000 keras-3.1.1/keras.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19990 2024-03-19 18:22:24.000000 keras-3.1.1/keras.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-03-19 18:22:24.000000 keras-3.1.1/keras.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-03-19 18:22:24.000000 keras-3.1.1/keras.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-03-19 18:22:24.000000 keras-3.1.1/keras.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-03-19 18:22:24.453784 keras-3.1.1/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1861 2024-03-19 18:22:09.000000 keras-3.1.1/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.817716 keras-3.2.0/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-04-08 21:21:53.817468 keras-3.2.0/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4673 2024-04-08 21:21:45.000000 keras-3.2.0/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.716620 keras-3.2.0/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2095 2024-04-08 21:21:50.000000 keras-3.2.0/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.717671 keras-3.2.0/keras/_tf_keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.717834 keras-3.2.0/keras/_tf_keras/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2248 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718011 keras-3.2.0/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718187 keras-3.2.0/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718372 keras-3.2.0/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718562 keras-3.2.0/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718742 keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.718933 keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.719116 keras-3.2.0/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.719560 keras-3.2.0/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.719821 keras-3.2.0/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.720056 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.720243 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.720460 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.720656 keras-3.2.0/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.720830 keras-3.2.0/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721016 keras-3.2.0/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721213 keras-3.2.0/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721403 keras-3.2.0/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721578 keras-3.2.0/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721742 keras-3.2.0/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.721905 keras-3.2.0/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6809 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722147 keras-3.2.0/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722309 keras-3.2.0/keras/_tf_keras/keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722470 keras-3.2.0/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722621 keras-3.2.0/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722788 keras-3.2.0/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.722962 keras-3.2.0/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.723114 keras-3.2.0/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.723260 keras-3.2.0/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.723482 keras-3.2.0/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.723690 keras-3.2.0/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.723909 keras-3.2.0/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724133 keras-3.2.0/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724313 keras-3.2.0/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724468 keras-3.2.0/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724612 keras-3.2.0/keras/_tf_keras/keras/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724757 keras-3.2.0/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.724912 keras-3.2.0/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10079 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725084 keras-3.2.0/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725228 keras-3.2.0/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725365 keras-3.2.0/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3265 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725499 keras-3.2.0/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5156 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725711 keras-3.2.0/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.725862 keras-3.2.0/keras/_tf_keras/keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726019 keras-3.2.0/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8668 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726232 keras-3.2.0/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726379 keras-3.2.0/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726520 keras-3.2.0/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726676 keras-3.2.0/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5607 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.726891 keras-3.2.0/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727061 keras-3.2.0/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727202 keras-3.2.0/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727362 keras-3.2.0/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      757 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727510 keras-3.2.0/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1365 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727660 keras-3.2.0/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      510 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727820 keras-3.2.0/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.727963 keras-3.2.0/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728105 keras-3.2.0/keras/_tf_keras/keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728243 keras-3.2.0/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728384 keras-3.2.0/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      915 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728523 keras-3.2.0/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728672 keras-3.2.0/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728822 keras-3.2.0/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-08 21:21:50.000000 keras-3.2.0/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.728961 keras-3.2.0/keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-04-08 21:21:50.000000 keras-3.2.0/keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729098 keras-3.2.0/keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729236 keras-3.2.0/keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729376 keras-3.2.0/keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729528 keras-3.2.0/keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729672 keras-3.2.0/keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729815 keras-3.2.0/keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.729950 keras-3.2.0/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730088 keras-3.2.0/keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730231 keras-3.2.0/keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730371 keras-3.2.0/keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730516 keras-3.2.0/keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730676 keras-3.2.0/keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730830 keras-3.2.0/keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.730975 keras-3.2.0/keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731123 keras-3.2.0/keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731282 keras-3.2.0/keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731433 keras-3.2.0/keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731575 keras-3.2.0/keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-04-08 21:21:50.000000 keras-3.2.0/keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731729 keras-3.2.0/keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      884 2024-04-08 21:21:50.000000 keras-3.2.0/keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.731874 keras-3.2.0/keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-04-08 21:21:50.000000 keras-3.2.0/keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732026 keras-3.2.0/keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-04-08 21:21:50.000000 keras-3.2.0/keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732177 keras-3.2.0/keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-04-08 21:21:50.000000 keras-3.2.0/keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732315 keras-3.2.0/keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732459 keras-3.2.0/keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732624 keras-3.2.0/keras/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732769 keras-3.2.0/keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.732906 keras-3.2.0/keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.733040 keras-3.2.0/keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.733174 keras-3.2.0/keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.733313 keras-3.2.0/keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.733663 keras-3.2.0/keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-04-08 21:21:50.000000 keras-3.2.0/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.733867 keras-3.2.0/keras/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-04-08 21:21:50.000000 keras-3.2.0/keras/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734066 keras-3.2.0/keras/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-04-08 21:21:50.000000 keras-3.2.0/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734247 keras-3.2.0/keras/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-08 21:21:50.000000 keras-3.2.0/keras/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734408 keras-3.2.0/keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-04-08 21:21:50.000000 keras-3.2.0/keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734567 keras-3.2.0/keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9757 2024-04-08 21:21:50.000000 keras-3.2.0/keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734748 keras-3.2.0/keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-04-08 21:21:50.000000 keras-3.2.0/keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.734899 keras-3.2.0/keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-08 21:21:50.000000 keras-3.2.0/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735067 keras-3.2.0/keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2294 2024-04-08 21:21:50.000000 keras-3.2.0/keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735235 keras-3.2.0/keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4231 2024-04-08 21:21:50.000000 keras-3.2.0/keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735473 keras-3.2.0/keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-08 21:21:50.000000 keras-3.2.0/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735633 keras-3.2.0/keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-04-08 21:21:50.000000 keras-3.2.0/keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735819 keras-3.2.0/keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8668 2024-04-08 21:21:50.000000 keras-3.2.0/keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.735994 keras-3.2.0/keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-04-08 21:21:50.000000 keras-3.2.0/keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.736144 keras-3.2.0/keras/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-04-08 21:21:50.000000 keras-3.2.0/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.736308 keras-3.2.0/keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-04-08 21:21:50.000000 keras-3.2.0/keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.736492 keras-3.2.0/keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5607 2024-04-08 21:21:50.000000 keras-3.2.0/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.736773 keras-3.2.0/keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-04-08 21:21:50.000000 keras-3.2.0/keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.736938 keras-3.2.0/keras/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-04-08 21:21:50.000000 keras-3.2.0/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737082 keras-3.2.0/keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-04-08 21:21:50.000000 keras-3.2.0/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737217 keras-3.2.0/keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-04-08 21:21:50.000000 keras-3.2.0/keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737365 keras-3.2.0/keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      380 2024-04-08 21:21:50.000000 keras-3.2.0/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737513 keras-3.2.0/keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      180 2024-04-08 21:21:50.000000 keras-3.2.0/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737651 keras-3.2.0/keras/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-08 21:21:50.000000 keras-3.2.0/keras/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737802 keras-3.2.0/keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-04-08 21:21:50.000000 keras-3.2.0/keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.737957 keras-3.2.0/keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-04-08 21:21:50.000000 keras-3.2.0/keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.738116 keras-3.2.0/keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      915 2024-04-08 21:21:50.000000 keras-3.2.0/keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.738578 keras-3.2.0/keras/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      649 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.738899 keras-3.2.0/keras/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3541 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12453 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.743419 keras-3.2.0/keras/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24920 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16849 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25275 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40461 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16035 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14510 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15521 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17169 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17935 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23522 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30695 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19007 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6364 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9111 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9434 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12706 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.744088 keras-3.2.0/keras/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1972 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.745355 keras-3.2.0/keras/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      584 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9738 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9809 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2936 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8981 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2546 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3660 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17953 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7140 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.748487 keras-3.2.0/keras/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12772 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9680 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5711 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       26 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1756 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8758 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18796 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29444 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3688 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3595 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7559 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13805 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    36171 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.750620 keras-3.2.0/keras/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1013 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6862 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6920 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       28 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1921 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10587 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17760 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27723 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3962 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7659 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10708 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.753584 keras-3.2.0/keras/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1459 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9503 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2427 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7676 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6112 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11446 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26462 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    67409 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6819 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34607 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32141 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1994 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33608 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.756280 keras-3.2.0/keras/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1893 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16169 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9756 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1279 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1755 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15074 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24038 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    45949 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.758125 keras-3.2.0/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       79 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1673 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1890 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      151 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2422 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1804 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      791 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2054 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1176 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8293 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13711 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17489 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.760968 keras-3.2.0/keras/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6944 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9831 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5262 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3207 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8934 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1302 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2966 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18489 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3105 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5340 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2728 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6844 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26400 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      670 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.761287 keras-3.2.0/keras/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1716 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/constraints/constraints.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.762936 keras-3.2.0/keras/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      384 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2645 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3851 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3087 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2915 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2930 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7150 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2394 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7204 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.763292 keras-3.2.0/keras/src/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      719 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/distribution/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31208 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.763641 keras-3.2.0/keras/src/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1033 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9952 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.764042 keras-3.2.0/keras/src/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/export/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32837 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/export/export_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.764820 keras-3.2.0/keras/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3945 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4885 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2634 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23463 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.765407 keras-3.2.0/keras/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8786 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.766500 keras-3.2.0/keras/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      273 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1237 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      810 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1901 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3454 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2671 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2259 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.767333 keras-3.2.0/keras/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4331 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11890 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17953 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27410 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.770399 keras-3.2.0/keras/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12031 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10696 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11618 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12644 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7301 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5572 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5671 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5692 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5894 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5898 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6000 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6088 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6451 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6532 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.771948 keras-3.2.0/keras/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16970 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33719 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15723 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      824 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5108 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8996 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2630 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1536 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9834 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    62806 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.774071 keras-3.2.0/keras/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2151 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9250 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6587 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12808 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2213 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2685 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.775250 keras-3.2.0/keras/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13441 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8535 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9837 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4307 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1832 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.777790 keras-3.2.0/keras/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3345 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4151 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3236 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1461 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2426 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3132 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2470 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2358 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2452 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2586 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4126 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3226 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.783310 keras-3.2.0/keras/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14573 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5490 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13176 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29620 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8318 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10937 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    41400 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18459 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13921 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6462 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3815 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6316 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3806 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9646 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10615 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10816 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2178 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4615 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17735 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27821 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2140 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.784371 keras-3.2.0/keras/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1199 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3596 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3005 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2017 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2063 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7301 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.787020 keras-3.2.0/keras/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2761 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9045 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11266 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3060 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2088 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1336 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2323 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1593 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5993 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4911 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2107 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4647 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5061 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.790794 keras-3.2.0/keras/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27249 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8295 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8380 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8288 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27708 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26551 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18875 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17538 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4950 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4798 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.791583 keras-3.2.0/keras/src/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    70242 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/backend.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8413 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/layers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      524 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.792243 keras-3.2.0/keras/src/legacy/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    65546 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11173 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11111 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.793572 keras-3.2.0/keras/src/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7297 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22746 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      486 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9282 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21809 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.794198 keras-3.2.0/keras/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6173 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5899 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    66376 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/losses/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.796495 keras-3.2.0/keras/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7190 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15605 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61580 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11744 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3256 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26857 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8187 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26612 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10538 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7213 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19819 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.797975 keras-3.2.0/keras/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      144 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11101 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32036 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23000 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12905 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/sequential.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2165 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.801052 keras-3.2.0/keras/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      645 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22873 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15341 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31490 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17411 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30619 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    62114 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5585 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   189853 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10476 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13766 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1701 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.803976 keras-3.2.0/keras/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3932 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4568 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7446 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3727 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5718 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4892 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3593 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    36189 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8908 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4778 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11554 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5735 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      839 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5811 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.804336 keras-3.2.0/keras/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      520 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    35508 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4365 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.804672 keras-3.2.0/keras/src/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1580 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/quantizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3231 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.805253 keras-3.2.0/keras/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      421 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13439 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4660 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/random/seed_generator.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.805636 keras-3.2.0/keras/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11800 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.806587 keras-3.2.0/keras/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      615 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7359 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9668 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27009 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28701 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.807645 keras-3.2.0/keras/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      267 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26564 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6198 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/testing/test_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.808483 keras-3.2.0/keras/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25825 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.810238 keras-3.2.0/keras/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5424 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14330 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17068 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3102 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9724 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2870 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19413 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5231 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2650 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3924 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    45200 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/trainers/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.815978 keras-3.2.0/keras/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1415 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2877 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14203 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4144 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28538 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16372 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16624 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16545 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3492 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26523 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/jax_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      264 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/jax_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15071 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1219 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1777 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4572 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10350 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4004 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1678 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4715 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14519 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10575 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4631 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/tf_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9843 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4988 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/torch_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9004 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7908 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20703 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/utils/tree.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      190 2024-04-08 21:21:45.000000 keras-3.2.0/keras/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.816143 keras-3.2.0/keras/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-04-08 21:21:50.000000 keras-3.2.0/keras/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.816288 keras-3.2.0/keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-08 21:21:50.000000 keras-3.2.0/keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.816737 keras-3.2.0/keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-08 21:21:50.000000 keras-3.2.0/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-08 21:21:53.817041 keras-3.2.0/keras.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-04-08 21:21:53.000000 keras-3.2.0/keras.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19988 2024-04-08 21:21:53.000000 keras-3.2.0/keras.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-08 21:21:53.000000 keras-3.2.0/keras.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-08 21:21:53.000000 keras-3.2.0/keras.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-08 21:21:53.000000 keras-3.2.0/keras.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-08 21:21:53.817770 keras-3.2.0/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1861 2024-04-08 21:21:45.000000 keras-3.2.0/setup.py
```

### Comparing `keras-3.1.1/PKG-INFO` & `keras-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.1.1
+Version: 3.2.0
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-3.1.1/README.md` & `keras-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/__init__.py` & `keras-3.2.0/keras/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.1.1"
+__version__ = "3.2.0"
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/activations/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/applications/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/backend/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/config/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/constraints/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/distribution/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/initializers/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/layers/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/layers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,16 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
+from keras.src.utils.jax_layer import FlaxLayer
+from keras.src.utils.jax_layer import JaxLayer
 from keras.src.utils.torch_utils import TorchModuleWrapper
 
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/losses/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/losses/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
 from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
+from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
 from keras.src.losses.losses import KLDivergence
 from keras.src.losses.losses import LogCosh
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
@@ -30,14 +31,15 @@
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
+from keras.src.losses.losses import dice
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
 from keras.src.losses.losses import kl_divergence
 from keras.src.losses.losses import log_cosh
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/metrics/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/ops/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 from keras.src.ops.numpy import broadcast_to
 from keras.src.ops.numpy import ceil
 from keras.src.ops.numpy import clip
 from keras.src.ops.numpy import concatenate
 from keras.src.ops.numpy import conj
 from keras.src.ops.numpy import conjugate
 from keras.src.ops.numpy import copy
+from keras.src.ops.numpy import correlate
 from keras.src.ops.numpy import cos
 from keras.src.ops.numpy import cosh
 from keras.src.ops.numpy import count_nonzero
 from keras.src.ops.numpy import cross
 from keras.src.ops.numpy import cumprod
 from keras.src.ops.numpy import cumsum
 from keras.src.ops.numpy import diag
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from keras.src.ops.numpy import broadcast_to
 from keras.src.ops.numpy import ceil
 from keras.src.ops.numpy import clip
 from keras.src.ops.numpy import concatenate
 from keras.src.ops.numpy import conj
 from keras.src.ops.numpy import conjugate
 from keras.src.ops.numpy import copy
+from keras.src.ops.numpy import correlate
 from keras.src.ops.numpy import cos
 from keras.src.ops.numpy import cosh
 from keras.src.ops.numpy import count_nonzero
 from keras.src.ops.numpy import cross
 from keras.src.ops.numpy import cumprod
 from keras.src.ops.numpy import cumsum
 from keras.src.ops.numpy import diag
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/random/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/saving/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/saving/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 from keras.src.saving.object_registration import CustomObjectScope
 from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
+from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
+from keras.src.saving.saving_api import save_weights
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
```

### Comparing `keras-3.1.1/keras/_tf_keras/keras/tree/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/_tf_keras/keras/utils/__init__.py` & `keras-3.2.0/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/activations/__init__.py` & `keras-3.2.0/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/applications/__init__.py` & `keras-3.2.0/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/applications/convnext/__init__.py` & `keras-3.2.0/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/applications/efficientnet/__init__.py` & `keras-3.2.0/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/applications/efficientnet_v2/__init__.py` & `keras-3.2.0/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/backend/__init__.py` & `keras-3.2.0/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/callbacks/__init__.py` & `keras-3.2.0/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/config/__init__.py` & `keras-3.2.0/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/constraints/__init__.py` & `keras-3.2.0/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/distribution/__init__.py` & `keras-3.2.0/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/initializers/__init__.py` & `keras-3.2.0/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/layers/__init__.py` & `keras-3.2.0/keras/layers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,10 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
+from keras.src.utils.jax_layer import FlaxLayer
+from keras.src.utils.jax_layer import JaxLayer
 from keras.src.utils.torch_utils import TorchModuleWrapper
```

### Comparing `keras-3.1.1/keras/losses/__init__.py` & `keras-3.2.0/keras/losses/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
 from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
+from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
 from keras.src.losses.losses import KLDivergence
 from keras.src.losses.losses import LogCosh
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
@@ -30,14 +31,15 @@
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
+from keras.src.losses.losses import dice
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
 from keras.src.losses.losses import kl_divergence
 from keras.src.losses.losses import log_cosh
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
```

### Comparing `keras-3.1.1/keras/metrics/__init__.py` & `keras-3.2.0/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/mixed_precision/__init__.py` & `keras-3.2.0/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/ops/__init__.py` & `keras-3.2.0/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 from keras.src.ops.numpy import broadcast_to
 from keras.src.ops.numpy import ceil
 from keras.src.ops.numpy import clip
 from keras.src.ops.numpy import concatenate
 from keras.src.ops.numpy import conj
 from keras.src.ops.numpy import conjugate
 from keras.src.ops.numpy import copy
+from keras.src.ops.numpy import correlate
 from keras.src.ops.numpy import cos
 from keras.src.ops.numpy import cosh
 from keras.src.ops.numpy import count_nonzero
 from keras.src.ops.numpy import cross
 from keras.src.ops.numpy import cumprod
 from keras.src.ops.numpy import cumsum
 from keras.src.ops.numpy import diag
```

### Comparing `keras-3.1.1/keras/ops/linalg/__init__.py` & `keras-3.2.0/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/ops/nn/__init__.py` & `keras-3.2.0/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/ops/numpy/__init__.py` & `keras-3.2.0/keras/ops/numpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from keras.src.ops.numpy import broadcast_to
 from keras.src.ops.numpy import ceil
 from keras.src.ops.numpy import clip
 from keras.src.ops.numpy import concatenate
 from keras.src.ops.numpy import conj
 from keras.src.ops.numpy import conjugate
 from keras.src.ops.numpy import copy
+from keras.src.ops.numpy import correlate
 from keras.src.ops.numpy import cos
 from keras.src.ops.numpy import cosh
 from keras.src.ops.numpy import count_nonzero
 from keras.src.ops.numpy import cross
 from keras.src.ops.numpy import cumprod
 from keras.src.ops.numpy import cumsum
 from keras.src.ops.numpy import diag
```

### Comparing `keras-3.1.1/keras/optimizers/__init__.py` & `keras-3.2.0/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/optimizers/legacy/__init__.py` & `keras-3.2.0/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/optimizers/schedules/__init__.py` & `keras-3.2.0/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/random/__init__.py` & `keras-3.2.0/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/regularizers/__init__.py` & `keras-3.2.0/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/saving/__init__.py` & `keras-3.2.0/keras/saving/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 from keras.src.saving.object_registration import CustomObjectScope
 from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
+from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
+from keras.src.saving.saving_api import save_weights
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
```

### Comparing `keras-3.1.1/keras/src/__init__.py` & `keras-3.2.0/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/activations/__init__.py` & `keras-3.2.0/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/activations/activations.py` & `keras-3.2.0/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/api_export.py` & `keras-3.2.0/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/convnext.py` & `keras-3.2.0/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/densenet.py` & `keras-3.2.0/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/efficientnet.py` & `keras-3.2.0/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/efficientnet_v2.py` & `keras-3.2.0/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/imagenet_utils.py` & `keras-3.2.0/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/inception_resnet_v2.py` & `keras-3.2.0/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/inception_v3.py` & `keras-3.2.0/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/mobilenet.py` & `keras-3.2.0/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/mobilenet_v2.py` & `keras-3.2.0/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/mobilenet_v3.py` & `keras-3.2.0/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/nasnet.py` & `keras-3.2.0/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/resnet.py` & `keras-3.2.0/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/resnet_v2.py` & `keras-3.2.0/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/vgg16.py` & `keras-3.2.0/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/vgg19.py` & `keras-3.2.0/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/applications/xception.py` & `keras-3.2.0/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/__init__.py` & `keras-3.2.0/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/__init__.py` & `keras-3.2.0/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/backend_utils.py` & `keras-3.2.0/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/dtypes.py` & `keras-3.2.0/keras/src/backend/common/dtypes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 import functools
 
-from keras.src import backend
 from keras.src.api_export import keras_export
-from keras.src.backend.common.variables import ALLOWED_DTYPES
+from keras.src.backend import config
 from keras.src.backend.common.variables import standardize_dtype
 
-"""
-We adapted the type promotion lattice from JAX. Ref:
-https://github.com/google/jax/blob/main/jax/_src/dtypes.py
-"""
-
-BOOL_TYPES = ["bool"]
-INT_TYPES = [
+BOOL_TYPES = ("bool",)
+INT_TYPES = (
     "uint8",
     "uint16",
     "uint32",
     "uint64",
     "int8",
     "int16",
     "int32",
     "int64",
-]
-FLOAT_TYPES = ["bfloat16", "float16", "float32", "float64"]
-WEAK_TYPES = ["int", "float"]
+)
+FLOAT_TYPES = ("bfloat16", "float16", "float32", "float64")
+WEAK_TYPES = ("int", "float")
+# We need to separate float8 from float because there are no implicit
+# conversions from float8 dtypes to other dtypes.
+# Ref: https://github.com/google/jax/issues/16705
+FLOAT8_TYPES = ("float8_e4m3fn", "float8_e5m2")
+
+# All supported dtypes in Keras
+ALLOWED_DTYPES = (
+    "float16",
+    "float32",
+    "float64",
+    "uint8",
+    "uint16",
+    "uint32",
+    "uint64",
+    "int8",
+    "int16",
+    "int32",
+    "int64",
+    "bfloat16",
+    "bool",
+    "string",
+    "float8_e4m3fn",
+    "float8_e5m2",
+)
+PYTHON_DTYPES_MAP = {
+    bool: "bool",
+    int: "int64" if config.backend() == "tensorflow" else "int32",
+    float: "float32",
+    str: "string",
+    # special case for string value
+    "int": "int64" if config.backend() == "tensorflow" else "int32",
+}
+
+# We adapted the type promotion lattice from JAX. Ref:
+# https://github.com/google/jax/blob/main/jax/_src/dtypes.py
 
 
 def _type_promotion_lattice():
     """
     Return the type promotion lattice in the form of a DAG.
     This DAG maps each type to its immediately higher type on the lattice.
     """
@@ -164,15 +193,15 @@
             )
     return dtype
 
 
 @functools.lru_cache(maxsize=None)
 def _resolve_weak_type(dtype, precision="32"):
     """Resolve weak type by the precision of `backend.floatx()`."""
-    extended_allowed_dtypes = ALLOWED_DTYPES.union(WEAK_TYPES)
+    extended_allowed_dtypes = set(ALLOWED_DTYPES).union(WEAK_TYPES)
     if dtype not in extended_allowed_dtypes:
         raise ValueError(
             "Invalid value for argument `dtype`. Expected one of "
             f"{extended_allowed_dtypes}. Received: dtype={dtype}"
         )
     if precision not in ["16", "32", "64"]:
         raise ValueError(
@@ -230,15 +259,15 @@
     else:
         out_dtype = _least_upper_bound(
             *{_respect_weak_type(d, w) for d, w in zip(dtypes, weak_types)}
         )
         out_weak_type = any(out_dtype is t for t in WEAK_TYPES)
 
     out_weak_type = (out_dtype != "bool") and out_weak_type
-    precision = backend.floatx()[-2:]
+    precision = config.floatx()[-2:]
     if out_weak_type:
         out_dtype = _resolve_weak_type(out_dtype, precision=precision)
     return out_dtype
 
 
 @keras_export("keras.backend.result_type")
 def result_type(*dtypes):
@@ -266,12 +295,18 @@
     >>> y = keras.ops.ones((1,), dtype="float32")
     >>> keras.backend.result_type(x.dtype, y.dtype)
     "float32"
     """
     if len(dtypes) == 0:
         # If no dtypes provided, default to floatx, this matches
         # `ops.convert_to_tensor([])`
-        return backend.floatx()
+        return config.floatx()
+    for dtype in dtypes:
+        if dtype in FLOAT8_TYPES:
+            raise ValueError(
+                "There is no implicit conversions from float8 dtypes to others."
+                f" You must cast it internally. Received: {dtypes}"
+            )
     return _lattice_result_type(
-        *(backend.floatx() if arg is None else arg for arg in dtypes),
+        *(config.floatx() if arg is None else arg for arg in dtypes),
     )
```

### Comparing `keras-3.1.1/keras/src/backend/common/global_state.py` & `keras-3.2.0/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/keras_tensor.py` & `keras-3.2.0/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/name_scope.py` & `keras-3.2.0/keras/src/backend/common/name_scope.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,26 +7,37 @@
     Args:
         name: Name of the current scope (string).
         caller: Optional ID of a caller object (e.g. class instance).
         deduplicate: If `True`, if `caller` was passed,
             and the previous caller matches the current caller,
             and the previous name matches the current name,
             do not reenter a new namespace.
+        override_parent: Can be used to provide an absolute path
+            which would override any previously opened name scopes.
     """
 
-    def __init__(self, name, caller=None, deduplicate=True):
+    def __init__(
+        self, name, caller=None, deduplicate=True, override_parent=None
+    ):
         if not isinstance(name, str) or "/" in name:
             raise ValueError(
                 "Argument `name` must be a string and "
                 "cannot contain character `/`. "
                 f"Received: name={name}"
             )
         self.name = name
         self.caller = caller
         self.deduplicate = deduplicate
+        self.override_parent = override_parent
+        if (
+            override_parent is None
+            and deduplicate
+            and getattr(caller, "_parent_path", None) is not None
+        ):
+            self.override_parent = caller._parent_path
         self._pop_on_exit = False
 
     def __enter__(self):
         name_scope_stack = global_state.get_global_attribute(
             "name_scope_stack", default=[], set_to_default=True
         )
         if self.deduplicate and name_scope_stack:
@@ -50,9 +61,14 @@
             name_scope_stack.pop()
 
 
 def current_path():
     name_scope_stack = global_state.get_global_attribute("name_scope_stack")
     if name_scope_stack is None:
         return ""
-    return "/".join(x.name for x in name_scope_stack)
+    parts = []
+    for entry in name_scope_stack:
+        if entry.override_parent is not None:
+            parts = [p for p in entry.override_parent.split("/") if p]
+        parts.append(entry.name)
+    return "/".join(parts)
```

### Comparing `keras-3.1.1/keras/src/backend/common/stateless_scope.py` & `keras-3.2.0/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/common/variables.py` & `keras-3.2.0/keras/src/backend/common/variables.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 import numpy as np
 
 from keras.src.api_export import keras_export
 from keras.src.backend import config
+from keras.src.backend.common import dtypes
 from keras.src.backend.common import global_state
 from keras.src.backend.common.name_scope import current_path
 from keras.src.backend.common.stateless_scope import get_stateless_scope
 from keras.src.backend.common.stateless_scope import in_stateless_scope
 from keras.src.utils.module_utils import tensorflow as tf
 from keras.src.utils.naming import auto_name
 
 
 class KerasVariable:
     def __init__(
-        self, initializer, shape=None, dtype=None, trainable=True, name=None
+        self,
+        initializer,
+        shape=None,
+        dtype=None,
+        trainable=True,
+        autocast=True,
+        aggregation="mean",
+        name=None,
     ):
         name = name or auto_name(self.__class__.__name__)
         if not isinstance(name, str) or "/" in name:
             raise ValueError(
                 "Argument `name` must be a string and "
                 "cannot contain character `/`. "
                 f"Received: name={name}"
             )
+        if aggregation not in ("mean", "sum", "only_first_replica"):
+            raise ValueError(
+                "Invalid valid for argument `aggregation`. Expected "
+                "one of {'mean', 'sum', 'only_first_replica'}. "
+                f"Received: aggregation={aggregation}"
+            )
         self.name = name
         parent_path = current_path()
         if parent_path:
             self.path = current_path() + "/" + self.name
         else:
             self.path = self.name
         dtype = standardize_dtype(dtype)
         self._dtype = dtype
         self._shape = None
         self._initializer = None
         self._regularizer = None
         self._constraint = None
         self._trainable = trainable
+        self._autocast = autocast
+        self._aggregation = aggregation
         if isinstance(initializer, str):
             from keras.src import initializers
 
             initializer = initializers.get(initializer)
         if callable(initializer):
             if shape is None:
                 raise ValueError(
@@ -103,22 +119,26 @@
                 "fully-defined (no `None` dimensions). Received: "
                 f"shape={shape} for variable path='{self.path}'"
             )
         return shape
 
     def _maybe_autocast(self, value):
         autocast_scope = get_autocast_scope()
-        if autocast_scope is not None:
+        if self._autocast and autocast_scope is not None:
             return autocast_scope.maybe_cast(value)
         return value
 
     def numpy(self):
         return np.array(self)
 
     @property
+    def aggregation(self):
+        return self._aggregation
+
+    @property
     def value(self):
         if in_stateless_scope():
             scope = get_stateless_scope()
             value = scope.get_current_value(self)
             if value is not None:
                 return self._maybe_autocast(value)
         if self._value is None:
@@ -153,15 +173,19 @@
 
     def assign_sub(self, value):
         self.assign(self - value)
 
     @property
     def dtype(self):
         autocast_scope = get_autocast_scope()
-        if autocast_scope is not None and is_float_dtype(self._dtype):
+        if (
+            self._autocast
+            and autocast_scope is not None
+            and is_float_dtype(self._dtype)
+        ):
             return autocast_scope.dtype
         return self._dtype
 
     @property
     def shape(self):
         return self._shape
 
@@ -382,58 +406,31 @@
     collection = global_state.get_global_attribute("uninitialized_variables")
     if collection:
         for v in collection:
             v._deferred_initialize()
     global_state.set_global_attribute("uninitialized_variables", [])
 
 
-ALLOWED_DTYPES = {
-    "float16",
-    "float32",
-    "float64",
-    "uint8",
-    "uint16",
-    "uint32",
-    "uint64",
-    "int8",
-    "int16",
-    "int32",
-    "int64",
-    "bfloat16",
-    "bool",
-    "string",
-}
-
-PYTHON_DTYPES_MAP = {
-    bool: "bool",
-    int: "int64" if config.backend() == "tensorflow" else "int32",
-    float: "float32",
-    str: "string",
-    # special case for string value
-    "int": "int64" if config.backend() == "tensorflow" else "int32",
-}
-
-
 @keras_export(
     ["keras.utils.standardize_dtype", "keras.backend.standardize_dtype"]
 )
 def standardize_dtype(dtype):
     if dtype is None:
         return config.floatx()
-    dtype = PYTHON_DTYPES_MAP.get(dtype, dtype)
+    dtype = dtypes.PYTHON_DTYPES_MAP.get(dtype, dtype)
     if hasattr(dtype, "name"):
         dtype = dtype.name
     elif hasattr(dtype, "__str__") and (
         "torch" in str(dtype) or "jax.numpy" in str(dtype)
     ):
         dtype = str(dtype).split(".")[-1]
     elif hasattr(dtype, "__name__"):
         dtype = dtype.__name__
 
-    if dtype not in ALLOWED_DTYPES:
+    if dtype not in dtypes.ALLOWED_DTYPES:
         raise ValueError(f"Invalid dtype: {dtype}")
     return dtype
 
 
 def standardize_shape(shape):
     if not isinstance(shape, tuple):
         if shape is None:
```

### Comparing `keras-3.1.1/keras/src/backend/config.py` & `keras-3.2.0/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/exports.py` & `keras-3.2.0/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/__init__.py` & `keras-3.2.0/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/core.py` & `keras-3.2.0/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/distribution_lib.py` & `keras-3.2.0/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/image.py` & `keras-3.2.0/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/linalg.py` & `keras-3.2.0/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/math.py` & `keras-3.2.0/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/nn.py` & `keras-3.2.0/keras/src/backend/jax/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import jax
+import jax.experimental.sparse as jax_sparse
 import jax.numpy as jnp
 import numpy as np
 from jax import lax
 from jax import nn as jnn
 
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
@@ -400,27 +401,63 @@
         padding=padding_values,
         rhs_dilation=dilation_rate,
         dimension_numbers=dimension_numbers,
         transpose_kernel=True,
     )
 
 
-def one_hot(x, num_classes, axis=-1, dtype="float32"):
+def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     x = convert_to_tensor(x)
+    if sparse:
+        if axis < 0:
+            axis = axis + len(x.shape) + 1
+        if dtype is None:
+            dtype = "float32"
+        # We deal with negative inputs by having zeros in the output although
+        # it's useless. It makes shapes static.
+        values = jnp.greater_equal(jnp.ravel(x), 0).astype(dtype)
+        values_count = values.shape[0]
+        indices = [jnp.arange(dim) for dim in x.shape]
+        indices = jnp.meshgrid(*indices, indexing="ij")
+        indices.insert(axis, jnp.maximum(x, 0))  # Deal with negative indices
+        indices = [a.reshape(values_count, 1).astype("int32") for a in indices]
+        indices = jnp.concatenate(indices, axis=1)
+        shape = list(x.shape)
+        shape.insert(axis, num_classes)
+        shape = tuple(shape)
+        return jax_sparse.BCOO(
+            (values, indices),
+            shape=shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
     return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
 
 
-def multi_hot(x, num_classes, axis=-1, dtype="float32"):
+def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = jnp.max(
+    if sparse:
+        result = one_hot(
+            x, num_classes, axis=axis, dtype="int32", sparse=sparse
+        )
+        # JAX's BCOO does not support max reduction, use sum and compare with 0.
+        result = jax_sparse.bcoo_reduce_sum(result, axes=(reduction_axis,))
+        result = jax_sparse.bcoo_sum_duplicates(result)
+        values = jnp.greater_equal(result.data, 0).astype(dtype)
+        return jax_sparse.BCOO(
+            (values, result.indices),
+            shape=result.shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
+    return jnp.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
         axis=reduction_axis,
     )
-    return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
     target = jnp.array(target)
     output = jnp.array(output)
 
     if target.shape != output.shape:
```

### Comparing `keras-3.1.1/keras/src/backend/jax/numpy.py` & `keras-3.2.0/keras/src/backend/jax/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,46 @@
 import jax.numpy as jnp
 
 from keras.src.backend import config
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
 from keras.src.backend.common.variables import standardize_dtype
+from keras.src.backend.jax import nn
 from keras.src.backend.jax import sparse
 from keras.src.backend.jax.core import cast
 from keras.src.backend.jax.core import convert_to_tensor
 
 
 @sparse.elementwise_binary_union(linear=True, use_sparsify=True)
 def add(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.add(x1, x2)
 
 
-def bincount(x, weights=None, minlength=0):
+def bincount(x, weights=None, minlength=0, sparse=False):
+    if sparse:
+        reduction_axis = 1 if len(x.shape) > 1 else 0
+        maxlength = jnp.maximum(jnp.max(x) + 1, minlength)
+        one_hot_encoding = nn.one_hot(x, maxlength, sparse=sparse)
+        if weights is not None:
+            split_weights = split(
+                weights,
+                weights.shape[reduction_axis],
+                reduction_axis,
+            )
+            stacked_weights = stack(split_weights, axis=reduction_axis)
+            one_hot_encoding = one_hot_encoding * stacked_weights
+
+        outputs = jax_sparse.bcoo_reduce_sum(
+            one_hot_encoding,
+            axes=(reduction_axis,),
+        )
+        return outputs
     if len(x.shape) == 2:
         if weights is None:
 
             def bincount_fn(arr):
                 return jnp.bincount(arr, minlength=minlength)
 
             bincounts = list(map(bincount_fn, x))
@@ -704,17 +723,17 @@
         axis = tuple(axis)
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         x = cast(x, config.floatx())
 
     result = jnp.median(x, axis=axis, keepdims=keepdims)
 
-    # TODO: jnp.median failed to keepdims when axis is None
+    # TODO: with jax < 0.4.26 jnp.median failed to keepdims when axis is None
     if keepdims is True and axis is None:
-        for _ in range(x.ndim - 1):
+        while result.ndim < x.ndim:
             result = jnp.expand_dims(result, axis=-1)
     return result
 
 
 def meshgrid(*x, indexing="xy"):
     return jnp.meshgrid(*x, indexing=indexing)
 
@@ -795,17 +814,18 @@
     x = convert_to_tensor(x)
     q = convert_to_tensor(q)
     if standardize_dtype(x.dtype) == "int64":
         x = cast(x, config.floatx())
 
     result = jnp.quantile(x, q, axis=axis, method=method, keepdims=keepdims)
 
-    # TODO: jnp.quantile failed to keepdims when axis is None
+    # TODO: with jax < 0.4.26 jnp.quantile failed to keepdims when axis is None
     if keepdims is True and axis is None:
-        for _ in range(x.ndim - 1):
+        result_ndim = x.ndim + (1 if len(q.shape) > 0 else 0)
+        while result.ndim < result_ndim:
             result = jnp.expand_dims(result, axis=-1)
     return result
 
 
 def ravel(x):
     x = convert_to_tensor(x)
     return jnp.ravel(x)
@@ -1065,14 +1085,34 @@
         jnp.var(x, axis=axis, keepdims=keepdims, dtype=compute_dtype),
         result_dtype,
     )
 
 
 def sum(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
+    if isinstance(x, jax_sparse.BCOO):
+        if axis is None:
+            axis = tuple(range(len(x.shape)))
+        (
+            canonical_axis,
+            keep_dims_shape,
+            broadcast_dimensions,
+        ) = sparse.axis_shape_dims_for_broadcast_in_dim(
+            axis, x.shape, insert_dims=False
+        )
+        output = jax_sparse.bcoo_reduce_sum(x, axes=canonical_axis)
+        if keepdims:
+            # `bcoo_reduce_sum` does not support keepdims, neither does
+            # sparsify(jnp.sum), so we recreate the empty dimensions.
+            output = jax_sparse.bcoo_broadcast_in_dim(
+                output,
+                shape=keep_dims_shape,
+                broadcast_dimensions=broadcast_dimensions,
+            )
+        return output
     return jnp.sum(x, axis=axis, keepdims=keepdims)
 
 
 def eye(N, M=None, k=0, dtype=None):
     dtype = dtype or config.floatx()
     return jnp.eye(N, M=M, k=k, dtype=dtype)
 
@@ -1084,7 +1124,13 @@
 
 
 def logical_xor(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.logical_xor(x1, x2)
 
+
+def correlate(x1, x2, mode="valid"):
+    x1 = convert_to_tensor(x1)
+    x2 = convert_to_tensor(x2)
+    return jnp.correlate(x1, x2, mode)
+
```

### Comparing `keras-3.1.1/keras/src/backend/jax/optimizer.py` & `keras-3.2.0/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/random.py` & `keras-3.2.0/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/rnn.py` & `keras-3.2.0/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/sparse.py` & `keras-3.2.0/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/jax/trainer.py` & `keras-3.2.0/keras/src/backend/jax/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from functools import partial
 
 import jax
 import numpy as np
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
-from keras.src import ops
 from keras.src import optimizers as optimizers_module
 from keras.src.backend import distribution_lib as jax_distribution_lib
 from keras.src.distribution import distribution_lib
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
@@ -27,51 +26,67 @@
         self.predict_function = None
         self._jax_state_synced = True
 
     def compute_loss_and_updates(
         self,
         trainable_variables,
         non_trainable_variables,
+        metrics_variables,
         x,
         y,
         sample_weight,
         training=False,
         optimizer_variables=None,
     ):
         """This method is stateless and is intended for use with jax.grad."""
         kwargs = {}
         if self._call_has_training_arg:
             kwargs["training"] = training
+
+        # Run stateless forward pass
         y_pred, non_trainable_variables, losses = self.stateless_call(
             trainable_variables,
             non_trainable_variables,
             x,
             return_losses=True,
             **kwargs,
         )
+        if losses:
+            # Make forward pass losses available to compute_loss.
+            self._losses_override.clear()
+            self._losses_override = losses
 
-        var_mapping = list(zip(self.trainable_variables, trainable_variables))
-        var_mapping.extend(
-            zip(self.non_trainable_variables, non_trainable_variables)
-        )
-        with backend.StatelessScope(state_mapping=var_mapping):
-            # Note that this is needed for the regularization loss, which need
-            # the latest value of train/non-trainable variables.
-            loss = self.compute_loss(
-                x, y, y_pred, sample_weight, allow_empty=True
-            )
+        loss, variables = self.stateless_compute_loss(
+            trainable_variables,
+            non_trainable_variables,
+            metrics_variables,
+            x=x,
+            y=y,
+            y_pred=y_pred,
+            sample_weight=sample_weight,
+        )
         if losses:
-            loss += ops.sum(losses)
+            self._losses_override.clear()
+        (trainable_variables, non_trainable_variables, metrics_variables) = (
+            variables
+        )
+
+        # Handle loss scaling
         unscaled_loss = loss
         if training and self.optimizer is not None:
             # Scale loss with a StatelessScope, to use an update scale variable.
             mapping = list(zip(self.optimizer.variables, optimizer_variables))
             with backend.StatelessScope(state_mapping=mapping):
                 loss = self.optimizer.scale_loss(loss)
-        return loss, (unscaled_loss, y_pred, non_trainable_variables)
+        return loss, (
+            unscaled_loss,
+            y_pred,
+            non_trainable_variables,
+            metrics_variables,
+        )
 
     def train_step(self, state, data):
         (
             trainable_variables,
             non_trainable_variables,
             optimizer_variables,
             metrics_variables,
@@ -79,36 +94,41 @@
         x, y, sample_weight = data_adapter_utils.unpack_x_y_sample_weight(data)
         grad_fn = jax.value_and_grad(
             self.compute_loss_and_updates, has_aux=True
         )
         (loss, aux), grads = grad_fn(
             trainable_variables,
             non_trainable_variables,
+            metrics_variables,
             x,
             y,
             sample_weight,
             training=True,
             optimizer_variables=optimizer_variables,
         )
-        (unscaled_loss, y_pred, non_trainable_variables) = aux
+        (unscaled_loss, y_pred, non_trainable_variables, metrics_variables) = (
+            aux
+        )
 
         (
             trainable_variables,
             optimizer_variables,
         ) = self.optimizer.stateless_apply(
             optimizer_variables, grads, trainable_variables
         )
 
         with backend.StatelessScope(
             state_mapping=[
                 (ref_v, v)
                 for ref_v, v in zip(self.metrics_variables, metrics_variables)
             ]
         ) as scope:
-            self._loss_tracker.update_state(unscaled_loss)
+            self._loss_tracker.update_state(
+                unscaled_loss, sample_weight=tree.flatten(x)[0].shape[0]
+            )
             logs = self.compute_metrics(x, y, y_pred, sample_weight)
 
         new_metrics_variables = []
         for ref_v in self.metrics_variables:
             new_v = scope.get_current_value(ref_v)
             if new_v is None:
                 new_v = ref_v.value
@@ -129,28 +149,33 @@
             non_trainable_variables,
             metrics_variables,
         ) = state
         x, y, sample_weight = data_adapter_utils.unpack_x_y_sample_weight(data)
         loss, aux = self.compute_loss_and_updates(
             trainable_variables,
             non_trainable_variables,
+            metrics_variables,
             x,
             y,
             sample_weight,
             training=False,
         )
-        (unscaled_loss, y_pred, non_trainable_variables) = aux
+        (unscaled_loss, y_pred, non_trainable_variables, metrics_variables) = (
+            aux
+        )
 
         with backend.StatelessScope(
             state_mapping=[
                 (ref_v, v)
                 for ref_v, v in zip(self.metrics_variables, metrics_variables)
             ]
         ) as scope:
-            self._loss_tracker.update_state(unscaled_loss)
+            self._loss_tracker.update_state(
+                unscaled_loss, sample_weight=tree.flatten(x)[0].shape[0]
+            )
             logs = self.compute_metrics(x, y, y_pred, sample_weight)
 
         new_metrics_variables = []
         for ref_v in self.metrics_variables:
             new_v = scope.get_current_value(ref_v)
             if new_v is None:
                 new_v = ref_v.value
@@ -196,15 +221,15 @@
             optimizer_variables=None,
             metrics_variables=None,
         )
         return outputs, non_trainable_variables
 
     def make_train_function(self, force=False):
         if self.train_function is not None and not force:
-            return self.train_function
+            return
 
         def one_train_step(state, data):
             data = data[0]
             return self.train_step(state, data)
 
         def multi_train_steps(state, data):
             for single_step_data in data:
@@ -228,15 +253,15 @@
             self.train_function = compiled_train_step
 
         else:
             self.train_function = train_step
 
     def make_test_function(self, force=False):
         if self.test_function is not None and not force:
-            return self.test_function
+            return
 
         def one_test_step(state, data):
             data = data[0]
             return self.test_step(state, data)
 
         def multi_test_steps(state, data):
             for single_step_data in data:
```

### Comparing `keras-3.1.1/keras/src/backend/numpy/__init__.py` & `keras-3.2.0/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/core.py` & `keras-3.2.0/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/image.py` & `keras-3.2.0/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/linalg.py` & `keras-3.2.0/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/math.py` & `keras-3.2.0/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/nn.py` & `keras-3.2.0/keras/src/backend/numpy/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,15 +441,17 @@
             rhs_dilation=dilation_rate,
             dimension_numbers=dimension_numbers,
             transpose_kernel=True,
         )
     )
 
 
-def one_hot(x, num_classes, axis=-1, dtype="float32"):
+def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
     x = convert_to_tensor(x)
     input_shape = x.shape
 
     # Shrink the last dimension if the shape is (..., 1).
     if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
         input_shape = tuple(input_shape[:-1])
 
@@ -469,15 +471,17 @@
     # Then, move this new dimension to the right place (according to axis)
     if axis != -1:
         categorical = np.moveaxis(categorical, -1, axis)
 
     return categorical
 
 
-def multi_hot(x, num_classes, axis=-1, dtype="float32"):
+def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
     outputs = np.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
         axis=reduction_axis,
     )
     return outputs
```

### Comparing `keras-3.1.1/keras/src/backend/numpy/numpy.py` & `keras-3.2.0/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,17 @@
     dtype = dtypes.result_type(*dtypes_to_resolve)
     x = x.astype(dtype)
     if weights is not None:
         weights = weights.astype(dtype)
     return np.average(x, weights=weights, axis=axis)
 
 
-def bincount(x, weights=None, minlength=0):
+def bincount(x, weights=None, minlength=0, sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
     x = convert_to_tensor(x)
     dtypes_to_resolve = [x.dtype]
     if weights is not None:
         weights = convert_to_tensor(weights)
         dtypes_to_resolve.append(weights.dtype)
         dtype = dtypes.result_type(*dtypes_to_resolve)
     else:
@@ -1070,7 +1072,22 @@
     x2 = convert_to_tensor(x2, dtype)
     return np.floor_divide(x1, x2)
 
 
 def logical_xor(x1, x2):
     return np.logical_xor(x1, x2)
 
+
+def correlate(x1, x2, mode="valid"):
+    dtype = dtypes.result_type(
+        getattr(x1, "dtype", type(x1)),
+        getattr(x2, "dtype", type(x2)),
+    )
+    if dtype == "int64":
+        dtype = "float64"
+    elif dtype not in ["bfloat16", "float16", "float64"]:
+        dtype = "float32"
+
+    x1 = convert_to_tensor(x1, dtype)
+    x2 = convert_to_tensor(x2, dtype)
+    return np.correlate(x1, x2, mode)
+
```

### Comparing `keras-3.1.1/keras/src/backend/numpy/random.py` & `keras-3.2.0/keras/src/backend/numpy/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         random_numbers = np.append(random_numbers, valid)
 
     # Truncate the result array to the desired size and reshape it
     return random_numbers[:flat_shape].astype(dtype).reshape(shape)
 
 
 def dropout(inputs, rate, noise_shape=None, seed=None):
+    dtype = inputs.dtype
     seed = draw_seed(seed)
 
     keep_prob = 1.0 - rate
 
     # If noise_shape is not provided, use the shape of inputs
     if noise_shape is None:
         noise_shape = inputs.shape
@@ -81,15 +82,17 @@
             n if n is not None else inputs.shape[i]
             for i, n in enumerate(noise_shape)
         ]
 
     rng = np.random.default_rng(seed)
     mask = rng.uniform(size=noise_shape) < keep_prob
     mask = np.broadcast_to(mask, inputs.shape)
-    return np.where(mask, inputs / keep_prob, np.zeros_like(inputs))
+    return np.where(
+        mask, (inputs / keep_prob).astype(dtype), np.zeros_like(inputs)
+    )
 
 
 def shuffle(x, axis=0, seed=None):
     seed = draw_seed(seed)
     rng = np.random.default_rng(seed)
     return rng.permuted(x, axis=axis)
```

### Comparing `keras-3.1.1/keras/src/backend/numpy/rnn.py` & `keras-3.2.0/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/numpy/trainer.py` & `keras-3.2.0/keras/src/backend/numpy/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
             y_pred = self(x)
         loss = self.compute_loss(
             x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
         )
-        self._loss_tracker.update_state(loss)
+        self._loss_tracker.update_state(
+            loss, sample_weight=tree.flatten(x)[0].shape[0]
+        )
         return self.compute_metrics(x, y, y_pred, sample_weight=sample_weight)
 
     def predict_step(self, data):
         x, _, _ = data_adapter_utils.unpack_x_y_sample_weight(data)
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
```

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/__init__.py` & `keras-3.2.0/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/core.py` & `keras-3.2.0/keras/src/backend/tensorflow/core.py`

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

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/distribution_lib.py` & `keras-3.2.0/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/image.py` & `keras-3.2.0/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/layer.py` & `keras-3.2.0/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/linalg.py` & `keras-3.2.0/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/math.py` & `keras-3.2.0/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/nn.py` & `keras-3.2.0/keras/src/backend/tensorflow/nn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import warnings
 
 import tensorflow as tf
 
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
@@ -35,16 +36,16 @@
     return tf.math.softplus(x)
 
 
 def softsign(x):
     return tf.nn.softsign(x)
 
 
-def silu(x, beta=1.0):
-    return tf.nn.silu(x, beta=beta)
+def silu(x):
+    return tf.nn.silu(x)
 
 
 def log_sigmoid(x):
     return tf.math.log_sigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
@@ -440,27 +441,52 @@
         strides,
         padding=padding.upper(),
         data_format=tf_data_format,
         dilations=dilation_rate,
     )
 
 
-def one_hot(x, num_classes, axis=-1, dtype="float32"):
+def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     x = convert_to_tensor(x)
+    if dtype is None:
+        dtype = "float32"
+    if sparse:
+        # We don't use `tf.sparse.bincount`, it doesn't handle negative indices
+        # and only support rank 1 and 2 tensors (`one_hot` adds a dimension).
+        if axis < 0:
+            axis = axis + len(x.shape) + 1
+        values_count = math.prod(x.shape)
+        values = tf.reshape(x, (values_count,))
+        # We deal with negative inputs by having zeros in the output although
+        # it's useless. It makes shapes static.
+        values = tf.cast(tf.greater_equal(values, 0), dtype=dtype)
+        indices = [tf.range(dim) for dim in x.shape]
+        indices = tf.meshgrid(*indices, indexing="ij")
+        indices.insert(axis, tf.maximum(x, 0))  # Deal with negative indices
+        indices = [tf.reshape(a, (values_count, 1)) for a in indices]
+        indices = [tf.cast(a, tf.int64) for a in indices]
+        indices = tf.concat(indices, axis=1)
+        shape = list(x.shape)
+        shape.insert(axis, num_classes)
+        return tf.SparseTensor(indices, values, shape)
     return tf.one_hot(x, num_classes, axis=axis, dtype=dtype)
 
 
-def multi_hot(x, num_classes, axis=-1, dtype="float32"):
+def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = tf.reduce_max(
-        one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        axis=reduction_axis,
+    one_hot_outputs = one_hot(
+        cast(x, "int32"), num_classes, axis=axis, dtype=dtype, sparse=sparse
     )
-    return outputs
+    if sparse:
+        # We don't use `tf.sparse.bincount`, it doesn't handle negative indices.
+        return tf.sparse.reduce_max(
+            one_hot_outputs, axis=reduction_axis, output_is_sparse=True
+        )
+    return tf.reduce_max(one_hot_outputs, axis=reduction_axis)
 
 
 def _get_logits(output, from_logits, op_type, fn_name):
     """Retrieves logits tensor from maybe-softmax or maybe-sigmoid tensor."""
     output_ = output
     from_logits_ = from_logits
```

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/numpy.py` & `keras-3.2.0/keras/src/backend/tensorflow/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
 from keras.src.backend.tensorflow import sparse
+from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 from keras.src.utils import tree
 
 
 @sparse.elementwise_binary_union(tf.sparse.add)
 def add(x1, x2):
     if not isinstance(x1, (int, float)):
@@ -31,15 +32,15 @@
         getattr(x2, "dtype", type(x2)),
     )
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return tf.add(x1, x2)
 
 
-def bincount(x, weights=None, minlength=0):
+def bincount(x, weights=None, minlength=0, sparse=False):
     x = convert_to_tensor(x)
     dtypes_to_resolve = [x.dtype]
     if standardize_dtype(x.dtype) not in ["int32", "int64"]:
         x = tf.cast(x, tf.int32)
     if weights is not None:
         weights = convert_to_tensor(weights)
         dtypes_to_resolve.append(weights.dtype)
@@ -52,27 +53,32 @@
         ]:
             if "int" in standardize_dtype(weights.dtype):
                 weights = tf.cast(weights, tf.int32)
             else:
                 weights = tf.cast(weights, tf.float32)
     else:
         dtype = "int32"
-    if isinstance(x, tf.SparseTensor):
+    if sparse or isinstance(x, tf.SparseTensor):
         output = tf.sparse.bincount(
             x,
             weights=weights,
             minlength=minlength,
             axis=-1,
         )
-        output = tf.cast(output, dtype)
+        actual_length = output.shape[-1]
+        if actual_length is None:
+            actual_length = tf.shape(output)[-1]
+        output = cast(output, dtype)
         if x.shape.rank == 1:
-            output_shape = (minlength,)
+            output_shape = (actual_length,)
         else:
-            batch_size = tf.shape(output)[0]
-            output_shape = (batch_size, minlength)
+            batch_size = output.shape[0]
+            if batch_size is None:
+                batch_size = tf.shape(output)[0]
+            output_shape = (batch_size, actual_length)
         return tf.SparseTensor(
             indices=output.indices,
             values=output.values,
             dense_shape=output_shape,
         )
     return tf.cast(
         tf.math.bincount(x, weights=weights, minlength=minlength, axis=-1),
@@ -100,17 +106,22 @@
     subscripts = _normalize_einsum_subscripts(subscripts)
 
     def is_valid_for_custom_ops(subscripts, *operands):
         # Check that `subscripts` is supported and the shape of operands is not
         # `None`.
         if subscripts in [
             "a,b->ab",
+            "ab,b->a",
             "ab,bc->ac",
+            "ab,cb->ac",
             "abc,cd->abd",
+            "abc,dc->abd",
+            "abcd,abde->abce",
             "abcd,abed->abce",
+            "abcd,acbe->adbe",
             "abcd,adbe->acbe",
             "abcd,aecd->acbe",
             "abcd,aecd->aceb",
         ]:
             # These subscripts don't require the shape information
             return True
         elif subscripts == "abc,cde->abde":
@@ -123,21 +134,42 @@
         elif subscripts == "abc,dce->abde":
             _, b1, c1 = operands[0].shape
             d2, c2, e2 = operands[1].shape
             b, c, d, e = b1, c1 or c2, d2, e2
             if None in (b, c, d, e):
                 return False
             return True
+        elif subscripts == "abc,dec->abde":
+            _, b1, c1 = operands[0].shape
+            d2, e2, c2 = operands[1].shape
+            b, c, d, e = b1, c1 or c2, d2, e2
+            if None in (b, c, d, e):
+                return False
+            return True
         elif subscripts == "abcd,cde->abe":
             _, b1, c1, d1 = operands[0].shape
             c2, d2, e2 = operands[1].shape
             b, c, d, e = b1, c1 or c2, d1 or d2, e2
             if None in (b, c, d, e):
                 return False
             return True
+        elif subscripts == "abcd,ced->abe":
+            _, b1, c1, d1 = operands[0].shape
+            c2, e2, d2 = operands[1].shape
+            b, c, d, e = b1, c1 or c2, d1 or d2, e2
+            if None in (b, c, d, e):
+                return False
+            return True
+        elif subscripts == "abcd,ecd->abe":
+            _, b1, c1, d1 = operands[0].shape
+            e2, c2, d2 = operands[1].shape
+            b, c, d, e = b1, c1 or c2, d1 or d2, e2
+            if None in (b, c, d, e):
+                return False
+            return True
         elif subscripts == "abcde,aebf->adbcf":
             _, b1, c1, d1, e1 = operands[0].shape
             _, e2, b2, f2 = operands[1].shape
             b, c, d, e, f = b1 or b2, c1, d1, e1 or e2, f2
             if None in (b, c, d, e, f):
                 return False
             return True
@@ -156,36 +188,61 @@
         # Replace tf.einsum with custom ops to utilize hardware-accelerated
         # matmul
         x, y = operands[0], operands[1]
         if subscripts == "a,b->ab":
             x = tf.expand_dims(x, axis=-1)
             y = tf.expand_dims(y, axis=0)
             return tf.matmul(x, y, output_type=output_type)
+        elif subscripts == "ab,b->a":
+            y = tf.expand_dims(y, axis=-1)
+            result = tf.matmul(x, y, output_type=output_type)
+            return tf.squeeze(result, axis=-1)
         elif subscripts == "ab,bc->ac":
             return tf.matmul(x, y, output_type=output_type)
+        elif subscripts == "ab,cb->ac":
+            y = tf.transpose(y, [1, 0])
+            return tf.matmul(x, y, output_type=output_type)
         elif subscripts == "abc,cd->abd":
             return tf.matmul(x, y, output_type=output_type)
         elif subscripts == "abc,cde->abde":
             _, b1, c1 = x.shape
             c2, d2, e2 = y.shape
             b, c, d, e = b1, c1 or c2, d2, e2
             y = tf.reshape(y, [c, -1])
             result = tf.matmul(x, y, output_type=output_type)
             return tf.reshape(result, [-1, b, d, e])
+        elif subscripts == "abc,dc->abd":
+            y = tf.transpose(y, [1, 0])
+            return tf.matmul(x, y, output_type=output_type)
         elif subscripts == "abc,dce->abde":
             _, b1, c1 = x.shape
             d2, c2, e2 = y.shape
             b, c, d, e = b1, c1 or c2, d2, e2
             y = tf.transpose(y, [1, 0, 2])  # cde
             y = tf.reshape(y, [c, -1])
             result = tf.matmul(x, y, output_type=output_type)
             return tf.reshape(result, [-1, b, d, e])
+        elif subscripts == "abc,dec->abde":
+            _, b1, c1 = x.shape
+            d2, e2, c2 = y.shape
+            b, c, d, e = b1, c1 or c2, d2, e2
+            y = tf.transpose(y, [2, 0, 1])  # cde
+            y = tf.reshape(y, [c, -1])
+            result = tf.matmul(x, y, output_type=output_type)
+            return tf.reshape(result, [-1, b, d, e])
+        elif subscripts == "abcd,abde->abce":
+            return tf.matmul(x, y, output_type=output_type)
         elif subscripts == "abcd,abed->abce":
             y = tf.transpose(y, [0, 1, 3, 2])
             return tf.matmul(x, y, output_type=output_type)
+        elif subscripts == "abcd,acbe->adbe":
+            x = tf.transpose(x, [0, 1, 3, 2])
+            y = tf.transpose(y, [0, 2, 1, 3])
+            result = tf.matmul(x, y, output_type=output_type)
+            return tf.transpose(result, [0, 2, 1, 3])
         elif subscripts == "abcd,adbe->acbe":
             y = tf.transpose(y, [0, 2, 1, 3])  # abde
             result = tf.matmul(x, y, output_type=output_type)  # abce
             return tf.transpose(result, [0, 2, 1, 3])
         elif subscripts == "abcd,aecd->acbe":
             x = tf.transpose(x, [0, 2, 1, 3])  # acbd
             y = tf.transpose(y, [0, 2, 3, 1])  # acde
@@ -198,14 +255,30 @@
         elif subscripts == "abcd,cde->abe":
             _, b1, c1, d1 = x.shape
             c2, d2, e2 = y.shape
             b, c, d, e = b1, c1 or c2, d1 or d2, e2
             x = tf.reshape(x, [-1, b, c * d])
             y = tf.reshape(y, [-1, e])
             return tf.matmul(x, y, output_type=output_type)
+        elif subscripts == "abcd,ced->abe":
+            _, b1, c1, d1 = x.shape
+            c2, e2, d2 = y.shape
+            b, c, d, e = b1, c1 or c2, d1 or d2, e2
+            x = tf.reshape(x, [-1, b, c * d])
+            y = tf.transpose(y, [0, 2, 1])
+            y = tf.reshape(y, [-1, e])
+            return tf.matmul(x, y, output_type=output_type)
+        elif subscripts == "abcd,ecd->abe":
+            _, b1, c1, d1 = x.shape
+            e2, c2, d2 = y.shape
+            b, c, d, e = b1, c1 or c2, d1 or d2, e2
+            x = tf.reshape(x, [-1, b, c * d])
+            y = tf.transpose(y, [1, 2, 0])
+            y = tf.reshape(y, [-1, e])
+            return tf.matmul(x, y, output_type=output_type)
         elif subscripts == "abcde,aebf->adbcf":
             _, b1, c1, d1, e1 = x.shape
             _, e2, b2, f2 = y.shape
             b, c, d, e, f = b1 or b2, c1, d1, e1 or e2, f2
             x = tf.reshape(x, [-1, b, c * d, e])  # ab(cd)e
             y = tf.transpose(y, [0, 2, 1, 3])  # abef
             result = tf.matmul(x, y, output_type=output_type)  # ab(cd)f
@@ -875,19 +948,19 @@
     # bins must be float type
     bins = tree.map_structure(lambda x: float(x), bins)
 
     # TODO: tf.raw_ops.Bucketize doesn't support bool, bfloat16, float16, int8
     # int16, uint8, uint16, uint32
     ori_dtype = standardize_dtype(x.dtype)
     if ori_dtype in ("bool", "int8", "int16", "uint8", "uint16"):
-        x = tf.cast(x, "int32")
+        x = cast(x, "int32")
     elif ori_dtype == "uint32":
-        x = tf.cast(x, "int64")
+        x = cast(x, "int64")
     elif ori_dtype in ("bfloat16", "float16"):
-        x = tf.cast(x, "float32")
+        x = cast(x, "float32")
 
     if isinstance(x, tf.RaggedTensor):
         return tf.ragged.map_flat_values(
             lambda y: tf.raw_ops.Bucketize(input=y, boundaries=bins), x
         )
     elif isinstance(x, tf.SparseTensor):
         output = tf.SparseTensor(
@@ -1961,15 +2034,19 @@
     x = convert_to_tensor(x)
     dtype = standardize_dtype(x.dtype)
     # follow jax's rule
     if dtype in ("bool", "int8", "int16"):
         dtype = "int32"
     elif dtype in ("uint8", "uint16"):
         dtype = "uint32"
-    x = tf.cast(x, dtype)
+    x = cast(x, dtype)
+    if isinstance(x, tf.SparseTensor):
+        return tf.sparse.reduce_sum(
+            x, axis=axis, keepdims=keepdims, output_is_sparse=True
+        )
     return tf.reduce_sum(x, axis=axis, keepdims=keepdims)
 
 
 def eye(N, M=None, k=0, dtype=None):
     dtype = dtype or config.floatx()
     return tfnp.eye(N, M=M, k=k, dtype=dtype)
 
@@ -1989,7 +2066,49 @@
 
 
 def logical_xor(x1, x2):
     x1 = tf.cast(x1, "bool")
     x2 = tf.cast(x2, "bool")
     return tf.math.logical_xor(x1, x2)
 
+
+def correlate(x1, x2, mode="valid"):
+    x1 = convert_to_tensor(x1)
+    x2 = convert_to_tensor(x2)
+
+    dtype = dtypes.result_type(
+        getattr(x1, "dtype", type(x1)),
+        getattr(x2, "dtype", type(x2)),
+    )
+    if dtype == tf.int64:
+        dtype = tf.float64
+    elif dtype not in [tf.bfloat16, tf.float16, tf.float64]:
+        dtype = tf.float32
+
+    x1 = tf.cast(x1, dtype)
+    x2 = tf.cast(x2, dtype)
+
+    x1_len, x2_len = int(x1.shape[0]), int(x2.shape[0])
+
+    if mode == "full":
+        full_len = x1_len + x2_len - 1
+
+        x1_pad = (full_len - x1_len) / 2
+        x2_pad = (full_len - x2_len) / 2
+
+        x1 = tf.pad(
+            x1, paddings=[[tf.math.floor(x1_pad), tf.math.ceil(x1_pad)]]
+        )
+        x2 = tf.pad(
+            x2, paddings=[[tf.math.floor(x2_pad), tf.math.ceil(x2_pad)]]
+        )
+
+        x1 = tf.reshape(x1, (1, full_len, 1))
+        x2 = tf.reshape(x2, (full_len, 1, 1))
+
+        return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding="SAME"))
+
+    x1 = tf.reshape(x1, (1, x1_len, 1))
+    x2 = tf.reshape(x2, (x2_len, 1, 1))
+
+    return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
+
```

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/optimizer.py` & `keras-3.2.0/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/random.py` & `keras-3.2.0/keras/src/backend/tensorflow/random.py`

 * *Files 25% similar despite different names*

```diff
@@ -95,33 +95,46 @@
     x = tfnp.swapaxes(x, axis1=0, axis2=axis)
     return x
 
 
 def gamma(shape, alpha, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
-    return tf.random.stateless_gamma(
-        shape,
-        alpha=alpha,
-        dtype=dtype,
-        seed=seed,
+    # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    return tf.cast(
+        tf.random.stateless_gamma(
+            shape,
+            alpha=alpha,
+            dtype=intemediate_dtype,
+            seed=seed,
+        ),
+        dtype,
     )
 
 
 def binomial(shape, counts, probabilities, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
-    sample = tf.random.stateless_binomial(
-        shape=shape,
-        seed=seed,
-        counts=counts,
-        probs=probabilities,
-        output_dtype=dtype,
+    # TODO: `tf.random.stateless_binomial` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    return tf.cast(
+        tf.random.stateless_binomial(
+            shape=shape,
+            seed=seed,
+            counts=counts,
+            probs=probabilities,
+            output_dtype=intemediate_dtype,
+        ),
+        dtype,
     )
-    return sample
 
 
 def beta(shape, alpha, beta, dtype=None, seed=None):
     dtype = dtype or floatx()
     # since tensorflow doesn't offer a beta distribution function
     # so we'll use the formula U(a,b) = (X(a) / (X(a) + Y(b)),
     # where U(a,b) is a beta-distributed random variable with
@@ -134,32 +147,42 @@
     # due to the usage of same seed.
     seed_1 = tf_draw_seed(seed)
     # The choice of 12 is totally arbitrary, as we're
     # incrementing the first drawn seed by a CONSTANT to
     # ensure deterministic results.
     seed_2 = seed_1 + 12
 
-    alpha = tf.convert_to_tensor(alpha, dtype=dtype)
-    beta = tf.convert_to_tensor(beta, dtype=dtype)
+    # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
+    intemediate_dtype = dtype
+    if standardize_dtype(dtype) == "bfloat16":
+        intemediate_dtype = "float32"
+    alpha = tf.convert_to_tensor(alpha, dtype=intemediate_dtype)
+    beta = tf.convert_to_tensor(beta, dtype=intemediate_dtype)
 
     # tensorflow's tf.random.stateless_gamma has a bit of unconventional
     # implementation of the stateless_gamma function where it checks the
     # broadcastability of alpha's shape with ONLY the RIGHTMOST dimension of
     # the specified output shape instead of considering the whole.
     # Consequently, it then results in errors for perfectly broadcastable shapes
     # such as for output shape of (2, 3) and alpha shape of (1, 3)
     # So to resolve this, we explicitly broadcast alpha and beta to shape before
     # passing them to the stateless_gamma function.
     if tf.rank(alpha) > 1:
         alpha = tf.broadcast_to(alpha, shape)
     if tf.rank(beta) > 1:
         beta = tf.broadcast_to(beta, shape)
 
-    gamma_a = tf.random.stateless_gamma(
-        shape=shape, seed=seed_1, alpha=alpha, dtype=dtype
+    gamma_a = tf.cast(
+        tf.random.stateless_gamma(
+            shape=shape, seed=seed_1, alpha=alpha, dtype=intemediate_dtype
+        ),
+        dtype,
     )
-    gamma_b = tf.random.stateless_gamma(
-        shape=shape, seed=seed_2, alpha=beta, dtype=dtype
+    gamma_b = tf.cast(
+        tf.random.stateless_gamma(
+            shape=shape, seed=seed_2, alpha=beta, dtype=intemediate_dtype
+        ),
+        dtype,
     )
     sample = gamma_a / (gamma_a + gamma_b)
     return sample
```

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/rnn.py` & `keras-3.2.0/keras/src/backend/tensorflow/rnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,15 +464,15 @@
     cudnn_supported = cudnn_ok(
         activation,
         recurrent_activation,
         unroll,
         use_bias=bias is not None,
         reset_after=reset_after,
     )
-    if not cudnn_supported or mask is not None:
+    if not cudnn_supported:
         raise NotImplementedError
 
     from keras.src.backend.tensorflow import Variable
 
     if isinstance(kernel, Variable):
         kernel = kernel.value
     if isinstance(recurrent_kernel, Variable):
@@ -534,58 +534,47 @@
         and recurrent_activation
         in (activations.sigmoid, tf.sigmoid, ops.sigmoid)
         and not unroll
         and use_bias
     )
 
 
-def _is_sequence_right_padded(mask):
-    """Check the mask tensor and see if it right padded.
-
-    For cuDNN kernel, it uses the sequence length param to skip the tailing
-    timestep. If the data is left padded, or not a strict right padding (has
-    masked value in the middle of the sequence), then cuDNN kernel won't be work
-    properly in those cases.
-
-    Left padded data: [[False, False, True, True, True]].
-    Right padded data: [[True, True, True, False, False]].
-    Mixture of mask/unmasked data: [[True, False, True, False, False]].
-
-    Note that for the mixed data example above, the actually data RNN should see
-    are those 2 Trues (index 0 and 2), the index 1 False should be ignored and
-    not pollute the internal states.
-
-    Args:
-      mask: the Boolean tensor with shape [batch, timestep]
-
-    Returns:
-      boolean scalar tensor, whether the mask is strictly right padded.
-    """
-    max_seq_length = tf.shape(mask)[1]
-    count_of_true = tf.reduce_sum(tf.cast(mask, tf.int32), axis=1)
-    right_padded_mask = tf.sequence_mask(count_of_true, maxlen=max_seq_length)
-    return tf.reduce_all(
-        tf.equal(
-            tf.cast(mask, dtype="bool"),
-            tf.cast(right_padded_mask, dtype="bool"),
-        )
-    )
-
-
 def _has_fully_masked_sequence(mask):
     # Cudnn kernel will error out if the input sequence contains any
     # fully masked data. We walk around this issue by rerouting the computation
     # to standard kernel, until the issue on cudnn side has been fixed.  For a
     # fully masked sequence, it will contain all Falses. To make it easy to
     # check, we inverse the boolean, check if any of the sequence has all True.
     return tf.reduce_any(
         tf.reduce_all(tf.logical_not(tf.cast(mask, dtype="bool")), axis=1)
     )
 
 
+def _assert_valid_mask(mask):
+    valid = tf.logical_and(
+        tf.logical_not(_has_fully_masked_sequence(mask)),
+        _is_sequence_right_padded(mask),
+    )
+    tf.Assert(
+        valid,
+        [
+            (
+                "You are passing a RNN mask that does not correspond to "
+                "right-padded sequences, while using cuDNN, which is not "
+                "supported. With cuDNN, RNN masks can only be used for "
+                "right-padding, e.g. `[[True, True, False, False]]` would "
+                "be a valid mask, but any mask that isn't just contiguous "
+                "`True`'s on the left and contiguous `False`'s on the right "
+                "would be invalid. You can pass `use_cudnn=False` to your "
+                "RNN layer to stop using cuDNN (this may be slower)."
+            )
+        ],
+    )
+
+
 def _standardize_cudnn_weights(weights, biases, shape, transpose_weights=False):
     """Utility function convert variable to cuDNN compatible parameter.
 
     Note that Keras weights for kernels are different from the cuDNN format.
     Eg.:
 
     ```
@@ -611,33 +600,67 @@
         return tf.transpose(w) if transpose_weights else w
 
     weights = [tf.reshape(convert(x), shape) for x in weights]
     biases = [tf.reshape(x, shape) for x in biases]
     return tf.concat(weights + biases, axis=0)
 
 
+def _is_sequence_right_padded(mask):
+    """Check the mask tensor and see if it right padded.
+
+    cuDNN uses the sequence length param to skip the tailing
+    timestep. If the data is left padded, or not a strict right padding (has
+    masked value in the middle of the sequence), then cuDNN won't work
+    properly in those cases.
+
+    Left padded data: [[False, False, True, True, True]].
+    Right padded data: [[True, True, True, False, False]].
+    Mixture of mask/unmasked data: [[True, False, True, False, False]].
+
+    Note that for the mixed data example above, the actually data RNN should see
+    are those 2 Trues (index 0 and 2), the index 1 False should be ignored and
+    not pollute the internal states.
+
+    Args:
+        mask: the Boolean tensor with shape [batch, timestep]
+
+    Returns:
+        boolean scalar tensor, whether the mask is strictly right padded.
+    """
+    max_seq_length = tf.shape(mask)[1]
+    count_of_true = tf.reduce_sum(tf.cast(mask, tf.int32), axis=1)
+    right_padded_mask = tf.sequence_mask(count_of_true, maxlen=max_seq_length)
+    return tf.reduce_all(
+        tf.equal(
+            tf.cast(mask, dtype="bool"),
+            tf.cast(right_padded_mask, dtype="bool"),
+        )
+    )
+
+
 def _compute_sequence_length_from_mask(mask, time_major):
     """Calculate the sequence length tensor (1-D) based on the masking tensor.
 
     The masking tensor is a 2D boolean tensor with shape [batch, timestep]. For
     any timestep that should be masked, the corresponding field will be False.
     Consider the following example:
       a = [[True, True, False, False],
            [True, True, True, False]]
     It is a (2, 4) tensor, and the corresponding sequence length result should
     be 1D tensor with value [2, 3]. Note that the masking tensor must be right
     padded that could be checked by, e.g., `is_sequence_right_padded()`.
 
     Args:
-      mask: Boolean tensor with shape [batch, timestep] or [timestep, batch] if
-        time_major=True.
-      time_major: Boolean, which indicates whether the mask is time major or
-        batch major.
+        mask: Boolean tensor with shape [batch, timestep] or [timestep, batch]
+            if time_major=True.
+        time_major: Boolean, which indicates whether the mask is time major or
+            batch major.
+
     Returns:
-      sequence_length: 1D int32 tensor.
+        sequence_length: 1D int32 tensor.
     """
     timestep_index = 0 if time_major else 1
     return tf.reduce_sum(tf.cast(mask, tf.int32), axis=timestep_index)
 
 
 def _is_gpu_available():
     return bool(tf.config.list_logical_devices("GPU"))
@@ -652,23 +675,31 @@
     mask,
     time_major,
     go_backwards,
     return_sequences,
 ):
     """GRU with cuDNN implementation which is only available for GPU."""
     if mask is not None:
+        _assert_valid_mask(mask)
         sequence_lengths = _compute_sequence_length_from_mask(mask, time_major)
     else:
-        sequence_lengths = None
+        if time_major:
+            batch_dim = tf.shape(inputs)[1]
+            max_sequence_length = tf.shape(inputs)[0]
+        else:
+            batch_dim = tf.shape(inputs)[0]
+            max_sequence_length = tf.shape(inputs)[1]
+        sequence_lengths = tf.fill([batch_dim], max_sequence_length)
 
     if not time_major and sequence_lengths is None:
         inputs = tf.transpose(inputs, perm=(1, 0, 2))
         seq_axis, batch_axis = (0, 1)
     else:
         seq_axis, batch_axis = (0, 1) if time_major else (1, 0)
+
     # For init_h, cuDNN expects one more dim of num_layers before or after batch
     # dim for time major or batch major inputs respectively
     init_h = tf.expand_dims(initial_state, axis=seq_axis)
 
     weights = tf.split(kernel, 3, axis=1)
     weights += tf.split(recurrent_kernel, 3, axis=1)
     # Note that the bias was initialized as shape (2, 3 * units), flatten it to
@@ -691,57 +722,44 @@
     params = _standardize_cudnn_weights(
         weights=weights,
         biases=bias,
         shape=tf.constant([-1]),
         transpose_weights=True,
     )
 
-    if sequence_lengths is not None:
-        if go_backwards:
-            # Three reversals are required. E.g.,
-            # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
-            # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
-            # output_from_cudnn = [6, 5, 4, 0, 0]
-            # expected_output = [0, 0, 6, 5 ,4]
-            inputs = tf.reverse_sequence(
-                inputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-        outputs, h, _, _, _ = tf.raw_ops.CudnnRNNV3(
-            input=inputs,
-            input_h=init_h,
-            input_c=0,
-            params=params,
-            is_training=True,
-            rnn_mode="gru",
-            sequence_lengths=sequence_lengths,
-            time_major=time_major,
+    if go_backwards:
+        # Three reversals are required. E.g.,
+        # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
+        # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
+        # output_from_cudnn = [6, 5, 4, 0, 0]
+        # expected_output = [0, 0, 6, 5 ,4]
+        inputs = tf.reverse_sequence(
+            inputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
-        if go_backwards:
-            outputs = tf.reverse_sequence(
-                outputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-            outputs = tf.reverse(outputs, axis=[seq_axis])
-    else:
-        if go_backwards:
-            # Reverse axis 0 since the input is already convert to time major.
-            inputs = tf.reverse(inputs, axis=[0])
-        outputs, h, _, _ = tf.raw_ops.CudnnRNN(
-            input=inputs,
-            input_h=init_h,
-            input_c=0,
-            params=params,
-            is_training=True,
-            rnn_mode="gru",
+    outputs, h, _, _, _ = tf.raw_ops.CudnnRNNV3(
+        input=inputs,
+        input_h=init_h,
+        input_c=0,
+        params=params,
+        is_training=True,
+        rnn_mode="gru",
+        sequence_lengths=sequence_lengths,
+        time_major=time_major,
+    )
+    if go_backwards:
+        outputs = tf.reverse_sequence(
+            outputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
+        outputs = tf.reverse(outputs, axis=[seq_axis])
 
     last_output = outputs[-1]
     if not time_major and sequence_lengths is None and return_sequences:
         outputs = tf.transpose(outputs, perm=[1, 0, 2])
     state = tf.squeeze(h, axis=seq_axis)
 
     # In the case of variable length input, the cudnn kernel will fill zeros for
@@ -803,15 +821,15 @@
     go_backwards=False,
     unroll=False,
     time_major=False,
 ):
     cudnn_supported = cudnn_ok(
         activation, recurrent_activation, unroll, use_bias=bias is not None
     )
-    if not cudnn_supported or mask is not None:
+    if not cudnn_supported:
         raise NotImplementedError
 
     from keras.src.backend.tensorflow import Variable
 
     if isinstance(kernel, Variable):
         kernel = kernel.value
     if isinstance(recurrent_kernel, Variable):
@@ -849,17 +867,24 @@
     bias,
     mask,
     time_major,
     go_backwards,
     return_sequences,
 ):
     if mask is not None:
+        _assert_valid_mask(mask)
         sequence_lengths = _compute_sequence_length_from_mask(mask, time_major)
     else:
-        sequence_lengths = None
+        if time_major:
+            batch_dim = tf.shape(inputs)[1]
+            max_sequence_length = tf.shape(inputs)[0]
+        else:
+            batch_dim = tf.shape(inputs)[0]
+            max_sequence_length = tf.shape(inputs)[1]
+        sequence_lengths = tf.fill([batch_dim], max_sequence_length)
 
     if not time_major and sequence_lengths is None:
         inputs = tf.transpose(inputs, perm=(1, 0, 2))
         seq_axis, batch_axis = (0, 1)
     else:
         seq_axis, batch_axis = (0, 1) if time_major else (1, 0)
     # For init_h and init_c, cuDNN expects one more dim of num_layers before or
@@ -889,60 +914,44 @@
     params = _standardize_cudnn_weights(
         weights=weights,
         biases=tf.split(full_bias, 8),
         shape=tf.constant([-1]),
         transpose_weights=True,
     )
 
-    if sequence_lengths is not None:
-        if go_backwards:
-            # Three reversals are required. E.g.,
-            # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
-            # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
-            # output_from_cudnn = [6, 5, 4, 0, 0]
-            # expected_output = [0, 0, 6, 5 ,4]
-            inputs = tf.reverse_sequence(
-                inputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-        outputs, h, c, _, _ = tf.raw_ops.CudnnRNNV3(
-            input=inputs,
-            input_h=init_h,
-            input_c=init_c,
-            params=params,
-            is_training=True,
-            rnn_mode="lstm",
-            sequence_lengths=sequence_lengths,
-            time_major=time_major,
+    if go_backwards:
+        # Three reversals are required. E.g.,
+        # normal input = [1, 2, 3, 0, 0]  # where 0 need to be masked
+        # reversed_input_to_cudnn = [3, 2, 1, 0, 0]
+        # output_from_cudnn = [6, 5, 4, 0, 0]
+        # expected_output = [0, 0, 6, 5 ,4]
+        inputs = tf.reverse_sequence(
+            inputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
-        if go_backwards:
-            outputs = tf.reverse_sequence(
-                outputs,
-                sequence_lengths,
-                seq_axis=seq_axis,
-                batch_axis=batch_axis,
-            )
-            outputs = tf.reverse(outputs, axis=[seq_axis])
-    else:
-        # # Fill the array with shape [batch] with value of max timesteps.
-        # sequence_length = array_ops.fill([array_ops.shape(inputs)[1]],
-        #                                  array_ops.shape(inputs)[0])
-        if go_backwards:
-            # Reverse axis 0 since the input is already convert to time major.
-            inputs = tf.reverse(inputs, axis=[0])
-        outputs, h, c, _ = tf.raw_ops.CudnnRNN(
-            input=inputs,
-            input_h=init_h,
-            input_c=init_c,
-            params=params,
-            is_training=True,
-            rnn_mode="lstm",
+    outputs, h, c, _, _ = tf.raw_ops.CudnnRNNV3(
+        input=inputs,
+        input_h=init_h,
+        input_c=init_c,
+        params=params,
+        is_training=True,
+        rnn_mode="lstm",
+        sequence_lengths=sequence_lengths,
+        time_major=time_major,
+    )
+    if go_backwards:
+        outputs = tf.reverse_sequence(
+            outputs,
+            sequence_lengths,
+            seq_axis=seq_axis,
+            batch_axis=batch_axis,
         )
+        outputs = tf.reverse(outputs, axis=[seq_axis])
 
     last_output = outputs[-1]
     if not time_major and sequence_lengths is None and return_sequences:
         outputs = tf.transpose(outputs, perm=[1, 0, 2])
     h = tf.squeeze(h, axis=seq_axis)
     c = tf.squeeze(c, axis=seq_axis)
```

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/sparse.py` & `keras-3.2.0/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/trackable.py` & `keras-3.2.0/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/tensorflow/trainer.py` & `keras-3.2.0/keras/src/backend/tensorflow/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,17 @@
             if self._call_has_training_arg:
                 y_pred = self(x, training=True)
             else:
                 y_pred = self(x)
             loss = self.compute_loss(
                 x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
             )
-            self._loss_tracker.update_state(loss)
+            self._loss_tracker.update_state(
+                loss, sample_weight=tf.shape(tree.flatten(x)[0])[0]
+            )
             if self.optimizer is not None:
                 loss = self.optimizer.scale_loss(loss)
 
         # Compute gradients
         if self.trainable_weights:
             trainable_weights = self.trainable_weights
             gradients = tape.gradient(loss, trainable_weights)
@@ -81,15 +83,17 @@
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
             y_pred = self(x)
         loss = self.compute_loss(
             x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
         )
-        self._loss_tracker.update_state(loss)
+        self._loss_tracker.update_state(
+            loss, sample_weight=tf.shape(tree.flatten(x)[0])[0]
+        )
         return self.compute_metrics(x, y, y_pred, sample_weight=sample_weight)
 
     def predict_step(self, data):
         x, _, _ = data_adapter_utils.unpack_x_y_sample_weight(data)
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
```

### Comparing `keras-3.1.1/keras/src/backend/torch/__init__.py` & `keras-3.2.0/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/core.py` & `keras-3.2.0/keras/src/backend/torch/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     "uint32": torch.int64,  # TODO: Torch doesn't have `uint32` dtype.
     "int8": torch.int8,
     "int16": torch.int16,
     "int32": torch.int32,
     "int64": torch.int64,
     "bfloat16": torch.bfloat16,
     "bool": torch.bool,
+    "float8_e4m3fn": torch.float8_e4m3fn,
+    "float8_e5m2": torch.float8_e5m2,
 }
 
 
 @contextlib.contextmanager
 def device_scope(device_name):
     previous_device = global_state.get_global_attribute("torch_device", None)
     current_device = _parse_device_input(device_name)
@@ -432,13 +434,60 @@
     return variable.detach()
 
 
 def unstack(x, num=None, axis=0):
     return x.unbind(axis)
 
 
-def custom_gradient(fun):
-    # TODO: Support this function
-    raise NotImplementedError(
-        "`custom_gradient` is not supported with torch backend"
-    )
+class custom_gradient:
+    """Decorator for custom gradients.
+
+    Args:
+        forward_fn: Forward pass function.
+    """
+
+    def __init__(self, forward_fn):
+        self.forward_fn = forward_fn
+
+    def __call__(self, *args, **kwargs):
+        return CustomGradientFunction.apply(self.forward_fn, *args, **kwargs)
+
+
+class CustomGradientFunction(torch.autograd.Function):
+    """Enables custom forward & backward passes for gradient computation."""
+
+    @staticmethod
+    def forward(ctx, forward_fn, *args, **kwargs):
+        """Forward pass computation specification.
+
+        Args:
+            ctx: Context object.
+            forward_fn: Function to compute forward pass.
+            *args: Arguments for the forward pass.
+            **kwargs: Keyword arguments for the forward pass.
+        """
+        ctx.forward_fn = forward_fn
+        ctx.save_for_backward(*args)
+        try:
+            output, ctx.grad_fn = forward_fn(*args, **kwargs)
+        except:
+            output = forward_fn(*args, **kwargs)
+            ctx.grad_fn = lambda *args, **kwargs: torch.full((), float("nan"))
+        return output
+
+    @staticmethod
+    def backward(ctx, grad_output):
+        """Backward pass computation specification.
+
+        Args:
+            ctx: Context object.
+            grad_output: Gradient with respect to the output.
+        """
+        args = ctx.saved_tensors
+        grad_fn = ctx.grad_fn
+        if grad_fn is None:
+            raise ValueError("grad_fn must be provided for custom gradient")
+        grads = grad_fn(*args, upstream=grad_output)
+        if not isinstance(grads, tuple):
+            grads = (grads,)
+        return (None,) + grads
```

### Comparing `keras-3.1.1/keras/src/backend/torch/image.py` & `keras-3.2.0/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/layer.py` & `keras-3.2.0/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/linalg.py` & `keras-3.2.0/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/math.py` & `keras-3.2.0/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/nn.py` & `keras-3.2.0/keras/src/backend/torch/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
 
 def softsign(x):
     x = convert_to_tensor(x)
     return tnn.softsign(x)
 
 
-def silu(x, beta=1.0):
+def silu(x):
     x = convert_to_tensor(x)
-    return x * sigmoid(beta * x)
+    return tnn.silu(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
     return tnn.logsigmoid(x)
 
 
@@ -548,15 +548,17 @@
             f"shape: {inputs.shape}."
         )
     if data_format == "channels_last":
         outputs = _transpose_spatial_outputs(outputs)
     return outputs
 
 
-def one_hot(x, num_classes, axis=-1, dtype="float32"):
+def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
     # Axis is the output axis. By default, PyTorch, outputs to last axis.
     # If axis is not last, change output to axis and shift remaining elements.
     x = convert_to_tensor(x, dtype=torch.long)
 
     # Torch one_hot does not natively handle negative values, so we add some
     # manual handling for negatives in the input to one_hot by using max(x, 0).
     # The output will have some invalid results, so we set them back to 0 using
@@ -571,15 +573,17 @@
         # Shift remaining axes with offset by 1 since output moved to `axis`.
         for ax in range(axis + 1, dims):
             new_axes_order[ax] -= 1
         output = output.permute(new_axes_order)
     return output
 
 
-def multi_hot(x, num_classes, axis=-1, dtype="float32"):
+def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
     outputs = torch.amax(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
         dim=reduction_axis,
     )
     return outputs
```

### Comparing `keras-3.1.1/keras/src/backend/torch/numpy.py` & `keras-3.2.0/keras/src/backend/torch/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,17 @@
     if weights is not None:
         return torch.sum(torch.mul(x, weights), dim=axis) / torch.sum(
             weights, dim=-1
         )
     return torch.mean(x, axis)
 
 
-def bincount(x, weights=None, minlength=0):
+def bincount(x, weights=None, minlength=0, sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     dtypes_to_resolve = [x.dtype]
     if weights is not None:
         weights = convert_to_tensor(weights)
         dtypes_to_resolve.append(weights.dtype)
         dtype = dtypes.result_type(*dtypes_to_resolve)
     else:
@@ -1515,7 +1517,54 @@
     return cast(torch.floor_divide(x1, x2), dtype)
 
 
 def logical_xor(x1, x2):
     x1, x2 = convert_to_tensor(x1), convert_to_tensor(x2)
     return torch.logical_xor(x1, x2)
 
+
+def correlate(x1, x2, mode="valid"):
+    x1 = convert_to_tensor(x1)
+    x2 = convert_to_tensor(x2)
+
+    dtype = dtypes.result_type(
+        getattr(x1, "dtype", type(x1)),
+        getattr(x2, "dtype", type(x2)),
+    )
+    if dtype == "int64":
+        dtype = "float64"
+    elif dtype not in ["bfloat16", "float16", "float64"]:
+        dtype = "float32"
+
+    x1 = cast(x1, dtype)
+    x2 = cast(x2, dtype)
+
+    x1_len, x2_len = x1.size(0), x2.size(0)
+
+    if x1.shape[:-1] != x2.shape[:-1]:
+        new_shape = [max(i, j) for i, j in zip(x1.shape[:-1], x2.shape[:-1])]
+        x1 = torch.broadcast_to(x1, new_shape + [x1.shape[-1]])
+        x2 = torch.broadcast_to(x2, new_shape + [x2.shape[-1]])
+
+    num_signals = torch.tensor(x1.shape[:-1]).prod()
+    x1 = torch.reshape(x1, (int(num_signals), x1.size(-1)))
+    x2 = torch.reshape(x2, (int(num_signals), x2.size(-1)))
+
+    output = torch.nn.functional.conv1d(
+        x1, x2.unsqueeze(1), groups=x1.size(0), padding=x2.size(-1) - 1
+    )
+    output_shape = x1.shape[:-1] + (-1,)
+    result = output.reshape(output_shape)
+
+    if mode == "valid":
+        target_length = (
+            builtins.max(x1_len, x2_len) - builtins.min(x1_len, x2_len) + 1
+        )
+        start_idx = (result.size(-1) - target_length) // 2
+        result = result[..., start_idx : start_idx + target_length]
+
+    if mode == "same":
+        start_idx = (result.size(-1) - x1_len) // 2
+        result = result[..., start_idx : start_idx + x1_len]
+
+    return torch.squeeze(result)
+
```

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-3.2.0/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/random.py` & `keras-3.2.0/keras/src/backend/torch/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,21 @@
         generator=generator,
         dtype=dtype,
         device=get_device(),
     )
 
 
 def truncated_normal(shape, mean=0.0, stddev=1.0, dtype=None, seed=None):
+    dtype = to_torch_dtype(dtype)
     # Take a larger standard normal dist, discard values outside 2 * stddev
     # Offset by mean and stddev
     x = normal(tuple(shape) + (4,), mean=0, stddev=1, dtype=dtype, seed=seed)
     valid = (x > -2) & (x < 2)
     indexes = valid.max(-1, keepdim=True)[1]
-    trunc_x = torch.empty(shape, device=get_device())
+    trunc_x = torch.empty(shape, dtype=dtype, device=get_device())
     trunc_x.data.copy_(x.gather(-1, indexes).squeeze(-1))
     trunc_x.data.mul_(stddev).add_(mean)
     return trunc_x
 
 
 def _get_concrete_noise_shape(inputs, noise_shape):
     if noise_shape is None:
```

### Comparing `keras-3.1.1/keras/src/backend/torch/rnn.py` & `keras-3.2.0/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/backend/torch/trainer.py` & `keras-3.2.0/keras/src/backend/torch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         # Call torch.nn.Module.zero_grad() to clear the leftover gradients
         # for the weights from the previous train step.
         self.zero_grad()
 
         loss = self.compute_loss(
             x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
         )
-        self._loss_tracker.update_state(loss)
+        self._loss_tracker.update_state(
+            loss, sample_weight=tree.flatten(x)[0].shape[0]
+        )
         if self.optimizer is not None:
             loss = self.optimizer.scale_loss(loss)
 
         # Compute gradients
         if self.trainable_weights:
             # Call torch.Tensor.backward() on the loss to compute gradients
             # for the weights.
@@ -82,15 +84,17 @@
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
             y_pred = self(x)
         loss = self.compute_loss(
             x=x, y=y, y_pred=y_pred, sample_weight=sample_weight
         )
-        self._loss_tracker.update_state(loss)
+        self._loss_tracker.update_state(
+            loss, sample_weight=tree.flatten(x)[0].shape[0]
+        )
         return self.compute_metrics(x, y, y_pred, sample_weight=sample_weight)
 
     def predict_step(self, data):
         x, _, _ = data_adapter_utils.unpack_x_y_sample_weight(data)
         if self._call_has_training_arg:
             y_pred = self(x, training=False)
         else:
```

### Comparing `keras-3.1.1/keras/src/callbacks/__init__.py` & `keras-3.2.0/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/backup_and_restore.py` & `keras-3.2.0/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/callback.py` & `keras-3.2.0/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/callback_list.py` & `keras-3.2.0/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/csv_logger.py` & `keras-3.2.0/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/early_stopping.py` & `keras-3.2.0/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/history.py` & `keras-3.2.0/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/lambda_callback.py` & `keras-3.2.0/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/learning_rate_scheduler.py` & `keras-3.2.0/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/model_checkpoint.py` & `keras-3.2.0/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/progbar_logger.py` & `keras-3.2.0/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-3.2.0/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/remote_monitor.py` & `keras-3.2.0/keras/src/callbacks/remote_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Otherwise the serialized JSON will be sent within a form.
 
     Args:
         root: String; root url of the target server.
         path: String; path relative to `root` to which the events will be sent.
         field: String; JSON field under which the data will be stored.
             The field is used only if the payload is sent within a form
-            (i.e. send_as_json is set to False).
+            (i.e. when `send_as_json=False`).
         headers: Dictionary; optional custom HTTP headers.
         send_as_json: Boolean; whether the request should be
             sent as `"application/json"`.
     """
 
     def __init__(
         self,
```

### Comparing `keras-3.1.1/keras/src/callbacks/swap_ema_weights.py` & `keras-3.2.0/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/callbacks/tensorboard.py` & `keras-3.2.0/keras/src/callbacks/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,16 +86,14 @@
         embeddings_metadata: Dictionary which maps embedding layer names to the
             filename of a file in which to save metadata for the embedding layer.
             In case the same metadata file is to be
             used for all embedding layers, a single filename can be passed.
 
     Examples:
 
-    Basic usage:
-
     ```python
     tensorboard_callback = keras.callbacks.TensorBoard(log_dir="./logs")
     model.fit(x_train, y_train, epochs=2, callbacks=[tensorboard_callback])
     # Then run the tensorboard command to view the visualizations.
     ```
 
     Custom batch-level summaries in a subclassed Model:
```

### Comparing `keras-3.1.1/keras/src/callbacks/terminate_on_nan.py` & `keras-3.2.0/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/constraints/__init__.py` & `keras-3.2.0/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/constraints/constraints.py` & `keras-3.2.0/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/boston_housing.py` & `keras-3.2.0/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/california_housing.py` & `keras-3.2.0/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/cifar.py` & `keras-3.2.0/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/cifar10.py` & `keras-3.2.0/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/cifar100.py` & `keras-3.2.0/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/fashion_mnist.py` & `keras-3.2.0/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/imdb.py` & `keras-3.2.0/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/mnist.py` & `keras-3.2.0/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/datasets/reuters.py` & `keras-3.2.0/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/distribution/distribution_lib.py` & `keras-3.2.0/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/dtype_policies/__init__.py` & `keras-3.2.0/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/dtype_policies/dtype_policy.py` & `keras-3.2.0/keras/src/dtype_policies/dtype_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         # TODO: We should consider deprecating this behavior
         if cls is __class__:
             if name.startswith("int8"):
                 return QuantizedDTypePolicy(name)
             return FloatDTypePolicy(name)
         return super().__new__(cls)
 
+    def __getnewargs__(self):
+        # To support `copy`, `deepcopy` and `pickle`
+        return (self._name,)
+
     def __init__(self, name):
         self._name = name
         self._compute_dtype = backend.floatx()
         self._variable_dtype = backend.floatx()
 
     def _parse_name(self, name):
         """Parses a `DTypePolicy` name into a compute and variable dtype.
```

### Comparing `keras-3.1.1/keras/src/export/export_lib.py` & `keras-3.2.0/keras/src/export/export_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Library for exporting inference-only Keras models/layers."""
 
+import inspect
+import itertools
+import string
+
 from absl import logging
 
 from keras.src import backend
 from keras.src.api_export import keras_export
+from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.layers import Layer
 from keras.src.models import Functional
 from keras.src.models import Sequential
 from keras.src.utils import io_utils
 from keras.src.utils import tree
 from keras.src.utils.module_utils import tensorflow as tf
 
@@ -85,14 +90,19 @@
         self.tensorflow_version = tf.__version__
 
         self._tf_trackable = tf.__internal__.tracking.AutoTrackable()
         self._tf_trackable.variables = []
         self._tf_trackable.trainable_variables = []
         self._tf_trackable.non_trainable_variables = []
 
+        if backend.backend() == "jax":
+            self._backend_variables = []
+            self._backend_trainable_variables = []
+            self._backend_non_trainable_variables = []
+
         if backend.backend() not in ("tensorflow", "jax"):
             raise NotImplementedError(
                 "The export API is only compatible with JAX and TF backends."
             )
 
     @property
     def variables(self):
@@ -103,15 +113,27 @@
         return self._tf_trackable.trainable_variables
 
     @property
     def non_trainable_variables(self):
         return self._tf_trackable.non_trainable_variables
 
     def track(self, resource):
-        """Track the variables (and other assets) of a layer or model."""
+        """Track the variables (and other assets) of a layer or model.
+
+        By default, all variables used by an endpoint function
+        are automatically tracked when you call `add_endpoint()`.
+        However, non-variables assets such as lookup tables
+        need to be tracked manually. Note that lookup tables
+        used by built-in Keras layers
+        (`TextVectorization`, `IntegerLookup`, `StringLookup`)
+        are automatically tracked in `add_endpoint()`.
+
+        Arguments:
+            resource: A trackable TensorFlow resource.
+        """
         if backend.backend() == "tensorflow" and not isinstance(
             resource, tf.__internal__.tracking.Trackable
         ):
             raise ValueError(
                 "Invalid resource type. Expected an instance of a "
                 "TensorFlow `Trackable` (such as a Keras `Layer` or `Model`). "
                 f"Received instead an object of type '{type(resource)}'. "
@@ -140,37 +162,46 @@
             self._tracked = []
         self._tracked.append(resource)
 
         if isinstance(resource, Layer):
             # Variables in the lists below are actually part of the trackables
             # that get saved, because the lists are created in __init__.
             if backend.backend() == "jax":
-                self._tf_trackable.variables += tree.flatten(
-                    tree.map_structure(tf.Variable, resource.variables)
+
+                trainable_variables = tree.flatten(resource.trainable_variables)
+                non_trainable_variables = tree.flatten(
+                    resource.non_trainable_variables
                 )
-                self._tf_trackable.trainable_variables += tree.flatten(
-                    tree.map_structure(
-                        tf.Variable, resource.trainable_variables
-                    )
+                self._backend_trainable_variables += trainable_variables
+                self._backend_non_trainable_variables += non_trainable_variables
+                self._backend_variables = (
+                    self._backend_trainable_variables
+                    + self._backend_non_trainable_variables
                 )
-                self._tf_trackable.non_trainable_variables += tree.flatten(
-                    tree.map_structure(
-                        tf.Variable, resource.non_trainable_variables
-                    )
+
+                self._tf_trackable.trainable_variables += [
+                    tf.Variable(v) for v in trainable_variables
+                ]
+                self._tf_trackable.non_trainable_variables += [
+                    tf.Variable(v) for v in non_trainable_variables
+                ]
+                self._tf_trackable.variables = (
+                    self._tf_trackable.trainable_variables
+                    + self._tf_trackable.non_trainable_variables
                 )
             else:
                 self._tf_trackable.variables += resource.variables
                 self._tf_trackable.trainable_variables += (
                     resource.trainable_variables
                 )
                 self._tf_trackable.non_trainable_variables += (
                     resource.non_trainable_variables
                 )
 
-    def add_endpoint(self, name, fn, input_signature=None):
+    def add_endpoint(self, name, fn, input_signature=None, jax2tf_kwargs=None):
         """Register a new serving endpoint.
 
         Arguments:
             name: Str, name of the endpoint.
             fn: A function. It should only leverage resources
                 (e.g. `tf.Variable` objects or `tf.lookup.StaticHashTable`
                 objects) that are available on the models/layers
@@ -182,14 +213,23 @@
                 2) provide an `input_signature` argument that specifies the
                 shape and dtype of the inputs (see below).
             input_signature: Used to specify the shape and dtype of the
                 inputs to `fn`. List of `tf.TensorSpec` objects (one
                 per positional input argument of `fn`). Nested arguments are
                 allowed (see below for an example showing a Functional model
                 with 2 input arguments).
+            jax2tf_kwargs: Optional. A dict for arguments to pass to `jax2tf`.
+                Supported only when the backend is JAX. See documentation for
+                [`jax2tf.convert`](
+                    https://github.com/google/jax/blob/main/jax/experimental/jax2tf/README.md).
+                The values for `native_serialization` and `polymorphic_shapes`,
+                if not provided, are automatically computed.
+
+        Returns:
+            The `tf.function` wrapping `fn` that was added to the archive.
 
         Example:
 
         Adding an endpoint using the `input_signature` argument when the
         model has a single input argument:
 
         ```python
@@ -272,21 +312,64 @@
         export_archive.track(model)
         export_archive.add_endpoint(name="serve", fn=serving_fn)
         ```
         """
         if name in self._endpoint_names:
             raise ValueError(f"Endpoint name '{name}' is already taken.")
 
+        if jax2tf_kwargs and backend.backend() != "jax":
+            raise ValueError(
+                "'jax2tf_kwargs' is only supported with the jax backend. "
+                f"Current backend: {backend.backend()}"
+            )
+
         if input_signature:
             if backend.backend() == "tensorflow":
                 decorated_fn = tf.function(fn, input_signature=input_signature)
             else:  # JAX backend
-                fn = self._convert_jax2tf_function(fn, input_signature)
+
+                # 1. Create a stateless wrapper for `fn`
+                # 2. jax2tf the stateless wrapper
+                # 3. Create a stateful function that binds the variables with
+                #    the jax2tf converted stateless wrapper
+                # 4. Make the signature of the stateful function the same as the
+                #    original function
+                # 5. Wrap in a `tf.function`
+                def stateless_fn(variables, *args, **kwargs):
+                    state_mapping = zip(self._backend_variables, variables)
+                    with StatelessScope(state_mapping=state_mapping):
+                        return fn(*args, **kwargs)
+
+                jax2tf_stateless_fn = self._convert_jax2tf_function(
+                    stateless_fn,
+                    input_signature,
+                    jax2tf_kwargs=jax2tf_kwargs,
+                )
+
+                def stateful_fn(*args, **kwargs):
+                    return jax2tf_stateless_fn(
+                        # Change the trackable `ListWrapper` to a plain `list`
+                        list(self._tf_trackable.variables),
+                        *args,
+                        **kwargs,
+                    )
+
+                # Note: we truncate the number of parameters to what is
+                # specified by `input_signature`.
+                fn_signature = inspect.signature(fn)
+                fn_parameters = list(fn_signature.parameters.values())
+                stateful_fn.__signature__ = inspect.Signature(
+                    parameters=fn_parameters[0 : len(input_signature)],
+                    return_annotation=fn_signature.return_annotation,
+                )
+
                 decorated_fn = tf.function(
-                    fn, input_signature=input_signature, autograph=False
+                    stateful_fn,
+                    input_signature=input_signature,
+                    autograph=False,
                 )
             self._endpoint_signatures[name] = input_signature
         else:
             if isinstance(fn, tf.types.experimental.GenericFunction):
                 if not fn._list_all_concrete_functions():
                     raise ValueError(
                         f"The provided tf.function '{fn}' "
@@ -313,14 +396,15 @@
                     "            dtype=tf.float32,\n"
                     "        )\n"
                     "    ],\n"
                     ")"
                 )
         setattr(self._tf_trackable, name, decorated_fn)
         self._endpoint_names.append(name)
+        return decorated_fn
 
     def add_variable_collection(self, name, variables):
         """Register a set of variables to be retrieved after reloading.
 
         Arguments:
             name: The string name for the collection.
             variables: A tuple/list/set of `tf.Variable` instances.
@@ -450,33 +534,64 @@
                 for trackable in descendants:
                     if isinstance(
                         trackable,
                         (IntegerLookup, StringLookup, TextVectorization),
                     ):
                         self._tf_trackable._misc_assets.append(trackable)
 
-    def _convert_jax2tf_function(self, fn, input_signature):
+    def _convert_jax2tf_function(self, fn, input_signature, jax2tf_kwargs=None):
         from jax.experimental import jax2tf
 
-        native_serialization = self._check_device_compatible()
-        shapes = []
-        for spec in input_signature:
-            shapes.append(self._spec_to_poly_shape(spec))
-        return jax2tf.convert(
-            fn,
-            polymorphic_shapes=shapes,
-            native_serialization=native_serialization,
+        if jax2tf_kwargs is None:
+            jax2tf_kwargs = {}
+
+        if "native_serialization" not in jax2tf_kwargs:
+            jax2tf_kwargs["native_serialization"] = (
+                self._check_device_compatible()
+            )
+
+        variables_shapes = self._to_polymorphic_shape(
+            self._backend_variables, allow_none=False
         )
+        if "polymorphic_shapes" in jax2tf_kwargs:
+            input_shapes = jax2tf_kwargs["polymorphic_shapes"]
+        else:
+            input_shapes = self._to_polymorphic_shape(input_signature)
+        jax2tf_kwargs["polymorphic_shapes"] = [variables_shapes] + input_shapes
+
+        return jax2tf.convert(fn, **jax2tf_kwargs)
+
+    def _to_polymorphic_shape(self, struct, allow_none=True):
+        if allow_none:
+            # Generates unique names: a, b, ... z, aa, ab, ... az, ba, ... zz
+            # for unknown non-batch dims. Defined here to be scope per endpoint.
+            dim_names = itertools.chain(
+                string.ascii_lowercase,
+                itertools.starmap(
+                    lambda a, b: a + b,
+                    itertools.product(string.ascii_lowercase, repeat=2),
+                ),
+            )
+
+        def convert_shape(x):
+            poly_shape = []
+            for index, dim in enumerate(list(x.shape)):
+                if dim is not None:
+                    poly_shape.append(str(dim))
+                elif not allow_none:
+                    raise ValueError(
+                        f"Illegal None dimension in {x} with shape {x.shape}"
+                    )
+                elif index == 0:
+                    poly_shape.append("batch")
+                else:
+                    poly_shape.append(next(dim_names))
+            return "(" + ", ".join(poly_shape) + ")"
 
-    def _spec_to_poly_shape(self, spec):
-        if isinstance(spec, (dict, list)):
-            return tree.map_structure(self._spec_to_poly_shape, spec)
-        spec_shape = spec.shape
-        spec_shape = str(spec_shape).replace("None", "b")
-        return spec_shape
+        return tree.map_structure(convert_shape, struct)
 
     def _check_device_compatible(self):
         from jax import default_backend as jax_device
 
         if (
             jax_device() == "gpu"
             and len(tf.config.list_physical_devices("GPU")) == 0
@@ -517,22 +632,24 @@
 
 def _get_save_spec(model):
     shapes_dict = getattr(model, "_build_shapes_dict", None)
     if not shapes_dict:
         return None
 
     if len(shapes_dict) == 1:
-        return tf.TensorSpec(
-            shape=list(shapes_dict.values())[0], dtype=model.input_dtype
-        )
+        shape = list(shapes_dict.values())[0]
+        shape = (None,) + shape[1:]
+        return tf.TensorSpec(shape=shape, dtype=model.input_dtype)
 
     specs = {}
-    for key, value in shapes_dict.items():
+    for key, shape in shapes_dict.items():
         key = key.rstrip("_shape")
-        specs[key] = tf.TensorSpec(shape=value, dtype=model.input_dtype)
+        shape = (None,) + shape[1:]
+        specs[key] = tf.TensorSpec(shape=shape, dtype=model.input_dtype)
+
     return specs
 
 
 @keras_export("keras.layers.TFSMLayer")
 class TFSMLayer(Layer):
     """Reload a Keras model/layer that was saved via SavedModel / ExportArchive.
 
@@ -663,15 +780,16 @@
             "call_endpoint": self.call_endpoint,
             "call_training_endpoint": self.call_training_endpoint,
         }
         return {**base_config, **config}
 
 
 def _make_tensor_spec(x):
-    return tf.TensorSpec(x.shape, dtype=x.dtype, name=x.name)
+    shape = (None,) + x.shape[1:]
+    return tf.TensorSpec(shape, dtype=x.dtype, name=x.name)
 
 
 def _print_signature(fn, name):
     concrete_fn = fn._list_all_concrete_functions()[0]
     pprinted_signature = concrete_fn.pretty_printed_signature(verbose=True)
     lines = pprinted_signature.split("\n")
     lines = [f"* Endpoint '{name}'"] + lines[1:]
```

### Comparing `keras-3.1.1/keras/src/initializers/__init__.py` & `keras-3.2.0/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/initializers/constant_initializers.py` & `keras-3.2.0/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/initializers/initializer.py` & `keras-3.2.0/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/initializers/random_initializers.py` & `keras-3.2.0/keras/src/initializers/random_initializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             of `keras.backend.SeedGenerator`.
     """
 
     def __init__(self, mean=0.0, stddev=0.05, seed=None):
         self.mean = mean
         self.stddev = stddev
         self._init_seed = seed
-        self.seed = seed or random.make_default_seed()
+        self.seed = seed if seed is not None else random.make_default_seed()
         super().__init__()
 
     def __call__(self, shape, dtype=None):
         return random.normal(
             shape=shape,
             mean=self.mean,
             stddev=self.stddev,
@@ -103,15 +103,15 @@
             of `keras.backend.SeedGenerator`.
     """
 
     def __init__(self, mean=0.0, stddev=0.05, seed=None):
         self.mean = mean
         self.stddev = stddev
         self._init_seed = seed
-        self.seed = seed or random.make_default_seed()
+        self.seed = seed if seed is not None else random.make_default_seed()
         super().__init__()
 
     def __call__(self, shape, dtype=None):
         return random.truncated_normal(
             shape=shape,
             mean=self.mean,
             stddev=self.stddev,
@@ -160,15 +160,15 @@
             of `keras.backend.SeedGenerator`.
     """
 
     def __init__(self, minval=-0.05, maxval=0.05, seed=None):
         self.minval = minval
         self.maxval = maxval
         self._init_seed = seed
-        self.seed = seed or random.make_default_seed()
+        self.seed = seed if seed is not None else random.make_default_seed()
         super().__init__()
 
     def __call__(self, shape, dtype=None):
         return random.uniform(
             shape=shape,
             minval=self.minval,
             maxval=self.maxval,
@@ -264,15 +264,15 @@
                 f"Invalid `distribution` argument: {distribution}."
                 f"Please use one of {allowed_distributions}"
             )
         self.scale = scale
         self.mode = mode
         self.distribution = distribution
         self._init_seed = seed
-        self.seed = seed or random.make_default_seed()
+        self.seed = seed if seed is not None else random.make_default_seed()
 
     def __call__(self, shape, dtype=None):
         scale = self.scale
         fan_in, fan_out = compute_fans(shape)
         if self.mode == "fan_in":
             scale /= max(1.0, fan_in)
         elif self.mode == "fan_out":
@@ -665,15 +665,15 @@
 
     - [Saxe et al., 2014](https://openreview.net/forum?id=_wzZwKpTDF_9C)
     """
 
     def __init__(self, gain=1.0, seed=None):
         self.gain = gain
         self._init_seed = seed
-        self.seed = seed or random.make_default_seed()
+        self.seed = seed if seed is not None else random.make_default_seed()
 
     def __call__(self, shape, dtype=None):
         if len(shape) < 2:
             raise ValueError(
                 "The tensor to initialize must be "
                 "at least two-dimensional. Received: "
                 f"shape={shape} of rank {len(shape)}."
```

### Comparing `keras-3.1.1/keras/src/layers/__init__.py` & `keras-3.2.0/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/activation.py` & `keras-3.2.0/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/elu.py` & `keras-3.2.0/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/leaky_relu.py` & `keras-3.2.0/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/prelu.py` & `keras-3.2.0/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/relu.py` & `keras-3.2.0/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/activations/softmax.py` & `keras-3.2.0/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/attention/additive_attention.py` & `keras-3.2.0/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/attention/attention.py` & `keras-3.2.0/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/attention/grouped_query_attention.py` & `keras-3.2.0/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/attention/multi_head_attention.py` & `keras-3.2.0/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/convolutional/base_conv.py` & `keras-3.2.0/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-3.2.0/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-3.2.0/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/convolutional/base_separable_conv.py` & `keras-3.2.0/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv1d.py` & `keras-3.2.0/keras/src/layers/convolutional/conv1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     Returns:
         A 3D tensor representing `activation(conv1d(inputs, kernel) + bias)`.
 
     Raises:
         ValueError: when both `strides > 1` and `dilation_rate > 1`.
 
-    Examples:
+    Example:
 
     >>> # The inputs are 128-length vectors with 10 timesteps, and the
     >>> # batch size is 4.
     >>> x = np.random.rand(4, 10, 128)
     >>> y = keras.layers.Conv1D(32, 3, activation='relu')(x)
     >>> print(y.shape)
     (4, 8, 32)
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-3.2.0/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     References:
     - [A guide to convolution arithmetic for deep learning](
         https://arxiv.org/abs/1603.07285v1)
     - [Deconvolutional Networks](
         https://www.matthewzeiler.com/mattzeiler/deconvolutionalnetworks.pdf)
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 128)
     >>> y = keras.layers.Conv1DTranspose(32, 3, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 21, 32)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv2d.py` & `keras-3.2.0/keras/src/layers/convolutional/conv2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     Returns:
         A 4D tensor representing `activation(conv2d(inputs, kernel) + bias)`.
 
     Raises:
         ValueError: when both `strides > 1` and `dilation_rate > 1`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 10, 128)
     >>> y = keras.layers.Conv2D(32, 3, activation='relu')(x)
     >>> print(y.shape)
     (4, 8, 8, 32)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-3.2.0/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     References:
     - [A guide to convolution arithmetic for deep learning](
         https://arxiv.org/abs/1603.07285v1)
     - [Deconvolutional Networks](
         https://www.matthewzeiler.com/mattzeiler/deconvolutionalnetworks.pdf)
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 8, 128)
     >>> y = keras.layers.Conv2DTranspose(32, 2, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 20, 16, 32)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv3d.py` & `keras-3.2.0/keras/src/layers/convolutional/conv3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     Returns:
         A 5D tensor representing `activation(conv3d(inputs, kernel) + bias)`.
 
     Raises:
         ValueError: when both `strides > 1` and `dilation_rate > 1`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 10, 10, 128)
     >>> y = keras.layers.Conv3D(32, 3, activation='relu')(x)
     >>> print(y.shape)
     (4, 8, 8, 8, 32)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-3.2.0/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

```diff
@@ -84,15 +84,15 @@
 
     References:
     - [A guide to convolution arithmetic for deep learning](
         https://arxiv.org/abs/1603.07285v1)
     - [Deconvolutional Networks](
         https://www.matthewzeiler.com/mattzeiler/deconvolutionalnetworks.pdf)
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 8, 12, 128)
     >>> y = keras.layers.Conv3DTranspose(32, 2, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 20, 16, 24, 32)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-3.2.0/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     Returns:
         A 3D tensor representing
         `activation(depthwise_conv1d(inputs, kernel) + bias)`.
 
     Raises:
         ValueError: when both `strides > 1` and `dilation_rate > 1`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 12)
     >>> y = keras.layers.DepthwiseConv1D(3, 3, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 4, 36)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-3.2.0/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     Returns:
         A 4D tensor representing
         `activation(depthwise_conv2d(inputs, kernel) + bias)`.
 
     Raises:
         ValueError: when both `strides > 1` and `dilation_rate > 1`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 10, 12)
     >>> y = keras.layers.DepthwiseConv2D(3, 3, activation='relu')(x)
     >>> print(y.shape)
     (4, 8, 8, 36)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/separable_conv1d.py` & `keras-3.2.0/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     - If `data_format="channels_first"`:
         A 3D tensor with shape: `(batch_shape, filters, new_steps)`
 
     Returns:
         A 3D tensor representing
         `activation(separable_conv1d(inputs, kernel) + bias)`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 12)
     >>> y = keras.layers.SeparableConv1D(3, 4, 3, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 4, 4)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/convolutional/separable_conv2d.py` & `keras-3.2.0/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     - If `data_format="channels_first"`:
         A 4D tensor with shape: `(batch_size, filters, new_height, new_width)`
 
     Returns:
         A 4D tensor representing
         `activation(separable_conv2d(inputs, kernel) + bias)`.
 
-    Examples:
+    Example:
 
     >>> x = np.random.rand(4, 10, 10, 12)
     >>> y = keras.layers.SeparableConv2D(3, 4, 3, 2, activation='relu')(x)
     >>> print(y.shape)
     (4, 4, 4, 4)
     """
```

### Comparing `keras-3.1.1/keras/src/layers/core/dense.py` & `keras-3.2.0/keras/src/layers/core/dense.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
@@ -98,37 +96,40 @@
         self.lora_rank = lora_rank
         self.lora_enabled = False
         self.input_spec = InputSpec(min_ndim=2)
         self.supports_masking = True
 
     def build(self, input_shape):
         input_dim = input_shape[-1]
-        self._kernel = self.add_weight(
-            name="kernel",
-            shape=(input_dim, self.units),
-            initializer=self.kernel_initializer,
-            regularizer=self.kernel_regularizer,
-            constraint=self.kernel_constraint,
-        )
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            self.quantized_build(
+                input_shape, mode=self.dtype_policy.quantization_mode
+            )
+        else:
+            self._kernel = self.add_weight(
+                name="kernel",
+                shape=(input_dim, self.units),
+                initializer=self.kernel_initializer,
+                regularizer=self.kernel_regularizer,
+                constraint=self.kernel_constraint,
+            )
         if self.use_bias:
             self.bias = self.add_weight(
                 name="bias",
                 shape=(self.units,),
                 initializer=self.bias_initializer,
                 regularizer=self.bias_regularizer,
                 constraint=self.bias_constraint,
             )
         else:
             self.bias = None
         self.input_spec = InputSpec(min_ndim=2, axes={-1: input_dim})
         self.built = True
         if self.lora_rank:
             self.enable_lora(self.lora_rank)
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.quantize(self.dtype_policy.quantization_mode)
 
     @property
     def kernel(self):
         if not self.built:
             raise AttributeError(
                 "You must build the layer before accessing `kernel`."
             )
@@ -142,28 +143,14 @@
         x = ops.matmul(inputs, self.kernel)
         if self.bias is not None:
             x = ops.add(x, self.bias)
         if self.activation is not None:
             x = self.activation(x)
         return x
 
-    def quantized_call(self, inputs):
-        if self.lora_enabled:
-            raise ValueError("`quantized_call` doesn't support lora weights")
-        inputs, inputs_scale = self.inputs_quantizer(inputs)
-        x = ops.matmul(inputs, self.kernel)
-        # De-scale outputs
-        x = ops.cast(x, self.compute_dtype)
-        x = ops.divide(x, ops.multiply(inputs_scale, self.kernel_scale))
-        if self.bias is not None:
-            x = ops.add(x, self.bias)
-        if self.activation is not None:
-            x = self.activation(x)
-        return x
-
     def compute_output_shape(self, input_shape):
         output_shape = list(input_shape)
         output_shape[-1] = self.units
         return tuple(output_shape)
 
     def enable_lora(
         self, rank, a_initializer="he_uniform", b_initializer="zeros"
@@ -197,107 +184,222 @@
             regularizer=self.kernel_regularizer,
         )
         self._kernel.trainable = False
         self._tracker.lock()
         self.lora_enabled = True
         self.lora_rank = rank
 
+    def save_own_variables(self, store):
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        # The keys of the `store` will be saved as determined because the
+        # default ordering will change after quantization
+        kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
+        store["0"] = kernel_value
+        if self.use_bias:
+            store["1"] = self.bias
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            store["2"] = kernel_scale
+
+    def load_own_variables(self, store):
+        if not self.lora_enabled:
+            self._check_load_own_variables(store)
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        # The keys of the `store` will be saved as determined because the
+        # default ordering will change after quantization
+        self._kernel.assign(store["0"])
+        if self.use_bias:
+            self.bias.assign(store["1"])
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            self.kernel_scale.assign(store["2"])
+        if self.lora_enabled:
+            self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
+            self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
+
+    def get_config(self):
+        base_config = super().get_config()
+        config = {
+            "units": self.units,
+            "activation": activations.serialize(self.activation),
+            "use_bias": self.use_bias,
+            "kernel_initializer": initializers.serialize(
+                self.kernel_initializer
+            ),
+            "bias_initializer": initializers.serialize(self.bias_initializer),
+            "kernel_regularizer": regularizers.serialize(
+                self.kernel_regularizer
+            ),
+            "bias_regularizer": regularizers.serialize(self.bias_regularizer),
+            "kernel_constraint": constraints.serialize(self.kernel_constraint),
+            "bias_constraint": constraints.serialize(self.bias_constraint),
+        }
+        if self.lora_rank:
+            config["lora_rank"] = self.lora_rank
+        return {**base_config, **config}
+
+    def _check_load_own_variables(self, store):
+        all_vars = self._trainable_variables + self._non_trainable_variables
+        if len(store.keys()) != len(all_vars):
+            if len(all_vars) == 0 and not self.built:
+                raise ValueError(
+                    f"Layer '{self.name}' was never built "
+                    "and thus it doesn't have any variables. "
+                    f"However the weights file lists {len(store.keys())} "
+                    "variables for this layer.\n"
+                    "In most cases, this error indicates that either:\n\n"
+                    "1. The layer is owned by a parent layer that "
+                    "implements a `build()` method, but calling the "
+                    "parent's `build()` method did NOT create the state of "
+                    f"the child layer '{self.name}'. A `build()` method "
+                    "must create ALL state for the layer, including "
+                    "the state of any children layers.\n\n"
+                    "2. You need to implement "
+                    "the `def build_from_config(self, config)` method "
+                    f"on layer '{self.name}', to specify how to rebuild "
+                    "it during loading. "
+                    "In this case, you might also want to implement the "
+                    "method that generates the build config at saving time, "
+                    "`def get_build_config(self)`. "
+                    "The method `build_from_config()` is meant "
+                    "to create the state "
+                    "of the layer (i.e. its variables) upon deserialization.",
+                )
+            raise ValueError(
+                f"Layer '{self.name}' expected {len(all_vars)} variables, "
+                "but received "
+                f"{len(store.keys())} variables during loading. "
+                f"Expected: {[v.name for v in all_vars]}"
+            )
+
+    """Quantization-related methods"""
+
+    def quantized_build(self, input_shape, mode):
+        input_dim = input_shape[-1]
+        if mode == "int8":
+            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+            self._kernel = self.add_weight(
+                name="kernel",
+                shape=(input_dim, self.units),
+                initializer="zeros",
+                dtype="int8",
+                trainable=False,
+            )
+            self.kernel_scale = self.add_weight(
+                name="kernel_scale",
+                shape=(self.units,),
+                initializer="ones",
+                trainable=False,
+            )
+
+    def quantized_call(self, inputs):
+        @ops.custom_gradient
+        def matmul_with_inputs_gradient(inputs, kernel, kernel_scale):
+            def grad_fn(*args, upstream=None):
+                if upstream is None:
+                    (upstream,) = args
+                float_kernel = ops.divide(
+                    ops.cast(kernel, dtype=self.compute_dtype),
+                    kernel_scale,
+                )
+                inputs_grad = ops.matmul(upstream, ops.transpose(float_kernel))
+                return (inputs_grad, None, None)
+
+            inputs, inputs_scale = self.inputs_quantizer(inputs)
+            x = ops.matmul(inputs, kernel)
+            # De-scale outputs
+            x = ops.cast(x, self.compute_dtype)
+            x = ops.divide(x, ops.multiply(inputs_scale, kernel_scale))
+            return x, grad_fn
+
+        x = matmul_with_inputs_gradient(
+            inputs,
+            ops.convert_to_tensor(self._kernel),
+            ops.convert_to_tensor(self.kernel_scale),
+        )
+        if self.lora_enabled:
+            lora_x = ops.matmul(inputs, self.lora_kernel_a)
+            lora_x = ops.matmul(lora_x, self.lora_kernel_b)
+            x = ops.add(x, lora_x)
+        if self.bias is not None:
+            x = ops.add(x, self.bias)
+        if self.activation is not None:
+            x = self.activation(x)
+        return x
+
     def quantize(self, mode):
+        import gc
+
+        # Prevent quantization of the subclasses
+        if type(self) is not Dense:
+            raise NotImplementedError(
+                f"Layer {self.__class__.__name__} does not have a `quantize()` "
+                "method implemented."
+            )
         self._check_quantize_args(mode, self.compute_dtype)
         if mode == "int8":
             if backend.standardize_dtype(self._kernel.dtype) == "int8":
                 raise ValueError("`quantize` can only be done once per layer.")
-            # Merge lora-related parameters to make use of fully int8 kernel
-            self._merge_lora_into_kernel()
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=0
             )
-            kernel_scale = ops.cast(kernel_scale, self.compute_dtype)
+            kernel_scale = ops.squeeze(kernel_scale, axis=0)
             self._tracker.unlock()
             self._untrack_variable(self._kernel)
+            kernel_shape = self._kernel.shape
+            del self._kernel
             self._kernel = self.add_weight(
                 name="kernel",
-                shape=self._kernel.shape,
+                shape=kernel_shape,
                 # Prevent adding a large constant to the computation graph
                 initializer=lambda shape, dtype: kernel_value,
                 dtype="int8",
                 trainable=False,
             )
             self.kernel_scale = self.add_weight(
                 name="kernel_scale",
-                shape=kernel_scale.shape,
+                shape=(self.units,),
                 # Prevent adding a large constant to the computation graph
                 initializer=lambda shape, dtype: kernel_scale,
-                dtype=self.compute_dtype,
                 trainable=False,
             )
-            if self.bias is not None:
-                self.bias.trainable = False
             self._tracker.lock()
         else:
             NotImplementedError(
                 "Invalid quantization mode. Expected 'int8'. "
                 f"Received: mode={mode}"
             )
 
         # Set new dtype policy
         if not isinstance(
             self.dtype_policy, dtype_policies.QuantizedDTypePolicy
         ):
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             self.dtype_policy = dtype_policies.get(quantized_dtype)
 
-    def _merge_lora_into_kernel(self, untrack=False):
-        if not self.lora_enabled:
-            return
-        # Merge lora-enabled kernel into kernel
-        self._kernel.assign(self.kernel)
-        self.lora_enabled = False
-        if untrack:
-            self._tracker.unlock()
-            self.lora_kernel_a = self._untrack_variable(self.lora_kernel_a)
-            self.lora_kernel_b = self._untrack_variable(self.lora_kernel_b)
-            self._tracker.lock()
-            self.lora_rank = None
-
-    def save_own_variables(self, store):
-        if not self.lora_enabled:
-            return super().save_own_variables(store)
+        # Release memory manually because sometimes the backend doesn't
+        gc.collect()
 
-        kernel_value = self.kernel
-        store["0"] = kernel_value
-        if self.use_bias:
-            store["1"] = self.bias
-
-    def load_own_variables(self, store):
-        if not self.lora_enabled:
-            return super().load_own_variables(store)
-        self._kernel.assign(store["0"])
-        if self.use_bias:
-            self.bias.assign(store["1"])
-        self.lora_kernel_a.assign(np.zeros(self.lora_kernel_a.shape))
-        self.lora_kernel_b.assign(np.zeros(self.lora_kernel_b.shape))
-
-    def get_config(self):
-        base_config = super().get_config()
-        config = {
-            "units": self.units,
-            "activation": activations.serialize(self.activation),
-            "use_bias": self.use_bias,
-            "kernel_initializer": initializers.serialize(
-                self.kernel_initializer
-            ),
-            "bias_initializer": initializers.serialize(self.bias_initializer),
-            "kernel_regularizer": regularizers.serialize(
-                self.kernel_regularizer
-            ),
-            "bias_regularizer": regularizers.serialize(self.bias_regularizer),
-            "kernel_constraint": constraints.serialize(self.kernel_constraint),
-            "bias_constraint": constraints.serialize(self.bias_constraint),
-        }
-        if self.lora_rank:
-            config["lora_rank"] = self.lora_rank
-        return {**base_config, **config}
+    def _get_kernel_with_merged_lora(self):
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            kernel_value = self._kernel
+            kernel_scale = self.kernel_scale
+            if self.lora_enabled:
+                # Dequantize & quantize to merge lora weights into int8 kernel
+                # Note that this is a lossy compression
+                kernel_value = ops.divide(kernel_value, kernel_scale)
+                kernel_value = ops.add(
+                    kernel_value,
+                    ops.matmul(self.lora_kernel_a, self.lora_kernel_b),
+                )
+                kernel_value, kernel_scale = quantizers.abs_max_quantize(
+                    kernel_value, axis=0
+                )
+                kernel_scale = ops.squeeze(kernel_scale, axis=0)
+            return kernel_value, kernel_scale
+        return self.kernel, None
```

### Comparing `keras-3.1.1/keras/src/layers/core/einsum_dense.py` & `keras-3.2.0/keras/src/layers/core/einsum_dense.py`

 * *Files 12% similar despite different names*

```diff
@@ -149,42 +149,45 @@
             self.equation,
             self.bias_axes,
             input_shape,
             self.partial_output_shape,
         )
         kernel_shape, bias_shape, full_output_shape = shape_data
         self.full_output_shape = tuple(full_output_shape)
-        self._kernel = self.add_weight(
-            name="kernel",
-            shape=tuple(kernel_shape),
-            initializer=self.kernel_initializer,
-            regularizer=self.kernel_regularizer,
-            constraint=self.kernel_constraint,
-            dtype=self.dtype,
-            trainable=True,
-        )
-
+        # `quantized_build` needs `self.input_spec`
+        self.input_spec = InputSpec(ndim=len(input_shape))
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            self.quantized_build(
+                input_shape, mode=self.dtype_policy.quantization_mode
+            )
+        else:
+            self._kernel = self.add_weight(
+                name="kernel",
+                shape=tuple(kernel_shape),
+                initializer=self.kernel_initializer,
+                regularizer=self.kernel_regularizer,
+                constraint=self.kernel_constraint,
+                dtype=self.dtype,
+                trainable=True,
+            )
         if bias_shape is not None:
             self.bias = self.add_weight(
                 name="bias",
                 shape=tuple(bias_shape),
                 initializer=self.bias_initializer,
                 regularizer=self.bias_regularizer,
                 constraint=self.bias_constraint,
                 dtype=self.dtype,
                 trainable=True,
             )
         else:
             self.bias = None
-        self.input_spec = InputSpec(ndim=len(input_shape))
         self.built = True
         if self.lora_rank:
             self.enable_lora(self.lora_rank)
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.quantize(self.dtype_policy.quantization_mode)
 
     @property
     def kernel(self):
         if not self.built:
             raise AttributeError(
                 "You must build the layer before accessing `kernel`."
             )
@@ -193,71 +196,22 @@
                 self.lora_kernel_a, self.lora_kernel_b
             )
         return self._kernel
 
     def compute_output_shape(self, _):
         return self.full_output_shape
 
-    def get_config(self):
-        base_config = super().get_config()
-        config = {
-            "output_shape": self.partial_output_shape,
-            "equation": self.equation,
-            "activation": activations.serialize(self.activation),
-            "bias_axes": self.bias_axes,
-            "kernel_initializer": initializers.serialize(
-                self.kernel_initializer
-            ),
-            "bias_initializer": initializers.serialize(self.bias_initializer),
-            "kernel_regularizer": regularizers.serialize(
-                self.kernel_regularizer
-            ),
-            "bias_regularizer": regularizers.serialize(self.bias_regularizer),
-            "activity_regularizer": regularizers.serialize(
-                self.activity_regularizer
-            ),
-            "kernel_constraint": constraints.serialize(self.kernel_constraint),
-            "bias_constraint": constraints.serialize(self.bias_constraint),
-        }
-        if self.lora_rank:
-            config["lora_rank"] = self.lora_rank
-        return {**base_config, **config}
-
     def call(self, inputs):
         x = ops.einsum(self.equation, inputs, self.kernel)
         if self.bias is not None:
             x += self.bias
         if self.activation is not None:
             x = self.activation(x)
         return x
 
-    def quantized_call(self, inputs):
-        if self.lora_enabled:
-            raise ValueError("`quantized_call` doesn't support lora weights")
-        inputs, inputs_scale = self.inputs_quantizer(inputs)
-        x = ops.einsum(self.equation, inputs, self.kernel)
-        # Deal with `inputs_scale`
-        inputs_scale = ops.transpose(inputs_scale, self._input_transpose_axes)
-        if self._input_expand_axes:
-            inputs_scale = ops.expand_dims(
-                inputs_scale, axis=self._input_expand_axes
-            )
-        if self._input_squeeze_axes:
-            inputs_scale = ops.squeeze(
-                inputs_scale, axis=self._input_squeeze_axes
-            )
-        # De-scale outputs
-        x = ops.cast(x, self.compute_dtype)
-        x = ops.divide(x, ops.multiply(inputs_scale, self.kernel_scale))
-        if self.bias is not None:
-            x += self.bias
-        if self.activation is not None:
-            x = self.activation(x)
-        return x
-
     def enable_lora(
         self, rank, a_initializer="he_uniform", b_initializer="zeros"
     ):
         if self.kernel_constraint:
             raise ValueError(
                 "Lora is incompatible with kernel constraints. "
                 "In order to enable lora on this layer, remove the "
@@ -286,117 +240,319 @@
             regularizer=self.kernel_regularizer,
         )
         self._kernel.trainable = False
         self._tracker.lock()
         self.lora_enabled = True
         self.lora_rank = rank
 
+    def save_own_variables(self, store):
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        # The keys of the `store` will be saved as determined because the
+        # default ordering will change after quantization
+        kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
+        store["0"] = kernel_value
+        if self.bias is not None:
+            store["1"] = self.bias
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            store["2"] = kernel_scale
+
+    def load_own_variables(self, store):
+        if not self.lora_enabled:
+            self._check_load_own_variables(store)
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        # The keys of the `store` will be saved as determined because the
+        # default ordering will change after quantization
+        self._kernel.assign(store["0"])
+        if self.bias is not None:
+            self.bias.assign(store["1"])
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            self.kernel_scale.assign(store["2"])
+        if self.lora_enabled:
+            self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
+            self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
+
+    def get_config(self):
+        base_config = super().get_config()
+        config = {
+            "output_shape": self.partial_output_shape,
+            "equation": self.equation,
+            "activation": activations.serialize(self.activation),
+            "bias_axes": self.bias_axes,
+            "kernel_initializer": initializers.serialize(
+                self.kernel_initializer
+            ),
+            "bias_initializer": initializers.serialize(self.bias_initializer),
+            "kernel_regularizer": regularizers.serialize(
+                self.kernel_regularizer
+            ),
+            "bias_regularizer": regularizers.serialize(self.bias_regularizer),
+            "activity_regularizer": regularizers.serialize(
+                self.activity_regularizer
+            ),
+            "kernel_constraint": constraints.serialize(self.kernel_constraint),
+            "bias_constraint": constraints.serialize(self.bias_constraint),
+        }
+        if self.lora_rank:
+            config["lora_rank"] = self.lora_rank
+        return {**base_config, **config}
+
+    def _check_load_own_variables(self, store):
+        all_vars = self._trainable_variables + self._non_trainable_variables
+        if len(store.keys()) != len(all_vars):
+            if len(all_vars) == 0 and not self.built:
+                raise ValueError(
+                    f"Layer '{self.name}' was never built "
+                    "and thus it doesn't have any variables. "
+                    f"However the weights file lists {len(store.keys())} "
+                    "variables for this layer.\n"
+                    "In most cases, this error indicates that either:\n\n"
+                    "1. The layer is owned by a parent layer that "
+                    "implements a `build()` method, but calling the "
+                    "parent's `build()` method did NOT create the state of "
+                    f"the child layer '{self.name}'. A `build()` method "
+                    "must create ALL state for the layer, including "
+                    "the state of any children layers.\n\n"
+                    "2. You need to implement "
+                    "the `def build_from_config(self, config)` method "
+                    f"on layer '{self.name}', to specify how to rebuild "
+                    "it during loading. "
+                    "In this case, you might also want to implement the "
+                    "method that generates the build config at saving time, "
+                    "`def get_build_config(self)`. "
+                    "The method `build_from_config()` is meant "
+                    "to create the state "
+                    "of the layer (i.e. its variables) upon deserialization.",
+                )
+            raise ValueError(
+                f"Layer '{self.name}' expected {len(all_vars)} variables, "
+                "but received "
+                f"{len(store.keys())} variables during loading. "
+                f"Expected: {[v.name for v in all_vars]}"
+            )
+
+    """Quantization-related methods"""
+
+    def quantized_build(self, input_shape, mode):
+        shape_data = _analyze_einsum_string(
+            self.equation,
+            self.bias_axes,
+            input_shape,
+            self.partial_output_shape,
+        )
+        kernel_shape, _, _ = shape_data
+        if mode == "int8":
+            (
+                self._input_reduced_axes,
+                self._kernel_reduced_axes,
+                self._input_transpose_axes,
+                self._kernel_transpose_axes,
+                self._input_expand_axes,
+                self._kernel_expand_axes,
+                self._input_squeeze_axes,
+                self._kernel_squeeze_axes,
+                self._custom_gradient_equation,
+                self._kernel_reverse_transpose_axes,
+            ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
+            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+            self._kernel = self.add_weight(
+                name="kernel",
+                shape=kernel_shape,
+                initializer="zeros",
+                dtype="int8",
+                trainable=False,
+            )
+            kernel_scale_shape = np.array(kernel_shape)
+            kernel_scale_shape[self._kernel_reduced_axes] = 1
+            kernel_scale_shape = kernel_scale_shape[self._kernel_transpose_axes]
+            kernel_scale_shape = kernel_scale_shape.tolist()
+            for a in sorted(self._kernel_expand_axes):
+                kernel_scale_shape.insert(a, 1)
+            for a in sorted(self._kernel_squeeze_axes, reverse=True):
+                kernel_scale_shape.pop(a)
+            self.kernel_scale = self.add_weight(
+                name="kernel_scale",
+                shape=kernel_scale_shape,
+                initializer="ones",
+                trainable=False,
+            )
+
+    def quantized_call(self, inputs):
+        @ops.custom_gradient
+        def einsum_with_inputs_gradient(inputs, kernel, kernel_scale):
+            def grad_fn(*args, upstream=None):
+                if upstream is None:
+                    (upstream,) = args
+                # De-scale kernel
+                _kernel_scale = kernel_scale  # Overcome UnboundLocalError
+                if self._kernel_squeeze_axes:
+                    _kernel_scale = ops.expand_dims(
+                        _kernel_scale, axis=self._kernel_squeeze_axes
+                    )
+                if self._kernel_expand_axes:
+                    _kernel_scale = ops.squeeze(
+                        _kernel_scale, axis=self._kernel_expand_axes
+                    )
+                _kernel_scale = ops.transpose(
+                    _kernel_scale, self._kernel_reverse_transpose_axes
+                )
+                float_kernel = ops.divide(
+                    ops.cast(kernel, dtype=self.compute_dtype),
+                    _kernel_scale,
+                )
+                # From https://stackoverflow.com/a/47609896
+                inputs_grad = ops.einsum(
+                    self._custom_gradient_equation, upstream, float_kernel
+                )
+                return (inputs_grad, None, None)
+
+            inputs, inputs_scale = self.inputs_quantizer(inputs)
+            x = ops.einsum(self.equation, inputs, kernel)
+            # Deal with `inputs_scale`
+            inputs_scale = ops.transpose(
+                inputs_scale, self._input_transpose_axes
+            )
+            if self._input_expand_axes:
+                inputs_scale = ops.expand_dims(
+                    inputs_scale, axis=self._input_expand_axes
+                )
+            if self._input_squeeze_axes:
+                inputs_scale = ops.squeeze(
+                    inputs_scale, axis=self._input_squeeze_axes
+                )
+            # De-scale outputs
+            x = ops.cast(x, self.compute_dtype)
+            x = ops.divide(x, ops.multiply(inputs_scale, kernel_scale))
+            return x, grad_fn
+
+        x = einsum_with_inputs_gradient(
+            inputs,
+            ops.convert_to_tensor(self._kernel),
+            ops.convert_to_tensor(self.kernel_scale),
+        )
+        if self.lora_enabled:
+            lora_x = ops.einsum(self.equation, inputs, self.lora_kernel_a)
+            lora_x = ops.matmul(lora_x, self.lora_kernel_b)
+            x = ops.add(x, lora_x)
+        if self.bias is not None:
+            x += self.bias
+        if self.activation is not None:
+            x = self.activation(x)
+        return x
+
     def quantize(self, mode):
+        import gc
+
+        # Prevent quantization of the subclasses
+        if type(self) is not EinsumDense:
+            raise NotImplementedError(
+                f"Layer {self.__class__.__name__} does not have a `quantize()` "
+                "method implemented."
+            )
         self._check_quantize_args(mode, self.compute_dtype)
         if mode == "int8":
             if backend.standardize_dtype(self._kernel.dtype) == "int8":
                 raise ValueError("`quantize` can only be done once per layer.")
-            # Merge lora-related parameters to make use of fully int8 kernel
-            self._merge_lora_into_kernel()
-
-            if self.input_spec is None:
-                raise ValueError(
-                    f"Cannot quantize {self.name} that isn't yet built."
-                )
             (
                 self._input_reduced_axes,
                 self._kernel_reduced_axes,
                 self._input_transpose_axes,
                 self._kernel_transpose_axes,
                 self._input_expand_axes,
                 self._kernel_expand_axes,
                 self._input_squeeze_axes,
                 self._kernel_squeeze_axes,
+                self._custom_gradient_equation,
+                self._kernel_reverse_transpose_axes,
             ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
             # Configure `self.inputs_quantizer`
             self.inputs_quantizer = quantizers.AbsMaxQuantizer(
                 axis=self._input_reduced_axes
             )
             # Quantize `self._kernel` to int8 and compute corresponding scale
             kernel_value, kernel_scale = quantizers.abs_max_quantize(
                 self._kernel, axis=self._kernel_reduced_axes
             )
-            kernel_scale = ops.cast(kernel_scale, self.compute_dtype)
             kernel_scale = ops.transpose(
                 kernel_scale, self._kernel_transpose_axes
             )
             if self._kernel_expand_axes:
                 kernel_scale = ops.expand_dims(
                     kernel_scale, axis=self._kernel_expand_axes
                 )
             if self._kernel_squeeze_axes:
                 kernel_scale = ops.squeeze(
                     kernel_scale, axis=self._kernel_squeeze_axes
                 )
             self._tracker.unlock()
             self._untrack_variable(self._kernel)
+            kernel_shape = self._kernel.shape
+            del self._kernel
             self._kernel = self.add_weight(
                 name="kernel",
-                shape=self._kernel.shape,
+                shape=kernel_shape,
                 # Prevent adding a large constant to the computation graph
                 initializer=lambda shape, dtype: kernel_value,
                 dtype="int8",
                 trainable=False,
             )
             self.kernel_scale = self.add_weight(
                 name="kernel_scale",
                 shape=kernel_scale.shape,
                 # Prevent adding a large constant to the computation graph
                 initializer=lambda shape, dtype: kernel_scale,
-                dtype=self.compute_dtype,
                 trainable=False,
             )
-            if self.bias is not None:
-                self.bias.trainable = False
             self._tracker.lock()
         else:
             NotImplementedError()
 
         # Set new dtype policy
         if not isinstance(
             self.dtype_policy, dtype_policies.QuantizedDTypePolicy
         ):
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             self.dtype_policy = dtype_policies.get(quantized_dtype)
 
-    def _merge_lora_into_kernel(self, untrack=False):
-        if not self.lora_enabled:
-            return
-        # Merge lora-enabled kernel into kernel
-        self._kernel.assign(self.kernel)
-        self.lora_enabled = False
-        if untrack:
-            self._tracker.unlock()
-            self.lora_kernel_a = self._untrack_variable(self.lora_kernel_a)
-            self.lora_kernel_b = self._untrack_variable(self.lora_kernel_b)
-            self._tracker.lock()
-            self.lora_rank = None
-
-    def save_own_variables(self, store):
-        if not self.lora_enabled:
-            return super().save_own_variables(store)
+        # Release memory manually because sometimes the backend doesn't
+        gc.collect()
 
-        kernel_value = self.kernel
-        store["0"] = kernel_value
-        if self.bias is not None:
-            store["1"] = self.bias
-
-    def load_own_variables(self, store):
-        if not self.lora_enabled:
-            return super().load_own_variables(store)
-        self._kernel.assign(store["0"])
-        if self.bias is not None:
-            self.bias.assign(store["1"])
-        self.lora_kernel_a.assign(np.zeros(self.lora_kernel_a.shape))
-        self.lora_kernel_b.assign(np.zeros(self.lora_kernel_b.shape))
+    def _get_kernel_with_merged_lora(self):
+        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            kernel_value = self._kernel
+            kernel_scale = self.kernel_scale
+            if self.lora_enabled:
+                # Dequantize & quantize to merge lora weights into int8 kernel
+                # Note that this is a lossy compression
+                kernel_value = ops.divide(kernel_value, kernel_scale)
+                kernel_value = ops.add(
+                    kernel_value,
+                    ops.matmul(self.lora_kernel_a, self.lora_kernel_b),
+                )
+                kernel_value, kernel_scale = quantizers.abs_max_quantize(
+                    kernel_value, axis=self._kernel_reduced_axes
+                )
+                kernel_scale = ops.transpose(
+                    kernel_scale, self._kernel_transpose_axes
+                )
+                if self._kernel_expand_axes:
+                    kernel_scale = ops.expand_dims(
+                        kernel_scale, axis=self._kernel_expand_axes
+                    )
+                if self._kernel_squeeze_axes:
+                    kernel_scale = ops.squeeze(
+                        kernel_scale, axis=self._kernel_squeeze_axes
+                    )
+        else:
+            kernel_value = self.kernel
+            kernel_scale = None
+        return kernel_value, kernel_scale
 
 
 def _analyze_einsum_string(equation, bias_axes, input_shape, output_shape):
     """Analyzes an einsum string to determine the required weight shape."""
 
     dot_replaced_string = re.sub(r"\.\.\.", "0", equation)
 
@@ -655,18 +811,28 @@
         input_transpose_axes.insert(index, ori_index)
     for ori_index in weight_reduced_axes:
         try:
             index = weight_expand_axes.pop(0)
         except IndexError:
             weight_squeeze_axes.append(ori_index)
         weight_transpose_axes.insert(index, ori_index)
+    # Prepare equation for `einsum_with_inputs_gradient`
+    custom_gradient_equation = f"{output_spec},{weight_spec}->{input_spec}"
+    weight_reverse_transpose_axes = [
+        i
+        for (_, i) in sorted(
+            (v, i) for (i, v) in enumerate(weight_transpose_axes)
+        )
+    ]
     return (
         input_reduced_axes,
         weight_reduced_axes,
         input_transpose_axes,
         weight_transpose_axes,
         input_expand_axes,
         weight_expand_axes,
         input_squeeze_axes,
         weight_squeeze_axes,
+        custom_gradient_equation,
+        weight_reverse_transpose_axes,
     )
```

### Comparing `keras-3.1.1/keras/src/layers/core/identity.py` & `keras-3.2.0/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/core/input_layer.py` & `keras-3.2.0/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/core/lambda_layer.py` & `keras-3.2.0/keras/src/layers/core/lambda_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import types
 
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 from keras.src.utils import python_utils
-from keras.src.utils import shape_utils
 from keras.src.utils import tree
 
 
 @keras_export("keras.layers.Lambda")
 class Lambda(Layer):
     """Wraps arbitrary expressions as a `Layer` object.
 
@@ -82,15 +81,15 @@
         self._fn_expects_training_arg = "training" in function_args
         self._fn_expects_mask_arg = "mask" in function_args
 
     def compute_output_shape(self, input_shape):
         if self._output_shape is None:
             # Leverage backend shape inference
             try:
-                inputs = shape_utils.map_shape_structure(
+                inputs = tree.map_shape_structure(
                     lambda x: backend.KerasTensor(x, dtype=self.compute_dtype),
                     input_shape,
                 )
                 output_spec = backend.compute_output_spec(self.call, inputs)
                 return tree.map_structure(lambda x: x.shape, output_spec)
             except:
                 raise NotImplementedError(
@@ -104,15 +103,15 @@
 
         # Output shapes are passed directly and don't include batch dimension.
         batch_size = tree.flatten(input_shape)[0]
 
         def _add_batch(shape):
             return (batch_size,) + shape
 
-        return shape_utils.map_shape_structure(_add_batch, self._output_shape)
+        return tree.map_shape_structure(_add_batch, self._output_shape)
 
     def call(self, inputs, mask=None, training=None):
         # We must copy for thread safety,
         # but it only needs to be a shallow copy.
         kwargs = {k: v for k, v in self.arguments.items()}
         if self._fn_expects_mask_arg:
             kwargs["mask"] = mask
```

### Comparing `keras-3.1.1/keras/src/layers/core/masking.py` & `keras-3.2.0/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/core/wrapper.py` & `keras-3.2.0/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/input_spec.py` & `keras-3.2.0/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/layer.py` & `keras-3.2.0/keras/src/layers/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from keras.src.metrics.metric import Metric
 from keras.src.ops.operation import Operation
 from keras.src.utils import python_utils
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
 from keras.src.utils import tree
-from keras.src.utils.shape_utils import map_shape_structure
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.layer import TFLayer as BackendLayer
 elif backend.backend() == "jax":
     from keras.src.backend.jax.layer import JaxLayer as BackendLayer
 elif backend.backend() == "torch":
     from keras.src.backend.torch.layer import TorchLayer as BackendLayer
@@ -215,15 +214,15 @@
         # to add name scope support and serialization support.
         obj = super().__new__(cls, *args, **kwargs)
 
         original_build_method = obj.build
 
         @wraps(original_build_method)
         def build_wrapper(*args, **kwargs):
-            with backend.name_scope(obj.name, caller=obj):
+            with obj._open_name_scope():
                 original_build_method(*args, **kwargs)
             # Record build config.
             signature = inspect.signature(original_build_method)
             obj._build_shapes_dict = signature.bind(*args, **kwargs).arguments
             # Set built, post build actions, and lock state.
             obj.built = True
             obj._post_build()
@@ -271,14 +270,15 @@
         self._input_spec = None
         self._called = False
         self.supports_jit = True
 
         self._trainable = trainable
         self._losses = []
         self._loss_ids = set()
+        self._losses_override = []
 
         self._call_signature = inspect.signature(self.call)
         call_signature_parameters = [
             p.name for p in self._call_signature.parameters.values()
         ]
         self._call_has_training_arg = "training" in call_signature_parameters
         self._call_has_mask_arg = "mask" in call_signature_parameters
@@ -286,14 +286,16 @@
         self._supports_masking = not utils.is_default(self.compute_mask)
         # Whether to automatically convert (+ auto-cast) inputs to `call()`.
         self._convert_input_args = True
         # Whether to allow non-tensors as positional arguments in `call()`.
         self._allow_non_tensor_positional_args = False
         # Dict of shapes that were used to call `build()`.
         self._build_shapes_dict = None
+        # Parent path
+        self._parent_path = None
         self._initializer_tracker()
 
     @tracking.no_automatic_dependency_tracking
     def _initializer_tracker(self):
         if hasattr(self, "_tracker"):
             return
 
@@ -421,88 +423,97 @@
 
     def add_variable(
         self,
         shape,
         initializer,
         dtype=None,
         trainable=True,
+        autocast=True,
         regularizer=None,
         constraint=None,
         name=None,
     ):
         """Add a weight variable to the layer.
 
         Alias of `add_weight()`.
         """
         return self.add_weight(
             shape=shape,
             initializer=initializer,
             dtype=dtype,
             trainable=trainable,
+            autocast=autocast,
             regularizer=regularizer,
             constraint=constraint,
             name=name,
         )
 
     def add_weight(
         self,
         shape=None,
         initializer=None,
         dtype=None,
         trainable=True,
+        autocast=True,
         regularizer=None,
         constraint=None,
+        aggregation="mean",
         name=None,
     ):
         """Add a weight variable to the layer.
 
         Args:
-            shape: Shape tuple for the variable.
-                Must be fully-defined (no `None` entries).
-                Defaults to `()` (scalar) if unspecified.
-            initializer: Initializer object to use to
-                populate the initial variable value,
-                or string name of a built-in initializer
-                (e.g. `"random_normal"`). If unspecified,
-                defaults to `"glorot_uniform"`
-                for floating-point variables and to `"zeros"`
+            shape: Shape tuple for the variable. Must be fully-defined
+                (no `None` entries). Defaults to `()` (scalar) if unspecified.
+            initializer: Initializer object to use to populate the initial
+                variable value, or string name of a built-in initializer
+                (e.g. `"random_normal"`). If unspecified, defaults to
+                `"glorot_uniform"` for floating-point variables and to `"zeros"`
                 for all other types (e.g. int, bool).
-            dtype: Dtype of the variable to create,
-                e.g. `"float32"`. If unspecified,
-                defaults to the layer's
-                variable dtype (which itself defaults to
-                `"float32"` if unspecified).
-            trainable: Boolean, whether the variable should
-                be trainable via backprop or whether its
-                updates are managed manually.
-            constraint: Contrainst object to call on the
-                variable after any optimizer update,
-                or string name of a built-in constraint.
-            name: String name of the variable. Useful
-                for debugging purposes.
+            dtype: Dtype of the variable to create, e.g. `"float32"`. If
+                unspecified, defaults to the layer's variable dtype
+                (which itself defaults to `"float32"` if unspecified).
+            trainable: Boolean, whether the variable should be trainable via
+                backprop or whether its updates are managed manually. Defaults
+                to `True`.
+            autocast: Boolean, whether to autocast layers variables when
+                accessing them. Defaults to `True`.
+            regularizer: Regularizer object to call to apply penalty on the
+                weight. These penalties are summed into the loss function
+                during optimization. Defaults to `None`.
+            constraint: Contrainst object to call on the variable after any
+                optimizer update, or string name of a built-in constraint.
+                Defaults to `None`.
+            aggregation: String, one of `'mean'`, `'sum'`,
+                `'only_first_replica'`. Annotates the variable with the type
+                of multi-replica aggregation to be used for this variable
+                when writing custom data parallel training loops.
+            name: String name of the variable. Useful for debugging purposes.
         """
         self._check_super_called()
         if shape is None:
             shape = ()
         if dtype is not None:
             dtype = backend.standardize_dtype(dtype)
         else:
             dtype = self.variable_dtype
         if initializer is None:
             if "float" in dtype:
                 initializer = "glorot_uniform"
             else:
                 initializer = "zeros"
         initializer = initializers.get(initializer)
-        with backend.name_scope(self.name, caller=self):
+        with self._open_name_scope():
             variable = backend.Variable(
                 initializer=initializer,
                 shape=shape,
                 dtype=dtype,
                 trainable=trainable,
+                autocast=autocast,
+                aggregation=aggregation,
                 name=name,
             )
         # Will be added to layer.losses
         variable.regularizer = regularizers.get(regularizer)
         variable.constraint = constraints.get(constraint)
         self._track_variable(variable)
         return variable
@@ -731,15 +742,15 @@
         ############################################
         # 3. Check input spec for 1st positional arg.
         # TODO: consider extending this to all args and kwargs.
         self._assert_input_compatibility(call_spec.first_arg)
 
         ################
         # 4. Call build
-        with backend.name_scope(self.name, caller=self):
+        with self._open_name_scope():
             self._maybe_build(call_spec)
 
         ##########################
         # 5. Infer training value
         # Training phase for `Layer.call` is set via (in order of priority):
         # (1) The `training` argument passed to this `Layer.call`, if not None
         # (2) The training argument of an outer `Layer.call`.
@@ -786,15 +797,15 @@
                             lambda x: getattr(x, "_keras_mask", None), v
                         )
                         kwargs[expected_mask_arg_name] = mask
 
         ####################
         # 7. Call the layer.
         try:
-            with backend.name_scope(self.name, caller=self):
+            with self._open_name_scope():
                 current_scope = backend.get_autocast_scope()
                 new_scope = None
                 if current_scope is not None:
                     # Clear or update the current scope if necessary.
                     if not self.autocast:
                         new_scope = backend.AutocastScope(None)
                     elif not backend.is_float_dtype(self.compute_dtype):
@@ -964,18 +975,15 @@
             if return_losses:
                 losses = self.losses
 
         # Gather updated non-trainable variables
         non_trainable_variables = []
         for v in self.non_trainable_variables:
             new_v = scope.get_current_value(v)
-            if new_v is not None:
-                non_trainable_variables.append(new_v)
-            else:
-                non_trainable_variables.append(v)
+            non_trainable_variables.append(new_v)
 
         if return_losses:
             return outputs, non_trainable_variables, losses
         return outputs, non_trainable_variables
 
     def compute_output_spec(self, *args, **kwargs):
         if utils.is_default(self.compute_output_shape):
@@ -1013,15 +1021,15 @@
                 isinstance(output_shape, tuple)
                 and output_shape
                 and isinstance(output_shape[0], (int, type(None)))
             ):
                 return KerasTensor(output_shape, dtype=self.compute_dtype)
             # Case: nested. Could be a tuple/list of shapes, or a dict of
             # shapes. Could be deeply nested.
-            return map_shape_structure(
+            return tree.map_shape_structure(
                 lambda s: KerasTensor(s, dtype=self.compute_dtype), output_shape
             )
 
     @utils.default
     def compute_output_shape(self, *args, **kwargs):
         raise NotImplementedError(
             f"Layer {self.__class__.__name__} should implement "
@@ -1080,14 +1088,16 @@
                 v = variable
             weight_regularization_losses.append(variable.regularizer(v))
         return weight_regularization_losses
 
     @property
     def losses(self):
         """List of scalar losses from `add_loss`, regularizers and sublayers."""
+        if self._losses_override:
+            return self._losses_override
         losses = self._get_own_losses()
         for layer in self._flatten_layers(include_self=False):
             losses.extend(layer._get_own_losses())
         weight_regularization_losses = self._get_regularization_losses()
         losses.extend(weight_regularization_losses)
         return losses
 
@@ -1107,25 +1117,29 @@
         raise NotImplementedError(
             f"Layer {self.__class__.__name__} does not have a `quantize()` "
             "method implemented."
         )
 
     def _check_quantize_args(self, mode, compute_dtype):
         if not self.built:
-            raise ValueError("Cannot quantize on a layer that isn't yet built.")
+            raise ValueError(
+                "Cannot quantize a layer that isn't yet built. "
+                f"Layer '{self.name}' (of type '{self.__class__.__name__}') "
+                "is not built yet."
+            )
         if mode not in ("int8",):
             raise ValueError(
                 f"`quantize` must be one of ('int8'). Received: mode={mode}"
             )
         if mode == "int8" and compute_dtype == "float16":
             raise ValueError(
-                f"mode='{mode}' doesn't work well with "
+                f"Quantization mode='{mode}' doesn't work well with "
                 "compute_dtype='float16'. Consider loading model/layer with "
-                "other dtype policy such as 'mixed_bfloat16' before calling "
-                "`quantize`."
+                "another dtype policy such as 'mixed_bfloat16' or "
+                "'mixed_float16' before calling `quantize()`."
             )
 
     def save_own_variables(self, store):
         """Saves the state of the layer.
 
         You can override this method to take full control of how the state of
         the layer is saved upon calling `model.save()`.
@@ -1182,14 +1196,16 @@
             v.assign(store[f"{i}"])
 
     def _track_variable(self, variable):
         if variable.trainable:
             self._tracker.add_to_store("trainable_variables", variable)
         else:
             self._tracker.add_to_store("non_trainable_variables", variable)
+        if not self.trainable:
+            variable.trainable = False
 
     def _untrack_variable(self, variable):
         previous_lock_state = self._tracker.locked
         self._tracker.unlock()
         self._tracker.untrack(variable)
         if previous_lock_state is True:
             self._tracker.lock()
@@ -1260,15 +1276,15 @@
                     "children layers).\n"
                     f"Exception encountered: ''{e}''"
                 )
         self.build(first_shape)
 
     def _build_by_run_for_single_pos_arg(self, input_shape):
         # Case: all inputs are in the first arg (possibly nested).
-        input_tensors = map_shape_structure(
+        input_tensors = tree.map_shape_structure(
             lambda s: backend.KerasTensor(s), input_shape
         )
         try:
             backend.compute_output_spec(self.call, input_tensors)
             return True
         except:
             return False
@@ -1391,14 +1407,19 @@
         base_config = super().get_config()
         config = {
             "trainable": self.trainable,
             "dtype": self.dtype_policy.name,
         }
         return {**base_config, **config}
 
+    def _open_name_scope(self):
+        if self._parent_path is None:
+            self._parent_path = current_path()
+        return backend.name_scope(self.name, caller=self)
+
 
 def is_backend_tensor_or_symbolic(x):
     return backend.is_tensor(x) or isinstance(x, backend.KerasTensor)
 
 
 class CallSpec:
     def __init__(self, signature, args, kwargs):
```

### Comparing `keras-3.1.1/keras/src/layers/merging/add.py` & `keras-3.2.0/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/average.py` & `keras-3.2.0/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/base_merge.py` & `keras-3.2.0/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/concatenate.py` & `keras-3.2.0/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/dot.py` & `keras-3.2.0/keras/src/layers/merging/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     * `y.shape[0]` : 100 : do not append to output shape, always ignore
         first dimension of `y`
     * `y.shape[1]` : 30 : append to output shape
     * `y.shape[2]` : 20 : do not append to output shape, dimension 2 of
         `y` has been summed over.
         (`dot_axes[1]` = 2) `output_shape` = `(100, 30)`
 
-    Examples:
+    Example:
 
     >>> x_batch = np.ones(shape=(32, 20, 1))
     >>> y_batch = np.ones(shape=(32, 30, 20))
     >>> xy_batch_dot = batch_dot(x_batch, y_batch, axes=(1, 2))
 
     Args:
         x: Keras tensor or variable with `ndim >= 2`.
@@ -205,15 +205,15 @@
     Let's say `x` and `y` are the two input tensors with shapes
     `(2, 3, 5)` and `(2, 10, 3)`. The batch dimension should be
     of same size for both the inputs, and `axes` should correspond
     to the dimensions that have the same size in the corresponding
     inputs. e.g. with `axes=(1, 2)`, the dot product of `x`, and `y`
     will result in a tensor with shape `(2, 5, 10)`
 
-    Examples:
+    Example:
 
     >>> x = np.arange(10).reshape(1, 5, 2)
     >>> y = np.arange(10, 20).reshape(1, 2, 5)
     >>> keras.layers.Dot(axes=(1, 2))([x, y])
 
     Usage in a Keras model:
 
@@ -258,15 +258,18 @@
         self.axes = axes
         self.normalize = normalize
         self.supports_masking = True
         self._reshape_required = False
 
     def build(self, input_shape):
         # Used purely for shape validation.
-        if not isinstance(input_shape[0], tuple) or len(input_shape) != 2:
+        if (
+            not isinstance(input_shape[0], (tuple, list))
+            or len(input_shape) != 2
+        ):
             raise ValueError(
                 f"A `Dot` layer should be called on a list of 2 inputs. "
                 f"Received: input_shape={input_shape}"
             )
         shape1 = input_shape[0]
         shape2 = input_shape[1]
         if shape1 is None or shape2 is None:
@@ -359,15 +362,15 @@
 
     Args:
         inputs: A list of input tensors (at least 2).
         axes: Integer or tuple of integers,
             axis or axes along which to take the dot product.
         normalize: Whether to L2-normalize samples along the
             dot product axis before taking the dot product.
-            If set to True, then the output of the dot product
+            If set to `True`, then the output of the dot product
             is the cosine proximity between the two samples.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
         A tensor, the dot product of the samples from the inputs.
     """
     return Dot(axes=axes, **kwargs)(inputs)
```

### Comparing `keras-3.1.1/keras/src/layers/merging/maximum.py` & `keras-3.2.0/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/minimum.py` & `keras-3.2.0/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/multiply.py` & `keras-3.2.0/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/merging/subtract.py` & `keras-3.2.0/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/normalization/batch_normalization.py` & `keras-3.2.0/keras/src/layers/normalization/batch_normalization.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,35 +172,39 @@
             self.gamma = self.add_weight(
                 shape=shape,
                 name="gamma",
                 initializer=self.gamma_initializer,
                 regularizer=self.gamma_regularizer,
                 constraint=self.gamma_constraint,
                 trainable=True,
+                autocast=False,
             )
         if self.center:
             self.beta = self.add_weight(
                 shape=shape,
                 name="beta",
                 initializer=self.beta_initializer,
                 regularizer=self.beta_regularizer,
                 constraint=self.beta_constraint,
                 trainable=True,
+                autocast=False,
             )
         self.moving_mean = self.add_weight(
             shape=shape,
             name="moving_mean",
             initializer=self.moving_mean_initializer,
             trainable=False,
+            autocast=False,
         )
         self.moving_variance = self.add_weight(
             shape=shape,
             name="moving_variance",
             initializer=self.moving_variance_initializer,
             trainable=False,
+            autocast=False,
         )
         self.input_spec = InputSpec(
             ndim=len(input_shape), axes={self.axis: input_shape[self.axis]}
         )
         reduction_axes = list(range(len(input_shape)))
         del reduction_axes[self.axis]
         self._reduction_axes = reduction_axes
@@ -213,32 +217,23 @@
         input_dtype = standardize_dtype(inputs.dtype)
         if input_dtype in ("float16", "bfloat16"):
             # BN is prone to overflowing for float16/bfloat16 inputs, so we opt
             # out BN for mixed precision.
             inputs = ops.cast(inputs, "float32")
 
         if training and self.trainable:
-            mean, variance = self._moments(
-                inputs,
-                mask,
-            )
+            mean, variance = self._moments(inputs, mask)
             moving_mean = ops.cast(self.moving_mean, inputs.dtype)
             moving_variance = ops.cast(self.moving_variance, inputs.dtype)
             self.moving_mean.assign(
-                ops.cast(
-                    moving_mean * self.momentum + mean * (1.0 - self.momentum),
-                    inputs.dtype,
-                )
+                moving_mean * self.momentum + mean * (1.0 - self.momentum)
             )
             self.moving_variance.assign(
-                ops.cast(
-                    moving_variance * self.momentum
-                    + variance * (1.0 - self.momentum),
-                    inputs.dtype,
-                )
+                moving_variance * self.momentum
+                + variance * (1.0 - self.momentum)
             )
         else:
             moving_mean = ops.cast(self.moving_mean, inputs.dtype)
             moving_variance = ops.cast(self.moving_variance, inputs.dtype)
             mean = moving_mean
             variance = moving_variance
```

### Comparing `keras-3.1.1/keras/src/layers/normalization/group_normalization.py` & `keras-3.2.0/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/normalization/layer_normalization.py` & `keras-3.2.0/keras/src/layers/normalization/layer_normalization.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,26 +154,28 @@
             self.gamma = self.add_weight(
                 name="gamma",
                 shape=shape,
                 initializer=self.gamma_initializer,
                 regularizer=self.gamma_regularizer,
                 constraint=self.gamma_constraint,
                 trainable=True,
+                autocast=False,
             )
         else:
             self.gamma = None
 
         if self.center and not self.rms_scaling:
             self.beta = self.add_weight(
                 name="beta",
                 shape=shape,
                 initializer=self.beta_initializer,
                 regularizer=self.beta_regularizer,
                 constraint=self.beta_constraint,
                 trainable=True,
+                autocast=False,
             )
         else:
             self.beta = None
 
         self.built = True
 
     def call(self, inputs):
```

### Comparing `keras-3.1.1/keras/src/layers/normalization/spectral_normalization.py` & `keras-3.2.0/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/normalization/unit_normalization.py` & `keras-3.2.0/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/average_pooling1d.py` & `keras-3.2.0/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/average_pooling2d.py` & `keras-3.2.0/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/average_pooling3d.py` & `keras-3.2.0/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/base_global_pooling.py` & `keras-3.2.0/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/base_pooling.py` & `keras-3.2.0/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-3.2.0/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-3.2.0/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-3.2.0/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-3.2.0/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-3.2.0/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-3.2.0/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/max_pooling1d.py` & `keras-3.2.0/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/max_pooling2d.py` & `keras-3.2.0/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/pooling/max_pooling3d.py` & `keras-3.2.0/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-3.2.0/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/category_encoding.py` & `keras-3.2.0/keras/src/layers/preprocessing/category_encoding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from keras.src.api_export import keras_export
+from keras.src.backend import KerasTensor
 from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
 from keras.src.utils import backend_utils
 
 
 @keras_export("keras.layers.CategoryEncoding")
 class CategoryEncoding(TFDataLayer):
     """A preprocessing layer which encodes integer features.
@@ -69,23 +70,27 @@
                     `(..., num_tokens)`.
                 - `"count"`: Like `"multi_hot"`, but the int array contains a
                     count of the number of times the token at that index
                     appeared in the sample.
             For all output modes, currently only output up to rank 2 is
             supported.
             Defaults to `"multi_hot"`.
+        sparse: Whether to return a sparse tensor; for backends that support
+            sparse tensors.
 
     Call arguments:
         inputs: A 1D or 2D tensor of integer inputs.
         count_weights: A tensor in the same shape as `inputs` indicating the
             weight for each sample value when summing up in `count` mode.
             Not used in `"multi_hot"` or `"one_hot"` modes.
     """
 
-    def __init__(self, num_tokens=None, output_mode="multi_hot", **kwargs):
+    def __init__(
+        self, num_tokens=None, output_mode="multi_hot", sparse=False, **kwargs
+    ):
         super().__init__(**kwargs)
 
         # Support deprecated names for output_modes.
         if output_mode == "binary":
             output_mode = "multi_hot"
 
         # 'output_mode' must be one of ("count", "one_hot", "multi_hot")
@@ -100,22 +105,34 @@
             )
         if num_tokens < 1:
             raise ValueError(
                 f"`num_tokens` must be >= 1. Received: num_tokens={num_tokens}."
             )
         self.num_tokens = num_tokens
         self.output_mode = output_mode
+        self.sparse = sparse
         self._allow_non_tensor_positional_args = True
         self._convert_input_args = False
 
     def _count(self, inputs, axis=-1, count_weights=None):
+        # We don't use `ops.bincount` here because its output has a dynamic
+        # shape (the last dimension is calculated from the highest value of
+        # `inputs`). Instead, we reimplement a narrower use case where
+        # `minlength` and `maxlength` (not supported by `ops.bincount`) are a
+        # static value and the same value of `self.num_tokens`. Also, we don't
+        # need to support indices that are negative or greater than
+        # `self.num_tokens`.
         reduction_axis = 1 if len(inputs.shape) > 1 else 0
 
         one_hot_encoding = self.backend.nn.one_hot(
-            inputs, self.num_tokens, axis=axis, dtype=self.dtype
+            inputs,
+            self.num_tokens,
+            axis=axis,
+            dtype=self.dtype,
+            sparse=self.sparse,
         )
         if count_weights is not None:
             split_weights = self.backend.numpy.split(
                 count_weights,
                 count_weights.shape[reduction_axis],
                 reduction_axis,
             )
@@ -128,34 +145,49 @@
             one_hot_encoding,
             axis=reduction_axis,
         )
         return outputs
 
     def _encode(self, inputs, count_weights=None):
         if self.output_mode == "multi_hot":
-            outputs = self.backend.nn.multi_hot(
-                inputs, self.num_tokens, dtype=self.dtype
+            return self.backend.nn.multi_hot(
+                inputs, self.num_tokens, dtype=self.dtype, sparse=self.sparse
             )
         elif self.output_mode == "one_hot":
-            outputs = self.backend.nn.one_hot(
-                inputs, self.num_tokens, dtype=self.dtype
+            return self.backend.nn.one_hot(
+                inputs, self.num_tokens, dtype=self.dtype, sparse=self.sparse
             )
         elif self.output_mode == "count":
-            outputs = self._count(inputs, count_weights=count_weights)
-
-        return outputs
+            return self._count(inputs, count_weights=count_weights)
 
     def compute_output_shape(self, input_shape):
+        # Treat rank-0 inputs inconsistent with actual output .
+        if (input_shape is not None) & (len(input_shape) == 0):
+            # If output_mode == "multi_hot" return same shape .
+            if self.output_mode == "multi_hot":
+                return input_shape
+            # If output_mode == "one_hot" append num_tokens to shape .
+            # This is inline with actual output .
+            elif self.output_mode == "one_hot":
+                return (self.num_tokens,)
         if self.output_mode == "one_hot":
             if input_shape[-1] != 1:
                 return tuple(input_shape + (self.num_tokens,))
+            elif len(input_shape) == 1:
+                return tuple(input_shape + (self.num_tokens,))
             else:
                 return tuple(input_shape[:-1] + (self.num_tokens,))
         return tuple(input_shape[:-1] + (self.num_tokens,))
 
+    def compute_output_spec(self, inputs, count_weights=None):
+        output_shape = self.compute_output_shape(inputs.shape)
+        return KerasTensor(
+            output_shape, dtype=self.compute_dtype, sparse=self.sparse
+        )
+
     def get_config(self):
         config = {
             "num_tokens": self.num_tokens,
             "output_mode": self.output_mode,
         }
         base_config = super().get_config()
         return {**base_config, **config}
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/center_crop.py` & `keras-3.2.0/keras/src/layers/preprocessing/center_crop.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,21 @@
             [self.height, self.width],
             data_format=self.data_format,
             backend_module=self.backend,
         )
 
     def compute_output_shape(self, input_shape):
         input_shape = list(input_shape)
+        if isinstance(input_shape[0], (list, tuple)) or len(
+            input_shape
+        ) not in (3, 4):
+            raise ValueError(
+                "`input_shape` must be a non-nested tuple or list "
+                "of rank-1 with size 3 (unbatched) or 4 (batched). "
+            )
         if len(input_shape) == 4:
             if self.data_format == "channels_last":
                 input_shape[1] = self.height
                 input_shape[2] = self.width
             else:
                 input_shape[2] = self.height
                 input_shape[3] = self.width
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/discretization.py` & `keras-3.2.0/keras/src/layers/preprocessing/discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,19 @@
         if dtype is None:
             dtype = "int64" if output_mode == "int" else backend.floatx()
 
         super().__init__(name=name, dtype=dtype)
 
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
-                "`sparse` can only be set to True with the "
-                "TensorFlow backend."
+                "`sparse=True` can only be used with the " "TensorFlow backend."
             )
         if sparse and output_mode == "int":
             raise ValueError(
-                "`sparse` may only be true if `output_mode` is "
+                "`sparse=True` may only be used if `output_mode` is "
                 "`'one_hot'`, `'multi_hot'`, or `'count'`. "
                 f"Received: sparse={sparse} and "
                 f"output_mode={output_mode}"
             )
 
         argument_validation.validate_string_arg(
             output_mode,
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/feature_space.py` & `keras-3.2.0/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-3.2.0/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,15 @@
 
         if output_mode == "int" and dtype is None:
             dtype = "int64"
 
         super().__init__(name=name, dtype=dtype)
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
-                "`sparse` can only be set to True with the "
-                "TensorFlow backend."
+                "`sparse=True` can only be used with the " "TensorFlow backend."
             )
 
         argument_validation.validate_string_arg(
             output_mode,
             allowable_strings=("int", "one_hot"),
             caller_name=self.__class__.__name__,
             arg_name="output_mode",
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/hashing.py` & `keras-3.2.0/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/index_lookup.py` & `keras-3.2.0/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/integer_lookup.py` & `keras-3.2.0/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,30 +314,29 @@
             raise ImportError(
                 "Layer IntegerLookup requires TensorFlow. "
                 "Install it via `pip install tensorflow`."
             )
         if max_tokens is not None and max_tokens <= 1:
             raise ValueError(
                 "If `max_tokens` is set for `IntegerLookup`, it must be "
-                f"greater than 1. Received: max_tokens={max_tokens}."
+                f"greater than 1. Received: max_tokens={max_tokens}"
             )
         if num_oov_indices < 0:
             raise ValueError(
                 "The value of `num_oov_indices` argument for `IntegerLookup` "
-                "must >= 0. Received num_oov_indices="
-                f"{num_oov_indices}."
+                "must >= 0. Received: num_oov_indices="
+                f"{num_oov_indices}"
             )
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
-                "`sparse` can only be set to True with the "
-                "TensorFlow backend."
+                "`sparse=True` can only be used with the " "TensorFlow backend."
             )
         if vocabulary_dtype != "int64":
             raise ValueError(
-                "Only vocabulary_dtype='int64' is supported "
+                "Only `vocabulary_dtype='int64'` is supported "
                 "at this time. Received: "
                 f"vocabulary_dtype={vocabulary_dtype}"
             )
         super().__init__(
             max_tokens=max_tokens,
             num_oov_indices=num_oov_indices,
             mask_token=mask_token,
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/normalization.py` & `keras-3.2.0/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_brightness.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_brightness.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Output: 3D (HWC) or 4D (NHWC) tensor with brightness adjusted based on the
         `factor`. By default, the layer will output floats.
         The output value will be clipped to the range `[0, 255]`,
         the valid range of RGB colors, and
         rescaled based on the `value_range` if needed.
 
-    Sample usage:
+    Example:
 
     ```python
     random_bright = keras.layers.RandomBrightness(factor=0.2)
 
     # An image with shape [2, 2, 3]
     image = [[[1, 2, 3], [4 ,5 ,6]], [[7, 8, 9], [10, 11, 12]]]
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_contrast.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_crop.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 
     def __init__(
         self, height, width, seed=None, data_format=None, name=None, **kwargs
     ):
         super().__init__(name=name, **kwargs)
         self.height = height
         self.width = width
-        self.seed = seed or backend.random.make_default_seed()
+        self.seed = (
+            seed if seed is not None else backend.random.make_default_seed()
+        )
         self.generator = SeedGenerator(seed)
         self.data_format = backend.standardize_data_format(data_format)
 
         if self.data_format == "channels_first":
             self.height_axis = -2
             self.width_axis = -1
         elif self.data_format == "channels_last":
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_flip.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_rotation.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """A preprocessing layer which randomly rotates images during training.
 
     This layer will apply random rotations to each image, filling empty space
     according to `fill_mode`.
 
     By default, random rotations are only applied during training.
     At inference time, the layer does nothing. If you need to apply random
-    rotations at inference time, set `training` to True when calling the layer.
+    rotations at inference time, pass `training=True` when calling the layer.
 
     Input pixel values can be of any range (e.g. `[0., 1.)` or `[0, 255]`) and
     of integer or floating point dtype.
     By default, the layer will output floats.
 
     **Note:** This layer is safe to use inside a `tf.data` pipeline
     (independently of which backend you're using).
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_translation.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/random_zoom.py` & `keras-3.2.0/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/rescaling.py` & `keras-3.2.0/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/resizing.py` & `keras-3.2.0/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/string_lookup.py` & `keras-3.2.0/keras/src/layers/preprocessing/string_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,16 +310,15 @@
         if not tf.available:
             raise ImportError(
                 "Layer StringLookup requires TensorFlow. "
                 "Install it via `pip install tensorflow`."
             )
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
-                "`sparse` can only be set to True with the "
-                "TensorFlow backend."
+                "`sparse=True` can only be used with the " "TensorFlow backend."
             )
         super().__init__(
             max_tokens=max_tokens,
             num_oov_indices=num_oov_indices,
             mask_token=mask_token,
             oov_token=oov_token,
             vocabulary=vocabulary,
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/text_vectorization.py` & `keras-3.2.0/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,21 +222,19 @@
         if not tf.available:
             raise ImportError(
                 "Layer TextVectorization requires TensorFlow. "
                 "Install it via `pip install tensorflow`."
             )
         if sparse and backend.backend() != "tensorflow":
             raise ValueError(
-                "`sparse` can only be set to True with the "
-                "TensorFlow backend."
+                "`sparse=True` can only be used with the " "TensorFlow backend."
             )
         if ragged and backend.backend() != "tensorflow":
             raise ValueError(
-                "`ragged` can only be set to True with the "
-                "TensorFlow backend."
+                "`ragged=True` can only be used with the " "TensorFlow backend."
             )
 
         # 'standardize' must be one of
         # (None, "lower_and_strip_punctuation", "lower", "strip_punctuation",
         # callable)
         argument_validation.validate_string_arg(
             standardize,
```

### Comparing `keras-3.1.1/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-3.2.0/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/regularization/activity_regularization.py` & `keras-3.2.0/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/regularization/alpha_dropout.py` & `keras-3.2.0/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/regularization/dropout.py` & `keras-3.2.0/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/regularization/gaussian_dropout.py` & `keras-3.2.0/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     def call(self, inputs, training=False):
         if training and self.rate > 0:
             stddev = math.sqrt(self.rate / (1.0 - self.rate))
             return inputs * backend.random.normal(
                 shape=ops.shape(inputs),
                 mean=1.0,
                 stddev=stddev,
+                dtype=self.compute_dtype,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
```

### Comparing `keras-3.1.1/keras/src/layers/regularization/gaussian_noise.py` & `keras-3.2.0/keras/src/layers/regularization/gaussian_noise.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     def call(self, inputs, training=False):
         if training and self.stddev > 0:
             return inputs + backend.random.normal(
                 shape=ops.shape(inputs),
                 mean=0.0,
                 stddev=self.stddev,
+                dtype=self.compute_dtype,
                 seed=self.seed_generator,
             )
         return inputs
 
     def compute_output_shape(self, input_shape):
         return input_shape
```

### Comparing `keras-3.1.1/keras/src/layers/regularization/spatial_dropout.py` & `keras-3.2.0/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/cropping1d.py` & `keras-3.2.0/keras/src/layers/reshaping/cropping1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @keras_export("keras.layers.Cropping1D")
 class Cropping1D(Layer):
     """Cropping layer for 1D input (e.g. temporal sequence).
 
     It crops along the time dimension (axis 1).
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 3, 2)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> x
     [[[ 0  1]
       [ 2  3]
       [ 4  5]]
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/cropping2d.py` & `keras-3.2.0/keras/src/layers/reshaping/cropping2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 @keras_export("keras.layers.Cropping2D")
 class Cropping2D(Layer):
     """Cropping layer for 2D input (e.g. picture).
 
     It crops along spatial dimensions, i.e. height and width.
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 28, 28, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> y = keras.layers.Cropping2D(cropping=((2, 2), (4, 4)))(x)
     >>> y.shape
     (2, 24, 20, 3)
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/cropping3d.py` & `keras-3.2.0/keras/src/layers/reshaping/cropping3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from keras.src.utils import argument_validation
 
 
 @keras_export("keras.layers.Cropping3D")
 class Cropping3D(Layer):
     """Cropping layer for 3D data (e.g. spatial or spatio-temporal).
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 28, 28, 10, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> y = keras.layers.Cropping3D(cropping=(2, 4, 2))(x)
     >>> y.shape
     (2, 24, 20, 6, 3)
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/flatten.py` & `keras-3.2.0/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/permute.py` & `keras-3.2.0/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/repeat_vector.py` & `keras-3.2.0/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/reshape.py` & `keras-3.2.0/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/up_sampling1d.py` & `keras-3.2.0/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 @keras_export("keras.layers.UpSampling1D")
 class UpSampling1D(Layer):
     """Upsampling layer for 1D inputs.
 
     Repeats each temporal step `size` times along the time axis.
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 2, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> x
     [[[ 0  1  2]
       [ 3  4  5]]
      [[ 6  7  8]
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/up_sampling2d.py` & `keras-3.2.0/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class UpSampling2D(Layer):
     """Upsampling layer for 2D inputs.
 
     The implementation uses interpolative resizing, given the resize method
     (specified by the `interpolation` argument). Use `interpolation=nearest`
     to repeat the rows and columns of the data.
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 2, 1, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> print(x)
     [[[[ 0  1  2]]
       [[ 3  4  5]]]
      [[[ 6  7  8]]
@@ -136,19 +136,15 @@
             data_format: One of `"channels_first"`, `"channels_last"`.
             interpolation: A string, one of `"bicubic"`, `"bilinear"`,
             `"lanczos3"`, `"lanczos5"`, or `"nearest"`.
 
         Returns:
             A tensor.
         """
-        if data_format == "channels_first":
-            rows, cols = 2, 3
-        elif data_format == "channels_last":
-            rows, cols = 1, 2
-        else:
+        if data_format not in {"channels_last", "channels_first"}:
             raise ValueError(f"Invalid `data_format` argument: {data_format}")
 
         if data_format == "channels_first":
             x = ops.transpose(x, [0, 2, 3, 1])
         # https://github.com/keras-team/keras/issues/294
         # Use `ops.repeat` for `nearest` interpolation
         if interpolation == "nearest":
@@ -159,16 +155,16 @@
             # by hand (versus using element-wise multiplication
             # by np.array([height_factor, width_factor]) then
             # list-ifying the tensor by calling `.tolist()`)
             # since when running under torchdynamo, `new_shape`
             # will be traced as a symbolic variable (specifically
             # a `FakeTensor`) which does not have a `tolist()` method.
             new_shape = (
-                x.shape[rows] * height_factor,
-                x.shape[cols] * width_factor,
+                x.shape[1] * height_factor,
+                x.shape[2] * width_factor,
             )
             x = ops.image.resize(x, new_shape, interpolation=interpolation)
         if data_format == "channels_first":
             x = ops.transpose(x, [0, 3, 1, 2])
 
         return x
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/up_sampling3d.py` & `keras-3.2.0/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/reshaping/zero_padding1d.py` & `keras-3.2.0/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from keras.src.utils import argument_validation
 
 
 @keras_export("keras.layers.ZeroPadding1D")
 class ZeroPadding1D(Layer):
     """Zero-padding layer for 1D input (e.g. temporal sequence).
 
-    Examples:
+    Example:
 
     >>> input_shape = (2, 2, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> x
     [[[ 0  1  2]
       [ 3  4  5]]
      [[ 6  7  8]
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/zero_padding2d.py` & `keras-3.2.0/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 @keras_export("keras.layers.ZeroPadding2D")
 class ZeroPadding2D(Layer):
     """Zero-padding layer for 2D input (e.g. picture).
 
     This layer can add rows and columns of zeros at the top, bottom, left and
     right side of an image tensor.
 
-    Examples:
+    Example:
 
     >>> input_shape = (1, 1, 2, 2)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> x
     [[[[0 1]
        [2 3]]]]
     >>> y = keras.layers.ZeroPadding2D(padding=1)(x)
```

### Comparing `keras-3.1.1/keras/src/layers/reshaping/zero_padding3d.py` & `keras-3.2.0/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from keras.src.utils import argument_validation
 
 
 @keras_export("keras.layers.ZeroPadding3D")
 class ZeroPadding3D(Layer):
     """Zero-padding layer for 3D data (spatial or spatio-temporal).
 
-    Examples:
+    Example:
 
     >>> input_shape = (1, 1, 2, 2, 3)
     >>> x = np.arange(np.prod(input_shape)).reshape(input_shape)
     >>> y = keras.layers.ZeroPadding3D(padding=2)(x)
     >>> y.shape
     (1, 5, 6, 6, 3)
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/bidirectional.py` & `keras-3.2.0/keras/src/layers/rnn/bidirectional.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,21 +178,21 @@
             output_shape, state_shape = output_shape[0], output_shape[1:]
 
         if self.merge_mode == "concat":
             output_shape = list(output_shape)
             output_shape[-1] *= 2
             output_shape = tuple(output_shape)
         elif self.merge_mode is None:
-            output_shape = [output_shape, copy.copy(output_shape)]
+            output_shape = [output_shape, output_shape]
 
         if self.return_state:
             if self.merge_mode is None:
-                return output_shape + state_shape + copy.copy(state_shape)
-            return [output_shape] + state_shape + copy.copy(state_shape)
-        return output_shape
+                return tuple(output_shape) + state_shape + state_shape
+            return tuple([output_shape]) + (state_shape) + (state_shape)
+        return tuple(output_shape)
 
     def call(
         self,
         sequences,
         initial_state=None,
         mask=None,
         training=None,
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/conv_lstm.py` & `keras-3.2.0/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/conv_lstm1d.py` & `keras-3.2.0/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/conv_lstm2d.py` & `keras-3.2.0/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/conv_lstm3d.py` & `keras-3.2.0/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-3.2.0/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def get_recurrent_dropout_mask(self, step_input):
         if not hasattr(self, "_recurrent_dropout_mask"):
             self._recurrent_dropout_mask = None
         if self._recurrent_dropout_mask is None and self.recurrent_dropout > 0:
             ones = ops.ones_like(step_input)
             self._recurrent_dropout_mask = backend.random.dropout(
-                ones, rate=self.dropout, seed=self.seed_generator
+                ones, rate=self.recurrent_dropout, seed=self.seed_generator
             )
         return self._recurrent_dropout_mask
 
     def reset_dropout_mask(self):
         """Reset the cached dropout mask if any.
 
         The RNN layer invokes this in the `call()` method
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/gru.py` & `keras-3.2.0/keras/src/layers/rnn/gru.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,17 @@
             else a symbolic loop will be used.
             Unrolling can speed-up a RNN,
             although it tends to be more memory-intensive.
             Unrolling is only suitable for short sequences.
         reset_after: GRU convention (whether to apply reset gate after or
             before matrix multiplication). `False` is `"before"`,
             `True` is `"after"` (default and cuDNN compatible).
+        use_cudnn: Whether to use a cuDNN-backed implementation. `"auto"` will
+            attempt to use cuDNN when feasible, and will fallback to the
+            default implementation if not.
 
     Call arguments:
         inputs: A 3D tensor, with shape `(batch, timesteps, feature)`.
         mask: Binary tensor of shape `(samples, timesteps)` indicating whether
             a given timestep should be masked  (optional).
             An individual `True` entry indicates that the corresponding timestep
             should be utilized, while a `False` entry indicates that the
@@ -469,14 +472,15 @@
         seed=None,
         return_sequences=False,
         return_state=False,
         go_backwards=False,
         stateful=False,
         unroll=False,
         reset_after=True,
+        use_cudnn="auto",
         **kwargs,
     ):
         cell = GRUCell(
             units,
             activation=activation,
             recurrent_activation=recurrent_activation,
             use_bias=use_bias,
@@ -504,56 +508,74 @@
             go_backwards=go_backwards,
             stateful=stateful,
             unroll=unroll,
             activity_regularizer=activity_regularizer,
             **kwargs,
         )
         self.input_spec = InputSpec(ndim=3)
-        if backend.backend() == "tensorflow" and backend.cudnn_ok(
-            cell.activation,
-            cell.recurrent_activation,
-            self.unroll,
-            cell.use_bias,
-            reset_after=reset_after,
+        if use_cudnn not in ("auto", True, False):
+            raise ValueError(
+                "Invalid valid received for argument `use_cudnn`. "
+                "Expected one of {'auto', True, False}. "
+                f"Received: use_cudnn={use_cudnn}"
+            )
+        self.use_cudnn = use_cudnn
+        if (
+            backend.backend() == "tensorflow"
+            and backend.cudnn_ok(
+                cell.activation,
+                cell.recurrent_activation,
+                self.unroll,
+                cell.use_bias,
+                reset_after=reset_after,
+            )
+            and use_cudnn in (True, "auto")
         ):
             self.supports_jit = False
 
     def inner_loop(self, sequences, initial_state, mask, training=False):
         if tree.is_nested(initial_state):
             initial_state = initial_state[0]
         if tree.is_nested(mask):
             mask = mask[0]
-
-        if not self.dropout and not self.recurrent_dropout:
-            try:
-                # Backends are allowed to specify (optionally) optimized
-                # implementation of the inner GRU loop. In the case of
-                # TF for instance, it will leverage cuDNN when feasible, and
-                # it will raise NotImplementedError otherwise.
-                out = backend.gru(
-                    sequences,
-                    initial_state,
-                    mask,
-                    kernel=self.cell.kernel,
-                    recurrent_kernel=self.cell.recurrent_kernel,
-                    bias=self.cell.bias,
-                    activation=self.cell.activation,
-                    recurrent_activation=self.cell.recurrent_activation,
-                    return_sequences=self.return_sequences,
-                    go_backwards=self.go_backwards,
-                    unroll=self.unroll,
-                    reset_after=self.cell.reset_after,
-                )
-                # We disable jit_compile for the model in this case,
-                # since cuDNN ops aren't XLA compatible.
-                if backend.backend() == "tensorflow":
-                    self.supports_jit = False
-                return out
-            except NotImplementedError:
-                pass
+        if self.use_cudnn in ("auto", True):
+            if not self.dropout and not self.recurrent_dropout:
+                try:
+                    # Backends are allowed to specify (optionally) optimized
+                    # implementation of the inner GRU loop. In the case of
+                    # TF for instance, it will leverage cuDNN when feasible, and
+                    # it will raise NotImplementedError otherwise.
+                    out = backend.gru(
+                        sequences,
+                        initial_state,
+                        mask,
+                        kernel=self.cell.kernel,
+                        recurrent_kernel=self.cell.recurrent_kernel,
+                        bias=self.cell.bias,
+                        activation=self.cell.activation,
+                        recurrent_activation=self.cell.recurrent_activation,
+                        return_sequences=self.return_sequences,
+                        go_backwards=self.go_backwards,
+                        unroll=self.unroll,
+                        reset_after=self.cell.reset_after,
+                    )
+                    # We disable jit_compile for the model in this case,
+                    # since cuDNN ops aren't XLA compatible.
+                    if backend.backend() == "tensorflow":
+                        self.supports_jit = False
+                    return out
+                except NotImplementedError:
+                    pass
+        if self.use_cudnn is True:
+            raise ValueError(
+                "use_cudnn=True was specified, "
+                "but cuDNN is not supported for this layer configuration "
+                "with this backend. Pass use_cudnn='auto' to fallback "
+                "to a non-cuDNN implementation."
+            )
         return super().inner_loop(
             sequences, initial_state, mask=mask, training=training
         )
 
     def call(self, sequences, initial_state=None, mask=None, training=False):
         return super().call(
             sequences, mask=mask, training=training, initial_state=initial_state
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/lstm.py` & `keras-3.2.0/keras/src/layers/rnn/lstm.py`

 * *Files 6% similar despite different names*

```diff
@@ -408,14 +408,17 @@
             state for the sample of index i in the following batch.
         unroll: Boolean (default False).
             If `True`, the network will be unrolled,
             else a symbolic loop will be used.
             Unrolling can speed-up a RNN,
             although it tends to be more memory-intensive.
             Unrolling is only suitable for short sequences.
+        use_cudnn: Whether to use a cuDNN-backed implementation. `"auto"` will
+            attempt to use cuDNN when feasible, and will fallback to the
+            default implementation if not.
 
     Call arguments:
         inputs: A 3D tensor, with shape `(batch, timesteps, feature)`.
         mask: Binary tensor of shape `(samples, timesteps)` indicating whether
             a given timestep should be masked  (optional).
             An individual `True` entry indicates that the corresponding timestep
             should be utilized, while a `False` entry indicates that the
@@ -450,14 +453,15 @@
         recurrent_dropout=0.0,
         seed=None,
         return_sequences=False,
         return_state=False,
         go_backwards=False,
         stateful=False,
         unroll=False,
+        use_cudnn="auto",
         **kwargs,
     ):
         cell = LSTMCell(
             units,
             activation=activation,
             recurrent_activation=recurrent_activation,
             use_bias=use_bias,
@@ -486,53 +490,72 @@
             go_backwards=go_backwards,
             stateful=stateful,
             unroll=unroll,
             activity_regularizer=activity_regularizer,
             **kwargs,
         )
         self.input_spec = InputSpec(ndim=3)
-        if backend.backend() == "tensorflow" and backend.cudnn_ok(
-            cell.activation,
-            cell.recurrent_activation,
-            self.unroll,
-            cell.use_bias,
+        if use_cudnn not in ("auto", True, False):
+            raise ValueError(
+                "Invalid valid received for argument `use_cudnn`. "
+                "Expected one of {'auto', True, False}. "
+                f"Received: use_cudnn={use_cudnn}"
+            )
+        self.use_cudnn = use_cudnn
+        if (
+            backend.backend() == "tensorflow"
+            and backend.cudnn_ok(
+                cell.activation,
+                cell.recurrent_activation,
+                self.unroll,
+                cell.use_bias,
+            )
+            and use_cudnn in (True, "auto")
         ):
             self.supports_jit = False
 
     def inner_loop(self, sequences, initial_state, mask, training=False):
         if tree.is_nested(mask):
             mask = mask[0]
 
-        if not self.dropout and not self.recurrent_dropout:
-            try:
-                # Backends are allowed to specify (optionally) optimized
-                # implementation of the inner LSTM loop. In the case of
-                # TF for instance, it will leverage cuDNN when feasible, and
-                # it will raise NotImplementedError otherwise.
-                out = backend.lstm(
-                    sequences,
-                    initial_state[0],
-                    initial_state[1],
-                    mask,
-                    kernel=self.cell.kernel,
-                    recurrent_kernel=self.cell.recurrent_kernel,
-                    bias=self.cell.bias,
-                    activation=self.cell.activation,
-                    recurrent_activation=self.cell.recurrent_activation,
-                    return_sequences=self.return_sequences,
-                    go_backwards=self.go_backwards,
-                    unroll=self.unroll,
-                )
-                # We disable jit_compile for the model in this case,
-                # since cuDNN ops aren't XLA compatible.
-                if backend.backend() == "tensorflow":
-                    self.supports_jit = False
-                return out
-            except NotImplementedError:
-                pass
+        if self.use_cudnn in ("auto", True):
+            if not self.dropout and not self.recurrent_dropout:
+                try:
+                    # Backends are allowed to specify (optionally) optimized
+                    # implementation of the inner LSTM loop. In the case of
+                    # TF for instance, it will leverage cuDNN when feasible, and
+                    # it will raise NotImplementedError otherwise.
+                    out = backend.lstm(
+                        sequences,
+                        initial_state[0],
+                        initial_state[1],
+                        mask,
+                        kernel=self.cell.kernel,
+                        recurrent_kernel=self.cell.recurrent_kernel,
+                        bias=self.cell.bias,
+                        activation=self.cell.activation,
+                        recurrent_activation=self.cell.recurrent_activation,
+                        return_sequences=self.return_sequences,
+                        go_backwards=self.go_backwards,
+                        unroll=self.unroll,
+                    )
+                    # We disable jit_compile for the model in this case,
+                    # since cuDNN ops aren't XLA compatible.
+                    if backend.backend() == "tensorflow":
+                        self.supports_jit = False
+                    return out
+                except NotImplementedError:
+                    pass
+        if self.use_cudnn is True:
+            raise ValueError(
+                "use_cudnn=True was specified, "
+                "but cuDNN is not supported for this layer configuration "
+                "with this backend. Pass use_cudnn='auto' to fallback "
+                "to a non-cuDNN implementation."
+            )
         return super().inner_loop(
             sequences, initial_state, mask=mask, training=training
         )
 
     def call(self, sequences, initial_state=None, mask=None, training=False):
         return super().call(
             sequences, mask=mask, training=training, initial_state=initial_state
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/rnn.py` & `keras-3.2.0/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/simple_rnn.py` & `keras-3.2.0/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-3.2.0/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """Wrapper allowing a stack of RNN cells to behave as a single cell.
 
     Used to implement efficient stacked RNNs.
 
     Args:
       cells: List of RNN cell instances.
 
-    Examples:
+    Example:
 
     ```python
     batch_size = 3
     sentence_length = 5
     num_features = 2
     new_shape = (batch_size, sentence_length, num_features)
     x = np.reshape(np.arange(30), new_shape)
```

### Comparing `keras-3.1.1/keras/src/layers/rnn/time_distributed.py` & `keras-3.2.0/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/backend.py` & `keras-3.2.0/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/layers.py` & `keras-3.2.0/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/losses.py` & `keras-3.2.0/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/preprocessing/image.py` & `keras-3.2.0/keras/src/legacy/preprocessing/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1183,22 +1183,22 @@
                 "has_ext is deprecated, filenames in the dataframe have "
                 "to match the exact filenames in disk.",
                 DeprecationWarning,
             )
         if "sort" in kwargs:
             warnings.warn(
                 "sort is deprecated, batches will be created in the"
-                "same order than the filenames provided if shuffle"
-                "is set to False.",
+                "same order than the filenames provided if `shuffle`"
+                "is set to `False`.",
                 DeprecationWarning,
             )
         if class_mode == "other":
             warnings.warn(
-                '`class_mode` "other" is deprecated, please use '
-                '`class_mode` "raw".',
+                '`class_mode="other"` is deprecated, please use '
+                '`class_mode="raw"`.',
                 DeprecationWarning,
             )
             class_mode = "raw"
         if "drop_duplicates" in kwargs:
             warnings.warn(
                 "drop_duplicates is deprecated, you can drop duplicates "
                 "by using the pandas.DataFrame.drop_duplicates method.",
@@ -1462,15 +1462,16 @@
     def fit(self, x, augment=False, rounds=1, seed=None):
         """Fits the data generator to some sample data.
 
         This computes the internal data stats related to the
         data-dependent transformations, based on an array of sample data.
 
         Only required if `featurewise_center` or
-        `featurewise_std_normalization` or `zca_whitening` are set to True.
+        `featurewise_std_normalization` or `zca_whitening`
+        are set to `True`.
 
         When `rescale` is set to a value, rescaling is applied to
         sample data before computing the internal data stats.
 
         Args:
             x: Sample data. Should have rank 4.
              In case of grayscale data,
```

### Comparing `keras-3.1.1/keras/src/legacy/preprocessing/sequence.py` & `keras-3.2.0/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/preprocessing/text.py` & `keras-3.2.0/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/saving/json_utils.py` & `keras-3.2.0/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/saving/legacy_h5_format.py` & `keras-3.2.0/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             after loading.
 
     Returns:
         A Keras model instance. If an optimizer was found
         as part of the saved model, the model is already
         compiled. Otherwise, the model is uncompiled and
         a warning will be displayed. When `compile` is set
-        to False, the compilation is omitted without any
+        to `False`, the compilation is omitted without any
         warning.
 
     Raises:
         ImportError: if h5py is not available.
         ValueError: In case of an invalid savefile.
     """
     if h5py is None:
```

### Comparing `keras-3.1.1/keras/src/legacy/saving/saving_utils.py` & `keras-3.2.0/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/legacy/saving/serialization.py` & `keras-3.2.0/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/losses/__init__.py` & `keras-3.2.0/keras/src/losses/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from keras.src.api_export import keras_export
 from keras.src.losses.loss import Loss
 from keras.src.losses.losses import BinaryCrossentropy
+from keras.src.losses.losses import BinaryFocalCrossentropy
 from keras.src.losses.losses import CategoricalCrossentropy
+from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
+from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
 from keras.src.losses.losses import KLDivergence
 from keras.src.losses.losses import LogCosh
 from keras.src.losses.losses import LossFunctionWrapper
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
 from keras.src.losses.losses import binary_crossentropy
+from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
+from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
+from keras.src.losses.losses import dice
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
 from keras.src.losses.losses import kl_divergence
 from keras.src.losses.losses import log_cosh
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
@@ -38,46 +44,54 @@
     # Base
     Loss,
     LossFunctionWrapper,
     # Probabilistic
     KLDivergence,
     Poisson,
     BinaryCrossentropy,
+    BinaryFocalCrossentropy,
     CategoricalCrossentropy,
+    CategoricalFocalCrossentropy,
     SparseCategoricalCrossentropy,
     # Regression
     MeanSquaredError,
     MeanAbsoluteError,
     MeanAbsolutePercentageError,
     MeanSquaredLogarithmicError,
     CosineSimilarity,
     LogCosh,
     Huber,
     # Hinge
     Hinge,
     SquaredHinge,
     CategoricalHinge,
+    # Image segmentation
+    Dice,
     # Probabilistic
     kl_divergence,
     poisson,
     binary_crossentropy,
+    binary_focal_crossentropy,
     categorical_crossentropy,
+    categorical_focal_crossentropy,
     sparse_categorical_crossentropy,
     # Regression
     mean_squared_error,
     mean_absolute_error,
     mean_absolute_percentage_error,
     mean_squared_logarithmic_error,
     cosine_similarity,
     log_cosh,
     huber,
     # Hinge
     hinge,
     squared_hinge,
     categorical_hinge,
+    # Image segmentation
+    dice,
 }
 
 ALL_OBJECTS_DICT = {cls.__name__: cls for cls in ALL_OBJECTS}
 ALL_OBJECTS_DICT.update(
     {
         "bce": binary_crossentropy,
         "BCE": binary_crossentropy,
```

### Comparing `keras-3.1.1/keras/src/losses/loss.py` & `keras-3.2.0/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/losses/losses.py` & `keras-3.2.0/keras/src/losses/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1931,7 +1931,73 @@
     input_length = input_length * ops.ones((batch_length,), dtype="int32")
     label_length = label_length * ops.ones((batch_length,), dtype="int32")
 
     return ops.ctc_loss(
         y_true, y_pred, label_length, input_length, mask_index=0
     )
 
+
+@keras_export("keras.losses.Dice")
+class Dice(LossFunctionWrapper):
+    """Computes the Dice loss value between `y_true` and `y_pred`.
+
+    Formula:
+    ```python
+    loss = 1 - (2 * sum(y_true * y_pred)) / (sum(y_true) + sum(y_pred))
+    ```
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+
+    Returns:
+        Dice loss value.
+    """
+
+    def __init__(
+        self,
+        reduction="sum_over_batch_size",
+        name="dice",
+    ):
+        super().__init__(
+            dice,
+            name=name,
+            reduction=reduction,
+        )
+
+    def get_config(self):
+        return {
+            "name": self.name,
+            "reduction": self.reduction,
+        }
+
+
+@keras_export("keras.losses.dice")
+def dice(y_true, y_pred):
+    """Computes the Dice loss value between `y_true` and `y_pred`.
+
+    Formula:
+    ```python
+    loss = 1 - (2 * sum(y_true * y_pred)) / (sum(y_true) + sum(y_pred))
+    ```
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+
+    Returns:
+        Dice loss value.
+    """
+    y_pred = ops.convert_to_tensor(y_pred)
+    y_true = ops.cast(y_true, y_pred.dtype)
+
+    inputs = ops.reshape(y_true, [-1])
+    targets = ops.reshape(y_pred, [-1])
+
+    intersection = ops.sum(inputs * targets)
+    dice = ops.divide(
+        2.0 * intersection,
+        ops.sum(y_true) + ops.sum(y_pred) + backend.epsilon(),
+    )
+
+    return 1 - dice
+
```

### Comparing `keras-3.1.1/keras/src/metrics/__init__.py` & `keras-3.2.0/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/metrics/accuracy_metrics.py` & `keras-3.2.0/keras/src/metrics/accuracy_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     If `sample_weight` is `None`, weights default to 1.
     Use `sample_weight` of 0 to mask values.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Examples:
 
     >>> m = keras.metrics.Accuracy()
     >>> m.update_state([[1], [2], [3], [4]], [[0], [2], [3], [4]])
     >>> m.result()
     0.75
 
     >>> m.reset_state()
@@ -89,15 +89,15 @@
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
         threshold: (Optional) Float representing the threshold for deciding
         whether prediction values are 1 or 0.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.BinaryAccuracy()
     >>> m.update_state([[1], [1], [0], [0]], [[0.98], [1], [0], [0.6]])
     >>> m.result()
     0.75
 
     >>> m.reset_state()
@@ -188,15 +188,15 @@
     If `sample_weight` is `None`, weights default to 1.
     Use `sample_weight` of 0 to mask values.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.CategoricalAccuracy()
     >>> m.update_state([[0, 0, 1], [0, 1, 0]], [[0.1, 0.9, 0.8],
     ...                 [0.05, 0.95, 0]])
     >>> m.result()
     0.5
 
@@ -277,15 +277,15 @@
     If `sample_weight` is `None`, weights default to 1.
     Use `sample_weight` of 0 to mask values.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.SparseCategoricalAccuracy()
     >>> m.update_state([[2], [1]], [[0.1, 0.6, 0.3], [0.05, 0.95, 0]])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
@@ -348,15 +348,15 @@
 
     Args:
         k: (Optional) Number of top elements to look at for computing accuracy.
             Defaults to `5`.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.TopKCategoricalAccuracy(k=1)
     >>> m.update_state([[0, 0, 1], [0, 1, 0]],
     ...                [[0.1, 0.9, 0.8], [0.05, 0.95, 0]])
     >>> m.result()
     0.5
 
@@ -426,15 +426,15 @@
 
     Args:
         k: (Optional) Number of top elements to look at for computing accuracy.
             Defaults to `5`.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.SparseTopKCategoricalAccuracy(k=1)
     >>> m.update_state([2, 1], [[0.1, 0.9, 0.8], [0.05, 0.95, 0]])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
```

### Comparing `keras-3.1.1/keras/src/metrics/confusion_metrics.py` & `keras-3.2.0/keras/src/metrics/confusion_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             predictions (i.e., above the threshold is `True`, below is `False`).
             If used with a loss function that sets `from_logits=True` (i.e. no
             sigmoid applied to predictions), `thresholds` should be set to 0.
             One metric value is generated for each threshold value.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Examples:
 
     >>> m = keras.metrics.FalsePositives()
     >>> m.update_state([0, 1, 0, 0], [0, 0, 1, 1])
     >>> m.result()
     2.0
 
     >>> m.reset_state()
@@ -137,15 +137,15 @@
             predictions (i.e., above the threshold is `True`, below is `False`).
             If used with a loss function that sets `from_logits=True` (i.e. no
             sigmoid applied to predictions), `thresholds` should be set to 0.
             One metric value is generated for each threshold value.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.FalseNegatives()
     >>> m.update_state([0, 1, 1, 1], [0, 1, 0, 0])
     >>> m.result()
     2.0
 
     >>> m.reset_state()
@@ -181,15 +181,15 @@
             predictions (i.e., above the threshold is `True`, below is `False`).
             If used with a loss function that sets `from_logits=True` (i.e. no
             sigmoid applied to predictions), `thresholds` should be set to 0.
             One metric value is generated for each threshold value.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.TrueNegatives()
     >>> m.update_state([0, 1, 0, 0], [1, 1, 0, 0])
     >>> m.result()
     2.0
 
     >>> m.reset_state()
@@ -225,15 +225,15 @@
             predictions (i.e., above the threshold is `True`, below is `False`).
             If used with a loss function that sets `from_logits=True` (i.e. no
             sigmoid applied to predictions), `thresholds` should be set to 0.
             One metric value is generated for each threshold value.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.TruePositives()
     >>> m.update_state([0, 1, 1, 1], [1, 0, 1, 1])
     >>> m.result()
     2.0
 
     >>> m.reset_state()
@@ -287,15 +287,15 @@
             predictions to consider when calculating precision.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.Precision()
     >>> m.update_state([0, 1, 1, 1], [1, 0, 1, 1])
     >>> m.result()
     0.6666667
 
     >>> m.reset_state()
@@ -445,15 +445,15 @@
             predictions to consider when calculating recall.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.Recall()
     >>> m.update_state([0, 1, 1, 1], [1, 0, 1, 1])
     >>> m.result()
     0.6666667
 
     >>> m.reset_state()
@@ -706,15 +706,15 @@
             use for matching the given specificity.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.SensitivityAtSpecificity(0.5)
     >>> m.update_state([0, 0, 0, 1, 1], [0, 0.3, 0.8, 0.3, 0.8])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
@@ -810,15 +810,15 @@
             use for matching the given sensitivity.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.SpecificityAtSensitivity(0.5)
     >>> m.update_state([0, 0, 0, 1, 1], [0, 0.3, 0.8, 0.3, 0.8])
     >>> m.result()
     0.66666667
 
     >>> m.reset_state()
@@ -905,15 +905,15 @@
             use for matching the given recall.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.PrecisionAtRecall(0.5)
     >>> m.update_state([0, 0, 0, 1, 1], [0, 0.3, 0.8, 0.3, 0.8])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
@@ -995,15 +995,15 @@
             to use for matching the given precision.
         class_id: (Optional) Integer class ID for which we want binary metrics.
             This must be in the half-open interval `[0, num_classes)`, where
             `num_classes` is the last dimension of predictions.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.RecallAtPrecision(0.8)
     >>> m.update_state([0, 0, 1, 1], [0, 0.5, 0.3, 0.9])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
@@ -1132,15 +1132,15 @@
             handle predictions equal to exactly 0 or 1.
         multi_label: boolean indicating whether multilabel data should be
             treated as such, wherein AUC is computed separately for each label
             and then averaged across labels, or (when `False`) if the data
             should be flattened into a single label before AUC computation. In
             the latter case, when multilabel data is passed to AUC, each
             label-prediction pair is treated as an individual data point. Should
-            be set to False for multi-class data.
+            be set to `False` for multi-class data.
         num_labels: (Optional) The number of labels, used when `multi_label` is
             True. If `num_labels` is not specified, then state variables get
             created on the first call to `update_state`.
         label_weights: (Optional) list, array, or tensor of non-negative weights
             used to compute AUCs for multilabel data. When `multi_label` is
             True, the weights are applied to the individual label AUCs when they
             are averaged to produce the multi-label AUC. When it's False, they
@@ -1151,15 +1151,15 @@
             only on the index of that label before flattening; therefore
             `label_weights` should not be used for multi-class data.
         from_logits: boolean indicating whether the predictions (`y_pred` in
         `update_state`) are probabilities or sigmoid logits. As a rule of thumb,
         when using a keras loss, the `from_logits` constructor argument of the
         loss should match the AUC `from_logits` constructor argument.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.AUC(num_thresholds=3)
     >>> m.update_state([0, 0, 1, 1], [0, 0.5, 0.3, 0.9])
     >>> # threshold values are [0 - 1e-7, 0.5, 1 + 1e-7]
     >>> # tp = [2, 1, 0], fp = [2, 0, 0], fn = [0, 1, 2], tn = [0, 2, 2]
     >>> # tp_rate = recall = [1, 0.5, 0], fp_rate = [1, 0, 0]
     >>> # auc = ((((1 + 0.5) / 2) * (1 - 0)) + (((0.5 + 0) / 2) * (0 - 0)))
```

### Comparing `keras-3.1.1/keras/src/metrics/f_score_metrics.py` & `keras-3.2.0/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/metrics/hinge_metrics.py` & `keras-3.2.0/keras/src/metrics/hinge_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     `y_true` values are expected to be -1 or 1. If binary (0 or 1) labels are
     provided we will convert them to -1 or 1.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Examples:
 
     >>> m = keras.metrics.Hinge()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]])
     >>> m.result()
     1.3
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]],
@@ -45,15 +45,15 @@
     `y_true` values are expected to be -1 or 1. If binary (0 or 1) labels are
     provided we will convert them to -1 or 1.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.SquaredHinge()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]])
     >>> m.result()
     1.86
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]],
@@ -75,15 +75,15 @@
 class CategoricalHinge(reduction_metrics.MeanMetricWrapper):
     """Computes the categorical hinge metric between `y_true` and `y_pred`.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
     >>> m = keras.metrics.CategoricalHinge()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]])
     >>> m.result().numpy()
     1.4000001
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]],
     ...                sample_weight=[1, 0])
```

### Comparing `keras-3.1.1/keras/src/metrics/iou_metrics.py` & `keras-3.2.0/keras/src/metrics/iou_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,14 @@
             dense floating point vectors. If `False`, the `argmax` function
             is used to determine each sample's most likely associated label.
         axis: (Optional) -1 is the dimension containing the logits.
             Defaults to `-1`.
 
     Examples:
 
-    Standalone usage:
-
     >>> # cm = [[1, 1],
     >>> #        [1, 1]]
     >>> # sum_row = [2, 2], sum_col = [2, 2], true_positives = [1, 1]
     >>> # iou = true_positives / (sum_row + sum_col - true_positives))
     >>> # iou = [0.33, 0.33]
     >>> m = keras.metrics.IoU(num_classes=2, target_class_ids=[0])
     >>> m.update_state([0, 0, 1, 1], [0, 1, 0, 1])
@@ -334,17 +332,17 @@
             two classes is returned.
         threshold: A threshold that applies to the prediction logits to convert
             them to either predicted class 0 if the logit is below `threshold`
             or predicted class 1 if the logit is above `threshold`.
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.BinaryIoU(target_class_ids=[0, 1], threshold=0.3)
     >>> m.update_state([0, 1, 0, 1], [0.1, 0.2, 0.4, 0.7])
     >>> m.result()
     0.33333334
 
     >>> m.reset_state()
@@ -455,17 +453,17 @@
             dense floating point vectors. If `False`, the `argmax` function
             is used to determine each sample's most likely associated label.
         sparse_y_pred: Whether predictions are encoded using integers or
             dense floating point vectors. If `False`, the `argmax` function
             is used to determine each sample's most likely associated label.
         axis: (Optional) The dimension containing the logits. Defaults to `-1`.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> # cm = [[1, 1],
     >>> #        [1, 1]]
     >>> # sum_row = [2, 2], sum_col = [2, 2], true_positives = [1, 1]
     >>> # iou = true_positives / (sum_row + sum_col - true_positives))
     >>> # result = (1 / (2 + 2 - 1) + 1 / (2 + 2 - 1)) / 2 = 0.33
     >>> m = keras.metrics.MeanIoU(num_classes=2)
@@ -568,17 +566,17 @@
             segmentation maps. By default (`ignore_class=None`), all classes are
             considered.
         sparse_y_pred: Whether predictions are encoded using integers or
             dense floating point vectors. If `False`, the `argmax` function
             is used to determine each sample's most likely associated label.
         axis: (Optional) The dimension containing the logits. Defaults to `-1`.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> y_true = np.array([[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0]])
     >>> y_pred = np.array([[0.2, 0.3, 0.5], [0.1, 0.2, 0.7], [0.5, 0.3, 0.1],
     ...                       [0.1, 0.4, 0.5]])
     >>> sample_weight = [0.1, 0.2, 0.3, 0.4]
     >>> m = keras.metrics.OneHotIoU(num_classes=3, target_class_ids=[0, 2])
     >>> m.update_state(
@@ -684,17 +682,17 @@
             considered.
         sparse_y_pred: Whether predictions are encoded using natural numbers or
             probability distribution vectors. If `False`, the `argmax`
             function will be used to determine each sample's most likely
             associated label.
         axis: (Optional) The dimension containing the logits. Defaults to `-1`.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> y_true = np.array([[0, 0, 1], [1, 0, 0], [0, 1, 0], [1, 0, 0]])
     >>> y_pred = np.array([[0.2, 0.3, 0.5], [0.1, 0.2, 0.7], [0.5, 0.3, 0.1],
     ...                       [0.1, 0.4, 0.5]])
     >>> sample_weight = [0.1, 0.2, 0.3, 0.4]
     >>> m = keras.metrics.OneHotMeanIoU(num_classes=3)
     >>> m.update_state(
```

### Comparing `keras-3.1.1/keras/src/metrics/metric.py` & `keras-3.2.0/keras/src/metrics/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Metric:
     """Encapsulates metric logic and state.
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Example:
 
     ```python
     m = SomeMetric(...)
     for input in ...:
         m.update_state(input)
     print('Final result: ', m.result())
     ```
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
@@ -175,23 +175,26 @@
                 metric_variables.append(v)
         return metric_variables
 
     @property
     def dtype(self):
         return self._dtype
 
-    def add_variable(self, shape, initializer, dtype=None, name=None):
+    def add_variable(
+        self, shape, initializer, dtype=None, aggregation="sum", name=None
+    ):
         self._check_super_called()
         with backend.name_scope(self.name.replace("/", ">"), caller=self):
             initializer = initializers.get(initializer)
             variable = backend.Variable(
                 initializer=initializer,
                 shape=shape,
                 dtype=dtype,
                 trainable=False,
+                aggregation=aggregation,
                 name=name,
             )
         # Prevent double-tracking
         self._tracker.add_to_store("variables", variable)
         return variable
 
     def add_weight(self, shape=(), initializer=None, dtype=None, name=None):
```

### Comparing `keras-3.1.1/keras/src/metrics/metrics_utils.py` & `keras-3.2.0/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/metrics/probabilistic_metrics.py` & `keras-3.2.0/keras/src/metrics/probabilistic_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     metric = y_true * log(y_true / y_pred)
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Standalone usage:
+    Examples:
 
     >>> m = keras.metrics.KLDivergence()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]])
     >>> m.result()
     0.45814306
 
     >>> m.reset_state()
@@ -61,17 +61,17 @@
     metric = y_pred - y_true * log(y_pred)
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.Poisson()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     0.49999997
 
     >>> m.reset_state()
@@ -111,17 +111,17 @@
             that output encodes a probability distribution.
         label_smoothing: (Optional) Float in `[0, 1]`.
             When > 0, label values are smoothed,
             meaning the confidence on label values are relaxed.
             e.g. `label_smoothing=0.2` means that we will use
             a value of 0.1 for label "0" and 0.9 for label "1".
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.BinaryCrossentropy()
     >>> m.update_state([[0, 1], [0, 0]], [[0.6, 0.4], [0.4, 0.6]])
     >>> m.result()
     0.81492424
 
     >>> m.reset_state()
@@ -187,17 +187,17 @@
             When > 0, label values are smoothed, meaning the confidence
             on label values are relaxed. e.g. `label_smoothing=0.2` means
             that we will use a value of 0.1 for label
             "0" and 0.9 for label "1".
         axis: (Optional) Defaults to `-1`.
             The dimension along which entropy is computed.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> # EPSILON = 1e-7, y = y_true, y` = y_pred
     >>> # y` = clip_ops.clip_by_value(output, EPSILON, 1. - EPSILON)
     >>> # y` = [[0.05, 0.95, EPSILON], [0.1, 0.8, 0.1]]
     >>> # xent = -sum(y * log(y'), axis = -1)
     >>> #      = -((log 0.95), (log 0.1))
     >>> #      = [0.051, 2.302]
@@ -274,17 +274,17 @@
         dtype: (Optional) data type of the metric result.
         from_logits: (Optional) Whether output is expected
             to be a logits tensor. By default, we consider that output
             encodes a probability distribution.
         axis: (Optional) Defaults to `-1`.
             The dimension along which entropy is computed.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> # y_true = one_hot(y_true) = [[0, 1, 0], [0, 0, 1]]
     >>> # logits = log(y_pred)
     >>> # softmax = exp(logits) / sum(exp(logits), axis=-1)
     >>> # softmax = [[0.05, 0.95, EPSILON], [0.1, 0.8, 0.1]]
     >>> # xent = -sum(y * log(softmax), 1)
     >>> # log(softmax) = [[-2.9957, -0.0513, -16.1181],
```

### Comparing `keras-3.1.1/keras/src/metrics/reduction_metrics.py` & `keras-3.2.0/keras/src/metrics/reduction_metrics.py`

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

### Comparing `keras-3.1.1/keras/src/metrics/regression_metrics.py` & `keras-3.2.0/keras/src/metrics/regression_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,14 @@
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
     Examples:
 
-    Standalone usage:
-
     >>> m = keras.metrics.MeanAbsoluteError()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     0.25
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]],
     ...                sample_weight=[1, 0])
@@ -101,17 +99,17 @@
     loss = 100 * mean(abs((y_true - y_pred) / y_true))
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.MeanAbsolutePercentageError()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     250000000.0
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]],
@@ -148,17 +146,17 @@
     loss = mean(square(log(y_true + 1) - log(y_pred + 1)))
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.MeanSquaredLogarithmicError()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     0.12011322
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]],
@@ -195,17 +193,17 @@
     loss = sqrt(mean((y_pred - y_true) ** 2))
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.RootMeanSquaredError()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     0.5
 
     >>> m.reset_state()
@@ -268,17 +266,17 @@
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
         axis: (Optional) Defaults to `-1`. The dimension along which the cosine
             similarity is computed.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> # l2_norm(y_true) = [[0., 1.], [1./1.414, 1./1.414]]
     >>> # l2_norm(y_pred) = [[1., 0.], [1./1.414, 1./1.414]]
     >>> # l2_norm(y_true) . l2_norm(y_pred) = [[0., 0.], [0.5, 0.5]]
     >>> # result = mean(sum(l2_norm(y_true) . l2_norm(y_pred), axis=1))
     >>> #        = ((0. + 0.) +  (0.5 + 0.5)) / 2
     >>> m = keras.metrics.CosineSimilarity(axis=1)
@@ -321,17 +319,17 @@
     logcosh = mean(log((exp(error) + exp(-error))/2), axis=-1)
     ```
 
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
-    Examples:
+    Example:
 
-    Standalone usage:
+    Example:
 
     >>> m = keras.metrics.LogCoshError()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]])
     >>> m.result()
     0.10844523
     >>> m.reset_state()
     >>> m.update_state([[0, 1], [0, 0]], [[1, 1], [0, 0]],
```

### Comparing `keras-3.1.1/keras/src/models/cloning.py` & `keras-3.2.0/keras/src/models/cloning.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,15 @@
     Returns:
         An instance of `Model` reproducing the behavior
         of the original model, on top of new inputs tensors,
         using newly instantiated weights. The cloned model may behave
         differently from the original model if a custom `clone_function`
         modifies the layer.
 
-    Examples:
-
-    Basic usage:
+    Example:
 
     ```python
     # Create a test Sequential model.
     model = keras.Sequential([
         keras.layers.Input(shape=(728,)),
         keras.layers.Dense(32, activation='relu'),
         keras.layers.Dense(1, activation='sigmoid'),
```

### Comparing `keras-3.1.1/keras/src/models/functional.py` & `keras-3.2.0/keras/src/models/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from keras.src.layers.layer import Layer
 from keras.src.legacy.saving import saving_utils
 from keras.src.legacy.saving import serialization as legacy_serialization
 from keras.src.models.model import Model
 from keras.src.ops.function import Function
 from keras.src.ops.function import _build_map
 from keras.src.ops.function import make_node_key
+from keras.src.ops.node import KerasHistory
 from keras.src.ops.node import Node
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
 from keras.src.utils import tree
 
 
 class Functional(Function, Model):
@@ -387,15 +388,15 @@
             for original_node_index, node in enumerate(
                 operation._inbound_nodes
             ):
                 node_key = make_node_key(operation, original_node_index)
                 if node_key in self._nodes:
                     # The node is relevant to the model:
                     # add to filtered_inbound_nodes.
-                    node_data = serialize_node(node, node_reindexing_map)
+                    node_data = serialize_node(node, own_nodes=self._nodes)
                     if node_data is not None:
                         filtered_inbound_nodes.append(node_data)
 
             serialize_obj_fn = serialization_lib.serialize_keras_object
             if global_state.get_global_attribute("use_legacy_config", False):
                 # Legacy format serialization used for H5 and SavedModel
                 serialize_obj_fn = legacy_serialization.serialize_keras_object
@@ -590,21 +591,41 @@
 
 def unpack_singleton(x):
     if isinstance(x, (list, tuple)) and len(x) == 1:
         return x[0]
     return x
 
 
-def serialize_node(node, node_reindexing_map):
+def serialize_node(node, own_nodes=()):
     if not node.input_tensors:
         # Does not need to be serialized.
         return
 
+    def serialize_keras_tensor(x):
+        # Serialize KerasTensor while converting
+        # node indices to only include nodes relevant to `own_nodes`.
+        if isinstance(x, backend.KerasTensor):
+            operation, node_index, tensor_index = x._keras_history
+            irrelevant_node_count = 0
+            for node in operation._inbound_nodes[:node_index]:
+                if node not in own_nodes:
+                    irrelevant_node_count += 1
+            x._keras_history = KerasHistory(
+                operation, node_index - irrelevant_node_count, tensor_index
+            )
+            serialized = serialization_lib.serialize_keras_object(x)
+            x._keras_history = KerasHistory(operation, node_index, tensor_index)
+            return serialized
+        return x
+
     args = node.arguments.args
     kwargs = node.arguments.kwargs
+
+    args = tree.map_structure(serialize_keras_tensor, args)
+    kwargs = tree.map_structure(serialize_keras_tensor, kwargs)
     return {
         "args": serialization_lib.serialize_keras_object(args),
         "kwargs": serialization_lib.serialize_keras_object(kwargs),
     }
 
 
 def deserialize_node(node_data, created_layers):
```

### Comparing `keras-3.1.1/keras/src/models/model.py` & `keras-3.2.0/keras/src/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import inspect
 import json
-import os
 import warnings
 
 from keras.src import backend
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.models.variable_mapping import map_trackable_variables
 from keras.src.saving import saving_api
-from keras.src.saving import saving_lib
 from keras.src.trainers import trainer as base_trainer
-from keras.src.utils import io_utils
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.trainer import TensorFlowTrainer as Trainer
 elif backend.backend() == "jax":
     from keras.src.backend.jax.trainer import JAXTrainer as Trainer
@@ -311,28 +308,15 @@
         Args:
             filepath: `str` or `pathlib.Path` object.
                 Path where to save the model. Must end in `.weights.h5`.
             overwrite: Whether we should overwrite any existing model
                 at the target location, or instead ask the user
                 via an interactive prompt.
         """
-        if not str(filepath).endswith(".weights.h5"):
-            raise ValueError(
-                "The filename must end in `.weights.h5`. "
-                f"Received: filepath={filepath}"
-            )
-        try:
-            exists = os.path.exists(filepath)
-        except TypeError:
-            exists = False
-        if exists and not overwrite:
-            proceed = io_utils.ask_to_proceed_with_overwrite(filepath)
-            if not proceed:
-                return
-        saving_lib.save_weights_only(self, filepath)
+        return saving_api.save_weights(self, filepath, overwrite=True)
 
     @traceback_utils.filter_traceback
     def load_weights(self, filepath, skip_mismatch=False, **kwargs):
         """Load weights from a file saved via `save_weights()`.
 
         Weights are loaded based on the network's
         topology. This means the architecture should be the same as when the
@@ -457,18 +441,18 @@
         """
         from keras.src.saving import serialization_lib
 
         model_config = serialization_lib.serialize_keras_object(self)
         return json.dumps(model_config, **kwargs)
 
     def export(self, filepath, format="tf_saved_model"):
-        """[TF backend only]* Create a TF SavedModel artifact for inference
-        (e.g. via TF-Serving).
+        """Create a TF SavedModel artifact for inference.
 
-        **Note:** This can currently only be used with the TF backend.
+        **Note:** This can currently only be used with
+        the TensorFlow or JAX backends.
 
         This method lets you export a model to a lightweight SavedModel artifact
         that contains the model's forward pass only (its `call()` method)
         and can be served via e.g. TF-Serving. The forward pass is registered
         under the name `serve()` (see example below).
 
         The original code of the model (including any custom layers you may
@@ -559,15 +543,15 @@
         return store
 
 
 @keras_export("keras.models.model_from_json")
 def model_from_json(json_string, custom_objects=None):
     """Parses a JSON model configuration string and returns a model instance.
 
-    Usage:
+    Example:
 
     >>> model = keras.Sequential([
     ...     keras.layers.Dense(5, input_shape=(3,)),
     ...     keras.layers.Softmax()])
     >>> config = model.to_json()
     >>> loaded_model = keras.models.model_from_json(config)
```

### Comparing `keras-3.1.1/keras/src/models/sequential.py` & `keras-3.2.0/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/models/variable_mapping.py` & `keras-3.2.0/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/__init__.py` & `keras-3.2.0/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/core.py` & `keras-3.2.0/keras/src/ops/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -631,41 +631,81 @@
     """Decorator to define a function with a custom gradient.
 
     This decorator allows fine grained control over the gradients of a sequence
     for operations. This may be useful for multiple reasons, including providing
     a more efficient or numerically stable gradient for a sequence of
     operations.
 
-    Note that `custom_gradient` only supports TensorFlow and JAX backends.
-
     Args:
-        f: Function `f(*x)` that returns a tuple `(y, grad_fn)` where:
-            - `x` is a sequence of (nested structures of) tensor inputs to the
-                function.
-            - `y` is a (nested structure of) tensor outputs of applying
-                operations in `f` to `x`.
-            - `grad_fn` is a function with the signature `g(*grad_ys)` which
-                returns a list of tensors the same size as (flattened) `x`: the
-                derivatives of tensors in `y` with respect to the tensors in
-                `x`. `grad_ys` is a sequence of tensors the same size as
-                (flattened) `y` holding the initial value gradients for each
-                tensor in `y`.
+        f: Function `f(*args)` that returns a tuple
+            `(output, grad_fn)`, where:
+            - `args` is a sequence of (nested structures of) tensor inputs to
+                the function.
+            - `output` is a (nested structure of) tensor outputs of applying
+                operations in `forward_fn` to `args`.
+            - `grad_fn` is a function with the signature `grad_fn(*args,
+                upstream)` which returns a tuple of tensors the same size as
+                (flattened) `args`: the derivatives of tensors in `output` with
+                respect to the tensors in `args`. `upstream` is a tensor or
+                sequence of tensors holding the initial value gradients for each
+                tensor in `output`.
 
     Returns:
-        A function `h(x)` which returns the same value as `f(x)[0]` and whose
-        gradient is determined by `f(x)[1]`.
+        A function `h(*args)` which returns the same value as
+        `f(*args)[0]` and whose gradient is determined by
+        `f(*args)[1]`.
+
+
+    Examples:
 
-    Example:
+    1. Backend-agnostic example.
 
     ```python
     @ops.custom_gradient
     def log1pexp(x):
         e = ops.exp(x)
 
+        def grad(*args, upstream=None):
+            if upstream is None:
+                (upstream,) = args
+            return ops.multiply(upstream, 1.0 - 1.0 / ops.add(1, e))
+
+        return ops.log(1 + e), grad
+    ```
+
+    Note that the grad function that returns gradient computation
+    requires `args` as well as an `upstream` keyword argument, depending
+    on the backend being set. With the JAX and TensorFlow backends,
+    it requires only one argument, whereas it might use the `upstream`
+    argument in the case of the PyTorch backend.
+
+    When working with TensorFlow/JAX backend, `grad(upstream)`
+    is sufficient. With PyTorch, the `grad` function requires
+    `*args` as well as `upstream`, e.g. `def grad(*args, upstream)`.
+    Follow the previous example to use `@ops.custom_gradient` in
+    a way that is compatible with all backends.
+
+    2. Here's JAX & TensorFlow-specific example:
+
+    ```python
+    @ops.custom_gradient
+    def log1pexp(x):
+        e = ops.exp(x)
         def grad(upstream):
             return ops.multiply(upstream, 1.0 - 1.0 / ops.add(1, e))
+        return ops.log(1 + e), grad
+    ```
+
+    3. Lastly, here's a PyTorch-specific example,
+    using `*args` & `upstream`:
 
+    ```python
+    @ops.custom_gradient
+    def log1pexp(x):
+        e = ops.exp(x)
+        def grad(*args, upstream):
+            return ops.multiply(upstream, 1.0 - 1.0 / ops.add(1, e))
         return ops.log(1 + e), grad
     ```
     """
     return backend.core.custom_gradient(f)
```

### Comparing `keras-3.1.1/keras/src/ops/function.py` & `keras-3.2.0/keras/src/ops/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
     Args:
         inputs: List of input tensors.
         outputs: List of outputs tensors.
 
     Returns:
         A tuple `(nodes, nodes_by_depth, operations, operations_by_depth)`.
-        - network_nodes: dict mapping unique node keys to the Node instances
+        - nodes: set of Node instances
         - nodes_by_depth: dict mapping ints (depth) to lists of node instances.
         - operations: list of Operation instances.
         - operations_by_depth: dict mapping ints (depth) to lists of Operation
             instances.
     """
     # "depth" is number of operations between output Node and the Node.
     # Nodes are ordered from inputs -> outputs.
```

### Comparing `keras-3.1.1/keras/src/ops/image.py` & `keras-3.2.0/keras/src/ops/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,20 +503,20 @@
         fill_value,
     )
 
 
 class PadImages(Operation):
     def __init__(
         self,
-        top_padding,
-        bottom_padding,
-        left_padding,
-        right_padding,
-        target_height,
-        target_width,
+        top_padding=None,
+        bottom_padding=None,
+        left_padding=None,
+        right_padding=None,
+        target_height=None,
+        target_width=None,
     ):
         super().__init__()
         self.top_padding = top_padding
         self.bottom_padding = bottom_padding
         self.left_padding = left_padding
         self.right_padding = right_padding
         self.target_height = target_height
```

### Comparing `keras-3.1.1/keras/src/ops/linalg.py` & `keras-3.2.0/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/math.py` & `keras-3.2.0/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/nn.py` & `keras-3.2.0/keras/src/ops/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1251,41 +1251,46 @@
         output_padding,
         data_format,
         dilation_rate,
     )
 
 
 class OneHot(Operation):
-    def __init__(self, num_classes, axis=-1, dtype=None):
+    def __init__(self, num_classes, axis=-1, dtype=None, sparse=False):
         super().__init__()
         self.num_classes = num_classes
         self.axis = axis
         self.dtype = dtype or backend.floatx()
+        self.sparse = sparse
 
     def call(self, x):
         return backend.nn.one_hot(
-            x, self.num_classes, axis=self.axis, dtype=self.dtype
+            x,
+            self.num_classes,
+            axis=self.axis,
+            dtype=self.dtype,
+            sparse=self.sparse,
         )
 
     def compute_output_spec(self, x):
         x_shape = list(getattr(x, "shape", []))
         if self.axis == -1:
             x_shape.append(self.num_classes)
         elif self.axis >= 0 and self.axis < len(x_shape):
             x_shape.insert(self.axis, self.num_classes)
         else:
             raise ValueError(
                 f"axis must be -1 or between [0, {len(x.shape)}), but "
                 f"received {self.axis}."
             )
-        return KerasTensor(x_shape, dtype=self.dtype)
+        return KerasTensor(x_shape, dtype=self.dtype, sparse=self.sparse)
 
 
 @keras_export(["keras.ops.one_hot", "keras.ops.nn.one_hot"])
-def one_hot(x, num_classes, axis=-1, dtype=None):
+def one_hot(x, num_classes, axis=-1, dtype=None, sparse=False):
     """Converts integer tensor `x` into a one-hot tensor.
 
     The one-hot encoding is a representation where each integer value is
     converted into a binary vector with a length equal to `num_classes`,
     and the index corresponding to the integer value is marked as 1, while
     all other indices are marked as 0.
 
@@ -1293,14 +1298,16 @@
         x: Integer tensor to be encoded. The shape can be
             arbitrary, but the dtype should be integer.
         num_classes: Number of classes for the one-hot encoding.
         axis: Axis along which the encoding is performed. Defaults to
             `-1`, which represents the last axis.
         dtype: (Optional) Data type of the output tensor. If not
             provided, it defaults to the default data type of the backend.
+        sparse: Whether to return a sparse tensor; for backends that support
+            sparse tensors.
 
     Returns:
         Integer tensor: One-hot encoded tensor with the same shape as `x`
         except for the specified `axis` dimension, which will have
         a length of `num_classes`. The dtype of the output tensor
         is determined by `dtype` or the default data type of the backend.
 
@@ -1310,17 +1317,23 @@
     >>> one_hot(x, num_classes=4)
     array([[0. 1. 0. 0.]
            [0. 0. 0. 1.]
            [0. 0. 1. 0.]
            [1. 0. 0. 0.]], shape=(4, 4), dtype=float32)
     """
     if any_symbolic_tensors((x,)):
-        return OneHot(num_classes, axis=axis, dtype=dtype).symbolic_call(x)
+        return OneHot(
+            num_classes, axis=axis, dtype=dtype, sparse=sparse
+        ).symbolic_call(x)
     return backend.nn.one_hot(
-        x, num_classes, axis=axis, dtype=dtype or backend.floatx()
+        x,
+        num_classes,
+        axis=axis,
+        dtype=dtype or backend.floatx(),
+        sparse=sparse,
     )
 
 
 class BinaryCrossentropy(Operation):
     def __init__(self, from_logits=False):
         super().__init__()
         self.from_logits = from_logits
@@ -1554,24 +1567,25 @@
     return backend.nn.sparse_categorical_crossentropy(
         target, output, from_logits=from_logits, axis=axis
     )
 
 
 class MultiHot(Operation):
     def __init__(
-        self, num_classes=None, axis=-1, dtype=None, name=None, **kwargs
+        self, num_classes=None, axis=-1, dtype=None, sparse=False, **kwargs
     ):
         if num_classes is None and "num_tokens" in kwargs:
             num_classes = kwargs.pop("num_tokens")
         if num_classes is None:
             raise ValueError("Argument `num_classes` must be specified.")
-        super().__init__(name, **kwargs)
+        super().__init__(**kwargs)
         self.num_classes = num_classes
         self.axis = axis
         self.dtype = dtype or backend.floatx()
+        self.sparse = sparse
 
     def call(self, inputs):
         return backend.nn.multi_hot(
             inputs,
             num_classes=self.num_classes,
             axis=self.axis,
             dtype=self.dtype,
@@ -1590,36 +1604,40 @@
             )
 
         if len(x_shape) == 2:
             x_shape = [x_shape[-1]]
         else:
             x_shape = [x_shape[0]] + x_shape[2:]
 
-        return KerasTensor(x_shape, dtype=inputs.dtype)
+        return KerasTensor(x_shape, dtype=inputs.dtype, sparse=self.sparse)
 
 
 @keras_export(
     [
         "keras.ops.multi_hot",
         "keras.ops.nn.multi_hot",
     ]
 )
-def multi_hot(inputs, num_classes=None, axis=-1, dtype=None, **kwargs):
+def multi_hot(
+    inputs, num_classes=None, axis=-1, dtype=None, sparse=False, **kwargs
+):
     """Encodes integer labels as multi-hot vectors.
 
     This function encodes integer labels as multi-hot vectors, where each label
     is mapped to a binary value in the resulting vector.
 
     Args:
         inputs: Tensor of integer labels to be converted to multi-hot vectors.
         num_classes: Integer, the total number of unique classes.
         axis: (optional) Axis along which the multi-hot encoding should be
             added. Defaults to `-1`, which corresponds to the last dimension.
         dtype: (optional) The data type of the resulting tensor. Default
             is backend's float type.
+        sparse: Whether to return a sparse tensor; for backends that support
+            sparse tensors.
 
     Returns:
         Tensor: The multi-hot encoded tensor.
 
     Example:
 
     >>> data = keras.ops.convert_to_tensor([0, 4])
@@ -1629,22 +1647,22 @@
     """
     if num_classes is None and "num_tokens" in kwargs:
         num_classes = kwargs.pop("num_tokens")
     if num_classes is None:
         raise ValueError("Argument `num_classes` must be specified.")
 
     if any_symbolic_tensors((inputs,)):
-        return MultiHot(num_classes, axis, dtype).symbolic_call(inputs)
+        return MultiHot(num_classes, axis, dtype, sparse).symbolic_call(inputs)
 
-    return backend.nn.multi_hot(inputs, num_classes, axis, dtype)
+    return backend.nn.multi_hot(inputs, num_classes, axis, dtype, sparse)
 
 
 class Moments(Operation):
-    def __init__(self, axes, keepdims=False, synchronized=False, name=None):
-        super().__init__(name)
+    def __init__(self, axes, keepdims=False, synchronized=False):
+        super().__init__()
         self.axes = axes
         self.keepdims = keepdims
         self.synchronized = synchronized
 
     def call(self, x):
         return backend.nn.moments(
             x,
@@ -1705,16 +1723,16 @@
             x
         )
 
     return backend.nn.moments(x, axes, keepdims, synchronized=synchronized)
 
 
 class BatchNorm(Operation):
-    def __init__(self, axis, epsilon, name=None):
-        super().__init__(name)
+    def __init__(self, axis, epsilon):
+        super().__init__()
         self.axis = axis
         self.epsilon = epsilon
 
     def _check_shape(self, name, shape, expected_shape):
         if shape != expected_shape:
             raise ValueError(
                 f"Arguments `{name}` must be a vector of length "
```

### Comparing `keras-3.1.1/keras/src/ops/node.py` & `keras-3.2.0/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/numpy.py` & `keras-3.2.0/keras/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 broadcast_to
 ceil
 clip
 concatenate
 conj
 conjugate
 copy
+correlate
 cos
 cosh
 count_nonzero
 cross
 cumprod
 cumsum
 diag
@@ -1236,37 +1237,43 @@
     """
     if any_symbolic_tensors((x,)):
         return Average(axis=axis).symbolic_call(x, weights=weights)
     return backend.numpy.average(x, weights=weights, axis=axis)
 
 
 class Bincount(Operation):
-    def __init__(self, weights=None, minlength=0):
+    def __init__(self, weights=None, minlength=0, sparse=False):
         super().__init__()
         self.weights = weights
         self.minlength = minlength
+        self.sparse = sparse
 
     def call(self, x):
         return backend.numpy.bincount(
-            x, weights=self.weights, minlength=self.minlength
+            x,
+            weights=self.weights,
+            minlength=self.minlength,
+            sparse=self.sparse,
         )
 
     def compute_output_spec(self, x):
         dtypes_to_resolve = [x.dtype]
         if self.weights is not None:
             weights = backend.convert_to_tensor(self.weights)
             dtypes_to_resolve.append(weights.dtype)
             dtype = dtypes.result_type(*dtypes_to_resolve)
         else:
             dtype = "int32"
-        return KerasTensor(list(x.shape[:-1]) + [None], dtype=dtype)
+        return KerasTensor(
+            list(x.shape[:-1]) + [None], dtype=dtype, sparse=self.sparse
+        )
 
 
 @keras_export(["keras.ops.bincount", "keras.ops.numpy.bincount"])
-def bincount(x, weights=None, minlength=0):
+def bincount(x, weights=None, minlength=0, sparse=False):
     """Count the number of occurrences of each value in a tensor of integers.
 
     Args:
         x: Input tensor.
             It must be of dimension 1, and it must only contain non-negative
             integer(s).
         weights: Weight tensor.
@@ -1274,14 +1281,16 @@
             If specified, `x` is weighted by it, i.e. if `n = x[i]`,
             `out[n] += weight[i]` instead of the default behavior `out[n] += 1`.
         minlength: An integer.
             The default value is 0. If specified, there will be at least
             this number of bins in the output tensor. If greater than
             `max(x) + 1`, each value of the output at an index higher than
             `max(x)` is set to 0.
+        sparse: Whether to return a sparse tensor; for backends that support
+            sparse tensors.
 
     Returns:
         1D tensor where each element gives the number of occurrence(s) of its
         index value in x. Its length is the maximum between `max(x) + 1` and
         minlength.
 
     Examples:
@@ -1294,16 +1303,20 @@
     >>> keras.ops.bincount(x, weights=weights)
     array([0., 0.5, 2., 1.5], dtype=float64)
     >>> minlength = (keras.ops.max(x).numpy() + 1) + 2 # 6
     >>> keras.ops.bincount(x, minlength=minlength)
     array([0, 1, 2, 1, 0, 0], dtype=int32)
     """
     if any_symbolic_tensors((x,)):
-        return Bincount(weights=weights, minlength=minlength).symbolic_call(x)
-    return backend.numpy.bincount(x, weights=weights, minlength=minlength)
+        return Bincount(
+            weights=weights, minlength=minlength, sparse=sparse
+        ).symbolic_call(x)
+    return backend.numpy.bincount(
+        x, weights=weights, minlength=minlength, sparse=sparse
+    )
 
 
 class BroadcastTo(Operation):
     def __init__(self, shape):
         super().__init__()
         self.shape = shape
 
@@ -2691,14 +2704,16 @@
     def compute_output_spec(self, x, key):
         remaining_shape = list(x.shape)
         new_shape = []
         if isinstance(key, int):
             remaining_key = [key]
         elif isinstance(key, tuple):
             remaining_key = list(key)
+        elif isinstance(key, list):
+            remaining_key = key.copy()
         else:
             raise ValueError(
                 f"Unsupported key type for array slice. Recieved: `{key}`"
             )
         num_ellipses = remaining_key.count(Ellipsis)
         if num_ellipses > 1:
             raise ValueError(
@@ -5909,17 +5924,19 @@
         if dtype in ("bool", "int8", "int16"):
             dtype = "int32"
         elif dtype in ("uint8", "uint16"):
             dtype = "uint32"
         # TODO: torch doesn't support uint32
         if backend.backend() == "torch" and dtype == "uint32":
             dtype = "int32"
+        sparse = getattr(x, "sparse", False)
         return KerasTensor(
             reduce_shape(x.shape, axis=self.axis, keepdims=self.keepdims),
             dtype=dtype,
+            sparse=sparse,
         )
 
 
 @keras_export(["keras.ops.sum", "keras.ops.numpy.sum"])
 def sum(x, axis=None, keepdims=False):
     """Sum of a tensor over the given axes.
 
@@ -6066,7 +6083,74 @@
     Returns:
         Output boolean tensor.
     """
     if any_symbolic_tensors((x1, x2)):
         return LogicalXor().symbolic_call(x1, x2)
     return backend.numpy.logical_xor(x1, x2)
 
+
+class Correlate(Operation):
+    def __init__(self, mode="valid"):
+        super().__init__()
+        self.mode = mode
+
+    def call(self, x1, x2):
+        return backend.numpy.correlate(x1, x2, mode=self.mode)
+
+    def compute_output_spec(self, x1, x2):
+        x1_shape = getattr(x1, "shape", [])
+        x2_shape = getattr(x2, "shape", [])
+        if len(x1_shape) != 1:
+            raise ValueError(
+                "`x1` must be a 1-dimensional tensor, but received"
+                + f"shape {x1_shape}"
+            )
+        if len(x2_shape) != 1:
+            raise ValueError(
+                "`x2` must be a 1-dimensional tensor, but received"
+                + f"shape {x2_shape}"
+            )
+        x1_len, x2_len = x1_shape[0], x2_shape[0]
+        output_shape = (
+            np.maximum(x1_len, x2_len) - np.minimum(x1_len, x2_len) + 1,
+        )
+        if self.mode == "same":
+            output_shape = (np.maximum(x1_len, x2_len),)
+        elif self.mode == "full":
+            output_shape = (x1_len + x2_len - 1,)
+        if self.mode not in ("valid", "same", "full"):
+            raise ValueError(
+                "`mode` must be either `valid`, `same`, or `full`, but"
+                f"received: {self.mode}"
+            )
+        output_dtype = dtypes.result_type(
+            getattr(x1, "dtype", type(x1)),
+            getattr(x2, "dtype", type(x2)),
+        )
+        if output_dtype == "int64":
+            output_dtype = "float64"
+        elif output_dtype not in ["bfloat16", "float16", "float64"]:
+            output_dtype = "float32"
+        return KerasTensor(output_shape, dtype=output_dtype)
+
+
+@keras_export(["keras.ops.correlate", "keras.ops.numpy.correlate"])
+def correlate(x1, x2, mode="valid"):
+    """Compute the cross-correlation of two 1-dimensional tensors.
+
+    Args:
+        x1: First 1-dimensional input tensor of length M.
+        x2: Second 1-dimensional input tensor of length N.
+        mode: Either `valid`, `same` or `full`.
+            By default the mode is set to `valid`, which returns
+            an output of length max(M, N) - min(M, N) + 1.
+            `same` returns an output of length max(M, N).
+            `full` mode returns the convolution at each point of
+            overlap, with an output length of N+M-1
+
+    Returns:
+        Output tensor, cross-correlation of `x1` and `x2`.
+    """
+    if any_symbolic_tensors((x1, x2)):
+        return Correlate(mode=mode).symbolic_call(x1, x2)
+    return backend.numpy.correlate(x1, x2, mode=mode)
+
```

### Comparing `keras-3.1.1/keras/src/ops/operation.py` & `keras-3.2.0/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/operation_utils.py` & `keras-3.2.0/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/ops/symbolic_arguments.py` & `keras-3.2.0/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/__init__.py` & `keras-3.2.0/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/adadelta.py` & `keras-3.2.0/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/adafactor.py` & `keras-3.2.0/keras/src/optimizers/adafactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         epsilon_1: float, defaults to 1e-30. A small offset to keep denominator
             away from 0.
         epsilon_2: float, defaults to 1e-3. A small offset to avoid learning
             rate becoming too small by time.
         clip_threshold: float, defaults to 1.0. Clipping threshold. This is a
             part of Adafactor algorithm, independent from `clipnorm`,
             `clipvalue`, and `global_clipnorm`.
-        relative_step: bool, defaults to True. If `learning_rate` is a
+        relative_step: bool, defaults to `True`. If `learning_rate` is a
             constant and `relative_step=True`, learning rate will be adjusted
             based on current iterations. This is a default learning rate decay
             in Adafactor.
         {{base_optimizer_keyword_args}}
 
     Reference:
```

### Comparing `keras-3.1.1/keras/src/optimizers/adagrad.py` & `keras-3.2.0/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/adam.py` & `keras-3.2.0/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/adamax.py` & `keras-3.2.0/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/adamw.py` & `keras-3.2.0/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/base_optimizer.py` & `keras-3.2.0/keras/src/optimizers/base_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,19 @@
         self._trainable_variables_indices = {}
 
         # Create iteration variable
         # Note: dtype="int" will resolve to int32 in JAX
         # (since int64 is disallowed in JAX) and to int64 in TF.
         with backend.name_scope(self.name, caller=self):
             iterations = backend.Variable(
-                0, name="iteration", dtype="int", trainable=False
+                0,
+                name="iteration",
+                dtype="int",
+                trainable=False,
+                aggregation="only_first_replica",
             )
         self._track_variable(iterations)
         self.iterations = iterations
 
         # Create learning rate (schedule or variable)
         if isinstance(
             learning_rate, learning_rate_schedule.LearningRateSchedule
@@ -124,14 +128,15 @@
                 )
             with backend.name_scope(self.name, caller=self):
                 learning_rate = backend.Variable(
                     learning_rate,
                     name="learning_rate",
                     dtype=backend.floatx(),
                     trainable=False,
+                    aggregation="only_first_replica",
                 )
             self._track_variable(learning_rate)
             self._learning_rate = learning_rate
 
     def _track_variable(self, variable):
         self._tracker.add_to_store("variables", variable)
 
@@ -172,24 +177,26 @@
         return self._trainable_variables_indices[self._var_key(variable)]
 
     def add_variable(
         self,
         shape,
         initializer="zeros",
         dtype=None,
+        aggregation="mean",
         name=None,
     ):
         self._check_super_called()
         initializer = initializers.get(initializer)
         with backend.name_scope(self.name, caller=self):
             variable = backend.Variable(
                 initializer=initializer,
                 shape=shape,
                 dtype=dtype,
                 trainable=False,
+                aggregation=aggregation,
                 name=name,
             )
         self._track_variable(variable)
         return variable
 
     def add_variable_from_reference(
         self, reference_variable, name=None, initializer="zeros"
@@ -816,15 +823,16 @@
         weight_decay: Float. If set, weight decay is applied.
         clipnorm: Float. If set, the gradient of each weight is individually
             clipped so that its norm is no higher than this value.
         clipvalue: Float. If set, the gradient of each weight is clipped to be
             no higher than this value.
         global_clipnorm: Float. If set, the gradient of all weights is clipped
             so that their global norm is no higher than this value.
-        use_ema: Boolean, defaults to False. If True, exponential moving average
+        use_ema: Boolean, defaults to `False`.
+            If `True`, exponential moving average
             (EMA) is applied. EMA consists of computing an exponential moving
             average of the weights of the model (as the weight values change
             after each training batch), and periodically overwriting the
             weights with their moving average.
         ema_momentum: Float, defaults to 0.99. Only used if `use_ema=True`.
             This is the momentum to use when computing
             the EMA of the model's weights:
```

### Comparing `keras-3.1.1/keras/src/optimizers/ftrl.py` & `keras-3.2.0/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/lion.py` & `keras-3.2.0/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/loss_scale_optimizer.py` & `keras-3.2.0/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/nadam.py` & `keras-3.2.0/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/optimizer.py` & `keras-3.2.0/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/rmsprop.py` & `keras-3.2.0/keras/src/optimizers/rmsprop.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             to 1e-7.
         centered: Boolean. If `True`, gradients are normalized by the estimated
             variance of the gradient; if False, by the uncentered second moment.
             Setting this to `True` may help with training, but is slightly more
             expensive in terms of computation and memory. Defaults to `False`.
         {{base_optimizer_keyword_args}}
 
-    Usage:
+    Example:
 
     >>> opt = keras.optimizers.RMSprop(learning_rate=0.1)
     >>> var1 = keras.backend.Variable(10.0)
     >>> loss = lambda: (var1 ** 2) / 2.0  # d(loss) / d(var1) = var1
     >>> opt.minimize(loss, [var1])
     >>> var1
     9.683772
```

### Comparing `keras-3.1.1/keras/src/optimizers/schedules/__init__.py` & `keras-3.2.0/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-3.2.0/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,15 +778,15 @@
     the learning rate value across different invocations of optimizer functions.
 
     The learning rate multiplier first decays
     from 1 to `alpha` for `first_decay_steps` steps. Then, a warm
     restart is performed. Each new warm restart runs for `t_mul` times more
     steps and with `m_mul` times initial learning rate as the new learning rate.
 
-    Example usage:
+    Example:
     ```python
     first_decay_steps = 1000
     lr_decayed_fn = (
         keras.optimizers.schedules.CosineDecayRestarts(
             initial_learning_rate,
             first_decay_steps))
     ```
```

### Comparing `keras-3.1.1/keras/src/optimizers/sgd.py` & `keras-3.2.0/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/quantizers/__init__.py` & `keras-3.2.0/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/quantizers/quantizers.py` & `keras-3.2.0/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/random/random.py` & `keras-3.2.0/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/random/seed_generator.py` & `keras-3.2.0/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/regularizers/__init__.py` & `keras-3.2.0/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/regularizers/regularizers.py` & `keras-3.2.0/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/saving/__init__.py` & `keras-3.2.0/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/saving/object_registration.py` & `keras-3.2.0/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/saving/saving_api.py` & `keras-3.2.0/keras/src/saving/saving_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             model, filepath, overwrite, include_optimizer
         )
     else:
         raise ValueError(
             "Invalid filepath extension for saving. "
             "Please add either a `.keras` extension for the native Keras "
             f"format (recommended) or a `.h5` extension. "
-            "Use `tf.saved_model.save()` if you want to export a SavedModel "
+            "Use `model.export(filepath)` if you want to export a SavedModel "
             "for use with TFLite/TFServing/etc. "
             f"Received: filepath={filepath}."
         )
 
 
 @keras_export(["keras.saving.load_model", "keras.models.load_model"])
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
@@ -122,15 +122,15 @@
         custom_objects: Optional dictionary mapping names
             (strings) to custom classes or functions to be
             considered during deserialization.
         compile: Boolean, whether to compile the model after loading.
         safe_mode: Boolean, whether to disallow unsafe `lambda` deserialization.
             When `safe_mode=False`, loading an object has the potential to
             trigger arbitrary code execution. This argument is only
-            applicable to the Keras v3 model format. Defaults to True.
+            applicable to the Keras v3 model format. Defaults to `True`.
 
     Returns:
         A Keras model instance. If the original model was compiled,
         and the argument `compile=True` is set, then the returned model
         will be compiled. Otherwise, the model will be left uncompiled.
 
     Example:
@@ -199,26 +199,49 @@
             "`keras.layers.TFSMLayer("
             f"{filepath}, call_endpoint='serving_default')` "
             "(note that your `call_endpoint` "
             "might have a different name)."
         )
 
 
+@keras_export("keras.saving.save_weights")
+def save_weights(model, filepath, overwrite=True, **kwargs):
+    if not str(filepath).endswith(".weights.h5"):
+        raise ValueError(
+            "The filename must end in `.weights.h5`. "
+            f"Received: filepath={filepath}"
+        )
+    try:
+        exists = os.path.exists(filepath)
+    except TypeError:
+        exists = False
+    if exists and not overwrite:
+        proceed = io_utils.ask_to_proceed_with_overwrite(filepath)
+        if not proceed:
+            return
+    saving_lib.save_weights_only(model, filepath, **kwargs)
+
+
+@keras_export("keras.saving.load_weights")
 def load_weights(model, filepath, skip_mismatch=False, **kwargs):
     if str(filepath).endswith(".keras"):
         if kwargs:
             raise ValueError(f"Invalid keyword arguments: {kwargs}")
         saving_lib.load_weights_only(
             model, filepath, skip_mismatch=skip_mismatch
         )
     elif str(filepath).endswith(".weights.h5"):
+        objects_to_skip = kwargs.pop("objects_to_skip", None)
         if kwargs:
             raise ValueError(f"Invalid keyword arguments: {kwargs}")
         saving_lib.load_weights_only(
-            model, filepath, skip_mismatch=skip_mismatch
+            model,
+            filepath,
+            skip_mismatch=skip_mismatch,
+            objects_to_skip=objects_to_skip,
         )
     elif str(filepath).endswith(".h5") or str(filepath).endswith(".hdf5"):
         by_name = kwargs.pop("by_name", False)
         if kwargs:
             raise ValueError(f"Invalid keyword arguments: {kwargs}")
         if not h5py:
             raise ImportError(
```

### Comparing `keras-3.1.1/keras/src/saving/saving_lib.py` & `keras-3.2.0/keras/src/saving/saving_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 _CONFIG_FILENAME = "config.json"
 _METADATA_FILENAME = "metadata.json"
 _VARS_FNAME = "model.weights"  # Will become e.g. "model.weights.h5"
 _ASSETS_DIRNAME = "assets"
 
 
 def save_model(model, filepath, weights_format="h5"):
-    """Save a zip-archive representing a Keras model to the given filepath.
+    """Save a zip-archive representing a Keras model to the given file or path.
 
     The zip-based archive contains the following structure:
 
     - JSON-based configuration file (config.json): Records of model, layer, and
         other trackables' configuration.
     - H5-based trackable state files, found in respective directories, such as
         model/states.npz, model/dense_layer/states.npz, etc.
@@ -55,48 +55,59 @@
     `load_state()` APIs.
 
     For the case of layer states, the variables will be visited as long as
     they are either 1) referenced via layer attributes, or 2) referenced via a
     container (list, tuple, or dict), and the container is referenced via a
     layer attribute.
     """
-    filepath = str(filepath)
-    if not filepath.endswith(".keras"):
-        raise ValueError(
-            "Invalid `filepath` argument: expected a `.keras` extension. "
-            f"Received: filepath={filepath}"
-        )
     if weights_format == "h5" and h5py is None:
         raise ImportError("h5py must be installed in order to save a model.")
 
     if not model.built:
         warnings.warn(
             "You are saving a model that has not yet been built. "
             "It might not contain any weights yet. "
             "Consider building the model first by calling it "
             "on some data.",
             stacklevel=2,
         )
 
+    if isinstance(filepath, io.IOBase):
+        _save_model_to_fileobj(model, filepath, weights_format)
+        return
+
+    filepath = str(filepath)
+    if not filepath.endswith(".keras"):
+        raise ValueError(
+            "Invalid `filepath` argument: expected a `.keras` extension. "
+            f"Received: filepath={filepath}"
+        )
+    if file_utils.is_remote_path(filepath):
+        # Remote path. Zip to local memory byte io and copy to remote
+        zip_filepath = io.BytesIO()
+        _save_model_to_fileobj(model, zip_filepath, weights_format)
+        with file_utils.File(filepath, "wb") as f:
+            f.write(zip_filepath.getvalue())
+    else:
+        with open(filepath, "wb") as f:
+            _save_model_to_fileobj(model, f, weights_format)
+
+
+def _save_model_to_fileobj(model, fileobj, weights_format):
     with ObjectSharingScope():
         serialized_model_dict = serialize_keras_object(model)
     config_json = json.dumps(serialized_model_dict)
     metadata_json = json.dumps(
         {
             "keras_version": keras_version,
             "date_saved": datetime.datetime.now().strftime("%Y-%m-%d@%H:%M:%S"),
         }
     )
-    if file_utils.is_remote_path(filepath):
-        # Remote path. Zip to local memory byte io and copy to remote
-        zip_filepath = io.BytesIO()
-    else:
-        zip_filepath = filepath
 
-    with zipfile.ZipFile(zip_filepath, "w") as zf:
+    with zipfile.ZipFile(fileobj, "w") as zf:
         with zf.open(_METADATA_FILENAME, "w") as f:
             f.write(metadata_json.encode())
         with zf.open(_CONFIG_FILENAME, "w") as f:
             f.write(config_json.encode())
 
         if weights_format == "h5":
             weights_store = H5IOStore(_VARS_FNAME + ".h5", archive=zf, mode="w")
@@ -119,32 +130,36 @@
             assets_store=asset_store,
             inner_path="",
             visited_trackables=set(),
         )
         weights_store.close()
         asset_store.close()
 
-    if file_utils.is_remote_path(filepath):
-        with file_utils.File(filepath, "wb") as f:
-            f.write(zip_filepath.getvalue())
-
 
 def load_model(filepath, custom_objects=None, compile=True, safe_mode=True):
     """Load a zip archive representing a Keras model."""
-
-    filepath = str(filepath)
-    if not filepath.endswith(".keras"):
-        raise ValueError(
-            "Invalid filename: expected a `.keras` extension. "
-            f"Received: filepath={filepath}"
+    if isinstance(filepath, io.IOBase):
+        return _load_model_from_fileobj(
+            filepath, custom_objects, compile, safe_mode
         )
+    else:
+        filepath = str(filepath)
+        if not filepath.endswith(".keras"):
+            raise ValueError(
+                "Invalid filename: expected a `.keras` extension. "
+                f"Received: filepath={filepath}"
+            )
+        with open(filepath, "rb") as f:
+            return _load_model_from_fileobj(
+                f, custom_objects, compile, safe_mode
+            )
+
 
-    with file_utils.File(filepath, mode="r+b") as gfile_handle, zipfile.ZipFile(
-        gfile_handle, "r"
-    ) as zf:
+def _load_model_from_fileobj(fileobj, custom_objects, compile, safe_mode):
+    with zipfile.ZipFile(fileobj, "r") as zf:
         with zf.open(_CONFIG_FILENAME, "r") as f:
             config_json = f.read()
 
         # Note: we should NOT use a custom JSON decoder. Anything that
         # needs custom decoding must be handled in deserialize_keras_object.
         config_dict = json.loads(config_json)
         if not compile:
@@ -189,70 +204,77 @@
             asset_store.close()
 
         if failed_trackables:
             _raise_loading_failure(error_msgs)
     return model
 
 
-def save_weights_only(model, filepath):
+def save_weights_only(model, filepath, objects_to_skip=None):
     """Save only the weights of a model to a target filepath (.weights.h5).
 
     Note: only supports h5 for now.
     """
     # TODO: if h5 filepath is remote, create the file in a temporary directory
     # then upload it
     filepath = str(filepath)
     if not filepath.endswith(".weights.h5"):
         raise ValueError(
             "Invalid `filepath` argument: expected a `.weights.h5` extension. "
             f"Received: filepath={filepath}"
         )
     weights_store = H5IOStore(filepath, mode="w")
+    if objects_to_skip is not None:
+        visited_trackables = set(id(o) for o in objects_to_skip)
+    else:
+        visited_trackables = set()
     _save_state(
         model,
         weights_store=weights_store,
         assets_store=None,
         inner_path="",
-        visited_trackables=set(),
+        visited_trackables=visited_trackables,
     )
     weights_store.close()
 
 
-def load_weights_only(model, filepath, skip_mismatch=False):
+def load_weights_only(
+    model, filepath, skip_mismatch=False, objects_to_skip=None
+):
     """Load the weights of a model from a filepath (.keras or .weights.h5).
 
     Note: only supports h5 for now.
     """
-    temp_dir = None
     archive = None
     filepath = str(filepath)
     if filepath.endswith(".weights.h5"):
         # TODO: download file if h5 filepath is remote
         weights_store = H5IOStore(filepath, mode="r")
     elif filepath.endswith(".keras"):
         archive = zipfile.ZipFile(filepath, "r")
         weights_store = H5IOStore(
             _VARS_FNAME + ".h5", archive=archive, mode="r"
         )
 
     failed_trackables = set()
+    if objects_to_skip is not None:
+        visited_trackables = set(id(o) for o in objects_to_skip)
+    else:
+        visited_trackables = set()
     error_msgs = {}
     _load_state(
         model,
         weights_store=weights_store,
         assets_store=None,
         inner_path="",
         skip_mismatch=skip_mismatch,
-        visited_trackables=set(),
+        visited_trackables=visited_trackables,
         failed_trackables=failed_trackables,
         error_msgs=error_msgs,
     )
     weights_store.close()
-    if temp_dir and file_utils.exists(temp_dir):
-        file_utils.rmtree(temp_dir)
     if archive:
         archive.close()
 
     if failed_trackables:
         _raise_loading_failure(error_msgs, warn_only=skip_mismatch)
```

### Comparing `keras-3.1.1/keras/src/saving/serialization_lib.py` & `keras-3.2.0/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/testing/test_case.py` & `keras-3.2.0/keras/src/testing/test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
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
 from keras.src.utils import traceback_utils
 from keras.src.utils import tree
-from keras.src.utils.shape_utils import is_shape_tuple
 
 
 class TestCase(unittest.TestCase):
     maxDiff = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -72,14 +72,37 @@
                 e1 = backend.convert_to_numpy(e1)
                 e2 = backend.convert_to_numpy(e2)
                 self.assertEqual(e1, e2, msg=msg)
 
     def assertLen(self, iterable, expected_len, msg=None):
         self.assertEqual(len(iterable), expected_len, msg=msg)
 
+    def assertSparse(self, x, sparse=True):
+        if isinstance(x, KerasTensor):
+            self.assertEqual(x.sparse, sparse)
+        elif backend.backend() == "tensorflow":
+            import tensorflow as tf
+
+            if sparse:
+                self.assertIsInstance(x, tf.SparseTensor)
+            else:
+                self.assertNotIsInstance(x, tf.SparseTensor)
+        elif backend.backend() == "jax":
+            import jax.experimental.sparse as jax_sparse
+
+            if sparse:
+                self.assertIsInstance(x, jax_sparse.JAXSparse)
+            else:
+                self.assertNotIsInstance(x, jax_sparse.JAXSparse)
+        else:
+            self.assertFalse(
+                sparse,
+                f"Backend {backend.backend()} does not support sparse tensors",
+            )
+
     def run_class_serialization_test(self, instance, custom_objects=None):
         from keras.src.saving import custom_object_scope
         from keras.src.saving import deserialize_keras_object
         from keras.src.saving import serialize_keras_object
 
         # get_config roundtrip
         cls = instance.__class__
@@ -226,24 +249,17 @@
                     len(input_shape),
                     len(input_dtype),
                     msg="The number of input shapes and dtypes does not match",
                 )
             elif not isinstance(input_shape, tuple):
                 raise ValueError("The type of input_shape is not supported")
         if input_shape is not None and input_dtype is None:
-            if isinstance(input_shape, tuple) and is_shape_tuple(
-                input_shape[0]
-            ):
-                input_dtype = ["float32"] * len(input_shape)
-            elif isinstance(input_shape, dict):
-                input_dtype = {k: "float32" for k in input_shape.keys()}
-            elif isinstance(input_shape, list):
-                input_dtype = ["float32"] * len(input_shape)
-            else:
-                input_dtype = "float32"
+            input_dtype = tree.map_shape_structure(
+                lambda _: "float32", input_shape
+            )
 
         # Serialization test.
         layer = layer_cls(**init_kwargs)
         self.run_class_serialization_test(layer, custom_objects)
 
         # Basic masking test.
         if supports_masking is not None:
@@ -385,29 +401,15 @@
                     self.assertEqual(
                         expected_output_dtype,
                         backend.standardize_dtype(output_dtype),
                         msg="Unexpected output dtype",
                     )
             if expected_output_sparse:
                 for x in tree.flatten(output):
-                    if isinstance(x, KerasTensor):
-                        self.assertTrue(x.sparse)
-                    elif backend.backend() == "tensorflow":
-                        import tensorflow as tf
-
-                        self.assertIsInstance(x, tf.SparseTensor)
-                    elif backend.backend() == "jax":
-                        import jax.experimental.sparse as jax_sparse
-
-                        self.assertIsInstance(x, jax_sparse.JAXSparse)
-                    else:
-                        self.fail(
-                            "Sparse is unsupported with "
-                            f"backend {backend.backend()}"
-                        )
+                    self.assertSparse(x)
             if eager:
                 if expected_output is not None:
                     self.assertEqual(type(expected_output), type(output))
                     for ref_v, v in zip(
                         tree.flatten(expected_output), tree.flatten(output)
                     ):
                         self.assertAllClose(
@@ -544,14 +546,34 @@
                     self.assertEqual(dtype, spec.dtype)
                 for weight in layer.weights:
                     dtype = standardize_dtype(weight.dtype)
                     if is_float_dtype(dtype):
                         self.assertEqual(dtype, "float32")
 
 
+def tensorflow_uses_gpu():
+    return backend.backend() == "tensorflow" and uses_gpu()
+
+
+def jax_uses_gpu():
+    return backend.backend() == "jax" and uses_gpu()
+
+
+def torch_uses_gpu():
+    return backend.backend() == "torch" and uses_gpu()
+
+
+def uses_gpu():
+    # Condition used to skip tests when using the GPU
+    devices = distribution.list_devices()
+    if any(d.startswith("gpu") for d in devices):
+        return True
+    return False
+
+
 def create_keras_tensors(input_shape, dtype, sparse):
     if isinstance(input_shape, dict):
         return {
             utils.removesuffix(k, "_shape"): KerasTensor(
                 v, dtype=dtype[k], sparse=sparse
             )
             for k, v in input_shape.items()
@@ -609,14 +631,20 @@
         return {
             utils.removesuffix(k, "_shape"): create_fn(v, dtype[k])
             for k, v in input_shape.items()
         }
     return map_shape_dtype_structure(create_fn, input_shape, dtype)
 
 
+def is_shape_tuple(x):
+    return isinstance(x, (list, tuple)) and all(
+        isinstance(e, (int, type(None))) for e in x
+    )
+
+
 def map_shape_dtype_structure(fn, shape, dtype):
     """Variant of tree.map_structure that operates on shape tuples."""
     if is_shape_tuple(shape):
         return fn(tuple(shape), dtype)
     if isinstance(shape, list):
         return [
             map_shape_dtype_structure(fn, s, d) for s, d in zip(shape, dtype)
```

### Comparing `keras-3.1.1/keras/src/testing/test_utils.py` & `keras-3.2.0/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/compile_utils.py` & `keras-3.2.0/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/__init__.py` & `keras-3.2.0/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/array_slicing.py` & `keras-3.2.0/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/data_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-3.2.0/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Unpacks user-provided data tuple.
 
     This is a convenience utility to be used when overriding
     `Model.train_step`, `Model.test_step`, or `Model.predict_step`.
     This utility makes it easy to support data of the form `(x,)`,
     `(x, y)`, or `(x, y, sample_weight)`.
 
-    Standalone usage:
+    Example:
 
     >>> features_batch = ops.ones((10, 5))
     >>> labels_batch = ops.zeros((10, 5))
     >>> data = (features_batch, labels_batch)
     >>> # `y` and `sample_weight` will default to `None` if not provided.
     >>> x, y, sample_weight = unpack_x_y_sample_weight(data)
     >>> sample_weight is None
@@ -53,15 +53,15 @@
 @keras_export("keras.utils.pack_x_y_sample_weight")
 def pack_x_y_sample_weight(x, y=None, sample_weight=None):
     """Packs user-provided data into a tuple.
 
     This is a convenience utility for packing data into the tuple formats
     that `Model.fit()` uses.
 
-    Standalone usage:
+    Example:
 
     >>> x = ops.ones((10, 1))
     >>> data = pack_x_y_sample_weight(x)
     >>> isinstance(data, ops.Tensor)
     True
     >>> y = ops.ones((10, 1))
     >>> data = pack_x_y_sample_weight(x, y)
```

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-3.2.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/epoch_iterator.py` & `keras-3.2.0/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/trainers/trainer.py` & `keras-3.2.0/keras/src/trainers/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -259,15 +259,19 @@
         return vars
 
     def reset_metrics(self):
         for m in self.metrics:
             m.reset_state()
 
     def compute_loss(
-        self, x=None, y=None, y_pred=None, sample_weight=None, allow_empty=False
+        self,
+        x=None,
+        y=None,
+        y_pred=None,
+        sample_weight=None,
     ):
         """Compute the total loss, validate it, and return it.
 
         Subclasses can optionally override this method to provide custom loss
         computation logic.
 
         Example:
@@ -304,42 +308,81 @@
         ```
 
         Args:
             x: Input data.
             y: Target data.
             y_pred: Predictions returned by the model (output of `model(x)`)
             sample_weight: Sample weights for weighting the loss function.
-            allow_empty: If `False`, the method will error out if
-                no loss has been computed by the model. If `True`, then
-                if no loss is computed, the method returns 0.
 
         Returns:
             The total loss as a scalar tensor, or `None` if no loss results
             (which is the case when called by `Model.test_step`).
         """
         del x  # The default implementation does not use `x`.
         losses = []
         if self._compile_loss is not None:
             loss = self._compile_loss(y, y_pred, sample_weight)
             if loss is not None:
                 losses.append(loss)
         for loss in self.losses:
             losses.append(ops.cast(loss, dtype=backend.floatx()))
-        if not allow_empty and len(losses) == 0:
+        if backend.backend() != "jax" and len(losses) == 0:
             raise ValueError(
                 "No loss to compute. Provide a `loss` argument in `compile()`."
             )
         if len(losses) == 1:
             total_loss = losses[0]
         elif len(losses) == 0:
             total_loss = ops.zeros(())
         else:
             total_loss = ops.sum(losses)
         return total_loss
 
+    def stateless_compute_loss(
+        self,
+        trainable_variables,
+        non_trainable_variables,
+        metrics_variables,
+        x=None,
+        y=None,
+        y_pred=None,
+        sample_weight=None,
+    ):
+        var_mapping = list(zip(self.trainable_variables, trainable_variables))
+        var_mapping.extend(
+            zip(self.non_trainable_variables, non_trainable_variables)
+        )
+        var_mapping.extend(zip(self.metrics_variables, metrics_variables))
+        with backend.StatelessScope(state_mapping=var_mapping) as scope:
+            # Note that this is needed for the regularization loss, which need
+            # the latest value of train/non-trainable variables.
+            loss = self.compute_loss(
+                x,
+                y,
+                y_pred,
+                sample_weight=sample_weight,
+            )
+
+        # Update non trainable vars (may have been updated in compute_loss)
+        non_trainable_variables = []
+        for v in self.non_trainable_variables:
+            new_v = scope.get_current_value(v)
+            non_trainable_variables.append(new_v)
+
+        # Update metrics vars (may have been updated in compute_loss)
+        metrics_variables = []
+        for v in self.metrics_variables:
+            new_v = scope.get_current_value(v)
+            metrics_variables.append(new_v)
+        return loss, (
+            trainable_variables,
+            non_trainable_variables,
+            metrics_variables,
+        )
+
     def compute_metrics(self, x, y, y_pred, sample_weight=None):
         """Update metric states and collect all metrics to be returned.
 
         Subclasses can optionally override this method to provide custom metric
         updating and collection logic.
 
         Example:
@@ -861,15 +904,22 @@
                 except:
                     pass
                 result[key] = value
         return result
 
     def _flatten_metrics_in_order(self, logs):
         """Turns `logs` dict into a list as per key order of `metrics_names`."""
-        metric_names = [m.name for m in self.metrics]
+        metric_names = []
+        for metric in self.metrics:
+            if isinstance(metric, CompileMetrics):
+                metric_names += [
+                    sub_metric.name for sub_metric in metric.metrics
+                ]
+            else:
+                metric_names.append(metric.name)
         results = []
         for name in metric_names:
             if name in logs:
                 results.append(logs[name])
         for key in sorted(logs.keys()):
             if key not in metric_names:
                 results.append(logs[key])
@@ -913,14 +963,15 @@
 
             data_batch = tree.map_structure(to_symbolic_input, data_batch)
             (
                 x,
                 y,
                 sample_weight,
             ) = data_adapter_utils.unpack_x_y_sample_weight(data_batch)
+
             # Build all model state with `backend.compute_output_spec`.
             try:
                 y_pred = backend.compute_output_spec(self, x)
             except Exception as e:
                 raise RuntimeError(
                     "Unable to automatically build the model. "
                     "Please build it yourself before calling "
```

### Comparing `keras-3.1.1/keras/src/utils/__init__.py` & `keras-3.2.0/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/argument_validation.py` & `keras-3.2.0/keras/src/utils/argument_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     """Transforms non-negative/positive integer/integers into an integer tuple.
 
     Args:
         value: int or iterable of ints. The value to validate and convert.
         n: int. The size of the tuple to be returned.
         name: string. The name of the argument being validated, e.g. "strides"
             or "kernel_size". This is only used to format error messages.
-        allow_zero: bool, defaults to False. A ValueError will raised if zero is
-            received and this param is False.
+        allow_zero: bool, defaults to `False`. A `ValueError` will raised
+            if zero is received and this argument is `False`.
 
     Returns:
         A tuple of n integers.
     """
     error_msg = (
         f"The `{name}` argument must be a tuple of {n} integers. "
         f"Received {name}={value}"
```

### Comparing `keras-3.1.1/keras/src/utils/audio_dataset_utils.py` & `keras-3.2.0/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/backend_utils.py` & `keras-3.2.0/keras/src/utils/backend_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "in_tf_graph_scope", self._original_value
         )
 
 
 class DynamicBackend:
     """A class that can be used to switch from one backend to another.
 
-    Usage:
+    Example:
 
     ```python
     backend = DynamicBackend("tensorflow")
     y = backend.square(tf.constant(...))
     backend.set_backend("jax")
     y = backend.square(jax.numpy.array(...))
     ```
```

### Comparing `keras-3.1.1/keras/src/utils/code_stats.py` & `keras-3.2.0/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/dataset_utils.py` & `keras-3.2.0/keras/src/utils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,15 +515,15 @@
         formats: Allowlist of file extensions to index
             (e.g. `".jpg"`, `".txt"`).
         class_names: Only valid if `labels="inferred"`. This is the explicit
             list of class names (must match names of subdirectories). Used
             to control the order of the classes
             (otherwise alphanumerical order is used).
         shuffle: Whether to shuffle the data. Defaults to `True`.
-            If set to False, sorts the data in alphanumeric order.
+            If set to `False`, sorts the data in alphanumeric order.
         seed: Optional random seed for shuffling.
         follow_links: Whether to visits subdirectories pointed to by symlinks.
         verbose: Whether the function prints number of files found and classes.
             Defaults to `True`.
 
     Returns:
         tuple (file_paths, labels, class_names).
```

### Comparing `keras-3.1.1/keras/src/utils/dtype_utils.py` & `keras-3.2.0/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/file_utils.py` & `keras-3.2.0/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/image_dataset_utils.py` & `keras-3.2.0/keras/src/utils/image_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,16 @@
     img = tf.io.read_file(path)
     img = tf.image.decode_image(
         img, channels=num_channels, expand_animations=False
     )
 
     if pad_to_aspect_ratio and crop_to_aspect_ratio:
         raise ValueError(
-            "Only one of pad_to_aspect_ratio, crop_to_aspect_ratio"
-            " can be set to True"
+            "Only one of `pad_to_aspect_ratio`, `crop_to_aspect_ratio`"
+            " can be set to `True`."
         )
 
     if crop_to_aspect_ratio:
         from keras.src.backend import tensorflow as tf_backend
 
         if data_format == "channels_first":
             img = tf.transpose(img, (2, 0, 1))
```

### Comparing `keras-3.1.1/keras/src/utils/image_utils.py` & `keras-3.2.0/keras/src/utils/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "keras.utils.array_to_img",
         "keras.preprocessing.image.array_to_img",
     ]
 )
 def array_to_img(x, data_format=None, scale=True, dtype=None):
     """Converts a 3D NumPy array to a PIL Image instance.
 
-    Usage:
+    Example:
 
     ```python
     from PIL import Image
     img = np.random.random(size=(100, 100, 3))
     pil_img = keras.utils.array_to_img(img)
     ```
 
@@ -112,15 +112,15 @@
         "keras.utils.img_to_array",
         "keras.preprocessing.image.img_to_array",
     ]
 )
 def img_to_array(img, data_format=None, dtype=None):
     """Converts a PIL Image instance to a NumPy array.
 
-    Usage:
+    Example:
 
     ```python
     from PIL import Image
     img_data = np.random.random(size=(100, 100, 3))
     img = keras.utils.array_to_img(img_data)
     array = keras.utils.image.img_to_array(img)
     ```
@@ -190,15 +190,15 @@
     color_mode="rgb",
     target_size=None,
     interpolation="nearest",
     keep_aspect_ratio=False,
 ):
     """Loads an image into PIL format.
 
-    Usage:
+    Example:
 
     ```python
     image = keras.utils.load_img(image_path)
     input_arr = keras.utils.img_to_array(image)
     input_arr = np.array([input_arr])  # Convert single image to a batch.
     predictions = model.predict(input_arr)
     ```
```

### Comparing `keras-3.1.1/keras/src/utils/io_utils.py` & `keras-3.2.0/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/model_visualization.py` & `keras-3.2.0/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/module_utils.py` & `keras-3.2.0/keras/src/utils/module_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,9 @@
         return getattr(self.module, name)
 
 
 tensorflow = LazyModule("tensorflow")
 gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
 tensorflow_io = LazyModule("tensorflow_io")
 scipy = LazyModule("scipy")
+jax = LazyModule("jax")
```

### Comparing `keras-3.1.1/keras/src/utils/naming.py` & `keras-3.2.0/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/numerical_utils.py` & `keras-3.2.0/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/progbar.py` & `keras-3.2.0/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/python_utils.py` & `keras-3.2.0/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/rng_utils.py` & `keras-3.2.0/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/sequence_utils.py` & `keras-3.2.0/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/summary_utils.py` & `keras-3.2.0/keras/src/utils/summary_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,18 @@
             bold_text(" Optimizer params: ")
             + highlight_number(f"{optimizer_weight_count:,}")
             + f" ({readable_memory_size(optimizer_memory_size)})"
         )
 
     # Output captured summary for non-interactive logging.
     if print_fn:
-        print_fn(console.end_capture(), line_break=False)
+        if print_fn is io_utils.print_msg:
+            print_fn(console.end_capture(), line_break=False)
+        else:
+            print_fn(console.end_capture())
 
 
 def get_layer_index_bound_by_layer_name(layers, layer_range=None):
     """Get the layer indexes from the model based on layer names.
 
     The layer indexes can be used to slice the model into sub models for
     display.
```

### Comparing `keras-3.1.1/keras/src/utils/text_dataset_utils.py` & `keras-3.2.0/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/tf_utils.py` & `keras-3.2.0/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/timeseries_dataset_utils.py` & `keras-3.2.0/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/torch_utils.py` & `keras-3.2.0/keras/src/utils/torch_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Args:
         module: `torch.nn.Module` instance. If it's a `LazyModule`
             instance, then its parameters must be initialized before
             passing the instance to `TorchModuleWrapper` (e.g. by calling
             it once).
         name: The name of the layer (string).
 
-    Examples:
+    Example:
 
     Here's an example of how the `TorchModuleWrapper` can be used with vanilla
     PyTorch modules.
 
     ```python
     import torch.nn as nn
     import torch.nn.functional as F
```

### Comparing `keras-3.1.1/keras/src/utils/traceback_utils.py` & `keras-3.2.0/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/src/utils/tracking.py` & `keras-3.2.0/keras/src/utils/tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     and put them in appropriate lists in case of a match.
 
     Also passively tracks certain mutable collections
     (dict, list) so that items added to them later
     still get tracked. This is done by wrapping these
     collections into an equivalent, tracking-aware object.
 
-    Usage:
+    Example:
 
     ```python
     def __init__(self):
         self.tracker = Tracker(
             # Format: `name: (test_fn, store)`
             {
                 "variables":
```

### Comparing `keras-3.1.1/keras/src/utils/tree.py` & `keras-3.2.0/keras/src/utils/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,33 @@
         return _sequence_like(instance, args)
 
     return pack_sequence_as(
         structure, flatten(structure), sequence_fn=sequence_fn
     )
 
 
+def map_shape_structure(func, structure):
+    """Variant of tree.map_structure that operates on shape tuples."""
+
+    def is_shape_tuple(x):
+        return isinstance(x, (list, tuple)) and all(
+            isinstance(e, (int, type(None))) for e in x
+        )
+
+    if not callable(func):
+        raise TypeError(f"`func` must be callable. Received: func={func}")
+    return optree.tree_map(
+        func,
+        structure,
+        is_leaf=is_shape_tuple,
+        none_is_leaf=True,
+        namespace="keras",
+    )
+
+
 class _MapToNone:
     """A special object used as a sentinel within `traverse`."""
 
     def __repr__(self):
         return "keras.utils.tree._MAP_TO_NONE"
```

### Comparing `keras-3.1.1/keras/tree/__init__.py` & `keras-3.2.0/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras/utils/__init__.py` & `keras-3.2.0/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.1.1/keras.egg-info/PKG-INFO` & `keras-3.2.0/keras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.1.1
+Version: 3.2.0
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-3.1.1/keras.egg-info/SOURCES.txt` & `keras-3.2.0/keras.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -488,24 +488,24 @@
 keras/src/utils/code_stats.py
 keras/src/utils/dataset_utils.py
 keras/src/utils/dtype_utils.py
 keras/src/utils/file_utils.py
 keras/src/utils/image_dataset_utils.py
 keras/src/utils/image_utils.py
 keras/src/utils/io_utils.py
+keras/src/utils/jax_layer.py
 keras/src/utils/jax_utils.py
 keras/src/utils/model_visualization.py
 keras/src/utils/module_utils.py
 keras/src/utils/naming.py
 keras/src/utils/numerical_utils.py
 keras/src/utils/progbar.py
 keras/src/utils/python_utils.py
 keras/src/utils/rng_utils.py
 keras/src/utils/sequence_utils.py
-keras/src/utils/shape_utils.py
 keras/src/utils/summary_utils.py
 keras/src/utils/text_dataset_utils.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
 keras/src/utils/torch_utils.py
 keras/src/utils/traceback_utils.py
 keras/src/utils/tracking.py
```

### Comparing `keras-3.1.1/setup.py` & `keras-3.2.0/setup.py`

 * *Files identical despite different names*

