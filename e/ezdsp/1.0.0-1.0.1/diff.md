# Comparing `tmp/ezdsp-1.0.0.tar.gz` & `tmp/ezdsp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezdsp-1.0.0.tar", last modified: Mon Apr  8 04:20:08 2024, max compression
+gzip compressed data, was "ezdsp-1.0.1.tar", last modified: Mon Apr  8 04:26:57 2024, max compression
```

## Comparing `ezdsp-1.0.0.tar` & `ezdsp-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.724807 ezdsp-1.0.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.0.0/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:20:08.724807 ezdsp-1.0.0/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-1.0.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 04:20:08.724807 ezdsp-1.0.0/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.0.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.721807 ezdsp-1.0.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.722807 ezdsp-1.0.0/src/ezdsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.0.0/src/ezdsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 04:12:38.000000 ezdsp-1.0.0/src/ezdsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.0.0/src/ezdsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.0.0/src/ezdsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.0.0/src/ezdsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.0.0/src/ezdsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.0.0/src/ezdsp/_modulation_index.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.0.0/src/ezdsp/_pac.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.0.0/src/ezdsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.0.0/src/ezdsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.0.0/src/ezdsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.0.0/src/ezdsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.0.0/src/ezdsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6157 2024-04-08 03:52:52.000000 ezdsp-1.0.0/src/ezdsp/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.0.0/src/ezdsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.723807 ezdsp-1.0.0/src/ezdsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.0.0/src/ezdsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 ezdsp-1.0.0/src/ezdsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5906 2024-04-08 04:19:18.000000 ezdsp-1.0.0/src/ezdsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 ezdsp-1.0.0/src/ezdsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.0.0/src/ezdsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.0.0/src/ezdsp/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.0.0/src/ezdsp/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.0.0/src/ezdsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5227 2024-04-08 04:18:54.000000 ezdsp-1.0.0/src/ezdsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.0.0/src/ezdsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      444 2024-04-08 04:06:39.000000 ezdsp-1.0.0/src/ezdsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.0.0/src/ezdsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.723807 ezdsp-1.0.0/src/ezdsp.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      824 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       67 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.0.1/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:26:57.576150 ezdsp-1.0.1/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-1.0.1/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 04:26:57.576150 ezdsp-1.0.1/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.0.1/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.574150 ezdsp-1.0.1/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.575150 ezdsp-1.0.1/src/ezdsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.0.1/src/ezdsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 04:26:55.000000 ezdsp-1.0.1/src/ezdsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.0.1/src/ezdsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.0.1/src/ezdsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.0.1/src/ezdsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.0.1/src/ezdsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.0.1/src/ezdsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.0.1/src/ezdsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.0.1/src/ezdsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.0.1/src/ezdsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.0.1/src/ezdsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.0.1/src/ezdsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.0.1/src/ezdsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6157 2024-04-08 03:52:52.000000 ezdsp-1.0.1/src/ezdsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.0.1/src/ezdsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/src/ezdsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.0.1/src/ezdsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 ezdsp-1.0.1/src/ezdsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5906 2024-04-08 04:19:18.000000 ezdsp-1.0.1/src/ezdsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 ezdsp-1.0.1/src/ezdsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.0.1/src/ezdsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.0.1/src/ezdsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.0.1/src/ezdsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.0.1/src/ezdsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5227 2024-04-08 04:18:54.000000 ezdsp-1.0.1/src/ezdsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.0.1/src/ezdsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      444 2024-04-08 04:06:39.000000 ezdsp-1.0.1/src/ezdsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.0.1/src/ezdsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/src/ezdsp.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      824 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       67 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/top_level.txt
```

### Comparing `ezdsp-1.0.0/LICENSE` & `ezdsp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/PKG-INFO` & `ezdsp-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezdsp-1.0.0/setup.py` & `ezdsp-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/PARAMS.py` & `ezdsp-1.0.1/src/ezdsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/__init__.py` & `ezdsp-1.0.1/src/ezdsp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from ._pac import pac
 from ._psd import psd
 from ._resample import resample
 from ._transform import to_segments, to_sktime_df
 from ._wavelet import wavelet
 
 __copyright__ = "Copyright (C) 2024 Yusuke Watanabe"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __license__ = "MIT"
 __author__ = "ywatanabe1989"
 __author_email__ = "ywata1989@gmail.com"
 __url__ = "https://github.com/ywatanabe1989/ezdsp"
```

### Comparing `ezdsp-1.0.0/src/ezdsp/_demo_sig.py` & `ezdsp-1.0.1/src/ezdsp/_demo_sig.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_hilbert.py` & `ezdsp-1.0.1/src/ezdsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_mne.py` & `ezdsp-1.0.1/src/ezdsp/_mne.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_modulation_index.py` & `ezdsp-1.0.1/src/ezdsp/_modulation_index.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_pac.py` & `ezdsp-1.0.1/src/ezdsp/_pac.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_psd.py` & `ezdsp-1.0.1/src/ezdsp/_psd.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_resample.py` & `ezdsp-1.0.1/src/ezdsp/_resample.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_transform.py` & `ezdsp-1.0.1/src/ezdsp/_transform.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/_wavelet.py` & `ezdsp-1.0.1/src/ezdsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/add_noise.py` & `ezdsp-1.0.1/src/ezdsp/add_noise.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/example.py` & `ezdsp-1.0.1/src/ezdsp/example.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/filt.py` & `ezdsp-1.0.1/src/ezdsp/filt.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_ChannelGainChanger.py` & `ezdsp-1.0.1/src/ezdsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_DropoutChannels.py` & `ezdsp-1.0.1/src/ezdsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_Filters.py` & `ezdsp-1.0.1/src/ezdsp/nn/_Filters.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_FreqGainChanger.py` & `ezdsp-1.0.1/src/ezdsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_Hilbert.py` & `ezdsp-1.0.1/src/ezdsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_ModulationIndex.py` & `ezdsp-1.0.1/src/ezdsp/nn/_ModulationIndex.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_PAC.py` & `ezdsp-1.0.1/src/ezdsp/nn/_PAC.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_PSD.py` & `ezdsp-1.0.1/src/ezdsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/_Wavelet.py` & `ezdsp-1.0.1/src/ezdsp/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/nn/__init__.py` & `ezdsp-1.0.1/src/ezdsp/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp/ref.py` & `ezdsp-1.0.1/src/ezdsp/ref.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.0/src/ezdsp.egg-info/PKG-INFO` & `ezdsp-1.0.1/src/ezdsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ezdsp-1.0.0/src/ezdsp.egg-info/SOURCES.txt` & `ezdsp-1.0.1/src/ezdsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

