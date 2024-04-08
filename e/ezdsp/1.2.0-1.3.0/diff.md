# Comparing `tmp/ezdsp-1.2.0.tar.gz` & `tmp/ezdsp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezdsp-1.2.0.tar", last modified: Mon Apr  8 07:22:18 2024, max compression
+gzip compressed data, was "ezdsp-1.3.0.tar", last modified: Mon Apr  8 15:30:29 2024, max compression
```

## Comparing `ezdsp-1.2.0.tar` & `ezdsp-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 07:22:18.248856 ezdsp-1.2.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.2.0/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4084 2024-04-08 07:22:18.248856 ezdsp-1.2.0/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3340 2024-04-08 07:19:49.000000 ezdsp-1.2.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 07:22:18.248856 ezdsp-1.2.0/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.2.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 07:22:18.245856 ezdsp-1.2.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 07:22:18.247856 ezdsp-1.2.0/src/ezdsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.2.0/src/ezdsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 07:21:54.000000 ezdsp-1.2.0/src/ezdsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.2.0/src/ezdsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.2.0/src/ezdsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.2.0/src/ezdsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.2.0/src/ezdsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.2.0/src/ezdsp/_modulation_index.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.2.0/src/ezdsp/_pac.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.2.0/src/ezdsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.2.0/src/ezdsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.2.0/src/ezdsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5489 2024-04-08 05:14:40.000000 ezdsp-1.2.0/src/ezdsp/_utils.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.2.0/src/ezdsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.2.0/src/ezdsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.2.0/src/ezdsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 07:22:18.248856 ezdsp-1.2.0/src/ezdsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.2.0/src/ezdsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1344 2024-04-08 04:33:01.000000 ezdsp-1.2.0/src/ezdsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5907 2024-04-08 04:34:25.000000 ezdsp-1.2.0/src/ezdsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-04-08 04:38:01.000000 ezdsp-1.2.0/src/ezdsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.2.0/src/ezdsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.2.0/src/ezdsp/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.2.0/src/ezdsp/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.2.0/src/ezdsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5228 2024-04-08 04:42:46.000000 ezdsp-1.2.0/src/ezdsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.2.0/src/ezdsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      467 2024-04-08 04:40:51.000000 ezdsp-1.2.0/src/ezdsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.2.0/src/ezdsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 07:22:18.248856 ezdsp-1.2.0/src/ezdsp.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4084 2024-04-08 07:22:18.000000 ezdsp-1.2.0/src/ezdsp.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      823 2024-04-08 07:22:18.000000 ezdsp-1.2.0/src/ezdsp.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 07:22:18.000000 ezdsp-1.2.0/src/ezdsp.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-04-08 07:22:18.000000 ezdsp-1.2.0/src/ezdsp.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 07:22:18.000000 ezdsp-1.2.0/src/ezdsp.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:30:29.073214 ezdsp-1.3.0/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.3.0/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3731 2024-04-08 15:30:29.073214 ezdsp-1.3.0/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2960 2024-04-08 15:08:23.000000 ezdsp-1.3.0/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 15:30:29.073214 ezdsp-1.3.0/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.3.0/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:30:29.070214 ezdsp-1.3.0/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:30:29.071214 ezdsp-1.3.0/src/ezdsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.3.0/src/ezdsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 15:16:17.000000 ezdsp-1.3.0/src/ezdsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6033 2024-04-08 07:43:19.000000 ezdsp-1.3.0/src/ezdsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.3.0/src/ezdsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.3.0/src/ezdsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.3.0/src/ezdsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3772 2024-04-08 15:10:36.000000 ezdsp-1.3.0/src/ezdsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3966 2024-04-08 15:25:00.000000 ezdsp-1.3.0/src/ezdsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.3.0/src/ezdsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.3.0/src/ezdsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.3.0/src/ezdsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5489 2024-04-08 05:14:40.000000 ezdsp-1.3.0/src/ezdsp/_utils.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.3.0/src/ezdsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.3.0/src/ezdsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.3.0/src/ezdsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:30:29.072214 ezdsp-1.3.0/src/ezdsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.3.0/src/ezdsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1344 2024-04-08 04:33:01.000000 ezdsp-1.3.0/src/ezdsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5907 2024-04-08 07:37:32.000000 ezdsp-1.3.0/src/ezdsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-04-08 04:38:01.000000 ezdsp-1.3.0/src/ezdsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.3.0/src/ezdsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5834 2024-04-08 08:01:06.000000 ezdsp-1.3.0/src/ezdsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9608 2024-04-08 15:26:52.000000 ezdsp-1.3.0/src/ezdsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.3.0/src/ezdsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5228 2024-04-08 04:42:46.000000 ezdsp-1.3.0/src/ezdsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.3.0/src/ezdsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      467 2024-04-08 04:40:51.000000 ezdsp-1.3.0/src/ezdsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.3.0/src/ezdsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:30:29.072214 ezdsp-1.3.0/src/ezdsp.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     3731 2024-04-08 15:30:29.000000 ezdsp-1.3.0/src/ezdsp.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      823 2024-04-08 15:30:29.000000 ezdsp-1.3.0/src/ezdsp.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 15:30:29.000000 ezdsp-1.3.0/src/ezdsp.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-04-08 15:30:29.000000 ezdsp-1.3.0/src/ezdsp.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 15:30:29.000000 ezdsp-1.3.0/src/ezdsp.egg-info/top_level.txt
```

### Comparing `ezdsp-1.2.0/LICENSE` & `ezdsp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/PKG-INFO` & `ezdsp-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.2.0
+Version: 1.3.0
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
@@ -21,24 +21,22 @@
 Requires-Dist: ripple_detection
 Requires-Dist: scipy
 Requires-Dist: tensorpac
 Requires-Dist: torch
 Requires-Dist: torch_fn
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
+Requires-Dist: mngs==1.2.3
 
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/pip_install.yml/badge.svg)
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/run_example.yml/badge.svg)
 
-# EZDSP: Easy Digital Signal Processing
+# ezDSP: Easy Digital Signal Processing
 
-## Key Features
-- **PyTorch Integration**: With functions written in PyTorch ([`./src/ezdsp/nn/`](./src/ezdsp/nn/)), EZDSP leverages the power of parallel computation, making it ideal for machine learning applications.
-- **Automatic Data Handling**: Thanks to the [torch_fn decorator](https://github.com/ywatanabe1989/torch_fn), EZDSP functions accept torch.tensors (CPU & GPU), numpy.ndarray, and pd.DataFrame as input and return in the corresponding data type.
-- **Practical Examples**: [`./example.py`](./example.py) demonstrates all of the functions listed below and generates output figures in [`./example_outputs/`](./example_outputs/).
+ezDSP is a digital signal processing toolbox written in PyTorch (`./src/ezdsp/nn/`). However, ezDSP not only processes torch.tensors (CPU & GPU) but also handles numpy.ndarray and pd.DataFrame, enabling a consistent and intensive workflow.
 
 ## Installation
 ```bash
 $ pip install ezdsp
 $ python ./example.py # ./example_outputs/ will be generated.
 ```
 
@@ -51,78 +49,81 @@
 #### Wavelet Transformation
 <div align="center">
   <img src="./example_outputs/4_ripple/2_wavelet_orig.png" height="400">
 </div>
 
 #### Power Spectrum Density
 <div align="center">
+  <img src="./example_outputs/3_chirp/3_orig.png" height="400">
   <img src="./example_outputs/3_chirp/3_psd_bandstop_filted%20(20%20-%2050%20Hz).png" height="400">
 </div>
 
 #### Phase-Amplitude Coupling
 <div align="center">
-  <img src="./example_outputs/6_tensorpac/4_pac_orig.png" height="400">
+  <img src="./example_outputs/modulation_index_calculation_with_ezDSP_and_Tensorpac.png" height="400">
 </div>
 
 ## Quick Start
 ``` python
-import ezdsp
+import ezdsp as ed
 
 # Parameters
 SRC_FS = 1024  # Source sampling frequency
 TGT_FS = 512   # Target sampling frequency
 FREQS_HZ = [10, 30, 100]  # Frequencies in Hz
 LOW_HZ = 20    # Low frequency for bandpass filter
 HIGH_HZ = 50   # High frequency for bandpass filter
 SIGMA = 10     # Sigma for Gaussian filter
+SIG_TYPES = [
+    "uniform",
+    "gauss",
+    "periodic",
+    "chirp",
+    "ripple",
+    "meg",
+    "tensorpac",
+] # Available signal types
 
 
 # Demo Signal
-xx, tt, fs = ezdsp.demo_sig(
+xx, tt, fs = ed.demo_sig(
     t_sec=T_SEC, fs=SRC_FS, freqs_hz=FREQS_HZ, sig_type="chirp"
 )
-# xx is compatible with torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
+# xx is either of torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
 
 # Normalization
-xx_norm = ezdsp.norm.z(xx)
-xx_minmax = ezdsp.norm.minmax(xx)
+xx_norm = ed.norm.z(xx)
+xx_minmax = ed.norm.minmax(xx)
 
 # Resampling
-xx_resampled = ezdsp.resample(xx, fs, TGT_FS)
+xx_resampled = ed.resample(xx, fs, TGT_FS)
 
 # Noise addition
-xx_gauss = ezdsp.add_noise.gauss(xx)
-xx_white = ezdsp.add_noise.white(xx)
-xx_pink = ezdsp.add_noise.pink(xx)
-xx_brown = ezdsp.add_noise.brown(xx)
+xx_gauss = ed.add_noise.gauss(xx)
+xx_white = ed.add_noise.white(xx)
+xx_pink = ed.add_noise.pink(xx)
+xx_brown = ed.add_noise.brown(xx)
 
 # Filtering
-xx_filted_bandpass = ezdsp.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_bandstop = ezdsp.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_gauss = ezdsp.filt.gauss(xx, sigma=SIGMA)
+xx_filted_bandpass = ed.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_bandstop = ed.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_gauss = ed.filt.gauss(xx, sigma=SIGMA)
 
 # Hilbert Transformation
-phase, amplitude = ezdsp.hilbert(xx) # or envelope
+phase, amplitude = ed.hilbert(xx) # or envelope
 
 # Wavelet Transformation
-wavelet_coef, wavelet_freqs = ezdsp.wavelet(xx, fs)
+wavelet_coef, wavelet_freqs = ed.wavelet(xx, fs)
 
 # Power Spetrum Density
-psd, psd_freqs = ezdsp.psd(xx, fs)
+psd, psd_freqs = ed.psd(xx, fs)
 
 # Phase-Amplitude Coupling
-pac, freqs_pha, freqs_amp = ezdsp.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
+pac, freqs_pha, freqs_amp = ed.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
 ```
 
-# Citation
-To cite EZDSP in your work, please use the following format:
-``` bibtex
-@misc{ezdsp2024,
-  author = {Watanabe, Yusuke},
-  title = {{EZDSP: Easy Digital Signal Processing}},
-  year = {2023},
-  howpublished = {\url{https://github.com/ywatanabe1989/ezdsp}},
-}
-```
+# Alias
+[`mngs.dsp`](https://github.com/ywatanabe1989/mngs/src/mngs/dsp/) has the same functionalities.
 
 # Contact
 Yusuke Watanabe (ywata1989@gmail.com).
+
```

### Comparing `ezdsp-1.2.0/README.md` & `ezdsp-1.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/pip_install.yml/badge.svg)
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/run_example.yml/badge.svg)
 
-# EZDSP: Easy Digital Signal Processing
+# ezDSP: Easy Digital Signal Processing
 
-## Key Features
-- **PyTorch Integration**: With functions written in PyTorch ([`./src/ezdsp/nn/`](./src/ezdsp/nn/)), EZDSP leverages the power of parallel computation, making it ideal for machine learning applications.
-- **Automatic Data Handling**: Thanks to the [torch_fn decorator](https://github.com/ywatanabe1989/torch_fn), EZDSP functions accept torch.tensors (CPU & GPU), numpy.ndarray, and pd.DataFrame as input and return in the corresponding data type.
-- **Practical Examples**: [`./example.py`](./example.py) demonstrates all of the functions listed below and generates output figures in [`./example_outputs/`](./example_outputs/).
+ezDSP is a digital signal processing toolbox written in PyTorch (`./src/ezdsp/nn/`). However, ezDSP not only processes torch.tensors (CPU & GPU) but also handles numpy.ndarray and pd.DataFrame, enabling a consistent and intensive workflow.
 
 ## Installation
 ```bash
 $ pip install ezdsp
 $ python ./example.py # ./example_outputs/ will be generated.
 ```
 
@@ -23,78 +20,81 @@
 #### Wavelet Transformation
 <div align="center">
   <img src="./example_outputs/4_ripple/2_wavelet_orig.png" height="400">
 </div>
 
 #### Power Spectrum Density
 <div align="center">
+  <img src="./example_outputs/3_chirp/3_orig.png" height="400">
   <img src="./example_outputs/3_chirp/3_psd_bandstop_filted%20(20%20-%2050%20Hz).png" height="400">
 </div>
 
 #### Phase-Amplitude Coupling
 <div align="center">
-  <img src="./example_outputs/6_tensorpac/4_pac_orig.png" height="400">
+  <img src="./example_outputs/modulation_index_calculation_with_ezDSP_and_Tensorpac.png" height="400">
 </div>
 
 ## Quick Start
 ``` python
-import ezdsp
+import ezdsp as ed
 
 # Parameters
 SRC_FS = 1024  # Source sampling frequency
 TGT_FS = 512   # Target sampling frequency
 FREQS_HZ = [10, 30, 100]  # Frequencies in Hz
 LOW_HZ = 20    # Low frequency for bandpass filter
 HIGH_HZ = 50   # High frequency for bandpass filter
 SIGMA = 10     # Sigma for Gaussian filter
+SIG_TYPES = [
+    "uniform",
+    "gauss",
+    "periodic",
+    "chirp",
+    "ripple",
+    "meg",
+    "tensorpac",
+] # Available signal types
 
 
 # Demo Signal
-xx, tt, fs = ezdsp.demo_sig(
+xx, tt, fs = ed.demo_sig(
     t_sec=T_SEC, fs=SRC_FS, freqs_hz=FREQS_HZ, sig_type="chirp"
 )
-# xx is compatible with torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
+# xx is either of torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
 
 # Normalization
-xx_norm = ezdsp.norm.z(xx)
-xx_minmax = ezdsp.norm.minmax(xx)
+xx_norm = ed.norm.z(xx)
+xx_minmax = ed.norm.minmax(xx)
 
 # Resampling
-xx_resampled = ezdsp.resample(xx, fs, TGT_FS)
+xx_resampled = ed.resample(xx, fs, TGT_FS)
 
 # Noise addition
-xx_gauss = ezdsp.add_noise.gauss(xx)
-xx_white = ezdsp.add_noise.white(xx)
-xx_pink = ezdsp.add_noise.pink(xx)
-xx_brown = ezdsp.add_noise.brown(xx)
+xx_gauss = ed.add_noise.gauss(xx)
+xx_white = ed.add_noise.white(xx)
+xx_pink = ed.add_noise.pink(xx)
+xx_brown = ed.add_noise.brown(xx)
 
 # Filtering
-xx_filted_bandpass = ezdsp.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_bandstop = ezdsp.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_gauss = ezdsp.filt.gauss(xx, sigma=SIGMA)
+xx_filted_bandpass = ed.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_bandstop = ed.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_gauss = ed.filt.gauss(xx, sigma=SIGMA)
 
 # Hilbert Transformation
-phase, amplitude = ezdsp.hilbert(xx) # or envelope
+phase, amplitude = ed.hilbert(xx) # or envelope
 
 # Wavelet Transformation
-wavelet_coef, wavelet_freqs = ezdsp.wavelet(xx, fs)
+wavelet_coef, wavelet_freqs = ed.wavelet(xx, fs)
 
 # Power Spetrum Density
-psd, psd_freqs = ezdsp.psd(xx, fs)
+psd, psd_freqs = ed.psd(xx, fs)
 
 # Phase-Amplitude Coupling
-pac, freqs_pha, freqs_amp = ezdsp.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
+pac, freqs_pha, freqs_amp = ed.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
 ```
 
-# Citation
-To cite EZDSP in your work, please use the following format:
-``` bibtex
-@misc{ezdsp2024,
-  author = {Watanabe, Yusuke},
-  title = {{EZDSP: Easy Digital Signal Processing}},
-  year = {2023},
-  howpublished = {\url{https://github.com/ywatanabe1989/ezdsp}},
-}
-```
+# Alias
+[`mngs.dsp`](https://github.com/ywatanabe1989/mngs/src/mngs/dsp/) has the same functionalities.
 
 # Contact
 Yusuke Watanabe (ywata1989@gmail.com).
+
```

### Comparing `ezdsp-1.2.0/setup.py` & `ezdsp-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/PARAMS.py` & `ezdsp-1.3.0/src/ezdsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/__init__.py` & `ezdsp-1.3.0/src/ezdsp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from ._pac import pac
 from ._psd import psd
 from ._resample import resample
 from ._transform import to_segments, to_sktime_df
 from ._wavelet import wavelet
 
 __copyright__ = "Copyright (C) 2024 Yusuke Watanabe"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 __license__ = "MIT"
 __author__ = "ywatanabe1989"
 __author_email__ = "ywata1989@gmail.com"
 __url__ = "https://github.com/ywatanabe1989/ezdsp"
```

### Comparing `ezdsp-1.2.0/src/ezdsp/_demo_sig.py` & `ezdsp-1.3.0/src/ezdsp/_demo_sig.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 13:21:18 (ywatanabe)"
+# Time-stamp: "2024-04-08 17:43:19 (ywatanabe)"
 
 import random
 import warnings
 
 import mne
 import numpy as np
 from mne.datasets import sample
@@ -46,14 +46,16 @@
 
 
 def demo_sig(
     batch_size=8,
     n_chs=19,
     t_sec=4,
     fs=512,
+    f_pha=10,
+    f_amp=100,
     freqs_hz=None,
     sig_type="periodic",
     verbose=False,
 ):
 
     assert sig_type in [
         "uniform",
@@ -93,14 +95,16 @@
 
     elif sig_type == "tensorpac":
         xx, tt = _demo_sig_tensorpac(
             batch_size=batch_size,
             n_chs=n_chs,
             t_sec=t_sec,
             fs=fs,
+            f_pha=f_pha,
+            f_amp=f_amp,
         )
         return xx.astype(np.float32)[..., : len(tt)], tt, fs
 
     else:
         fn_1d = {
             "periodic": _demo_sig_periodic_1d,
             "chirp": _demo_sig_chirp_1d,
```

### Comparing `ezdsp-1.2.0/src/ezdsp/_hilbert.py` & `ezdsp-1.3.0/src/ezdsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_mne.py` & `ezdsp-1.3.0/src/ezdsp/_mne.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_modulation_index.py` & `ezdsp-1.3.0/src/ezdsp/_modulation_index.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,151 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 14:01:29 (ywatanabe)"
+# Time-stamp: "2024-04-09 01:10:36 (ywatanabe)"
 
 import torch
 from ezdsp.nn import ModulationIndex
 from torch_fn import torch_fn
 
 
 @torch_fn
-def modulation_index(pha, amp, n_bins=18):
+def modulation_index(pha, amp, n_bins=18, device="cuda"):
     """
     pha: (batch_size, n_chs, n_freqs_pha, n_segments, seq_len)
     amp: (batch_size, n_chs, n_freqs_amp, n_segments, seq_len)
     """
     return ModulationIndex(n_bins=n_bins)(pha, amp)
 
 
-def plot_comodulogram_tensorpac(xx, fs, t_sec, ts=None):
+def calc_pac_with_tensorpac(xx, fs, t_sec):
     import tensorpac
-    from tensorpac import Pac
 
     # Morlet's Wavelet Transfrmation
-    p = tensorpac.Pac(f_pha="hres", f_amp="hres", dcomplex="wavelet")
+    p = tensorpac.Pac(f_pha="hres", f_amp="demon", dcomplex="wavelet")
+    #
+    # n_bands: | lres, 10 | mres, 30 | hres, 50 | demon, 70 | hulk, 100 |
 
     # Bandpass Filtering and Hilbert Transformation
     i_batch, i_ch = 0, 0
     phases = p.filter(
         fs, xx[i_batch, i_ch], ftype="phase", n_jobs=1
     )  # (50, 20, 2048)
     amplitudes = p.filter(
         fs, xx[i_batch, i_ch], ftype="amplitude", n_jobs=1
     )  # (50, 20, 2048)
 
     # Calculates xpac
     k = 2
     p.idpac = (k, 0, 0)
-    xpac = p.fit(phases, amplitudes)  # (50, 50, 20)
-    pac = xpac.mean(axis=-1)  # (50, 50)
+    xpac = p.fit(phases, amplitudes)  # (50, 30, 20)
+    pac = xpac.mean(axis=-1)  # (50, 30)
+    # Transposes `pac_tp` to make the x-axis for phase and the y-axis for amplitude.
+    pac = pac.T  # (30, 50)
 
-    ## Plot
-    fig, ax = plt.subplots()
-    ax = p.comodulogram(
-        pac, title=p.method.replace(" (", f" ({k})\n("), cmap="viridis"
-    )
-    # ax = mngs.plt.ax.set_n_ticks(ax)
-    # import ipdb
-
-    # ipdb.set_trace()
     freqs_amp = p.f_amp.mean(axis=-1)
     freqs_pha = p.f_pha.mean(axis=-1)
 
-    return phases, amplitudes, freqs_pha, freqs_amp
-    # return phases and amplitudes for future use in my implementation
-    # as the aim of this code is to confirm the calculation of Modulation Index only
-    # without considering bandpass filtering and hilbert transformation.
+    return phases, amplitudes, freqs_pha, freqs_amp, pac
+    # return phases and amplitudes for future use in ezDSP calculation
+    # to confirm the calculation of Modulation Index, without considering
+    # bandpass filtering and hilbert transformation.
 
 
 @torch_fn
-def reshape_pha_amp(pha, amp, batch_size=2, n_chs=4):
-    pha = torch.tensor(pha).half()
-    amp = torch.tensor(amp).half()
-    pha = pha.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    amp = amp.unsqueeze(0).unsqueeze(0).repeat(batch_size, n_chs, 1, 1, 1)
-    return pha, amp
+def reshape(x, batch_size=2, n_chs=4):
+    return (
+        torch.tensor(x)
+        .unsqueeze(0)
+        .unsqueeze(0)
+        .repeat(batch_size, n_chs, 1, 1, 1)
+    )
 
 
 if __name__ == "__main__":
+    import ezdsp
     import matplotlib.pyplot as plt
+    import mngs
+
+    # Congig
+    mngs.plt.configure_mpl(plt, fig_scale=5)
 
     # Parameters
-    fs = 128
-    t_sec = 5
+    FS = 128
+    T_SEC = 5
 
     # Demo signal
-    xx, tt, fs = ezdsp.demo_sig(fs=fs, t_sec=t_sec, sig_type="tensorpac")
-    # xx.shape: (8, 19, 20, 512)
+    xx, tt, fs = ezdsp.demo_sig(
+        fs=FS, t_sec=T_SEC, sig_type="tensorpac"
+    )  # (8, 19, 20, 512)
 
     # Tensorpac calculation
-    pha, amp, freqs_pha, freqs_amp = plot_comodulogram_tensorpac(
+    (
+        pha_tp,
+        amp_tp,
+        freqs_pha_tp,  # (10,)
+        freqs_amp_tp,  # (30,)
+        pac_tp,  # (30, 10)
+    ) = calc_pac_with_tensorpac(
         xx,
         fs,
-        t_sec=t_sec,
+        t_sec=T_SEC,
     )
 
-    # GPU calculation
-    pha, amp = reshape_pha_amp(pha, amp)
-    pac = ezdsp.modulation_index(pha, amp)
-
-    ## Convert y-axis
+    # ezDSP calculation (on CPU now, due to the limitation in computational resources)
     i_batch, i_ch = 0, 0
+    pac_ed = ezdsp.modulation_index(
+        reshape(pha_tp), reshape(amp_tp), device="cpu"
+    )[
+        i_batch, i_ch
+    ]  # (10, 30)
+
+    # Plots
+    fig, axes = mngs.plt.subplots(ncols=3, sharex=True, sharey=True)
+
+    # To align scalebars
+    vmin = min(np.min(pac_ed), np.min(pac_tp))
+    vmax = max(np.max(pac_ed), np.max(pac_tp))
+
+    # EZDSP
+    axes[0].imshow2d(
+        pac_ed,
+        cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
+    )
+    axes[0].set_title("ezDSP (on GPU)")
 
-    fig, ax = mngs.plt.subplots()
-    ax.imshow2d(
-        pac[i_batch, i_ch],
+    # Tensorpac
+    axes[1].imshow2d(
+        pac_tp,
         cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
     )
-    ax = mngs.plt.ax.set_ticks(
-        ax, xticks=freqs_pha.astype(int), yticks=freqs_amp.astype(int)
+    axes[1].set_title("Tensorpac")
+
+    # Diff.
+    axes[2].imshow2d(
+        pac_ed - pac_tp,
+        cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
     )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    ax.set_xlabel("Frequency for phase [Hz]")
-    ax.set_ylabel("Frequency for amplitude [Hz]")
-    ax.set_title("GPU calculation")
+    axes[2].set_title("Difference\n(EZDSP - Tensorpac)")
 
-    plt.show()
+    for ax in axes:
+        ax = mngs.plt.ax.set_ticks(
+            ax,
+            xticks=freqs_pha_tp.astype(int),
+            yticks=freqs_amp_tp.astype(int),
+        )
+        ax = mngs.plt.ax.set_n_ticks(ax)
+
+    fig.supxlabel("Frequency for phase [Hz]")
+    fig.supylabel("Frequency for amplitude [Hz]")
+
+    # plt.show()
+
+    mngs.io.save(
+        fig,
+        "./example_outputs/modulation_index_calculation_with_ezDSP_and_Tensorpac.png",
+    )
```

### Comparing `ezdsp-1.2.0/src/ezdsp/_pac.py` & `ezdsp-1.3.0/src/ezdsp/_pac.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 14:03:01 (ywatanabe)"
+# Time-stamp: "2024-04-09 01:25:00 (ywatanabe)"
 
+import ezdsp
+from ezdsp._modulation_index import calc_pac_with_tensorpac
 from ezdsp.nn import PAC
 from torch_fn import torch_fn
 
 
 @torch_fn
 def pac(
     x,
     fs,
     pha_start_hz=2,
     pha_end_hz=20,
     pha_n_bands=100,
     amp_start_hz=60,
     amp_end_hz=160,
     amp_n_bands=100,
+    device="cuda",
 ):
     """
     Compute the phase-amplitude coupling (PAC) for signals. This function automatically handles inputs as
     PyTorch tensors, NumPy arrays, or pandas DataFrames.
 
     Arguments:
-    - x (torch.Tensor | np.ndarray | pd.DataFrame): Input signal. Shape can be either (batch_size, n_chs, seq_len) or
+    - x (torch.Tensor | np.ndarray | pd.DataFrame): Input signal. Shape can be either 4D (batch_size, n_chs, n_segments, seq_len) or 3D (batch_size, n_chs, seq_len), which will be treated as 1 segment.
     - fs (float): Sampling frequency of the input signal.
     - pha_start_hz (float, optional): Start frequency for phase bands. Default is 2 Hz.
     - pha_end_hz (float, optional): End frequency for phase bands. Default is 20 Hz.
     - pha_n_bands (int, optional): Number of phase bands. Default is 100.
     - amp_start_hz (float, optional): Start frequency for amplitude bands. Default is 60 Hz.
     - amp_end_hz (float, optional): End frequency for amplitude bands. Default is 160 Hz.
     - amp_n_bands (int, optional): Number of amplitude bands. Default is 100.
@@ -53,38 +56,88 @@
         amp_end_hz=amp_end_hz,
         amp_n_bands=amp_n_bands,
     )
     return m(x), m.BANDS_PHA, m.BANDS_AMP
 
 
 if __name__ == "__main__":
+    import ezdsp as ed
+
     # Parameters
     FS = 512
-    T_SEC = 4
+    T_SEC = 5
 
     xx, tt, fs = ezdsp.demo_sig(
         batch_size=1, n_chs=1, fs=FS, t_sec=T_SEC, sig_type="tensorpac"
     )
-    pac, pha_bands_pha, amp_bands = ezdsp.pac(xx, fs)
 
-    xx, tt, fs = ezdsp.demo_sig(
-        batch_size=1, n_chs=1, fs=FS, t_sec=T_SEC, sig_type="ripple"
+    # Tensorpac calculation
+    (
+        pha_tp,
+        amp_tp,
+        freqs_pha_tp,  # (50,)
+        freqs_amp_tp,  # (70,)
+        pac_tp,  # (50, 70)
+    ) = calc_pac_with_tensorpac(
+        xx,
+        fs,
+        t_sec=T_SEC,
+    )
+
+    # ezDSP calculation (on CPU now, due to the limitation in computational resources)
+    pac_ed, pha_bands, amp_bands = ed.pac(
+        xx, fs, pha_n_bands=50, amp_n_bands=70, device="cpu"
+    )
+    i_batch, i_ch = 0, 0
+    pac_ed = pac_ed[i_batch, i_ch]
+
+    # Plots
+    fig, axes = mngs.plt.subplots(ncols=3, sharex=True, sharey=True)
+
+    # To align scalebars
+    vmin = min(np.min(pac_ed), np.min(pac_tp))
+    vmax = max(np.max(pac_ed), np.max(pac_tp))
+
+    # EZDSP
+    axes[0].imshow2d(
+        pac_ed,
+        cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
+    )
+    axes[0].set_title("ezDSP")
+
+    # Tensorpac
+    axes[1].imshow2d(
+        pac_tp,
+        cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
+    )
+    axes[1].set_title("Tensorpac")
+
+    # Diff.
+    axes[2].imshow2d(
+        pac_ed - pac_tp,
+        cbar_label="PAC values",
+        vmin=vmin,
+        vmax=vmax,
     )
-    pac, pha_bands_pha, amp_bands = ezdsp.pac(xx, fs)
+    axes[2].set_title("Difference\n(EZDSP - Tensorpac)")
+
+    for ax in axes:
+        ax = mngs.plt.ax.set_ticks(
+            ax,
+            xticks=freqs_pha_tp.astype(int),
+            yticks=freqs_amp_tp.astype(int),
+        )
+        ax = mngs.plt.ax.set_n_ticks(ax)
+
+    fig.supxlabel("Frequency for phase [Hz]")
+    fig.supylabel("Frequency for amplitude [Hz]")
 
-    # Plots PAC, the final output
-    i_batch = 0
-    i_ch = 0
-    fig, ax = mngs.plt.subplots()
-    ax.imshow2d(
-        pac[i_batch, i_ch].cpu().numpy(),
-    )
-    ax = mngs.plt.ax.set_ticks(
-        ax,
-        xticks=np.array(BANDS_PHA).mean(axis=-1).astype(int),
-        yticks=np.array(BANDS_AMP).mean(axis=-1).astype(int),
-    )
-    ax = mngs.plt.ax.set_n_ticks(ax)
-    ax.set_xlabel("Frequency for phase [Hz]")
-    ax.set_ylabel("Frequency for amplitude [Hz]")
-    ax.set_title("PAC values")
-    plt.show()
+    # plt.show()
+
+    mngs.io.save(
+        fig,
+        "./example_outputs/pac_calculation_with_ezDSP_and_Tensorpac.png",
+    )
```

### Comparing `ezdsp-1.2.0/src/ezdsp/_psd.py` & `ezdsp-1.3.0/src/ezdsp/_psd.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_resample.py` & `ezdsp-1.3.0/src/ezdsp/_resample.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_transform.py` & `ezdsp-1.3.0/src/ezdsp/_transform.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_utils.py` & `ezdsp-1.3.0/src/ezdsp/_utils.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/_wavelet.py` & `ezdsp-1.3.0/src/ezdsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/add_noise.py` & `ezdsp-1.3.0/src/ezdsp/add_noise.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/filt.py` & `ezdsp-1.3.0/src/ezdsp/filt.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_ChannelGainChanger.py` & `ezdsp-1.3.0/src/ezdsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_DropoutChannels.py` & `ezdsp-1.3.0/src/ezdsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_Filters.py` & `ezdsp-1.3.0/src/ezdsp/nn/_Filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 14:34:25 (ywatanabe)"
+# Time-stamp: "2024-04-08 17:37:32 (ywatanabe)"
 
 import math
 import warnings
 
 import ezdsp
 import numpy as np
 import torch
```

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_FreqGainChanger.py` & `ezdsp-1.3.0/src/ezdsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_Hilbert.py` & `ezdsp-1.3.0/src/ezdsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_ModulationIndex.py` & `ezdsp-1.3.0/src/ezdsp/nn/_ModulationIndex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 11:30:02 (ywatanabe)"
+# Time-stamp: "2024-04-08 18:01:06 (ywatanabe)"
 
 
 import math
 import time
 
 import numpy as np
 import torch
@@ -145,14 +145,15 @@
 
 @torch_fn
 def modulation_index(pha, amp, n_bins=18):
     return ModulationIndex(n_bins=18)(pha, amp)
 
 
 if __name__ == "__main__":
+    import ezdsp
     import matplotlib.pyplot as plt
     import mngs
     import seaborn as sns
     import tensorpac
     from tensorpac import Pac
     from tqdm import tqdm
```

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_PAC.py` & `ezdsp-1.3.0/src/ezdsp/nn/_PAC.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 12:28:28 (ywatanabe)"
+# Time-stamp: "2024-04-09 01:26:52 (ywatanabe)"
 
 
 import warnings
 
 import torch
 import torch.nn as nn
 from ezdsp.nn import BandPassFilter, Hilbert, ModulationIndex
@@ -58,53 +58,53 @@
         I_BATCH_SIZE = 0
         I_CHS = 1
         I_FREQS = 2
         I_SEGMENTS = 3
         I_SEQ_LEN = 4
 
         # Phase
-        pha = torch.stack(
-            [bf_pha(x_3d) for bf_pha in self.bandpass_filters_pha],
-            dim=I_FREQS - 1,
-        )
-        pha = self.hilbert(pha)[..., 0]
-        pha = pha.reshape(batch_size, n_chs, *pha.shape[1:])
-        assert pha.ndim == 5
-
-        # Amplitude
-        amp = torch.stack(
-            [bf_amp(x_3d) for bf_amp in self.bandpass_filters_amp],
-            dim=I_FREQS - 1,
-        )
-        amp = self.hilbert(amp)[..., 1]
-        amp = amp.reshape(batch_size, n_chs, *amp.shape[1:])
-        assert amp.ndim == 5
-
-        # pha = (
-        #     torch.stack(
-        #         [
-        #             self.hilbert(bf_pha(x.squeeze(0)))
-        #             for bf_pha in self.bandpass_filters_pha
-        #         ],
-        #         dim=I_FREQS,
-        #     )[..., 0]
-        #     .unsqueeze(I_CHS)
-        #     .transpose(I_FREQS, I_SEGMENTS)
+        # pha = torch.stack(
+        #     [bf_pha(x_3d) for bf_pha in self.bandpass_filters_pha],
+        #     dim=I_FREQS - 1,
         # )
-        # amp = (
-        #     torch.stack(
-        #         [
-        #             self.hilbert(bf_amp(x.squeeze(0)))
-        #             for bf_amp in self.bandpass_filters_amp
-        #         ],
-        #         dim=I_FREQS,
-        #     )[..., 1]
-        #     .unsqueeze(I_CHS)
-        #     .transpose(I_FREQS, I_SEGMENTS)
+        # pha = self.hilbert(pha)[..., 0]
+        # pha = pha.reshape(batch_size, n_chs, *pha.shape[1:])
+        # assert pha.ndim == 5
+
+        # # Amplitude
+        # amp = torch.stack(
+        #     [bf_amp(x_3d) for bf_amp in self.bandpass_filters_amp],
+        #     dim=I_FREQS - 1,
         # )
+        # amp = self.hilbert(amp)[..., 1]
+        # amp = amp.reshape(batch_size, n_chs, *amp.shape[1:])
+        # assert amp.ndim == 5
+
+        pha = (
+            torch.stack(
+                [
+                    self.hilbert(bf_pha(x.squeeze(0)))
+                    for bf_pha in self.bandpass_filters_pha
+                ],
+                dim=I_FREQS,
+            )[..., 0]
+            .unsqueeze(I_CHS)
+            .transpose(I_FREQS, I_SEGMENTS)
+        )
+        amp = (
+            torch.stack(
+                [
+                    self.hilbert(bf_amp(x.squeeze(0)))
+                    for bf_amp in self.bandpass_filters_amp
+                ],
+                dim=I_FREQS,
+            )[..., 1]
+            .unsqueeze(I_CHS)
+            .transpose(I_FREQS, I_SEGMENTS)
+        )
         pac = self.modulation_index(pha, amp)
         return pac
 
     @staticmethod
     def calc_bands_pha(start_hz=2, end_hz=20, n_bands=100):
         start_hz = start_hz if start_hz is not None else 2
         end_hz = end_hz if end_hz is not None else 20
@@ -142,15 +142,16 @@
     @staticmethod
     def _ensure_4d_input(x):
         if x.ndim != 4:
             message = f"Input tensor must be 4D with the shape (batch_size, n_chs, n_segments, seq_len). Received shape: {x.shape}"
 
         if x.ndim == 3:
             warnings.warn(
-                "'n_segments' was determined to be 1, assuming your input is (batch_size, n_chs, seq_len).",
+                message
+                + f"\n'n_segments' was determined to be 1, assuming your input is (batch_size, n_chs, seq_len).",
                 UserWarning,
             )
             x = x.unsqueeze(-2)
 
         if x.ndim != 4:
             raise ValueError(message)
```

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_PSD.py` & `ezdsp-1.3.0/src/ezdsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/_Wavelet.py` & `ezdsp-1.3.0/src/ezdsp/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/nn/__init__.py` & `ezdsp-1.3.0/src/ezdsp/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp/ref.py` & `ezdsp-1.3.0/src/ezdsp/ref.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.2.0/src/ezdsp.egg-info/PKG-INFO` & `ezdsp-1.3.0/src/ezdsp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.2.0
+Version: 1.3.0
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
@@ -21,24 +21,22 @@
 Requires-Dist: ripple_detection
 Requires-Dist: scipy
 Requires-Dist: tensorpac
 Requires-Dist: torch
 Requires-Dist: torch_fn
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
+Requires-Dist: mngs==1.2.3
 
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/pip_install.yml/badge.svg)
 ![CI](https://github.com/ywatanabe1989/ezdsp/actions/workflows/run_example.yml/badge.svg)
 
-# EZDSP: Easy Digital Signal Processing
+# ezDSP: Easy Digital Signal Processing
 
-## Key Features
-- **PyTorch Integration**: With functions written in PyTorch ([`./src/ezdsp/nn/`](./src/ezdsp/nn/)), EZDSP leverages the power of parallel computation, making it ideal for machine learning applications.
-- **Automatic Data Handling**: Thanks to the [torch_fn decorator](https://github.com/ywatanabe1989/torch_fn), EZDSP functions accept torch.tensors (CPU & GPU), numpy.ndarray, and pd.DataFrame as input and return in the corresponding data type.
-- **Practical Examples**: [`./example.py`](./example.py) demonstrates all of the functions listed below and generates output figures in [`./example_outputs/`](./example_outputs/).
+ezDSP is a digital signal processing toolbox written in PyTorch (`./src/ezdsp/nn/`). However, ezDSP not only processes torch.tensors (CPU & GPU) but also handles numpy.ndarray and pd.DataFrame, enabling a consistent and intensive workflow.
 
 ## Installation
 ```bash
 $ pip install ezdsp
 $ python ./example.py # ./example_outputs/ will be generated.
 ```
 
@@ -51,78 +49,81 @@
 #### Wavelet Transformation
 <div align="center">
   <img src="./example_outputs/4_ripple/2_wavelet_orig.png" height="400">
 </div>
 
 #### Power Spectrum Density
 <div align="center">
+  <img src="./example_outputs/3_chirp/3_orig.png" height="400">
   <img src="./example_outputs/3_chirp/3_psd_bandstop_filted%20(20%20-%2050%20Hz).png" height="400">
 </div>
 
 #### Phase-Amplitude Coupling
 <div align="center">
-  <img src="./example_outputs/6_tensorpac/4_pac_orig.png" height="400">
+  <img src="./example_outputs/modulation_index_calculation_with_ezDSP_and_Tensorpac.png" height="400">
 </div>
 
 ## Quick Start
 ``` python
-import ezdsp
+import ezdsp as ed
 
 # Parameters
 SRC_FS = 1024  # Source sampling frequency
 TGT_FS = 512   # Target sampling frequency
 FREQS_HZ = [10, 30, 100]  # Frequencies in Hz
 LOW_HZ = 20    # Low frequency for bandpass filter
 HIGH_HZ = 50   # High frequency for bandpass filter
 SIGMA = 10     # Sigma for Gaussian filter
+SIG_TYPES = [
+    "uniform",
+    "gauss",
+    "periodic",
+    "chirp",
+    "ripple",
+    "meg",
+    "tensorpac",
+] # Available signal types
 
 
 # Demo Signal
-xx, tt, fs = ezdsp.demo_sig(
+xx, tt, fs = ed.demo_sig(
     t_sec=T_SEC, fs=SRC_FS, freqs_hz=FREQS_HZ, sig_type="chirp"
 )
-# xx is compatible with torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
+# xx is either of torch.tensor (on cpu / cuda), numpy.ndarray, or pd.DataFrame.
 
 # Normalization
-xx_norm = ezdsp.norm.z(xx)
-xx_minmax = ezdsp.norm.minmax(xx)
+xx_norm = ed.norm.z(xx)
+xx_minmax = ed.norm.minmax(xx)
 
 # Resampling
-xx_resampled = ezdsp.resample(xx, fs, TGT_FS)
+xx_resampled = ed.resample(xx, fs, TGT_FS)
 
 # Noise addition
-xx_gauss = ezdsp.add_noise.gauss(xx)
-xx_white = ezdsp.add_noise.white(xx)
-xx_pink = ezdsp.add_noise.pink(xx)
-xx_brown = ezdsp.add_noise.brown(xx)
+xx_gauss = ed.add_noise.gauss(xx)
+xx_white = ed.add_noise.white(xx)
+xx_pink = ed.add_noise.pink(xx)
+xx_brown = ed.add_noise.brown(xx)
 
 # Filtering
-xx_filted_bandpass = ezdsp.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_bandstop = ezdsp.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
-xx_filted_gauss = ezdsp.filt.gauss(xx, sigma=SIGMA)
+xx_filted_bandpass = ed.filt.bandpass(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_bandstop = ed.filt.bandstop(xx, fs, low_hz=LOW_HZ, high_hz=HIGH_HZ)
+xx_filted_gauss = ed.filt.gauss(xx, sigma=SIGMA)
 
 # Hilbert Transformation
-phase, amplitude = ezdsp.hilbert(xx) # or envelope
+phase, amplitude = ed.hilbert(xx) # or envelope
 
 # Wavelet Transformation
-wavelet_coef, wavelet_freqs = ezdsp.wavelet(xx, fs)
+wavelet_coef, wavelet_freqs = ed.wavelet(xx, fs)
 
 # Power Spetrum Density
-psd, psd_freqs = ezdsp.psd(xx, fs)
+psd, psd_freqs = ed.psd(xx, fs)
 
 # Phase-Amplitude Coupling
-pac, freqs_pha, freqs_amp = ezdsp.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
+pac, freqs_pha, freqs_amp = ed.pac(x_3d, fs) # This function is computationally demanding. Please monitor the RAM/VRAM usage.
 ```
 
-# Citation
-To cite EZDSP in your work, please use the following format:
-``` bibtex
-@misc{ezdsp2024,
-  author = {Watanabe, Yusuke},
-  title = {{EZDSP: Easy Digital Signal Processing}},
-  year = {2023},
-  howpublished = {\url{https://github.com/ywatanabe1989/ezdsp}},
-}
-```
+# Alias
+[`mngs.dsp`](https://github.com/ywatanabe1989/mngs/src/mngs/dsp/) has the same functionalities.
 
 # Contact
 Yusuke Watanabe (ywata1989@gmail.com).
+
```

### Comparing `ezdsp-1.2.0/src/ezdsp.egg-info/SOURCES.txt` & `ezdsp-1.3.0/src/ezdsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

