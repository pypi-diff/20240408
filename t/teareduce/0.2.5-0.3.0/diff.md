# Comparing `tmp/teareduce-0.2.5.tar.gz` & `tmp/teareduce-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teareduce-0.2.5.tar", last modified: Thu Apr  4 14:34:39 2024, max compression
+gzip compressed data, was "teareduce-0.3.0.tar", last modified: Mon Apr  8 19:37:29 2024, max compression
```

## Comparing `teareduce-0.2.5.tar` & `teareduce-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.194696 teareduce-0.2.5/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.2.5/LICENSE.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-04 14:34:39.194434 teareduce-0.2.5/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.2.5/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)     1624 2024-01-12 07:48:48.000000 teareduce-0.2.5/pyproject.toml
--rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-04-04 14:34:39.194746 teareduce-0.2.5/setup.cfg
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.184920 teareduce-0.2.5/src/
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.193036 teareduce-0.2.5/src/teareduce/
--rw-r--r--   0 cardiel    (501) staff       (20)      909 2024-01-24 16:46:28.000000 teareduce-0.2.5/src/teareduce/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.2.5/src/teareduce/avoid_astropy_warnings.py
--rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.2.5/src/teareduce/cosmicrays.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.2.5/src/teareduce/ctext.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.2.5/src/teareduce/draw_rectangle.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.2.5/src/teareduce/elapsed_time.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.2.5/src/teareduce/imshow.py
--rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.2.5/src/teareduce/peaks_spectrum.py
--rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.2.5/src/teareduce/polfit.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.2.5/src/teareduce/robust_std.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5806 2024-04-04 14:31:24.000000 teareduce-0.2.5/src/teareduce/sdistortion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.2.5/src/teareduce/sliceregion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5426 2024-04-04 14:31:46.000000 teareduce-0.2.5/src/teareduce/statsummary.py
--rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-04-04 14:32:39.000000 teareduce-0.2.5/src/teareduce/version.py
--rw-r--r--   0 cardiel    (501) staff       (20)    68706 2024-04-04 14:24:28.000000 teareduce-0.2.5/src/teareduce/wavecal.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.2.5/src/teareduce/zscale.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.194128 teareduce-0.2.5/src/teareduce.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      668 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       77 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/top_level.txt
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.757660 teareduce-0.3.0/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.3.0/LICENSE.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-08 19:37:29.757423 teareduce-0.3.0/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.3.0/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)     1624 2024-01-12 07:48:48.000000 teareduce-0.3.0/pyproject.toml
+-rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-04-08 19:37:29.757713 teareduce-0.3.0/setup.cfg
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.748712 teareduce-0.3.0/src/
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.755976 teareduce-0.3.0/src/teareduce/
+-rw-r--r--   0 cardiel    (501) staff       (20)      982 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.3.0/src/teareduce/avoid_astropy_warnings.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1685 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/correct_pincushion_distortion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.3.0/src/teareduce/cosmicrays.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.3.0/src/teareduce/ctext.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.3.0/src/teareduce/draw_rectangle.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.3.0/src/teareduce/elapsed_time.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.3.0/src/teareduce/imshow.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.3.0/src/teareduce/peaks_spectrum.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.3.0/src/teareduce/polfit.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.3.0/src/teareduce/robust_std.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5916 2024-04-08 18:48:08.000000 teareduce-0.3.0/src/teareduce/sdistortion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.3.0/src/teareduce/sliceregion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5426 2024-04-04 14:31:46.000000 teareduce-0.3.0/src/teareduce/statsummary.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/version.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    68706 2024-04-04 14:24:28.000000 teareduce-0.3.0/src/teareduce/wavecal.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.3.0/src/teareduce/zscale.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.757123 teareduce-0.3.0/src/teareduce.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      715 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       77 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/top_level.txt
```

### Comparing `teareduce-0.2.5/LICENSE.txt` & `teareduce-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/PKG-INFO` & `teareduce-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.2.5
+Version: 0.3.0
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `teareduce-0.2.5/README.md` & `teareduce-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/pyproject.toml` & `teareduce-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/__init__.py` & `teareduce-0.3.0/src/teareduce/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # This file is part of teareduce
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 # License-Filename: LICENSE.txt
 #
 
 from .avoid_astropy_warnings import avoid_astropy_warnings
+from .correct_pincushion_distortion import correct_pincushion_distortion
 from .cosmicrays import cr2images, apply_cr2images_ccddata, crmedian
 from .ctext import ctext
 from .draw_rectangle import draw_rectangle
 from .elapsed_time import elapsed_time
 from .imshow import imshow
 from .peaks_spectrum import find_peaks_spectrum, refine_peaks_spectrum
 from .polfit import polfit_residuals, polfit_residuals_with_sigma_rejection
```

### Comparing `teareduce-0.2.5/src/teareduce/avoid_astropy_warnings.py` & `teareduce-0.3.0/src/teareduce/avoid_astropy_warnings.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/cosmicrays.py` & `teareduce-0.3.0/src/teareduce/cosmicrays.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/ctext.py` & `teareduce-0.3.0/src/teareduce/ctext.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/draw_rectangle.py` & `teareduce-0.3.0/src/teareduce/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/elapsed_time.py` & `teareduce-0.3.0/src/teareduce/elapsed_time.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/imshow.py` & `teareduce-0.3.0/src/teareduce/imshow.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/peaks_spectrum.py` & `teareduce-0.3.0/src/teareduce/peaks_spectrum.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/polfit.py` & `teareduce-0.3.0/src/teareduce/polfit.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/robust_std.py` & `teareduce-0.3.0/src/teareduce/robust_std.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/sdistortion.py` & `teareduce-0.3.0/src/teareduce/sdistortion.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     kwargs : dictionary
         Additional arguments for imshow call.
 
     Returns
     -------
     data_straight : numpy array
         2D spectroscopic image corrected from S distortion.
+    poly_funct_peaks : `~numpy.polynomial.polynomial.Polynomial`
+        Fitted polynomial.
 
     """
 
     if ywindow % 2 != 1:
         raise ValueError(f'ywindow={ywindow} must be an odd integer')
     semiwindow = (int(ywindow) - 1) // 2
     if semiwindow < 1:
@@ -173,8 +175,8 @@
         fig, ax = plt.subplots(figsize=(15, 5))
         imshow(fig, ax, data_straight, vmin=vmin, vmax=vmax, title='initial data', aspect=aspect, **kwargs)
         ax.set_ylim(ns_min-0.5, ns_max+0.5)
         plt.tight_layout()
         plt.show()
 
     # return result
-    return data_straight
+    return data_straight, poly_funct_peaks
```

### Comparing `teareduce-0.2.5/src/teareduce/sliceregion.py` & `teareduce-0.3.0/src/teareduce/sliceregion.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/statsummary.py` & `teareduce-0.3.0/src/teareduce/statsummary.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/wavecal.py` & `teareduce-0.3.0/src/teareduce/wavecal.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce/zscale.py` & `teareduce-0.3.0/src/teareduce/zscale.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.5/src/teareduce.egg-info/PKG-INFO` & `teareduce-0.3.0/src/teareduce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.2.5
+Version: 0.3.0
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `teareduce-0.2.5/src/teareduce.egg-info/SOURCES.txt` & `teareduce-0.3.0/src/teareduce.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/teareduce/__init__.py
 src/teareduce/avoid_astropy_warnings.py
+src/teareduce/correct_pincushion_distortion.py
 src/teareduce/cosmicrays.py
 src/teareduce/ctext.py
 src/teareduce/draw_rectangle.py
 src/teareduce/elapsed_time.py
 src/teareduce/imshow.py
 src/teareduce/peaks_spectrum.py
 src/teareduce/polfit.py
```

