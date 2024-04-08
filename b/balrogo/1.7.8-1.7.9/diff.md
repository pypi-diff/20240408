# Comparing `tmp/balrogo-1.7.8.tar.gz` & `tmp/balrogo-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balrogo-1.7.8.tar", max compression
+gzip compressed data, was "balrogo-1.7.9.tar", max compression
```

## Comparing `balrogo-1.7.8.tar` & `balrogo-1.7.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1090 2022-11-20 02:34:33.007100 balrogo-1.7.8/LICENSE
--rw-r--r--   0        0        0     5130 2022-11-20 02:34:33.007295 balrogo-1.7.8/README.md
--rw-r--r--   0        0        0      153 2022-11-20 02:34:33.007442 balrogo-1.7.8/balrogo/__init__.py
--rwxr-xr-x   0        0        0    31718 2024-03-23 15:20:14.611207 balrogo-1.7.8/balrogo/angle.py
--rw-r--r--   0        0        0    88940 2023-06-23 19:28:29.032557 balrogo-1.7.8/balrogo/dynamics.py
--rwxr-xr-x   0        0        0    33854 2023-06-23 19:28:29.033693 balrogo-1.7.8/balrogo/gaia.py
--rwxr-xr-x   0        0        0     5538 2022-11-20 02:34:33.008292 balrogo-1.7.8/balrogo/hrd.py
--rwxr-xr-x   0        0        0    26747 2023-11-26 21:09:08.310718 balrogo-1.7.8/balrogo/marginals.py
--rw-r--r--   0        0        0    10097 2022-11-20 02:34:33.008613 balrogo-1.7.8/balrogo/mock.py
--rwxr-xr-x   0        0        0     5745 2022-11-20 02:34:33.008725 balrogo-1.7.8/balrogo/parallax.py
--rw-r--r--   0        0        0    58955 2023-10-05 21:23:13.404103 balrogo-1.7.8/balrogo/pm.py
--rw-r--r--   0        0        0   111164 2023-11-27 22:27:30.805604 balrogo-1.7.8/balrogo/position.py
--rw-r--r--   0        0        0      875 2024-03-23 15:20:14.611740 balrogo-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 balrogo-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-11-20 02:34:33.007100 balrogo-1.7.9/LICENSE
+-rw-r--r--   0        0        0     5130 2022-11-20 02:34:33.007295 balrogo-1.7.9/README.md
+-rw-r--r--   0        0        0      153 2022-11-20 02:34:33.007442 balrogo-1.7.9/balrogo/__init__.py
+-rwxr-xr-x   0        0        0    31964 2024-04-08 13:44:13.360401 balrogo-1.7.9/balrogo/angle.py
+-rw-r--r--   0        0        0    88940 2023-06-23 19:28:29.032557 balrogo-1.7.9/balrogo/dynamics.py
+-rwxr-xr-x   0        0        0    33854 2023-06-23 19:28:29.033693 balrogo-1.7.9/balrogo/gaia.py
+-rwxr-xr-x   0        0        0     5538 2022-11-20 02:34:33.008292 balrogo-1.7.9/balrogo/hrd.py
+-rwxr-xr-x   0        0        0    26747 2023-11-26 21:09:08.310718 balrogo-1.7.9/balrogo/marginals.py
+-rw-r--r--   0        0        0    10097 2022-11-20 02:34:33.008613 balrogo-1.7.9/balrogo/mock.py
+-rwxr-xr-x   0        0        0     5745 2022-11-20 02:34:33.008725 balrogo-1.7.9/balrogo/parallax.py
+-rw-r--r--   0        0        0    58955 2023-10-05 21:23:13.404103 balrogo-1.7.9/balrogo/pm.py
+-rw-r--r--   0        0        0   117653 2024-04-08 13:44:13.361637 balrogo-1.7.9/balrogo/position.py
+-rw-r--r--   0        0        0      875 2024-04-08 13:44:13.362320 balrogo-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6214 1970-01-01 00:00:00.000000 balrogo-1.7.9/PKG-INFO
```

### Comparing `balrogo-1.7.8/LICENSE` & `balrogo-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/README.md` & `balrogo-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/angle.py` & `balrogo-1.7.9/balrogo/angle.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,17 @@
     d = np.copy(d) * 180 / np.pi
 
     return a, d
 
 
 def sky_to_polar(a, d, a0, d0, ea=None, ed=None):
     """
-    Transforms uncertainties from sky coordinates, in degrees (RA,Dec),
-    into uncertainties from spherical polar coordinates (r,phi).
+    Transforms positions and uncertainties from sky coordinates,
+    in degrees (RA,Dec), into uncertainties from spherical polar
+    coordinates (r,phi).
 
     NOTE: The current version of this function neglects any
     correlations between a and d, and any uncertainties/correlations
     associated to a0 and d0.
 
     Parameters
     ----------
@@ -202,14 +203,20 @@
         The default is None.
     ed : array_like, optional
         Uncertainty in declination, in degrees.
         The default is None.
 
     Returns
     -------
+    r : array_like
+        Radial distance from center, in radians.
+    p : array_like
+        Angle from North to East (pointing towards the source), in radians.
+
+    NOTE: If ea and ed are provided, the functino also returns:
     er : array_like
         Uncertainty in radial distance from center.
     ep : array_like
         Uncertainty in angle between increasing declination and
         the projected radius (pointing towards the source), in radians.
 
     """
```

### Comparing `balrogo-1.7.8/balrogo/dynamics.py` & `balrogo-1.7.9/balrogo/dynamics.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/gaia.py` & `balrogo-1.7.9/balrogo/gaia.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/hrd.py` & `balrogo-1.7.9/balrogo/hrd.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/marginals.py` & `balrogo-1.7.9/balrogo/marginals.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/mock.py` & `balrogo-1.7.9/balrogo/mock.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/parallax.py` & `balrogo-1.7.9/balrogo/parallax.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/pm.py` & `balrogo-1.7.9/balrogo/pm.py`

 * *Files identical despite different names*

### Comparing `balrogo-1.7.8/balrogo/position.py` & `balrogo-1.7.9/balrogo/position.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 from scipy.special import gamma, gammainc, kn, hyp2f1
 from scipy.interpolate import PchipInterpolator
 from scipy.signal import find_peaks
 
 import numdifftools as ndt
 import emcee
 from multiprocessing import Pool
-from multiprocessing import cpu_count
-
-ncpu = cpu_count()
+import os
 
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "Peak position"
 # ---------------------------------------------------------------------------
 
@@ -78,15 +76,23 @@
     # Assigns sigma as the minimum between the distance took to depass the
     # threshold in the left and in the right of the peak
     sigma = min(x_axis[index_right] - peak, peak - x_axis[index_left])
 
     return sigma
 
 
-def find_center(x, y, method="mle", ra0=None, dec0=None, hybrid=True, full_fit=False):
+def find_center(
+    x,
+    y,
+    method="mle",
+    ra0=None,
+    dec0=None,
+    hybrid=True,
+    full_fit=False,
+):
     """
     Fit a center (peak) of the [x,y] data.
 
     Parameters
     ----------
     x : array_like
         Data in x-direction
@@ -172,19 +178,27 @@
 
     """
 
     bins_x = good_bin(x)
     bins_y = good_bin(y)
 
     # Gets the histogram in RA
-    x_hist, x_axis = np.histogram(x, bins=bins_x, range=(np.amin(x), np.amax(x)))
+    x_hist, x_axis = np.histogram(
+        x,
+        bins=bins_x,
+        range=(np.amin(x), np.amax(x)),
+    )
     x_axis = 0.5 * (x_axis[1:] + x_axis[:-1])
 
     # Gets the histogram in Dec
-    y_hist, y_axis = np.histogram(y, bins=bins_y, range=(np.amin(y), np.amax(y)))
+    y_hist, y_axis = np.histogram(
+        y,
+        bins=bins_y,
+        range=(np.amin(y), np.amax(y)),
+    )
     y_axis = 0.5 * (y_axis[1:] + y_axis[:-1])
 
     # Gets the histogram of the 2d (RA,Dec) data
     hist, xedges, yedges = np.histogram2d(x, y, bins=[bins_x, bins_y])
     hist = hist.T
 
     # Estimates the RA and Dec means from the galactic object by taking the
@@ -203,31 +217,53 @@
     unc = np.nan
 
     many_tracers = True
     shift = list()
     count = 0
     while many_tracers is True:
         idx = np.where(
-            angle.sky_distance_deg(x, y, center[0], center[1]) < (0.9**count) * sigma
+            angle.sky_distance_deg(
+                x,
+                y,
+                center[0],
+                center[1],
+            )
+            < (0.9**count) * sigma,
         )
 
         bins_x = good_bin(x[idx])
         bins_y = good_bin(y[idx])
 
         if len(idx[0]) < bins_x * bins_y and count > 0:
             many_tracers = False
             return center, unc
 
-        hist, xedges, yedges = np.histogram2d(x[idx], y[idx], bins=[bins_x, bins_y])
+        hist, xedges, yedges = np.histogram2d(
+            x[idx],
+            y[idx],
+            bins=[bins_x, bins_y],
+        )
 
         xedges = 0.5 * (xedges[1:] + xedges[:-1])
         yedges = 0.5 * (yedges[1:] + yedges[:-1])
 
-        cmx = np.nansum(xedges * np.sum(hist, axis=1)) / np.nansum(np.sum(hist, axis=1))
-        cmy = np.nansum(yedges * np.sum(hist, axis=0)) / np.nansum(np.sum(hist, axis=0))
+        cmx = np.nansum(
+            xedges
+            * np.sum(
+                hist,
+                axis=1,
+            )
+        ) / np.nansum(np.sum(hist, axis=1))
+        cmy = np.nansum(
+            yedges
+            * np.sum(
+                hist,
+                axis=0,
+            )
+        ) / np.nansum(np.sum(hist, axis=0))
 
         shift.append(angle.sky_distance_deg(cmx, cmy, center[0], center[1]))
 
         center = np.asarray([cmx, cmy])
         unc = np.median(shift)
 
         count += 1
@@ -278,15 +314,18 @@
         (np.nanquantile(y, 0.16), np.nanquantile(y, 0.84)),
     ]
 
     mle_model = differential_evolution(
         lambda c: likelihood_plummer_freec(c, x, y), bounds
     )
     results = mle_model.x
-    hfun = ndt.Hessian(lambda c: likelihood_plummer_freec(c, x, y), full_output=True)
+    hfun = ndt.Hessian(
+        lambda c: likelihood_plummer_freec(c, x, y),
+        full_output=True,
+    )
 
     hessian_ndt, info = hfun(results)
     if hybrid is False:
         arg_null = np.argmin(np.abs(np.diag(hessian_ndt)))
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=1)
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=0)
         results = np.delete(results, arg_null)
@@ -361,15 +400,16 @@
     ]
 
     mle_model = differential_evolution(
         lambda c: likelihood_plummer_center(c, x, y, ra0, dec0, rmax), bounds
     )
     results = mle_model.x
     hfun = ndt.Hessian(
-        lambda c: likelihood_plummer_center(c, x, y, ra0, dec0, rmax), full_output=True
+        lambda c: likelihood_plummer_center(c, x, y, ra0, dec0, rmax),
+        full_output=True,
     )
 
     hessian_ndt, info = hfun(results)
     if hybrid is False:
         arg_null = np.argmin(np.abs(np.diag(hessian_ndt)))
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=1)
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=0)
@@ -600,15 +640,26 @@
 
         density = surface_density(x=x, y=y, x0=x0, y0=y0)
         size = len(x)
 
     mw_dens = np.nanmin(density[1])
     density[1] = density[1] - mw_dens
     nilop = (
-        mw_dens * np.pi * (density[0][len(density[0]) - 1] ** 2 - density[0][0] ** 2)
+        mw_dens
+        * np.pi
+        * (
+            density[0][
+                len(
+                    density[0],
+                )
+                - 1
+            ]
+            ** 2
+            - density[0][0] ** 2
+        )
     )
     n_local = np.zeros(len(density[0]))
     for i in range(len(density[0])):
         n_local[i] = (
             np.nansum(n_local)
             + 2 * np.pi * density[1][i] * density[0][i] * density[3][i]
         )
@@ -1006,15 +1057,18 @@
 
     term1 = (
         -(1 + X * X)
         * (-3 + X * X + gam)
         * hyp2f1(1, (5 - gam) / 2, -1 / 2, -1 / (X * X))
     )
     term2 = (-17 + X**4 - X * X * (gam - 8) - gam * (gam - 9)) * hyp2f1(
-        1, (5 - gam) / 2, 1 / 2, -1 / (X * X)
+        1,
+        (5 - gam) / 2,
+        1 / 2,
+        -1 / (X * X),
     )
     term3 = (gam - 3 - X * X) * (term1 + term2)
 
     num = -(gam - 3) * (X * X * (gam - 4) * (gam - 2) + term3)
     den = 2 * X**4 * (1 + X * X) * (gam - 4) * (gam - 2)
 
     sd = num / den
@@ -1041,15 +1095,20 @@
     -------
     VD : array_like (same shape as gam), float
         Normalized volume density profile.
 
     """
 
     num = (
-        2 * x ** (-gam) * (1 + x * x) ** (0.5 * (gam - bet)) * gamma(0.5 * (bet - gam))
+        2
+        * x ** (-gam)
+        * (1 + x * x) ** (0.5 * (gam - bet))
+        * gamma(
+            0.5 * (bet - gam),
+        )
     )
 
     den = gamma(0.5 * (bet - 3)) * gamma(0.5 * (3 - gam))
 
     vd = num / den
 
     return vd
@@ -1073,35 +1132,45 @@
     N : array_like (same shape as gam), float
         gPlummer projected number.
 
     """
 
     term1 = 1 / (X * X * (gam - 4) * (gam - 2))
     term2 = (
-        (1 + X * X) * (X * X + gam - 3) * hyp2f1(1, (5 - gam) / 2, -1 / 2, -1 / (X * X))
+        (1 + X * X)
+        * (X * X + gam - 3)
+        * hyp2f1(
+            1,
+            (5 - gam) / 2,
+            -1 / 2,
+            -1 / (X * X),
+        )
     )
     term3 = (17 - X**4 + X * X * (gam - 8) + gam * (gam - 9)) * hyp2f1(
-        1, (5 - gam) / 2, 1 / 2, -1 / (X * X)
+        1,
+        (5 - gam) / 2,
+        1 / 2,
+        -1 / (X * X),
     )
 
     N = 1 + term1 * (term2 + term3) * (3 - gam)
 
     return N
 
 
 def likelihood_gplummer(params, Ri):
     """
     Likelihood function of the gPlummer profile plus a constant contribution
     from fore/background tracers.
 
     Parameters
     ----------
-    Parameters to be fitted: gPlummer inner slope, gPlummer characteristic radius a and
-                             log-ratio of galactic objects and Milky
-                             Way stars.
+    Parameters to be fitted:
+        gPlummer inner slope, gPlummer characteristic radius a and
+        log-ratio of galactic objects and Milky Way stars.
     Ri : array_like
         Array containing the ensemble of projected radii.
 
     Returns
     -------
     L : float
        Likelihood.
@@ -1174,15 +1243,24 @@
         gam = np.asarray([gam])
         bet = np.asarray([bet])
         a = np.asarray([a])
         frac = np.asarray([frac])
 
     fi = 0
     for i in range(len(gam)):
-        dens = (ri / a[i]) * (ri / a[i]) * vd_gplummer(gam[i], bet[i], ri / a[i]) / a[i]
+        dens = (
+            (ri / a[i])
+            * (ri / a[i])
+            * vd_gplummer(
+                gam[i],
+                bet[i],
+                ri / a[i],
+            )
+            / a[i]
+        )
         fi = fi + frac[i] * dens
 
     idx_valid = np.logical_not(np.isnan(np.log(fi)))
 
     L = -np.sum(np.log(fi[idx_valid]))
 
     return L
@@ -1190,17 +1268,17 @@
 
 def lnprior_gp(params, guess, bounds):
     """
     Prior assumptions on the parameters.
 
     Parameters
     ----------
-    Parameters to be fitted: gPlummer inner slope, gPlummer characteristic radius a and
-                             log-ratio of galactic objects and Milky
-                             Way stars.
+    Parameters to be fitted:
+        gPlummer inner slope, gPlummer characteristic radius a and
+        log-ratio of galactic objects and Milky Way stars.
     guess : array_like
         Array containing the initial guess of the parameters.
     bounds : array_like
         Array containing the interval of variation of the parameters.
 
 
     Returns
@@ -1261,17 +1339,17 @@
 
 def lnprob_gp(params, Ri, guess, bounds):
     """
     log-probability of fit parameters.
 
     Parameters
     ----------
-    Parameters to be fitted: gPlummer inner slope, gPlummer characteristic radius a and
-                             log-ratio of galactic objects and Milky
-                             Way stars.
+    Parameters to be fitted:
+        gPlummer inner slope, gPlummer characteristic radius a and
+        log-ratio of galactic objects and Milky Way stars.
     Ri : array_like
         Array containing the ensemble of projected radii.
     guess : array_like
         Array containing the initial guess of the parameters.
     bounds : array_like
         Array containing the interval of variation of the parameters.
 
@@ -1291,17 +1369,17 @@
 
 def lnprob_gp_dens(params, ri, bounds, gauss, shells):
     """
     log-probability of fit parameters.
 
     Parameters
     ----------
-    Parameters to be fitted: gPlummer inner slope, gPlummer characteristic radius a and
-                             log-ratio of galactic objects and Milky
-                             Way stars.
+    Parameters to be fitted:
+        gPlummer inner slope, gPlummer characteristic radius a and
+        log-ratio of galactic objects and Milky Way stars.
     Ri : array_like
         Array containing the ensemble of projected radii.
     bounds : array_like
         Array containing the interval of variation of the parameters.
     gauss : array_like
         Gaussian priors.
 
@@ -1346,15 +1424,20 @@
     Returns
     -------
     VD : array_like (same shape as gam), float
         Normalized volume density profile.
 
     """
 
-    fac = ((3 - gam) / (2 - gam)) ** (3 - gam) / hyp2f1(1, 1, 4 - gam, -2 + gam)
+    fac = ((3 - gam) / (2 - gam)) ** (3 - gam) / hyp2f1(
+        1,
+        1,
+        4 - gam,
+        -2 + gam,
+    )
     vd = fac * x ** (-gam) * (1 + x) ** (gam - 3)
 
     return vd
 
 
 def m_nfw(gam, x):
     """
@@ -1372,16 +1455,30 @@
     Returns
     -------
     M : array_like (same shape as gam), float
         Normalized mass profile.
 
     """
 
-    fac = ((3 - gam) / (2 - gam)) ** (3 - gam) / hyp2f1(1, 1, 4 - gam, -2 + gam)
-    m = hyp2f1(3 - gam, 3 - gam, 4 - gam, -x) * x ** (3 - gam) / (fac * (3 - gam))
+    fac = ((3 - gam) / (2 - gam)) ** (3 - gam) / hyp2f1(
+        1,
+        1,
+        4 - gam,
+        -2 + gam,
+    )
+    m = (
+        hyp2f1(
+            3 - gam,
+            3 - gam,
+            4 - gam,
+            -x,
+        )
+        * x ** (3 - gam)
+        / (fac * (3 - gam))
+    )
 
     return m
 
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "King 1962 profile functions"
@@ -1420,15 +1517,20 @@
     idx_nvalid = np.where(X > Xt)
 
     X = X * X
     Xt = Xt * Xt
 
     num = 1 / np.sqrt(1 + X) - 1 / np.sqrt(1 + Xt)
     num = num * num
-    den = np.log(1 + Xt) - (3 * np.sqrt(1 + Xt) - 1) * (np.sqrt(1 + Xt) - 1) / (1 + Xt)
+    den = np.log(1 + Xt) - (3 * np.sqrt(1 + Xt) - 1) * (
+        np.sqrt(
+            1 + Xt,
+        )
+        - 1
+    ) / (1 + Xt)
 
     sd = num / den
 
     sd[idx_nvalid] = 0
 
     return sd
 
@@ -1457,16 +1559,29 @@
         X = np.asarray([X])
 
     idx_nvalid = np.where(X > Xt)
 
     X = X * X
     Xt = Xt * Xt
 
-    num = np.log(1 + X) - 4 * (np.sqrt(1 + X) - 1) / np.sqrt(1 + Xt) + X / (1 + Xt)
-    den = np.log(1 + Xt) - (3 * np.sqrt(1 + Xt) - 1) * (np.sqrt(1 + Xt) - 1) / (1 + Xt)
+    num = (
+        np.log(1 + X)
+        - 4
+        * (np.sqrt(1 + X) - 1)
+        / np.sqrt(
+            1 + Xt,
+        )
+        + X / (1 + Xt)
+    )
+    den = np.log(1 + Xt) - (3 * np.sqrt(1 + Xt) - 1) * (
+        np.sqrt(
+            1 + Xt,
+        )
+        - 1
+    ) / (1 + Xt)
 
     N = num / den
 
     N[idx_nvalid] = 1
 
     return N
 
@@ -1678,16 +1793,16 @@
     N = term1 + term2 * (term3a - 3 * X * X * term3b)
 
     return N
 
 
 def likelihood_chernquist(params, Ri):
     """
-    Likelihood function of the Cored Hernquist profile plus a constant contribution
-    from fore/background tracers.
+    Likelihood function of the Cored Hernquist profile plus a
+    constant contribution from fore/background tracers.
 
     Parameters
     ----------
     Parameters to be fitted: Scale radius,
                              log-ratio of galactic objects and Milky
                              Way stars.
     Ri : array_like
@@ -1972,15 +2087,23 @@
         frac = 1
         gam = np.asarray([gam])
         a = np.asarray([a])
         frac = np.asarray([frac])
 
     fi = 0
     for i in range(len(gam)):
-        dens = (ri / a[i]) * (ri / a[i]) * vd_kazantzidis(gam[i], ri / a[i]) / a[i]
+        dens = (
+            (ri / a[i])
+            * (ri / a[i])
+            * vd_kazantzidis(
+                gam[i],
+                ri / a[i],
+            )
+            / a[i]
+        )
         fi = fi + frac[i] * dens
 
     idx_valid = np.logical_not(np.isnan(np.log(fi)))
 
     L = -np.sum(np.log(fi[idx_valid]))
 
     return L
@@ -2192,19 +2315,19 @@
     else:
         if R >= d + Rmax:
             return 1
         arg1 = (R * R + d * d - Rmax * Rmax) / (2 * R * d)
         term1 = -a * a * np.arccos(arg1) / (np.pi * (a * a + R * R))
 
         arg2 = np.sqrt(
-            -(d**4) - (R * R - Rmax * Rmax) ** 2 + 2 * d * d * (R * R + Rmax * Rmax)
+            -(d**4) - (R * R - Rmax * Rmax) ** 2 + 2 * d * d * (R * R + Rmax * Rmax),
         )
 
         arg3 = -np.sqrt(
-            a**4 + (d * d - Rmax * Rmax) ** 2 + 2 * a * a * (d * d + Rmax * Rmax)
+            a**4 + (d * d - Rmax * Rmax) ** 2 + 2 * a * a * (d * d + Rmax * Rmax),
         )
 
         arg4 = (d * d - Rmax * Rmax) ** 2 - R * R * (d * d + Rmax * Rmax)
 
         arg5 = np.arctan(arg4 / (arg2 * (d * d - Rmax * Rmax)))
 
         term2 = arg3 * arg5
@@ -2436,76 +2559,79 @@
     Likelihood function of the Plummer profile plus a constant contribution
     from fore/background tracers. Fits the center considering an
     elliptical Plummer.
 
     Parameters
     ----------
     params : array_like
-        Parameters to be fitted: Plummer characteristic radius a and
-                                 log-ratio of galactic objects and Milky
-                                 Way stars.
+        Parameters to be fitted:
+            - log-Plummer major axis, a [degree]
+            - Projected ellipticity, e = 1 - b/a
+            - Major axis angle, from North to East, phi [radians]
+            - log-ratio of galactic objects and Milky Way stars.
+            - R.A. of galactic object center.
+            - Dec. of galactic object center.
     x : array_like
         Array containing the ensemble of ra data.
     y : array_like
         Array containing the ensemble of dec data.
 
     Returns
     -------
     L : float
        Likelihood.
 
     """
 
     a = 10 ** params[0]
-    b = 10 ** params[1]
-    theta = params[2]
+    el = params[1]
+    phi = params[2]
     if params[3] < -10:
         norm = 0
     else:
         norm = 10 ** params[3]
 
     cmx = params[4]
     cmy = params[5]
 
-    # Transforms data in radians
-    x = x * (np.pi / 180)
-    y = y * (np.pi / 180)
-
+    # TRANSFORMS DATA FROM DEGREES TO RADIANS
+    a = np.copy(a) * (np.pi / 180)
+    x = np.copy(x) * (np.pi / 180)
+    y = np.copy(y) * (np.pi / 180)
     x0 = cmx * (np.pi / 180)
     y0 = cmy * (np.pi / 180)
 
-    # projects the data
+    # PROJECTS THE DATA, CORRECTING FOR ZERO-POINT
     xp = np.sin(x - x0) * np.cos(y)
     yp = np.cos(y0) * np.sin(y) - np.sin(y0) * np.cos(y) * np.cos(x - x0)
 
-    # Transforms data back to degree
-    xp = xp * (180 / np.pi)
-    yp = yp * (180 / np.pi)
-
-    xnew = (xp) * np.cos(theta) + (yp) * np.sin(theta)
-    ynew = -(xp) * np.sin(theta) + (yp) * np.cos(theta)
+    # ROTATES ELLIPSE SO MAJOR AXIS ALIGNS WITH X DIRECTION
+    theta = phi - np.pi * 0.5
+    xnew = (xp) * np.cos(theta) - (yp) * np.sin(theta)
+    ynew = (xp) * np.sin(theta) + (yp) * np.cos(theta)
 
-    m = np.sqrt((xnew / a) * (xnew / a) + (ynew / b) * (ynew / b))
+    # DEFINES VARIABLES OF INTEREST
     r = np.sqrt(xnew * xnew + ynew * ynew)
+    xi = np.arctan2(ynew, xnew)
+    x = r / a
+    xmax = np.amax(r) / a
+    xmin = np.amin(r) / a
+
+    # COMPUTES TERMS OF GLOBAL EXPRESSION
+    num1 = (1 - el * el) ** 1.5
+    den1a = ((x * el * np.cos(xi)) ** 2 + el * el - (1 + x * x)) ** 2
+    den1b = xmax * xmax / np.sqrt(
+        (1 + xmax * xmax) * (xmax * xmax + 1 - el * el)
+    ) - xmin * xmin / np.sqrt((1 + xmin * xmin) * (xmin * xmin + 1 - el * el))
+    term1 = num1 / (den1a * den1b)
 
-    mmax = np.amax(m)
-    mmin = np.amin(m)
+    term2 = norm / (xmax**2 - xmin**2)
 
-    rmax = np.amax(r)
-    rmin = np.amin(r)
-
-    N_sys_tot = n_plummer(mmax) - n_plummer(mmin)
-
-    SD = sd_plummer(m) + norm * N_sys_tot * a * b * 0.5 * (np.pi / 180) ** 2 / (
-        np.cos(rmin * np.pi / 180) - np.cos(rmax * np.pi / 180)
-    )
-
-    Ntot = N_sys_tot * (1 + norm)
-
-    fi = (SD / Ntot) / (a * b)
+    # ASSIGNS PDF
+    fi = x * (term1 + term2) / (a * np.pi * (1 + norm))
 
     idx_valid = np.logical_not(np.isnan(np.log(fi)))
 
     L = -np.sum(np.log(fi[idx_valid]))
 
     return L
 
@@ -2536,53 +2662,51 @@
     if (guess[0] - bounds[0] <= params[0] <= guess[0] + bounds[0]) and (
         guess[1] - bounds[1] <= params[1] <= guess[1] + bounds[1]
     ):
         return 0.0
     return -np.inf
 
 
-def lnprior_ep(params, bounds, gauss):
+def lnprior_plummer_ell_center(params, bounds, gauss):
     """
     Prior assumptions on the parameters.
 
     Parameters
     ----------
     params : array_like
-        Parameters to be fitted: Plummer characteristic radius a and
-                                 log-ratio of galactic objects and Milky
-                                 Way stars.
+        Parameters to be fitted:
+            - log-Plummer major axis, a [degree]
+            - Projected ellipticity, e = 1 - b/a
+            - Major axis angle, from North to East, phi [radians]
+            - log-ratio of galactic objects and Milky Way stars.
+            - R.A. of galactic object center.
+            - Dec. of galactic object center.
     bounds : array_like
         Array containing the interval of variation of the parameters.
     gauss : array_like
         Gaussian priors.
 
     Returns
     -------
     log-prior probability : float
         0, if the parameters are within the prior range,
         - Infinity otherwise.
 
     """
 
-    if (
-        (bounds[0, 0] < params[0] < bounds[0, 1])
-        and (bounds[1, 0] < params[1] < bounds[1, 1])
-        and (bounds[2, 0] < params[2] < bounds[2, 1])
-        and (bounds[3, 0] < params[3] < bounds[3, 1])
-        and (bounds[4, 0] < params[4] < bounds[4, 1])
-        and (bounds[5, 0] < params[5] < bounds[5, 1])
-    ):
-        lprior = 0
-        for i in range(len(params)):
+    lprior = 0
+    for i in range(len(params)):
+        if bounds[i, 0] < params[i] < bounds[i, 1]:
             if gauss[i, 1] > 0:
-                nutmp = (params[i] - gauss[i, 0]) / gauss[i, 1]
-                lprior = lprior - 0.5 * nutmp * nutmp
-        return lprior
-    else:
-        return -np.inf
+                lprior -= 0.5 * ((params[i] - gauss[i, 0]) / gauss[i, 1]) ** 2
+            else:
+                lprior -= 0.0
+        else:
+            lprior -= np.inf
+    return lprior
 
 
 def lnprob_p(params, Ri, guess, bounds):
     """
     log-probability of fit parameters.
 
     Parameters
@@ -2608,43 +2732,51 @@
 
     lp = lnprior_p(params, guess, bounds)
     if not np.isfinite(lp):
         return -np.inf
     return lp - likelihood_plummer(params, Ri)
 
 
-def lnprob_ep(params, x, y, bounds, gauss):
+def lnprob_plummer_ell_center(params, x, y, bounds, gauss):
     """
     log-probability of fit parameters.
 
     Parameters
     ----------
     params : array_like
-    Parameters to be fitted: Plummer characteristic radius a and
-                             log-ratio of galactic objects and Milky
-                             Way stars.
-    Ri : array_like
-        Array containing the ensemble of projected radii.
-    guess : array_like
-        Array containing the initial guess of the parameters.
+        Parameters to be fitted:
+            - log-Plummer major axis, a [degree]
+            - Projected ellipticity, e = 1 - b/a
+            - Major axis angle, from North to East, phi [radians]
+            - log-ratio of galactic objects and Milky Way stars.
+            - R.A. of galactic object center.
+            - Dec. of galactic object center.
+    x : array_like
+        Array containing the ensemble of ra data.
+    y : array_like
+        Array containing the ensemble of dec data.
     bounds : array_like
         Array containing the interval of variation of the parameters.
+    gauss : array_like
+        Array containing Gaussian priors. Axis = 1 should contain
+        zeros if one is to assume flat priors based on bounds.
 
 
     Returns
     -------
     log-prior probability : float
         log-probability of fit parameters.
 
     """
 
-    lp = lnprior_ep(params, bounds, gauss)
+    lp = lnprior_plummer_ell_center(params, bounds, gauss)
     if not np.isfinite(lp):
-        return -np.inf
-    return lp - likelihood_plummer_ell_center(params, x, y)
+        return -np.inf, -np.inf
+    lprob = lp - likelihood_plummer_ell_center(params, x, y)
+    return lprob, lp
 
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "DM profile functions"
 # ---------------------------------------------------------------------------
 
@@ -2914,15 +3046,23 @@
         frac = 1
         n = np.asarray([n])
         ra = np.asarray([ra])
         frac = np.asarray([frac])
 
     fi = 0
     for i in range(len(n)):
-        dens = (ri / ra[i]) * (ri / ra[i]) * vd_einasto(n[i], ri / ra[i]) / ra[i]
+        dens = (
+            (ri / ra[i])
+            * (ri / ra[i])
+            * vd_einasto(
+                n[i],
+                ri / ra[i],
+            )
+            / ra[i]
+        )
         fi = fi + frac[i] * dens
 
     idx_valid = np.logical_not(np.isnan(np.log(fi)))
 
     L = -np.sum(np.log(fi[idx_valid]))
 
     return L
@@ -3070,15 +3210,18 @@
     """
 
     peaks, _ = find_peaks(f)
 
     valididx = np.arange(int(0.2 * len(f)), int(0.8 * len(f)))
     validpeak = peaks[
         np.intersect1d(
-            np.where(peaks > np.nanmin(valididx)), np.where(peaks < np.nanmax(valididx))
+            np.where(peaks > np.nanmin(valididx)),
+            np.where(
+                peaks < np.nanmax(valididx),
+            ),
         )
     ]
     size = len(validpeak)
     if size < 2:
         return validpeak
 
     peak1 = np.nanargmax(f[peaks])
@@ -3096,15 +3239,22 @@
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "Fitting procedure"
 # ---------------------------------------------------------------------------
 
 
-def maximum_likelihood(x=None, y=None, model="plummer", x0=None, y0=None, hybrid=True):
+def maximum_likelihood(
+    x=None,
+    y=None,
+    model="plummer",
+    x0=None,
+    y0=None,
+    hybrid=True,
+):
     """
     Calls a maximum likelihood fit of the surface density paramters of
     the joint distribution of galactic object plus Milky Way stars.
 
     Parameters
     ----------
     x : array_like, optional
@@ -3177,64 +3327,100 @@
     hmr = np.log10(hmr)
     norm = np.log10(norm)
     if hybrid is False:
         norm = -50
 
     if model == "sersic":
         bounds = [(0.5, 10), (hmr - 2, hmr + 2), (norm - 2, norm + 2)]
-        mle_model = differential_evolution(lambda c: likelihood_sersic(c, ri), bounds)
+        mle_model = differential_evolution(
+            lambda c: likelihood_sersic(c, ri),
+            bounds,
+        )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_sersic(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_sersic(c, ri),
+            full_output=True,
+        )
 
     elif model == "kazantzidis":
         bounds = [(hmr - 2, hmr + 2), (norm - 2, norm + 2)]
         mle_model = differential_evolution(
             lambda c: likelihood_kazantzidis(c, ri), bounds
         )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_kazantzidis(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_kazantzidis(c, ri),
+            full_output=True,
+        )
 
     elif model == "plummer":
         bounds = [(hmr - 2, hmr + 2), (norm - 2, norm + 2)]
-        mle_model = differential_evolution(lambda c: likelihood_plummer(c, ri), bounds)
+        mle_model = differential_evolution(
+            lambda c: likelihood_plummer(c, ri),
+            bounds,
+        )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_plummer(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_plummer(c, ri),
+            full_output=True,
+        )
 
     elif model == "gplummer":
         bounds = [(0, 2), (hmr - 2, hmr + 2), (norm - 2, norm + 2)]
-        mle_model = differential_evolution(lambda c: likelihood_gplummer(c, ri), bounds)
+        mle_model = differential_evolution(
+            lambda c: likelihood_gplummer(c, ri),
+            bounds,
+        )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_gplummer(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_gplummer(c, ri),
+            full_output=True,
+        )
 
     elif model == "king62":
         conc = np.log10(np.nanmax(ri)) - hmr
-        bounds = [(0, max(conc + 2, 3)), (hmr - 3, hmr + 1), (norm - 2, norm + 2)]
-        mle_model = differential_evolution(lambda c: likelihood_king62(c, ri), bounds)
+        bounds = [
+            (0, max(conc + 2, 3)),
+            (hmr - 3, hmr + 1),
+            (norm - 2, norm + 2),
+        ]
+        mle_model = differential_evolution(
+            lambda c: likelihood_king62(c, ri),
+            bounds,
+        )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_king62(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_king62(c, ri),
+            full_output=True,
+        )
 
     elif model == "chernquist":
         bounds = [(hmr - 2, hmr + 2), (norm - 2, norm + 2)]
         mle_model = differential_evolution(
             lambda c: likelihood_chernquist(c, ri), bounds
         )
         results = mle_model.x
-        hfun = ndt.Hessian(lambda c: likelihood_chernquist(c, ri), full_output=True)
+        hfun = ndt.Hessian(
+            lambda c: likelihood_chernquist(c, ri),
+            full_output=True,
+        )
 
     hessian_ndt, info = hfun(results)
     if hybrid is False:
         arg_null = np.argmin(np.abs(np.diag(hessian_ndt)))
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=1)
         hessian_ndt = np.delete(hessian_ndt, arg_null, axis=0)
 
     try:
         var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
     except np.linalg.LinAlgError as err:
         if "Singular matrix" in str(err):
-            print("WARNING: Errors are deprecated --> assigning uncertainties as -1.")
+            print(
+                "WARNING: Errors are deprecated --> assigning uncertainties as -1.",
+            )
             var = -np.ones(len(results))
         else:
             raise ValueError("Error when computing uncertainties.")
 
     return results, var
 
 
@@ -3246,17 +3432,19 @@
     steps=1000,
     ini=None,
     bounds=None,
     use_pool=False,
     x0=None,
     y0=None,
     hybrid=True,
-    center_fit=False,
-    gaussp=False,
+    gaussp=None,
     values=None,
+    filepath=None,
+    continue_run=False,
+    show_progress=False,
 ):
     """
     MCMC routine based on the emcee package (Foreman-Mackey et al, 2013).
 
     The user is strongly encouraged to provide initial guesses,
     which can be derived with the "maximum_likelihood" method,
     previously checked to provide reasonable fits.
@@ -3271,14 +3459,15 @@
         Surface density model to be considered. Available options are:
              - 'sersic'
              - 'kazantzidis'
              - 'plummer'
              - 'gplummer'
              - 'king62'
              - 'chernquist'
+             - 'eplummer'
         The default is 'plummer'.
     nwalkers : int, optional
         Number of Markov chains. The default is None.
     steps : int, optional
         Number of steps for each chain. The default is 1000.
     ini : array_like, optional
         Array containing the initial guess of the parameters.
@@ -3297,35 +3486,42 @@
     x0 : float, optional
         Peak of data in x-direction. The default is None.
     y0 : float, optional
         Peak of data in y-direction. The default is None.
     hydrid :  boolean, optional
         "True", if the user whises to consider field stars in the fit.
         The default is True.
-    center_fit :  boolean, optional
-        "True", if the user whises to allow for center fit.
-        Currently only available for model "eplummer".
-        The default is False.
     gaussp : boolean, optional
         "True", if the user wishes Gaussian priors to be considered.
         The default is False.
     values : array_like, optional
         Array containing some of the parameters already fitted. If not fitted,
         they are filled with np.nan.
         The default is None.
+    filepath : string, optional
+        Path in your machine where to store steps of MCMC chain.
+        The default is None.'
+    continue_run : bool, optional
+        "True", if the user wishes to continue a MCMC realization that was
+        interrupted. Only available if filepath is provided.
+        The default is False.
+    show_progress : bool, optional
+        "True, if the user wishes to keep track of MCMC progress.
+        The default is False.
 
     Raises
     ------
     ValueError
         Surface density model is not one of the following:
             - 'sersic'
             - 'kazantzidis'
             - 'plummer'
             - 'gplummer'
             - 'king62'
+            - 'eplummer'
         No data is provided.
 
     Returns
     -------
     chain : array_like
         Set of chains from the MCMC.
 
@@ -3341,107 +3537,192 @@
     ]:
         raise ValueError("Does not recognize surface density model.")
 
     if (x is None and y is None) or (x is None):
         raise ValueError("Please provide the data to be fitted.")
 
     if model == "eplummer":
-        func = lnprob_ep
+        if filepath is None:
+            raise ValueError("Please provide a path to store the fit results.")
 
-        cmx, cmy = np.nanquantile(x, 0.5), np.nanquantile(y, 0.5)
-        hmr, norm = initial_guess_sd(x=x, y=y, x0=cmx, y0=cmy)
+        func = lnprob_plummer_ell_center
 
-        hmr = np.log10(hmr)
-        norm = np.log10(norm)
+        if ini is None:
+            cmx, cmy = np.nanquantile(x, 0.5), np.nanquantile(y, 0.5)
+            hmr, norm = initial_guess_sd(x=x, y=y, x0=cmx, y0=cmy)
+
+            hmr = np.log10(hmr)
+            norm = np.log10(norm)
+        else:
+            hmr = ini[0]
+            norm = ini[2]
 
         if hybrid is False:
             values[2] = -50
 
-        bounds = [
-            (hmr - 2, hmr + 2),
-            (hmr - 2, hmr + 2),
-            (-np.pi / 2, np.pi / 2),
-            (norm - 2, norm + 2),
-            (np.nanquantile(x, 0.16), np.nanquantile(x, 0.84)),
-            (np.nanquantile(y, 0.16), np.nanquantile(y, 0.84)),
-        ]
+        if bounds is None:
+            bounds = [
+                (hmr - 2, hmr + 2),
+                (0, 1),
+                (0, np.pi),
+                (norm - 2, norm + 2),
+                (np.nanquantile(x, 0.16), np.nanquantile(x, 0.84)),
+                (np.nanquantile(y, 0.16), np.nanquantile(y, 0.84)),
+            ]
 
         if values is None:
             values = np.zeros(len(bounds))
             values[:] = np.nan
 
         for i in range(len(values)):
             if np.logical_not(np.isnan(values[i])):
                 bounds[i] = (
                     values[i] - 1e-7 * np.abs(values[i]),
                     values[i] + 1e-7 * np.abs(values[i]),
                 )
 
-        mle_model = differential_evolution(
-            lambda c: likelihood_plummer_ell_center(c, x, y), bounds
-        )
-        results = mle_model.x
-        hfun = ndt.Hessian(
-            lambda c: likelihood_plummer_ell_center(c, x, y), full_output=True
-        )
-
-        hessian_ndt, info = hfun(results)
-        for i in range(len(values) - 1, -1, -1):
-            if np.logical_not(np.isnan(values[i])):
-                hessian_ndt = np.delete(hessian_ndt, i, axis=1)
-                hessian_ndt = np.delete(hessian_ndt, i, axis=0)
-                results[i] = values[i]
-
-        var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
-        for i in range(len(values)):
-            if np.logical_not(np.isnan(values[i])):
-                var = np.insert(var, i, 1e-9 * np.abs(values[i]))
-
         if ini is None:
-            ini = np.zeros(len(results))
-            for i in range(len(results)):
-                if bounds[i][0] < results[i] < bounds[i][1]:
-                    ini[i] = results[i]
-                else:
-                    ini[i] = 0.5 * (bounds[i][0] + bounds[i][1])
+            mle_model = differential_evolution(
+                lambda c: likelihood_plummer_ell_center(c, x, y), bounds
+            )
+            results = mle_model.x
+            hfun = ndt.Hessian(
+                lambda c: likelihood_plummer_ell_center(c, x, y),
+                full_output=True,
+            )
 
-        bounds = np.asarray(bounds)
+            hessian_ndt, info = hfun(results)
+            for i in range(len(values) - 1, -1, -1):
+                if np.logical_not(np.isnan(values[i])):
+                    hessian_ndt = np.delete(hessian_ndt, i, axis=1)
+                    hessian_ndt = np.delete(hessian_ndt, i, axis=0)
+                    results[i] = values[i]
+
+            var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
+            for i in range(len(values)):
+                if np.logical_not(np.isnan(values[i])):
+                    var = np.insert(var, i, 1e-9 * np.abs(values[i]))
+
+            if ini is None:
+                ini = np.zeros(len(results))
+                for i in range(len(results)):
+                    if bounds[i][0] < results[i] < bounds[i][1]:
+                        ini[i] = results[i]
+                    else:
+                        ini[i] = 0.5 * (bounds[i][0] + bounds[i][1])
 
-        ndim = len(ini)  # number of dimensions.
+        # ASSURES THAT MCMC INPUTS ARE VALID
+        bounds = np.asarray(bounds)
+        ndim = np.shape(bounds)[0]
         if nwalkers is None or nwalkers < 2 * ndim:
             nwalkers = int(2 * ndim + 1)
 
-        if gaussp is True:
-            gaussp = np.zeros((ndim, 2))
-            for i in range(ndim):
-                if np.logical_not(np.isnan(var[i])):
-                    gaussp[i, 0] = ini[i]
-                    gaussp[i, 1] = var[i]
-        else:
+        if gaussp is None:
             gaussp = np.zeros((ndim, 2))
 
-        for i in range(ndim):
-            if np.isnan(var[i]):
-                var[i] = 0.5 * (bounds[i, 1] - bounds[i, 0])
+        ranges = 0.5 * (bounds[:, 1] - bounds[:, 0])
+
+        pos = [
+            ini
+            + 1e-3
+            * ranges
+            * np.random.randn(
+                ndim,
+            )
+            for i in range(
+                nwalkers,
+            )
+        ]
 
-        pos = [ini + 1e-4 * var * np.random.randn(ndim) for i in range(nwalkers)]
+        if filepath is not None:
+            # We'll track how the average autocorrelation time estimate changes
+            index = 0
+            autocorr = np.empty(steps)
+            # This will be useful to testing convergence
+            old_tau = np.inf
+
+            if continue_run is False:
+                # Clear file before starting a new one
+                try:
+                    os.remove(filepath)
+                except FileNotFoundError:
+                    pass
+                backend = emcee.backends.HDFBackend(filepath)
+                backend.reset(nwalkers, ndim)
+            else:
+                backend = emcee.backends.HDFBackend(filepath)
+                steps -= backend.iteration
 
         if use_pool:
             with Pool() as pool:
+                # #### CALL MCMC ROUTINE
                 sampler = emcee.EnsembleSampler(
-                    nwalkers, ndim, func, args=(x, y, bounds, gaussp), pool=pool
+                    nwalkers,
+                    ndim,
+                    func,
+                    args=(x, y, bounds, gaussp),
+                    backend=backend,
+                    pool=pool,
                 )
-                sampler.run_mcmc(pos, steps)
+                # Now we'll sample for up to max_n steps
+                for sample in sampler.sample(
+                    pos,
+                    iterations=steps,
+                    progress=show_progress,
+                ):
+                    # Only check convergence every 100 steps
+                    if sampler.iteration % 100:
+                        continue
+
+                    # Compute the autocorrelation time so far
+                    # Using tol=0 means that we'll always get an estimate even
+                    # if it isn't trustworthy
+                    tau = sampler.get_autocorr_time(tol=0)
+                    autocorr[index] = np.mean(tau)
+                    index += 1
+
+                    # Check convergence
+                    converged = np.all(tau * 100 < sampler.iteration)
+                    converged &= np.all(np.abs(old_tau - tau) / tau < 0.01)
+                    if converged:
+                        break
+                    old_tau = tau
         else:
             sampler = emcee.EnsembleSampler(
-                nwalkers, ndim, func, args=(x, y, bounds, gaussp)
+                nwalkers,
+                ndim,
+                func,
+                args=(x, y, bounds, gaussp),
+                backend=backend,
             )
-            sampler.run_mcmc(pos, steps)
+            # Now we'll sample for up to max_n steps
+            for sample in sampler.sample(
+                pos,
+                iterations=steps,
+                progress=show_progress,
+            ):
+                # Only check convergence every 100 steps
+                if sampler.iteration % 100:
+                    continue
+
+                # Compute the autocorrelation time so far
+                # Using tol=0 means that we'll always get an estimate even
+                # if it isn't trustworthy
+                tau = sampler.get_autocorr_time(tol=0)
+                autocorr[index] = np.mean(tau)
+                index += 1
+
+                # Check convergence
+                converged = np.all(tau * 100 < sampler.iteration)
+                converged &= np.all(np.abs(old_tau - tau) / tau < 0.01)
+                if converged:
+                    break
+                old_tau = tau
 
-        return sampler.chain
+        return
 
     if y is None:
         ri = x
         if ini is None:
             ini, var = maximum_likelihood(x=x, model=model)
     else:
         if x0 is None or y0 is None:
@@ -3496,29 +3777,45 @@
     if use_pool:
         with Pool() as pool:
             sampler = emcee.EnsembleSampler(
                 nwalkers, ndim, func, args=(ri, ini, bounds), pool=pool
             )
             sampler.run_mcmc(pos, steps)
     else:
-        sampler = emcee.EnsembleSampler(nwalkers, ndim, func, args=(ri, ini, bounds))
+        sampler = emcee.EnsembleSampler(
+            nwalkers,
+            ndim,
+            func,
+            args=(
+                ri,
+                ini,
+                bounds,
+            ),
+        )
         sampler.run_mcmc(pos, steps)
 
     chain = sampler.chain
 
     return chain
 
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "Ellipsoidal fitting"
 # ---------------------------------------------------------------------------
 
 
-def ellipse_likelihood(x=None, y=None, model="sersic", x0=None, y0=None, hybrid=True):
+def ellipse_likelihood(
+    x=None,
+    y=None,
+    model="sersic",
+    x0=None,
+    y0=None,
+    hybrid=True,
+):
     """
     Calls a maximum likelihood fit of the surface density paramters of
     the joint distribution of galactic object plus Milky Way stars.
 
     Parameters
     ----------
     x : array_like, optional
@@ -3611,15 +3908,22 @@
 
 # %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 # ---------------------------------------------------------------------------
 "Mass profile fitting"
 # ---------------------------------------------------------------------------
 
 
-def mass_likelihood(x=None, y=None, model="gplummer", x0=None, y0=None, shells=True):
+def mass_likelihood(
+    x=None,
+    y=None,
+    model="gplummer",
+    x0=None,
+    y0=None,
+    shells=True,
+):
     """
     Calls a maximum likelihood fit of the mass profile paramters of
     a radial distribution.
 
     Parameters
     ----------
     x : array_like, optional
@@ -3754,15 +4058,16 @@
 
     if model == "gplummer":
         mle_model = differential_evolution(
             lambda c: likelihood_gplummer_dens(c, ri, shells=shells), bounds
         )
         results = mle_model.x
         hfun = ndt.Hessian(
-            lambda c: likelihood_gplummer_dens(c, ri, shells=shells), full_output=True
+            lambda c: likelihood_gplummer_dens(c, ri, shells=shells),
+            full_output=True,
         )
     elif model == "kazantzidis":
         mle_model = differential_evolution(
             lambda c: likelihood_kazantzidis_dens(c, ri, shells=shells), bounds
         )
         results = mle_model.x
         hfun = ndt.Hessian(
@@ -3771,23 +4076,25 @@
         )
     elif model == "dm":
         mle_model = differential_evolution(
             lambda c: likelihood_dm_dens(c, ri, shells=shells), bounds
         )
         results = mle_model.x
         hfun = ndt.Hessian(
-            lambda c: likelihood_dm_dens(c, ri, shells=shells), full_output=True
+            lambda c: likelihood_dm_dens(c, ri, shells=shells),
+            full_output=True,
         )
     elif model == "einasto":
         mle_model = differential_evolution(
             lambda c: likelihood_einasto_dens(c, ri, shells=shells), bounds
         )
         results = mle_model.x
         hfun = ndt.Hessian(
-            lambda c: likelihood_einasto_dens(c, ri, shells=shells), full_output=True
+            lambda c: likelihood_einasto_dens(c, ri, shells=shells),
+            full_output=True,
         )
 
     hessian_ndt, info = hfun(results)
 
     var = np.sqrt(np.diag(np.linalg.inv(hessian_ndt)))
 
     return results, var
@@ -3963,36 +4270,39 @@
             results = mle_model.x
             hfun = ndt.Hessian(
                 lambda c: likelihood_gplummer_dens(c, r, shells=shells),
                 full_output=True,
             )
         elif model == "kazantzidis":
             mle_model = differential_evolution(
-                lambda c: likelihood_kazantzidis_dens(c, r, shells=shells), bounds
+                lambda c: likelihood_kazantzidis_dens(c, r, shells=shells),
+                bounds,
             )
             results = mle_model.x
             hfun = ndt.Hessian(
                 lambda c: likelihood_kazantzidis_dens(c, r, shells=shells),
                 full_output=True,
             )
         elif model == "dm":
             mle_model = differential_evolution(
                 lambda c: likelihood_dm_dens(c, r, shells=shells), bounds
             )
             results = mle_model.x
             hfun = ndt.Hessian(
-                lambda c: likelihood_dm_dens(c, r, shells=shells), full_output=True
+                lambda c: likelihood_dm_dens(c, r, shells=shells),
+                full_output=True,
             )
         elif model == "einasto":
             mle_model = differential_evolution(
                 lambda c: likelihood_einasto_dens(c, r, shells=shells), bounds
             )
             results = mle_model.x
             hfun = ndt.Hessian(
-                lambda c: likelihood_einasto_dens(c, r, shells=shells), full_output=True
+                lambda c: likelihood_einasto_dens(c, r, shells=shells),
+                full_output=True,
             )
 
         hessian_ndt, info = hfun(results)
         for i in range(len(values) - 1, -1, -1):
             if np.logical_not(np.isnan(values[i])):
                 hessian_ndt = np.delete(hessian_ndt, i, axis=1)
                 hessian_ndt = np.delete(hessian_ndt, i, axis=0)
@@ -4065,29 +4375,53 @@
                     args=(r, bounds, gaussp, shells),
                     pool=pool,
                 )
                 sampler.run_mcmc(pos, steps)
     else:
         if model == "gplummer":
             sampler = emcee.EnsembleSampler(
-                nwalkers, ndim, lnprob_gp_dens, args=(r, bounds, gaussp, shells)
+                nwalkers,
+                ndim,
+                lnprob_gp_dens,
+                args=(
+                    r,
+                    bounds,
+                    gaussp,
+                    shells,
+                ),
             )
             sampler.run_mcmc(pos, steps)
         elif model == "kazantzidis":
             sampler = emcee.EnsembleSampler(
                 nwalkers, ndim, lnprob_k_dens, args=(r, bounds, gaussp, shells)
             )
             sampler.run_mcmc(pos, steps)
         elif model == "dm":
             sampler = emcee.EnsembleSampler(
-                nwalkers, ndim, lnprob_dm_dens, args=(r, bounds, gaussp, shells)
+                nwalkers,
+                ndim,
+                lnprob_dm_dens,
+                args=(
+                    r,
+                    bounds,
+                    gaussp,
+                    shells,
+                ),
             )
             sampler.run_mcmc(pos, steps)
         elif model == "einasto":
             sampler = emcee.EnsembleSampler(
-                nwalkers, ndim, lnprob_einasto_dens, args=(r, bounds, gaussp, shells)
+                nwalkers,
+                ndim,
+                lnprob_einasto_dens,
+                args=(
+                    r,
+                    bounds,
+                    gaussp,
+                    shells,
+                ),
             )
             sampler.run_mcmc(pos, steps)
 
     chain = sampler.chain
 
     return chain
```

### Comparing `balrogo-1.7.8/pyproject.toml` & `balrogo-1.7.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balrogo"
-version = "1.7.8"
+version = "1.7.9"
 description = "Bayesian Astrometric Likelihood Recovery of Galactic Objects"
 authors = ["Eduardo Vitral <vitral@iap.fr>", "Alexandre Macedo <arj.macedo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/eduardo-vitral/balrogo"
 
 [tool.poetry.dependencies]
```

### Comparing `balrogo-1.7.8/PKG-INFO` & `balrogo-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balrogo
-Version: 1.7.8
+Version: 1.7.9
 Summary: Bayesian Astrometric Likelihood Recovery of Galactic Objects
 Home-page: https://gitlab.com/eduardo-vitral/balrogo
 License: MIT
 Author: Eduardo Vitral
 Author-email: vitral@iap.fr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

