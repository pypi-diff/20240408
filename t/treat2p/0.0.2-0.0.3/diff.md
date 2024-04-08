# Comparing `tmp/treat2p-0.0.2.tar.gz` & `tmp/treat2p-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat2p-0.0.2.tar", last modified: Wed Mar 20 18:10:26 2024, max compression
+gzip compressed data, was "treat2p-0.0.3.tar", last modified: Mon Apr  8 17:56:35 2024, max compression
```

## Comparing `treat2p-0.0.2.tar` & `treat2p-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 18:10:26.118494 treat2p-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      845 2024-03-20 18:10:26.118494 treat2p-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1280 2024-03-20 18:10:15.000000 treat2p-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 18:10:26.118494 treat2p-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-03-20 18:10:15.000000 treat2p-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 18:10:26.118494 treat2p-0.0.2/treat2p/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16912 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/calculations.py
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     4885 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/normalisation.py
--rw-rw-rw-   0 root         (0) root         (0)    14005 2024-03-20 18:10:15.000000 treat2p-0.0.2/treat2p/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 18:10:26.118494 treat2p-0.0.2/treat2p.egg-info/
--rw-r--r--   0 root         (0) root         (0)      845 2024-03-20 18:10:26.000000 treat2p-0.0.2/treat2p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2024-03-20 18:10:26.000000 treat2p-0.0.2/treat2p.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 18:10:26.000000 treat2p-0.0.2/treat2p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-20 18:10:26.000000 treat2p-0.0.2/treat2p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-20 18:10:26.000000 treat2p-0.0.2/treat2p.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-08 17:56:35.377806 treat2p-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2024-04-08 17:56:25.000000 treat2p-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 17:56:35.377806 treat2p-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-08 17:56:25.000000 treat2p-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/treat2p/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17525 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/calculations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     4905 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/normalisation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13631 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/treat2p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/top_level.txt
```

### Comparing `treat2p-0.0.2/PKG-INFO` & `treat2p-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.2
+Version: 0.0.3
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `treat2p-0.0.2/README.md` & `treat2p-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.2/setup.py` & `treat2p-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.2/treat2p/calculations.py` & `treat2p-0.0.3/treat2p/calculations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from logging import getLogger
-from scipy.signal import savgol_filter, filtfilt
+from scipy.signal import savgol_filter, filtfilt, butter
 from scipy.signal.windows import boxcar
 from .utils import filter_save_kwargs
 
 ### Main functions, used directly in correction
 
 
 @filter_save_kwargs("F")
@@ -12,16 +12,21 @@
     F,
     *,
     window=120,
     slow_trend_percentile=10,
     fps=30,
     step=10,
     filter_savgol=True,
+    filter_lowpass=False,
+    filter_percentiles=True,
     savgol_window_length=50,
     savgol_polyorder=2,
+    lowpass_order=3,
+    lowpass_fcut=0.001,  # in Hz
+    lowpass_method="gust",
 ):
     """
     Calculate a slow trend in a calcium imaging trace and correct for it.
 
     Args:
         F (1D array): The F trace to correct.
         window (int): Time window in seconds to use for percentile
@@ -37,34 +42,50 @@
             filter. Defaults to 50.
         savgol_polyorder (int): Polynomial order of Savitzky-Golay
             filter. Defaults to 2.
 
     Returns:
         numpy.array: The corrected trace with the slow trend removed.
     """
-    frames_half_window = int((fps * window) / 2)
-    slow_trend = []
-    for i in range(0, len(F), 10):
-        start = i - frames_half_window
-        start = start if start >= 0 else 0
-        stop = i + frames_half_window
-        stop = stop if stop <= len(F) else len(F)
 
-        value = np.percentile(F[start:stop], slow_trend_percentile)
-        slow_trend.extend([value for _ in range(step)])
+    slow_trend = F.copy()
+
+    if filter_percentiles:
+        _slow_trend = []
+        frames_half_window = int((fps * window) / 2)
+        for i in range(0, len(F), 10):
+            start = i - frames_half_window
+            start = start if start >= 0 else 0
+            stop = i + frames_half_window
+            stop = stop if stop <= len(F) else len(F)
+
+            value = np.percentile(F[start:stop], slow_trend_percentile)
+            _slow_trend.extend([value for _ in range(step)])
+        slow_trend = np.asarray(_slow_trend)
 
     if filter_savgol:
-        slow_trend = savgol_filter(
-            slow_trend, window_length=savgol_window_length, polyorder=savgol_polyorder
+        slow_trend = savgol_filter(slow_trend, window_length=savgol_window_length, polyorder=savgol_polyorder)
+
+    if filter_lowpass:
+        b, a = butter(lowpass_order, lowpass_fcut, btype="low", fs=fps, output="ba", analog=False)
+        slow_trend = filtfilt(
+            b,
+            a,
+            slow_trend,
+            padlen=None,
+            padtype="odd",
+            method=lowpass_method,
+            irlen=None,
+            axis=0,
         )
 
-    return np.array(slow_trend)[0 : len(F)]
+    return np.asarray(slow_trend)[0 : len(F)]
 
 
-@filter_save_kwargs("F_Cell","F_Neu")
+@filter_save_kwargs("F_Cell", "F_Neu")
 def neuropil_factor_ARDSIP(
     F_Cell,
     F_Neu,
     *,
     max_iterations=10,
     long_window_length=30,
     short_window_length=3,
@@ -82,21 +103,24 @@
         F_Cell (numpy.ndarray): The array of fluorescence intensity for the cell.
         F_Neu (numpy.ndarray): The array of fluorescence intensity for the neuropil.
         max_iterations (int, optional): The maximum number of iterations to perform. Default is 10.
         long_window_length (int, optional): The length of the long sliding window. Default is 30.
         short_window_length (int, optional): The length of the short sliding window. Default is 3.
         baseline_percentile (float, optional): The percentile of the baseline fluorescence. Default is 10.
         convergence_criteria (float, optional): The criteria for convergence. Default is 0.025.
-        autoregressed_activity_threshold (float, optional): The threshold for determining if there is activity in the cell based on autoregression. Default is 0.5.
+        autoregressed_activity_threshold (float, optional): The threshold for determining if there is activity in the
+            cell based on autoregression. Default is 0.5.
         initial_neuropil_factor (float, optional): The initial neuropil factor. Default is 0.5.
-        downsampling (float, optional): How much downsampled is the original aray when computing baseline. 1 means no downsampling, 4 means 1 smple out of 4 is used.
+        downsampling (float, optional): How much downsampled is the original aray when computing baseline.
+            1 means no downsampling, 4 means 1 smple out of 4 is used.
             Higher values speedup the computation at fidelity cost. Default is 4.
         zscoring_mid_percentile (float, optional): Upper percentile used for zscoring. Default is 16.
         zscoring_low_percentile (float, optional): Lower percentile used for zscoring. Default is 2.3.
-            Both of zscoring_mid_percentile and zscoring_low_percentile refer to z_score_from_percentile arguments. See that function for more details.
+            Both of zscoring_mid_percentile and zscoring_low_percentile refer to z_score_from_percentile arguments.
+            See that function for more details.
 
     Returns:
         dict: A dictionary containing :
             the calculated neuropil factor (float),
             the final neuropil factor after bounding to [0.1, 0.7] (float),
             a list of the neuropil factor across all iterations (list[float])
             a boolean indicating whether the function converged (bool).
@@ -112,25 +136,25 @@
     iteration_results = [initial_neuropil_factor]
     converged = False
 
     iteration = 0
     activity_periods_mask = None
 
     for iteration in range(max_iterations):
-        local_log.debug(
-            f"Starting new iteration with neuropil_factor : {neuropil_factor:.2f} "
-        )
+        local_log.debug(f"Starting new iteration with neuropil_factor : {neuropil_factor:.2f} ")
         F_Corrected = F_Cell - (neuropil_factor * F_Neu)
 
-        if iteration == 0: # activity_periods_mask is None at that stage, and for further iterations, it has an array shape like F_Corrected
+        if iteration == 0:  # activity_periods_mask is None at that stage, and for further iterations,
+            # it has an array shape like F_Corrected
             activity_periods_mask = np.zeros_like(F_Corrected, dtype=bool)
 
         F_Corrected_activity_removed = F_Corrected.copy()
         F_Corrected_activity_removed[activity_periods_mask] = np.nan
-        # suppress periods of ROI activity , in the first iteration include all data ( activity_periods_mask is redefined later)
+        # suppress periods of ROI activity , in the first iteration include all data
+        # ( activity_periods_mask is redefined later)
 
         low_percentiles = sliding_window_percentile(
             F_Corrected_activity_removed,
             percentile=baseline_percentile,
             window_length=long_window_length,
             window_sample_displacement=downsampling,
             window_internal_downsampling=downsampling + 1,
@@ -144,34 +168,30 @@
         )
 
         F_Autoregressed = autoregress(F_Corrected_normalized)
 
         bool_no_activity = (F_Autoregressed < autoregressed_activity_threshold) & (
             F_Autoregressed > -autoregressed_activity_threshold
         )  # periods without activity
-        bool_state_nochange = ~np.abs(
-            np.diff(bool_no_activity.astype(int), prepend=False)
-        ).astype(
+        bool_state_nochange = ~np.abs(np.diff(bool_no_activity.astype(int), prepend=False)).astype(
             bool
         )  # periods of changes between activity / non activity
         bool_stable_no_activity = (
             bool_no_activity & bool_state_nochange
         )  # stable periods without activity nor instantaneous changes
 
         if np.sum(bool_stable_no_activity) < 0.1 * len(bool_stable_no_activity):
             local_log.warning(
                 "Non activity periods cannot realistically consist of less than 10% of all time. Skipping."
             )
             iteration_results.append(np.nan)
             neuropil_factor = neuropil_factor + convergence_criteria
             continue
 
-        activity_periods_mask = (
-            ~bool_stable_no_activity
-        )  # activity periods are the inverse of no  activity periods
+        activity_periods_mask = ~bool_stable_no_activity  # activity periods are the inverse of no  activity periods
 
         # loop's final estimation of neuropil_factor through
 
         F_Cell_copy = F_Cell.copy()
         F_Cell_copy[activity_periods_mask] = np.nan
 
         F_Neu_copy = F_Neu.copy()
@@ -186,41 +206,40 @@
 
         F_Cell_windows = F_Cell_copy[short_window_indices]
         F_Neu_windows = F_Neu_copy[short_window_indices]
 
         new_neuropil_factor = []
         for cell_chunk, neu_chunk in zip(F_Cell_windows, F_Neu_windows):
             non_nan_vec = ~np.isnan(cell_chunk)
-            if (
-                sum(non_nan_vec) > 5
-            ):  # at least 5 non nan data points needed for regression
-                new_neuropil_factor.append(
-                    np.polyfit(neu_chunk[non_nan_vec], cell_chunk[non_nan_vec], 1)[0]
-                )
+            if sum(non_nan_vec) > 5:  # at least 5 non nan data points needed for regression
+                new_neuropil_factor.append(np.polyfit(neu_chunk[non_nan_vec], cell_chunk[non_nan_vec], 1)[0])
             else:
                 new_neuropil_factor.append(np.nan)
         new_neuropil_factor = np.array(new_neuropil_factor)
         local_log.debug(
-            f"Finished calculating chunks regressions with {len(new_neuropil_factor[~np.isnan(new_neuropil_factor)])} valid chunks"
+            "Finished calculating chunks regressions with "
+            f"{len(new_neuropil_factor[~np.isnan(new_neuropil_factor)])} valid chunks"
         )
         new_neuropil_factor_mean = np.nanmean(new_neuropil_factor)
 
         divergence = abs(neuropil_factor - new_neuropil_factor_mean)
         neuropil_factor = new_neuropil_factor_mean
-        iteration_results.append(neuropil_factor)
+        iteration_results.append(neuropil_factor)  # type: ignore
         if divergence < convergence_criteria:
             local_log.info(
-                f"Found convergence in {iteration+1} iterations. Ending with neuropil_factor value : {neuropil_factor:.2f} (last run divergence : {divergence:.3f})."
+                f"Found convergence in {iteration + 1} iterations. Ending with neuropil_factor value : "
+                f"{neuropil_factor:.2f} (last run divergence : {divergence:.3f})."
             )
             converged = True
             break
 
     if converged == False:
         local_log.info(
-            f"Found no convergence in {iteration+1} iterations. Ending with neuropil_factor value : {neuropil_factor:.2f}."
+            f"Found no convergence in {iteration + 1} iterations. "
+            f"Ending with neuropil_factor value : {neuropil_factor:.2f}."
         )
 
     if neuropil_factor < 0.1:
         constrained_neuropil_factor = 0.1
     elif neuropil_factor > 0.7:
         constrained_neuropil_factor = 0.7
     else:
@@ -236,100 +255,103 @@
 
 ### Helper functions made to make life easy / enhance speed of above calculations
 
 
 def rolling_indices(
     array,
     *,
-    window_displacement=None, # how much each window moves from the next one, in seconds units. Results in general downsampling from initial array length after collapsing windows to one number by merging operations such as averaging etc.
-    window_length=30, # in seconds units
-    samples_per_sec=30, 
+    window_displacement=None,  # how much each window moves from the next one, in seconds units.
+    # Results in general downsampling from initial array length
+    # after collapsing windows to one number by merging operations such as averaging etc.
+    window_length=30,  # in seconds units
+    samples_per_sec=30,
     window_internal_downsampling=4,  # if more than one, downsample INSIDE a window. In index units
-
-    window_sample_length=None,  # same as window_length but in sample index units instead of seconds. will skip window_length value if used.
-    window_sample_displacement=4,  # same as window_displacement but in sample index units. will skip window_displacement value is used
+    window_sample_length=None,  # same as window_length but in sample index units instead of seconds.
+    # will skip window_length value if used.
+    window_sample_displacement=4,  # same as window_displacement but in sample index units.
+    # will skip window_displacement value is used
 ):
     """
     Specifies the indices in an input 'array' over which rolling windows are defined.
-    The indices can be used later to easily and efficiently create such windows with vanilla numpy slicing (leveraging SIMD).
+    The indices can be used later to easily and efficiently create such windows with vanilla numpy slicing
+    (leveraging SIMD).
     The resulting windows can have optional downsampling and are defined by their length and displacement.
 
     Args:
         array (numpy.ndarray): Input array over which rolling windows are to be calculated.
         window_displacement (int, optional): Defines how much each window moves from the next one. Defaults to None.
         window_length (int, optional): Defines the desired window length in seconds. Defaults to 30.
         samples_per_sec (int, optional): Defines the number of samples per second in the array. Defaults to 30.
         window_internal_downsampling (int, optional): If more than one, downsample within window. Defaults to 4.
-        window_sample_length (int, optional): Same as window_length but in sample indices instead of seconds. Will skip window_length value if used. Defaults to None.
-        window_sample_displacement (int, optional): Same as window_displacement but in seconds instead of sample points. Will skip window_displacement value if used. Defaults to 4.
+        window_sample_length (int, optional): Same as window_length but in sample indices instead of seconds.
+            Will skip window_length value if used. Defaults to None.
+        window_sample_displacement (int, optional): Same as window_displacement but in seconds instead of sample points.
+            Will skip window_displacement value if used. Defaults to 4.
 
     Returns:
         tuple: Tuple containing numpy.ndarray of rolling window indices and numpy.ndarray
                of indices central to each window.
     """
 
     if window_sample_length is None:
         window_sample_length = round(window_length * samples_per_sec)
     else:
         window_sample_length = round(window_sample_length)
     if window_sample_displacement is None:
-        if window_displacement is None :
+        if window_displacement is None:
             raise ValueError("window_displacement cannot be None if window_sample_displacement is None.")
         window_sample_displacement = round(window_displacement * samples_per_sec)
     else:
         window_sample_displacement = round(window_sample_displacement)
     half_window_length = round(window_sample_length / 2)
     windows_indices = []
     indices = []
     for i in range(0, len(array) - window_sample_length, window_sample_displacement):
-        window = np.array(
-            range(i, i + window_sample_length, window_internal_downsampling), dtype=int
-        )
+        window = np.array(range(i, i + window_sample_length, window_internal_downsampling), dtype=int)
         windows_indices.append(window)
         indices.append(i + half_window_length)
     return np.array(windows_indices), np.array(indices)
 
 
 def sliding_window_percentile(input_array, percentile=10, **kwargs):
-    """This function applies sliding window computation on an input data array, computing a user-specified percentile within each window.
-    It uses the 'rolling_indices' to generate windows in the input data. For each generated window, it computes the specified percentile and assigns this value to the representative sample for the window.
+    """This function applies sliding window computation on an input data array, computing a user-specified percentile
+    within each window.
+    It uses the 'rolling_indices' to generate windows in the input data. For each generated window,
+    it computes the specified percentile and assigns this value to the representative sample for the window.
     For samples not directly represented by a window, the function interpolates the percentile values.
 
     Args:
         input_array (numpy.ndarray): The array on which sliding window computation is to be performed.
         percentile (int, optional): The percentile to be computed within each window. Defaults to 10.
         **kwargs: Additional keyword arguments to passed to the 'rolling_indices' function.
 
     Returns:
-        numpy.ndarray : Array filled with the computed percentile values for each window, with the same shape as 'input_array'.
+        numpy.ndarray : Array filled with the computed percentile values for each window,
+            with the same shape as 'input_array'.
             For positions between windows, the percentile values are interpolated."""
 
     long_windows_indices, downsampled_indices = rolling_indices(input_array, **kwargs)
 
     input_array_long_windows = input_array[long_windows_indices]
 
     low_percentiles = np.nanpercentile(input_array_long_windows, percentile, axis=1)
 
     x_indices = np.arange(len(input_array))
-    interped_indices = np.setdiff1d(
-        x_indices[downsampled_indices[0] : downsampled_indices[-1]], downsampled_indices
-    )
+    interped_indices = np.setdiff1d(x_indices[downsampled_indices[0] : downsampled_indices[-1]], downsampled_indices)
     interped_values = np.interp(interped_indices, downsampled_indices, low_percentiles)
 
     interped_low_percentiles = np.full_like(input_array, np.nan, dtype=float)
     interped_low_percentiles[downsampled_indices] = low_percentiles
     interped_low_percentiles[interped_indices] = interped_values
     return interped_low_percentiles
 
 
 def autoregress(input_array, lag=1, boxcar_value=3):
     prefilter = boxcar_filtering(input_array, boxcar_value=boxcar_value) / 2
-    postfilter = (
-        boxcar_filtering(np.roll(input_array, -lag), boxcar_value=boxcar_value) / 2
-    )
+    postfilter = boxcar_filtering(np.roll(input_array, -lag), boxcar_value=boxcar_value) / 2
     autoregressed = prefilter * postfilter
     return autoregressed
 
 
 def boxcar_filtering(x, boxcar_value=3):
     """Applies boxcar filtering on the input data.
 
@@ -342,33 +364,32 @@
     """
     filter_window = boxcar(boxcar_value)
     return filtfilt(filter_window / sum(filter_window), [1.0], x)
 
 
 def z_score_percentile(input_array, mid_percentile=16, low_percentile=2.3):
     """
-    This function performs autoregression on a given data array by applying boxcar filtering first to the array and then to a copy of the array rolled by a certain lag. The results of these filterings are then elementwise multiplied.
+    This function performs autoregression on a given data array by applying boxcar filtering first to the array and
+    then to a copy of the array rolled by a certain lag. The results of these filterings
+    are then multiplied elementwise.
     Need to explain the choice of values for this weird zscoring. Why not using standard zscoring ?
 
     Args:
         input_array (numpy.ndarray): The array on which to perform autoregression.
-        lag (int, optional): The size of the shift applied to the input array for the 'rolled' boxcar filtering. Default is 1.
+        lag (int, optional): The size of the shift applied to the input array for the 'rolled' boxcar filtering.
+        Default is 1.
         boxcar_value (int, optional): The width of the boxcar window to be applied. Default is 3.
 
     Returns:
         numpy.ndarray: The array of the resulting autoregressed values. It has the same shape as the input array.
     """
     local_log = getLogger("zscore_percentile")
     low_p_value = np.nanpercentile(input_array, low_percentile)
     mid_p_value = np.nanpercentile(input_array, mid_percentile)
     sigma = mid_p_value - low_p_value
     mean = low_p_value + (
         2 * sigma
     )  # why this weird thing and not simply np.nanpercentile(input_array, 50) as a median ?
-    local_log.debug(
-        f"Percentile 'mean' is : {mean}, real median is : {np.nanpercentile(input_array, 50)}"
-    )
-    local_log.debug(
-        f"Percentile based 'sigma' is : {sigma}, real std is : {np.nanstd(input_array)}"
-    )
+    local_log.debug(f"Percentile 'mean' is : {mean}, real median is : {np.nanpercentile(input_array, 50)}")
+    local_log.debug(f"Percentile based 'sigma' is : {sigma}, real std is : {np.nanstd(input_array)}")
 
     return (input_array - mean) / sigma
```

### Comparing `treat2p-0.0.2/treat2p/core.py` & `treat2p-0.0.3/treat2p/core.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.2/treat2p/corrections.py` & `treat2p-0.0.3/treat2p/corrections.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.2/treat2p/normalisation.py` & `treat2p-0.0.3/treat2p/normalisation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,99 @@
-
 from scipy.stats import zscore
-from . utils import filter_save_kwargs
+from .utils import filter_save_kwargs
 import numpy as np
 
 zscore = filter_save_kwargs("a")(zscore)
 
+
 @filter_save_kwargs("array")
-def delta_over_F(array, F0_index = 0, F0_span = 1):
-    """Performs deltaF over F0 ( with eq : DF0 = F - F0 / F0 )    
-    """
-    
+def delta_over_F(array, F0_index=0, F0_span=1):
+    """Performs deltaF over F0 ( with eq : DF0 = F - F0 / F0 )"""
+
     if array.min() <= 0:
         array = non_zero_raw_fluorescence(array.copy())
-    
-    F0_frame = array[F0_index:F0_index+F0_span].mean(axis = 0)
-    
-    F0_frames = np.repeat( F0_frame[np.newaxis], array.shape[0], axis = 0)
-    return (array - F0_frames) / F0_frames 
+
+    F0_frame = array[F0_index : F0_index + F0_span].mean(axis=0)
+
+    F0_frames = np.repeat(F0_frame[np.newaxis], array.shape[0], axis=0)
+    return (array - F0_frames) / F0_frames
+
 
 def non_zero_raw_fluorescence(array):
     """This simply ensures that raw fluorescence is strictly positive to avoid 0 division errors."""
-    return (array - array.min() ) + 1
+    return (array - array.min()) + 1
+
 
-def normalize(values, outmin = 0, outmax = 1, min_val = None, max_val = None) :
-    """This function normalizes the input values between a specified range [outmin, outmax]. 
+def normalize(values, outmin=0, outmax=1, min_val=None, max_val=None):
+    """This function normalizes the input values between a specified range [outmin, outmax].
 
     The minimum value of the provided values array will be snapped to outmin and the maximum value, to outmax,
     in the output array.
-    However, in case you want to account for extra cases of unelikely data 
+    However, in case you want to account for extra cases of unelikely data
     (ex : minimum of unrealistically low value compared to all the resto of calues)
-    you can supply min_val and max_val directly to the function, for example by externally calculating the 99.9 percentile 
-    of the values, thus not taking into account the uncannyly large single value. 
+    you can supply min_val and max_val directly to the function, for example by externally calculating the 99.9
+    percentile of the values, thus not taking into account the uncannyly large single value.
     If min_val and max_val are set to None, they are automatically detected with min() and max() from values.
     If they are supplied, the output values can then be out of the range defined by min and max.
 
     Args:
         values (array_like): The input values to be normalized.
         outmin (float, optional): The lower boundary of the output range. Defaults to 0.
         outmax (float, optional): The upper boundary of the output range. Defaults to 1.
-        min_val (float, optional): The curent values lower bound that will be snapped to outmin. If none, it is automatically calculated from values.min() 
-            Defaults to None.
-        max_val (float, optional): The curent values upper bound that will be snapped to outmax. If none, it is automatically calculated from values.max() 
+        min_val (float, optional): The curent values lower bound that will be snapped to outmin.
+            If none, it is automatically calculated from values.min(). Defaults to None.
+        max_val (float, optional): The curent values upper bound that will be snapped to outmax.
+            If none, it is automatically calculated from values.max(). Defaults to None.
 
     Raises:
         ValueError: If the provided min is not strictly inferior to max.
 
     Returns:
         norm (array_like): The normalized values.
     """
-    if outmin >= outmax :
+    if outmin >= outmax:
         raise ValueError("min must be strictly inferior to max")
-    
-    min_val =  values.min() if min_val is None else min_val
-    max_val =  values.max() if max_val is None else max_val
+
+    min_val = values.min() if min_val is None else min_val
+    max_val = values.max() if max_val is None else max_val
 
     ampl = max_val - min_val
-    norm = (values-min_val)/ampl #normalisation between 0 and 1 with eq : Fnorm = F - Fmin / Fmax - Fmin
+    norm = (values - min_val) / ampl  # normalisation between 0 and 1 with eq : Fnorm = F - Fmin / Fmax - Fmin
     target_ampl = outmax - outmin
-    norm = (norm * target_ampl) + outmin #normalization between arbitraty values
+    norm = (norm * target_ampl) + outmin  # normalization between arbitraty values
     return norm
 
-def center_normalize(array, outmin = 0, outmax = 1, percentile = None):
-    """Normalizes and centers an input array around its mean. 
+
+def center_normalize(array, outmin=0, outmax=1, percentile=None):
+    """Normalizes and centers an input array around its mean.
     The values are then scaled so that the mean will be at equidistance of outmin and outmax in the output array.
     The relationship between outmin and outmax and the original data values are :
-    outmin, outmax values are snapped from - , + (respectively) of max( abolute (min) vs abolute(max)) from the values of the data after mean substraction (at 0)
+    outmin, outmax values are snapped from - , + (respectively) of max( abolute (min) vs abolute(max))
+    from the values of the data after mean substraction (at 0)
 
-    It accepts an input array, subtracts its mean (thus centering it around zero), 
-    and then normalizes it to be within a specified range (outmin and outmax). 
+    It accepts an input array, subtracts its mean (thus centering it around zero),
+    and then normalizes it to be within a specified range (outmin and outmax).
     By default, the range is between 0 and 1.
 
     Args:
         array (numpy.ndarray): Input array to be centered and normalized.
         outmin (float, optional): Minimum value for the output normalized array. Defaults to 0.
         outmax (float, optional): Maximum value for the output normalized array. Defaults to 1.
-        percentile (float, optionnal) : The maximum percentile that corresponds to the un-normalized value that will snap to the output bounds (symetrically around the mean)
-            If set to None (default) the current value snapped to the bounds is the maximum absolute value between array.min() and array.max() 
-            (e.g. normalization via scaling but not translation, to stay centered around the mean at 0, that occurs at the 2n line in the code)
+        percentile (float, optionnal) : The maximum percentile that corresponds to the un-normalized value that
+            will snap to the output bounds (symetrically around the mean)
+            If set to None (default) the current value snapped to the bounds is the maximum absolute value
+            between array.min() and array.max() (e.g. normalization via scaling but not translation,
+            to stay centered around the mean at 0, that occurs at the 2n line in the code)
 
     Returns:
         numpy.ndarray: Normalized and centered array with values ranging between specified minimum and maximum values.
     """
 
     mean = array.mean()
     centered_array = array - mean
-    if percentile :
-        outermost_bound = max( abs(np.percentile( centered_array, 100-percentile )), abs(np.percentile( centered_array, percentile)))
-    else :
-        outermost_bound = max( abs(centered_array.min()), abs(centered_array.max()))
-    return normalize(centered_array, min_val = -outermost_bound, max_val = outermost_bound, outmin = outmin, outmax = outmax)
+    if percentile:
+        outermost_bound = max(
+            abs(np.percentile(centered_array, 100 - percentile)), abs(np.percentile(centered_array, percentile))
+        )
+    else:
+        outermost_bound = max(abs(centered_array.min()), abs(centered_array.max()))
+    return normalize(centered_array, min_val=-outermost_bound, max_val=outermost_bound, outmin=outmin, outmax=outmax)
```

### Comparing `treat2p-0.0.2/treat2p/utils.py` & `treat2p-0.0.3/treat2p/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from functools import wraps
 from collections import OrderedDict
 import inspect
+import contextlib
+import joblib
 
 
 def filter_save_kwargs(*excluded_save_kwargs, register=True):
-    """Create decorator that wraps function, track its keyword arguments and output them along with the normal output of the function
+    """Create decorator that wraps function, track its keyword arguments and output them along with the normal output
+    of the function
     It also filters out any keyword argument that is not accepted by the input function.
 
     It can handle correctly (i.e. same behavior as raw python) :
       - functions with signatures containing **kwargs
       - positionnal/kwargs passed as keyword arguments
 
     For arguments to be saved in the output dictionnary :
@@ -18,15 +21,16 @@
         text / numbers and that we want to register their values.
         If not, you can exclude them manually using excluded_save_kwargs.)
         To ensure that they are keyword only, you may place them after an asterisk separated by
         commas in your argument list (eg. arg1, arg2, *, kwarg1, kwarg2)
       - they must be present in the function signature (of course).
         Thus if you send arguments that are not in function signature and yet captured with a **kwargs,
         they can still be passed to child functions but will not be registered here.
-        This is intended to be sure to have the actual values used by the proper functions saved as parameters that were used.
+        This is intended to be sure to have the actual values used by the proper functions saved as parameters
+        that were used.
     That's all !
 
     Args:
         excluded_save_kwargs : any number of string representing wich argument to not include in the
         kwargs values saved and returned as second object of the wrapped function
 
     Returns:
@@ -45,85 +49,76 @@
         has_a_capture_all = False
 
         # iterate through function signature parameters
         for name, param in sig.parameters.items():
             # Check if parameters in signature are keyword or positionnal, with or without default value
             if param.default == inspect.Parameter.empty:
                 if param.kind == param.KEYWORD_ONLY:
-                    ori_required_kwargs.append(
-                        name
-                    )  # The parameter is a required keyword only argument
+                    ori_required_kwargs.append(name)  # The parameter is a required keyword only argument
                 elif param.kind == param.VAR_KEYWORD:
                     has_a_capture_all = True
                 else:
-                    ori_args.append(
-                        name
-                    )  # The parameter is a required positionnal argument
+                    ori_args.append(name)  # The parameter is a required positionnal argument
             else:
-                ori_kwargs[
-                    name
-                ] = param.default  # The parameter is keyword with a default value
+                ori_kwargs[name] = param.default  # The parameter is keyword with a default value
 
         # Use wraps to preserve the metadata of the original function
         @wraps(func)
         def wrap(*args, **kwargs):
             # Check for missing keyword arguments
-            missing_kwargs = [
-                name for name in ori_required_kwargs if name not in kwargs.keys()
-            ]
+            missing_kwargs = [name for name in ori_required_kwargs if name not in kwargs.keys()]
             if missing_kwargs:
-                raise ValueError(
-                    f'Missing required keword arguments: {", ".join(missing_kwargs)}'
-                )
+                raise ValueError(f'Missing required keword arguments: {", ".join(missing_kwargs)}')
 
             # Filter kwargs to include original function required only kwargs
             filtered_kwargs = {name: kwargs[name] for name in ori_required_kwargs}
 
             # Update the filtered kwargs with optionnal only kwargs, that are in the function signature and in input
             filtered_kwargs.update(
                 {
                     name: kwargs[name]
                     for name in kwargs
-                    if name in ori_kwargs.keys() and not name in filtered_kwargs.keys()
+                    if name in ori_kwargs.keys() and name not in filtered_kwargs.keys()
                 }
             )
 
             # Create an output dict with default kwargs, overriding default values if present as input.
             saved_kwargs = ori_kwargs.copy()
             saved_kwargs.update(filtered_kwargs)
 
             # Remove excluded kwargs
             for key in excluded_save_kwargs:
                 saved_kwargs.pop(key, None)
 
             # if function has capture all, after we determined the saved_kwargs values
-            # we can run it normally as python's default behaviour already captures the used kwargs in their associated variables.
+            # we can run it normally as python's default behaviour
+            # already captures the used kwargs in their associated variables.
             if has_a_capture_all:
                 if register:
                     ParameterRegistrator.register(saved_kwargs)
                     return func(*args, **kwargs)
                 else:
                     return func(*args, **kwargs), saved_kwargs
 
-            # if positionnal/kw arguments without defaults are passed as keyword arguments, we add them into filtered_kwargs.
+            # if positionnal/kw arguments without defaults are passed as keyword arguments,
+            # we add them into filtered_kwargs.
             # (otherwise they will be skipped and an error will be thrown)
             # note that since this happends after we created the saved_kwargs variable,
             # "recovering" args by name into filtered_kwargs doesn't save them. This is intended as saved_kargs must be
             # positionnal or having defaul values.
             if len(args) < len(ori_args):
                 nb_missing = len(ori_args) - len(args)
-                missing_args_indices = range(
-                    len(ori_args) - nb_missing, len(ori_args), 1
-                )
+                missing_args_indices = range(len(ori_args) - nb_missing, len(ori_args), 1)
                 for index in missing_args_indices:
                     name = ori_args[index]
                     try:
                         filtered_kwargs[name] = kwargs[name]
-                    except:
-                        pass  # we pass to raise the natural error (TypeError: missing X required positional arguments) below.
+                    except Exception as e:
+                        pass
+                        # we pass to raise the natural error (TypeError: missing X required positional arguments) below.
 
             # Return original result and the kwargs used
             if register:
                 ParameterRegistrator.register(saved_kwargs)
                 return func(*args, **filtered_kwargs)
             else:
                 return func(*args, **filtered_kwargs), saved_kwargs
@@ -158,69 +153,58 @@
     has_a_capture_all = False
 
     # iterate through function signature parameters
     for name, param in sig.parameters.items():
         # Check if parameters in signature are keyword or positionnal, with or without default value
         if param.default == inspect.Parameter.empty:
             if param.kind == param.KEYWORD_ONLY:
-                ori_required_kwargs.append(
-                    name
-                )  # The parameter is a required keyword only argument
+                ori_required_kwargs.append(name)  # The parameter is a required keyword only argument
             elif param.kind == param.VAR_KEYWORD:
                 has_a_capture_all = True
             else:
-                ori_args.append(
-                    name
-                )  # The parameter is a required positionnal argument
+                ori_args.append(name)  # The parameter is a required positionnal argument
         else:
-            ori_kwargs[
-                name
-            ] = param.default  # The parameter is keyword with a default value
+            ori_kwargs[name] = param.default  # The parameter is keyword with a default value
 
     @wraps(func)
     def wrap(*args, **kwargs):
         if has_a_capture_all:
             return func(*args, **kwargs)
 
-        missing_kwargs = [
-            name for name in ori_required_kwargs if name not in kwargs.keys()
-        ]
+        missing_kwargs = [name for name in ori_required_kwargs if name not in kwargs.keys()]
         if missing_kwargs:
-            raise ValueError(
-                f'Missing required keword arguments: {", ".join(missing_kwargs)}'
-            )
+            raise ValueError(f'Missing required keword arguments: {", ".join(missing_kwargs)}')
 
         # Filter kwargs to include original function required only kwargs
         filtered_kwargs = {name: kwargs[name] for name in ori_required_kwargs}
 
         # Update the filtered kwargs with optionnal only kwargs, that are in the function signature and in input
         filtered_kwargs.update(
-            {
-                name: kwargs[name]
-                for name in kwargs
-                if name in ori_kwargs.keys() and not name in filtered_kwargs.keys()
-            }
+            {name: kwargs[name] for name in kwargs if name in ori_kwargs.keys() and name not in filtered_kwargs.keys()}
         )
 
-        # if positionnal/kw arguments without defaults are passed as keyword arguments, we add them into filtered_kwargs.
+        # if positionnal/kw arguments without defaults are passed as keyword arguments,
+        #  we add them into filtered_kwargs.
         # (otherwise they will be skipped and an error will be thrown)
         if len(args) < len(ori_args):
             nb_missing = len(ori_args) - len(args)
             missing_args_indices = range(len(ori_args) - nb_missing, len(ori_args), 1)
             for index in missing_args_indices:
                 name = ori_args[index]
                 try:
                     filtered_kwargs[name] = kwargs[name]
-                except:
-                    pass  # we pass to raise the natural error (TypeError: missing X required positional arguments) below.
+                except Exception as e:
+                    pass
+                    # we pass to raise the natural error (TypeError: missing X required positional arguments) below.
 
         return func(*args, **filtered_kwargs)
 
     return wrap
 
+
 class ParameterRegistrator:
     """A class to manage the registration of parameters.
     It maintains a stack of ParameterRegistrators. The most recently created, but not yet exited,
     one is considered active and used for parameter registration.
 
     It is best used when working with a wrapper that creates a dictionnary to register function arguments automatically,
     such as filter_save_kwargs defined above.
@@ -254,71 +238,66 @@
     """
 
     _instance = OrderedDict()
 
     def __new__(cls, name, *args, **kwargs):
         obj = super(ParameterRegistrator, cls).__new__(cls)
         obj.name = name
-        cls._instance[
-            name
-        ] = obj  # cls is the class object. So the _instance dict stays shared by the class members with this statement
+        cls._instance[name] = (
+            obj  # cls is the class object. So the _instance dict stays shared by the class members with this statement
+        )
         return obj
 
     def __enter__(self):
         """Clear the _parameter_registry and return it for usage."""
         self._parameter_registry = {}
         self._parameter_registry["registrator_name"] = self.name
         return self._parameter_registry
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        """Remove the instance from _instance dictionary when it is not in use. Happends after a 'with' statement exits"""
+        """Remove the instance from _instance dictionary when it is not in use.
+        Happends after a 'with' statement exits
+        """
         self._instance.pop(self.name)
 
     @classmethod
     def get_registry(cls):
         """Get the parameter registry of the last created, but not yet exited, instance.
         If no instances are existing or all instances have exited, it returns an empty dictionary.
 
         Returns:
             dict: The last non-exited instance's registry or an empty dictionary.
         """
         try:
-            last_instance_name, last_instance = list(cls._instance.items())[
-                -1
-            ]  # Get the last Registrator instance
+            last_instance_name, last_instance = list(cls._instance.items())[-1]  # Get the last Registrator instance
             return last_instance._parameter_registry  # Return last instance's registry
-        except:
+        except Exception as e:
             return {}  # Return empty dictionary if no non-exited instances are found
 
     @classmethod
     def register(cls, dictionnary):
         """Update the parameter registry of the last created, but not yet exited, instance with a new dictionary.
 
         Args:
             dictionnary (dict): The dictionary to combine with the last non-exited instance's registry.
         """
         try:
-            last_instance_dict = (
-                cls.get_registry()
-            )  # Get the last non-exited instance's registry
-            last_instance_dict.update(
-                dictionnary
-            )  # Update the registry using provided dictionary
-        except:
+            last_instance_dict = cls.get_registry()  # Get the last non-exited instance's registry
+            last_instance_dict.update(dictionnary)  # Update the registry using provided dictionary
+        except Exception as e:
             pass  # Do nothing if no non-exited instances are found
 
 
-import contextlib
-import joblib
-
 # credits to featuredpeow : https://stackoverflow.com/questions/24983493/tracking-progress-of-joblib-parallel-execution
 
+
 @contextlib.contextmanager
 def tqdm_joblib(tqdm_object):
     """Context manager to patch joblib to report into tqdm progress bar given as argument"""
+
     class TqdmBatchCompletionCallback(joblib.parallel.BatchCompletionCallBack):
         def __call__(self, *args, **kwargs):
             tqdm_object.update(n=self.batch_size)
             return super().__call__(*args, **kwargs)
 
     old_batch_callback = joblib.parallel.BatchCompletionCallBack
     joblib.parallel.BatchCompletionCallBack = TqdmBatchCompletionCallback
```

### Comparing `treat2p-0.0.2/treat2p.egg-info/PKG-INFO` & `treat2p-0.0.3/treat2p.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.2
+Version: 0.0.3
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

