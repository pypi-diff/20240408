# Comparing `tmp/imax-0.0.1b7.tar.gz` & `tmp/imax-0.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imax-0.0.1b7.tar", last modified: Sun Nov 12 22:48:20 2023, max compression
+gzip compressed data, was "imax-0.0.1b8.tar", last modified: Mon Apr  8 10:29:31 2024, max compression
```

## Comparing `imax-0.0.1b7.tar` & `imax-0.0.1b8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:48:20.391100 imax-0.0.1b7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-12 22:48:07.000000 imax-0.0.1b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-11-12 22:48:20.391100 imax-0.0.1b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-11-12 22:48:07.000000 imax-0.0.1b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:48:20.387100 imax-0.0.1b7/imax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-12 22:48:07.000000 imax-0.0.1b7/imax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2023-11-12 22:48:07.000000 imax-0.0.1b7/imax/color_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2023-11-12 22:48:07.000000 imax-0.0.1b7/imax/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2023-11-12 22:48:07.000000 imax-0.0.1b7/imax/randaugment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2023-11-12 22:48:07.000000 imax-0.0.1b7/imax/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:48:20.391100 imax-0.0.1b7/imax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-11-12 22:48:20.000000 imax-0.0.1b7/imax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-11-12 22:48:20.000000 imax-0.0.1b7/imax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 22:48:20.000000 imax-0.0.1b7/imax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-12 22:48:20.000000 imax-0.0.1b7/imax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-12 22:48:20.000000 imax-0.0.1b7/imax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-12 22:48:20.391100 imax-0.0.1b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-12 22:48:07.000000 imax-0.0.1b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 22:48:20.391100 imax-0.0.1b7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-11-12 22:48:07.000000 imax-0.0.1b7/tests/test_color_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2023-11-12 22:48:07.000000 imax-0.0.1b7/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 10:29:27.000000 imax-0.0.1b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 10:29:31.893623 imax-0.0.1b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-08 10:29:27.000000 imax-0.0.1b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/imax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/color_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/randaugment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8075 2024-04-08 10:29:27.000000 imax-0.0.1b8/imax/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/imax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-08 10:29:31.000000 imax-0.0.1b8/imax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:29:31.893623 imax-0.0.1b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-08 10:29:27.000000 imax-0.0.1b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:29:31.893623 imax-0.0.1b8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-08 10:29:27.000000 imax-0.0.1b8/tests/test_color_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-08 10:29:27.000000 imax-0.0.1b8/tests/test_transforms.py
```

### Comparing `imax-0.0.1b7/LICENSE` & `imax-0.0.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b7/PKG-INFO` & `imax-0.0.1b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imax
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: Image augmentation library for Jax
 Home-page: https://github.com/4rtemi5/imax
 Author: Raphael Pisoni
 Author-email: raphael.pisoni@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `imax-0.0.1b7/README.md` & `imax-0.0.1b8/README.md`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b7/imax/color_transforms.py` & `imax-0.0.1b8/imax/color_transforms.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b7/imax/project.py` & `imax-0.0.1b8/imax/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 # ==============================================================================
 '''
 Image transformations with nearest neighbor and bilinear sampling.
 '''
 import jax
 import jax.numpy as jnp
 
+def extend3to4(intrinsics):
+    """ Extrend size of 3x3 intrinsics to 4x4 intrinsics.
+    """
+    filler = jnp.array([[0.0, 0.0, 0.0, 1.0]])
+    intrinsics = jnp.concatenate([intrinsics, jnp.zeros([3, 1])], axis=1)
+    intrinsics = jnp.concatenate([intrinsics, filler], axis=0)
+    return intrinsics
+
 
 def pixel2cam(depth, pixel_coords, intrinsics, is_homogeneous=True):
     """Transforms coordinates in the pixel frame to the camera frame.
     Args:
         depth: [batch, height, width]
         pixel_coords: homogeneous pixel coordinates [batch, 3, height, width]
         intrinsics: camera intrinsics [batch, 3, 3]
@@ -47,15 +55,14 @@
     if is_homogeneous:
         ones = jnp.ones([1, height * width])
         cam_coords = jnp.concatenate([cam_coords, ones], axis=0)
     cam_coords = jnp.reshape(cam_coords, [-1, height, width])
     return cam_coords
 
 
-@jax.jit
 def cam2pixel(cam_coords, proj):
     """Transforms coordinates in a camera frame to the pixel frame.
     Args:
         cam_coords: [batch, 4, height, width]
         proj: [batch, 4, 4]
     Returns:
         Pixel coordinates projected from the camera frame [b, h, w, 2]
@@ -64,16 +71,16 @@
     cam_coords = jnp.reshape(cam_coords, [4, -1])
     unnormalized_pixel_coords = jnp.matmul(proj, cam_coords)
     x_u = unnormalized_pixel_coords[0:1, :]  # [0:0:0, -1:1:-1]
     y_u = unnormalized_pixel_coords[1:2, :]  # [0:1:0, -1:1:-1]
     z_u = unnormalized_pixel_coords[2:3, :]  # [0:2:0, -1:1:-1]
     x_n = x_u / (z_u + 1e-10)
     y_n = y_u / (z_u + 1e-10)
-    pixel_coords = jnp.concatenate([x_n, y_n], axis=0)
-    pixel_coords = jnp.reshape(pixel_coords, [2, height, width])
+    pixel_coords = jnp.concatenate([x_n, y_n, z_u], axis=0)
+    pixel_coords = jnp.reshape(pixel_coords, [3, height, width])
     return jnp.transpose(pixel_coords, axes=[1, 2, 0])
 
 
 def meshgrid(height, width, is_homogeneous=True):
     """Construct a 2D meshgrid.
     Args:
         height: height of the grid
@@ -94,15 +101,126 @@
         coords = jnp.stack([x_t, y_t, ones], axis=0)
     else:
         coords = jnp.stack([x_t, y_t], axis=0)
     # coords = jnp.tile(jnp.expand_dims(coords, 0), [batch, 1, 1, 1])
     return coords
 
 
-def compute_mask(x0, x1, y0, y1, x_max, y_max):
+def bilinear_project(points_yx, depth, values, height, width, mask_value=0):
+    # Create empty matrices, starting from 0 to p.max
+    channels = values.shape[-1] + 1
+    w = jnp.zeros((height, width))
+    i = jnp.zeros((height, width, channels))
+
+    valid_mask = (
+        jnp.isfinite(depth) 
+        # & jnp.greater_equal(depth, 0)
+        & jnp.isfinite(points_yx).all(axis=1)
+        # & ~compute_occlusions(points_yx, depth)
+        & jnp.greater_equal(points_yx, 0.).all(axis=1)
+        & (points_yx[:, 0] < (height))
+        & (points_yx[:, 1] < (width))
+    )
+    
+    # Calc weights
+    floor = jnp.floor(points_yx)
+    ceil = floor + 1
+    upper_diff = ceil - points_yx
+    lower_diff = points_yx - floor
+    w1 = upper_diff[:, 0] * upper_diff[:, 1] * valid_mask
+    w2 = upper_diff[:, 0] * lower_diff[:, 1] * valid_mask
+    w3 = lower_diff[:, 0] * upper_diff[:, 1] * valid_mask
+    w4 = lower_diff[:, 0] * lower_diff[:, 1] * valid_mask
+    
+    # Get indices
+    ix = floor[:, 0].astype("uint32")
+    iy = floor[:, 1].astype("uint32")
+
+    w = w.at[ix, iy].add(w1, mode="drop")
+    w = w.at[ix, iy + 1].add(w2, mode="drop")
+    w = w.at[ix + 1, iy].add(w3, mode="drop")
+    w = w.at[ix + 1, iy + 1].add(w4, mode="drop")
+    #w += 1e-6
+
+    values = jnp.concatenate([
+        values,
+        depth[..., None],
+    ], axis=1)
+
+    values = values.flatten()
+    ix = ix.repeat(channels)
+    iy = iy.repeat(channels)
+    iz = jnp.tile(jnp.arange(channels), height * width)
+
+    w1 = w1.repeat(channels)
+    w2 = w2.repeat(channels)
+    w3 = w3.repeat(channels)
+    w4 = w4.repeat(channels)
+
+    i = i.at[ix, iy, iz].add(w1 * values, mode="drop")
+    i = i.at[ix, iy + 1, iz].add(w2 * values, mode="drop")
+    i = i.at[ix + 1, iy, iz].add(w3 * values, mode="drop")
+    i = i.at[ix + 1, iy + 1, iz].add(w4 * values, mode="drop")
+
+    i = i / jnp.clip(w[..., None], 1e-6, 1.0) * jnp.greater(w[..., None], 0.0)
+    values_out, depth_out = i[..., :-1], i[..., -1:]
+
+    values_out = jnp.where(
+        jnp.equal(w[..., None], 0),
+        mask_value,
+        values_out
+    )
+
+    return values_out, depth_out
+
+
+def depth_warp(
+    input_image,
+    input_depth,
+    intrinsics,
+    transform,
+    mask_value=0,
+):
+    # intrinsics = extend3to4(intrinsics)
+    height, width = input_depth.shape
+
+    # Construct pixel grid coordinates
+    pixel_coords = meshgrid(height, width, is_homogeneous=False)
+    depth = input_depth.reshape((1, -1))
+    ones = jnp.ones_like(depth)
+    pixel_mesh = jnp.reshape(pixel_coords, [2, -1])
+
+    pixel_coords = jnp.concatenate([pixel_mesh, ones], axis=0)
+
+    target_pixel_coords = jnp.linalg.inv(intrinsics) @ pixel_coords
+
+    target_pixel_coords = jnp.concatenate([target_pixel_coords, ones], axis=0)
+    target_pixel_coords = jnp.concatenate(
+        [target_pixel_coords[:2] * depth, depth, ones], axis=0
+    )
+
+    target_pixel_coords = transform @ target_pixel_coords
+    
+    x, y, z, _ = jnp.split(target_pixel_coords, 4, axis=0)
+    target_pixel_coords = jnp.concatenate([target_pixel_coords[:2] / jnp.clip(depth, 1.0, jnp.inf), ones], axis=0)
+    target_pixel_coords = intrinsics @ target_pixel_coords
+
+    coords = jnp.concatenate([target_pixel_coords[0:1], target_pixel_coords[1:2]], axis=0).T  # new y, x coordinates
+
+    values = jnp.concatenate([
+        input_image.reshape((-1, input_image.shape[-1])),  # original image values (eg. rgb)
+    ], axis=1)
+    
+    new_depth = z.reshape((-1,))  # new z-coordinates
+
+    projected_values, projected_depth = bilinear_project(coords, new_depth, values, height, width, mask_value)
+    return projected_values, projected_depth
+
+
+def compute_mask(x0, x1, y0, y1, z, x_max, y_max):
     """
     Computes invalid pixel coordinates.
     Args:
         coords_x: flattened vector of x coordinates
         coords_y: flattened vector of y coordinates
         x_max: maximum x coordinate
         y_max: maximum y coordinate
@@ -110,37 +228,44 @@
     Returns:
         vector of mask values
     """
     x_not_underflow = x0 >= 0.0
     y_not_underflow = y0 >= 0.0
     x_not_overflow = x1 <= x_max
     y_not_overflow = y1 <= y_max
-    # z_positive = z >= 0.0
+    z_positive = z >= 0.0
     # x_not_nan = jnp.logical_not(jnp.isnan(coords_x))
     # y_not_nan = jnp.logical_not(jnp.isnan(coords_y))
     # not_nan = jnp.logical_and(x_not_nan, y_not_nan)
     # not_nan_mask = not_nan.astype('float32')
     # coords_x = tf.math.multiply_no_nan(coords_x, not_nan_mask)
     # coords_y = tf.math.multiply_no_nan(coords_y, not_nan_mask)
     
     mask_stack = jnp.stack([
         x_not_underflow,
         y_not_underflow,
         x_not_overflow,
         y_not_overflow,
-        # z_positive,
+        z_positive,
         # not_nan
     ],
         axis=0)
     mask = jnp.all(mask_stack, axis=0)
     return mask
 
 
-def projective_inverse_warp(img, transform, mask_value,
-                            intrinsics, depth, bilinear=True):
+def projective_inverse_warp(
+    img,
+    depth,
+    image_intrinsics,
+    depth_intrinsics,
+    transform,
+    mask_value,
+    bilinear=True,
+):
     """
     Inverse warp a source image to the target image plane based on projection.
     Args:
         img: the source image [batch, height_s, width_s, 3]
         transform: 4x4 transformation matrix
         mask_value: mask value of rgb/a mask value
         depth: depth map of the target image [batch, height_t, width_t]
@@ -150,23 +275,20 @@
         Source image inverse warped to the target image plane [batch, height_t,
         width_t, 3]
     """
     height, width, _ = img.shape
     # Construct pixel grid coordinates
     pixel_coords = meshgrid(height, width)
     # Convert pixel coordinates to the camera frame
-    cam_coords = pixel2cam(depth, pixel_coords, intrinsics)
+    cam_coords = pixel2cam(depth, pixel_coords, depth_intrinsics)
     # Construct a 4x4 intrinsic matrix
-    filler = jnp.array([[0.0, 0.0, 0.0, 1.0]])
-    # filler = jnp.tile(filler, [batch, 1, 1])
-    intrinsics = jnp.concatenate([intrinsics, jnp.zeros([3, 1])], axis=1)
-    intrinsics = jnp.concatenate([intrinsics, filler], axis=0)
+    image_intrinsics = extend3to4(image_intrinsics)
     # Get a 4x4 transformation matrix from 'target' camera frame to 'source'
     # pixel frame.
-    proj_tgt_cam_to_src_pixel = jnp.matmul(intrinsics, transform)
+    proj_tgt_cam_to_src_pixel = jnp.matmul(image_intrinsics, transform)
     src_pixel_coords = cam2pixel(cam_coords, proj_tgt_cam_to_src_pixel)
 
     output_img = jnp.where(bilinear,
                            bilinear_sampler(img, src_pixel_coords, mask_value),
                            nearest_sampler(img, src_pixel_coords, mask_value))
     return output_img
 
@@ -180,24 +302,24 @@
             height_t/width_t correspond to the dimensions of the output
             image (don't need to be the same as height_s/width_s).
             The two channels correspond to x and y coordinates respectively.
         mask_value: value of points outside of image. -1 for edge sampling.
         Returns:
             A new sampled image [height_t, width_t, channels]
     """
-    coords_x, coords_y = jnp.split(coords, 2, axis=2)
+    coords_x, coords_y, z = jnp.split(coords, 3, axis=2)
     inp_size = imgs.shape
     out_size = list(coords.shape)
     out_size[2] = imgs.shape[2]
 
     coords_x = jnp.array(coords_x, dtype='float32')
     coords_y = jnp.array(coords_y, dtype='float32')
 
-    y_max = jnp.array(jnp.shape(imgs)[0], dtype='float32')
-    x_max = jnp.array(jnp.shape(imgs)[1], dtype='float32')
+    y_max = jnp.array(jnp.shape(imgs)[0], dtype='float32') - 1
+    x_max = jnp.array(jnp.shape(imgs)[1], dtype='float32') - 1
     zero = jnp.zeros([1], dtype='float32')
     eps = jnp.array([1e-6], dtype='float32')
 
     coords_x_clipped = jnp.clip(coords_x, zero - 0.5 + eps, x_max + 0.5 + eps)
     coords_y_clipped = jnp.clip(coords_y, zero - 0.5 + eps, y_max + 0.5 + eps)
 
     x0 = jnp.round(coords_x_clipped)
@@ -215,15 +337,15 @@
     # sample from imgs
     imgs_flat = jnp.reshape(imgs, [-1, inp_size[2]])
     imgs_flat = imgs_flat.astype('float32')
     output = jnp.reshape(
         jnp.take(imgs_flat, idx00.astype('int32'), axis=0),
         out_size
     )
-    valid_mask = compute_mask(x0, x0, y0, y0, x_max, y_max)
+    valid_mask = compute_mask(x0, x0, y0, y0, z, x_max, y_max)
 
     return jnp.where(
         jnp.any(mask_value > 0),
         jnp.where(
             valid_mask,
             output,
             jnp.ones_like(output) *
@@ -241,24 +363,24 @@
             height_t/width_t correspond to the dimensions of the output
             image (don't need to be the same as height_s/width_s).
             The two channels correspond to x and y coordinates respectively.
         mask_value: value of points outside of image. -1 for edge sampling.
         Returns:
             A new sampled image [height_t, width_t, channels]
     """
-    coords_x, coords_y = jnp.split(coords, 2, axis=2)
+    coords_x, coords_y, z = jnp.split(coords, 3, axis=2)
     inp_size = imgs.shape
     out_size = list(coords.shape)
     out_size[2] = imgs.shape[2]
 
     coords_x = jnp.array(coords_x, dtype='float32')
     coords_y = jnp.array(coords_y, dtype='float32')
 
-    y_max = jnp.array(jnp.shape(imgs)[0], dtype='float32')
-    x_max = jnp.array(jnp.shape(imgs)[1], dtype='float32')
+    y_max = jnp.array(jnp.shape(imgs)[0], dtype='int32')
+    x_max = jnp.array(jnp.shape(imgs)[1], dtype='int32')
     zero = jnp.zeros([1], dtype='float32')
     eps = jnp.array([1e-6], dtype='float32')
     
     coords_x_clipped = jnp.clip(coords_x, zero - 0.5 - eps, x_max + 0.5 + eps)
     coords_y_clipped = jnp.clip(coords_y, zero - 0.5 - eps, y_max + 0.5 + eps)
 
     x0 = jnp.round(coords_x_clipped)
@@ -354,15 +476,15 @@
 
     w00 = w_x0 * w_y0
     w01 = w_x0 * w_y1
     w10 = w_x1 * w_y0
     w11 = w_x1 * w_y1
 
     output = w00 * im00 + w01 * im01 + w10 * im10 + w11 * im11
-    valid_mask = compute_mask(x0, x1, y0, y1, x_max, y_max)
+    valid_mask = compute_mask(x0, x1, y0, y1, z, x_max, y_max)
 
     return jnp.where(jnp.all(mask_value >= 0),
                      jnp.where(
                          valid_mask,
                          output,
                          jnp.ones_like(output) *
                          jnp.reshape(mask_value, [1, 1, -1])
```

### Comparing `imax-0.0.1b7/imax/randaugment.py` & `imax-0.0.1b8/imax/randaugment.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b7/imax/transforms.py` & `imax-0.0.1b8/imax/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # limitations under the License.
 # ==============================================================================
 """
 Geometric Transforms in Jax.
 """
 import jax
 import jax.numpy as jnp
-from imax.project import projective_inverse_warp
+from imax.project import projective_inverse_warp, depth_warp
 
 I = jnp.identity(4)
 
 
-@jax.jit
+# @jax.jit
 def scale_3d(scale_x=1., scale_y=1., scale_z=1., scale_xyz=1.):
     """
     Returns transformation matrix for 3d scaling.
     Args:
         scale_x: scaling factor in x-direction
         scale_y: scaling factor in y-direction
         scale_z: scaling factor in z-direction
@@ -38,29 +38,29 @@
     matrix = jnp.array([[1 / scale_x, 0, 0, 0],
                         [0, 1 / scale_y, 0, 0],
                         [0, 0, 1 / scale_z, 0],
                         [0, 0, 0, 1 / scale_xyz]], dtype='float32')
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def scale(x_factor=1.0, y_factor=1.0):
     """
     Returns transformation matrix for 2d scaling.
     Args:
         x_factor: scaling factor in x direction
         y_factor: scaling factor in y direction
 
     Returns:
         A 4x4 float32 transformation matrix.
     """
     return scale_3d(scale_x=x_factor, scale_y=y_factor)
 
 
-@jax.jit
+# @jax.jit
 def shear_3d(sxy=0., sxz=0., syx=0., syz=0., szx=0., szy=0.):
     """
     Returns transformation matrix for 3d shearing.
     Args:
         sxy: xy shearing factor
         sxz: xz shearing factor
         syx: yx shearing factor
@@ -74,29 +74,29 @@
     matrix = jnp.array([[  1, sxy, sxz, 0],
                         [syx,   1, syz, 0],
                         [szx, szy,   1, 0],
                         [  0,   0,   0, 1]], dtype='float32')
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def shear(horizontal=0., vertical=0.):
     """
     Returns transformation matrix for 2d shearing.
     Args:
         horizontal: horizontal shearing factor
         vertical: vertical shearing factor
 
     Returns:
         A 4x4 float32 transformation matrix.
     """
     return shear_3d(sxy=horizontal, syx=vertical)
 
 
-@jax.jit
+# @jax.jit
 def translate_3d(translate_x=0, translate_y=0, translate_z=0):
     """
     Returns transformation matrix for 3d translation.
     Args:
         translate_x: x translation factor
         translate_y: y translation factor
         translate_z: z translation factor
@@ -107,29 +107,29 @@
     matrix = jnp.array([[1, 0, 0, translate_x],
                         [0, 1, 0, translate_y],
                         [0, 0, 1, translate_z],
                         [0, 0, 0, 1]], dtype='float32')
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def translate(horizontal, vertical):
     """
     Returns transformation matrix for 2d translation.
     Args:
         horizontal: horizontal translation factor
         vertical: vertical translation factor
 
     Returns:
         A 4x4 float32 transformation matrix.
     """
     return translate_3d(translate_x=horizontal, translate_y=vertical)
 
 
-@jax.jit
+# @jax.jit
 def flip(horizontal=False, vertical=False):
     """
     Returns transformation matrix for 2d flipping.
     Args:
         horizontal: bool horizontal flipping
         vertical: bool vertical flipping
 
@@ -152,15 +152,15 @@
                             [  0, 1,    0, 0],
                             [rsy, 0,  rcy, 0],
                             [  0, 0,    0, 1]])
     matrix = rotation_x @ rotation_y
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def rotate90(n=0):
     """
     Returns transformation matrix for 2d rotation of multiples of 90°.
     Args:
         n: number of 90° rotations
 
     Returns:
@@ -171,15 +171,15 @@
     matrix = jnp.array([[ rcz, rsz, 0, 0],
                         [-rsz, rcz, 0, 0],
                         [   0,   0, 1, 0],
                         [   0,   0, 0, 1]])
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def rotate_3d(angle_x=0, angle_y=0, angle_z=0):
     """
     Returns transformation matrix for 3d rotation.
     Args:
         angle_x: rotation angle around x axis in radians
         angle_y: rotation angle around y axis in radians
         angle_z: rotation angle around z axis in radians
@@ -207,31 +207,31 @@
                     [-rsz, rcz, 0, 0],
                     [   0,   0, 1, 0],
                     [   0,   0, 0, 1]])
     matrix = rotation_x @ rotation_y @ rotation_z
     return matrix
 
 
-@jax.jit
+# @jax.jit
 def rotate(rad):
     """
     Returns transformation matrix for 2d rotation around the z axis.
     Args:
         rad: rotation angle in radians around z axis
 
     Returns:
         A 4x4 float32 transformation matrix.
     """
     return rotate_3d(angle_z=rad)
 
 
-@jax.jit
+# @jax.jit
 def apply_transform(image,
                     transform,
-                    mask_value=-1,
+                    mask_value=jnp.nan,
                     depth=-1,
                     intrinsic_matrix=-1,
                     bilinear=True):
     """
     Applies a 3d transformation to an image.
     Can deal with depth data and intrinsic matrices.
     Args:
@@ -256,13 +256,25 @@
     intrinsic_matrix = jnp.where(jnp.any(intrinsic_matrix >= 0),
                                  intrinsic_matrix,
                                  jnp.array([[1, 0, (width - 1) / 2.],
                                             [0, 1, (height - 1) / 2.],
                                             [0, 0, 1]],
                                            dtype='float32'))
 
-    return projective_inverse_warp(image,
-                                   transform,
-                                   mask_value,
-                                   intrinsic_matrix,
-                                   depth,
-                                   bilinear=bilinear)
+
+    projected_image, projected_depth =  depth_warp(
+        image,
+        depth,
+        intrinsic_matrix,
+        transform,
+        mask_value
+    )
+    return projected_image
+    # return projective_inverse_warp(
+    #     image,
+    #     depth,
+    #     image_intrinsics=intrinsic_matrix,
+    #     depth_intrinsics=intrinsic_matrix,
+    #     transform=transform,
+    #     mask_value=mask_value,
+    #     bilinear=bilinear,
+    # )
```

### Comparing `imax-0.0.1b7/imax.egg-info/PKG-INFO` & `imax-0.0.1b8/imax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imax
-Version: 0.0.1b7
+Version: 0.0.1b8
 Summary: Image augmentation library for Jax
 Home-page: https://github.com/4rtemi5/imax
 Author: Raphael Pisoni
 Author-email: raphael.pisoni@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `imax-0.0.1b7/setup.py` & `imax-0.0.1b8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imax",
-    version="0.0.1-beta7",
+    version="0.0.1-beta8",
     author="Raphael Pisoni",
     author_email="raphael.pisoni@gmail.com",
     description="Image augmentation library for Jax",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/4rtemi5/imax",
     classifiers=[
```

### Comparing `imax-0.0.1b7/tests/test_color_transforms.py` & `imax-0.0.1b8/tests/test_color_transforms.py`

 * *Files identical despite different names*

### Comparing `imax-0.0.1b7/tests/test_transforms.py` & `imax-0.0.1b8/tests/test_transforms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from imax import transforms
 from jax import numpy as jnp
 from utils import compare
 
 
-from jax.config import config
+from jax import config
 config.update("jax_debug_nans", True)
 
 # test_img_rgba = jnp.asarray(Image.open('./test.jpeg').convert('RGBA')).astype('uint8')
 # test_img_rgb = jnp.asarray(Image.open('./test.jpeg').convert('RGB')).astype('uint8')
 
 rgb_img = jnp.array(
     [
@@ -31,14 +31,35 @@
 def test_data():
     inputs = None
     targets = rgb_img
     outputs = rgba_img[:, :, :3]
     compare(inputs, targets, outputs)
 
 
+def test_identity():
+    inputs = rgba_img
+    targets = rgba_img
+    
+    outputs = transforms.apply_transform(
+        rgba_img,
+        jnp.eye(4),
+        mask_value=jnp.array([255., 255., 255., 255.]),
+        bilinear=False,
+    )
+    compare(inputs, targets, outputs)
+
+    outputs = transforms.apply_transform(
+        rgba_img,
+        jnp.eye(4),
+        mask_value=jnp.array([255., 255., 255., 255.]),
+        bilinear=True,
+    )
+    compare(inputs, targets, jnp.round(outputs))
+
+
 def test_horizontal_flip():
     inputs = rgba_img
     targets = rgba_img[:, ::-1]
     
     outputs = transforms.apply_transform(
         rgba_img,
         transforms.flip(horizontal=True, vertical=False),
@@ -100,15 +121,15 @@
 def test_scale():
     factor = 3
     inputs = jnp.pad(
         jnp.ones((1, 1, 4), dtype="uint8") * 255,
         ((1, 1), (1, 1), (0, 0)),
         constant_values=0,
     )
-    targets = jnp.ones_like(rgba_img) * 255
+    targets = inputs  # jnp.ones_like(rgba_img) * 255
     outputs = transforms.apply_transform(
         jnp.pad(
             jnp.ones((1, 1, 4), dtype="uint8"),
             ((1, 1), (1, 1), (0, 0)),
             constant_values=0,
         )
         * 255,
```

