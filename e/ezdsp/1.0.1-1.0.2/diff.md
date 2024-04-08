# Comparing `tmp/ezdsp-1.0.1.tar.gz` & `tmp/ezdsp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezdsp-1.0.1.tar", last modified: Mon Apr  8 04:26:57 2024, max compression
+gzip compressed data, was "ezdsp-1.0.2.tar", last modified: Mon Apr  8 04:35:42 2024, max compression
```

## Comparing `ezdsp-1.0.1.tar` & `ezdsp-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.0.1/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:26:57.576150 ezdsp-1.0.1/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-1.0.1/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 04:26:57.576150 ezdsp-1.0.1/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.0.1/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.574150 ezdsp-1.0.1/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.575150 ezdsp-1.0.1/src/ezdsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.0.1/src/ezdsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 04:26:55.000000 ezdsp-1.0.1/src/ezdsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.0.1/src/ezdsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.0.1/src/ezdsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.0.1/src/ezdsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.0.1/src/ezdsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.0.1/src/ezdsp/_modulation_index.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.0.1/src/ezdsp/_pac.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.0.1/src/ezdsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.0.1/src/ezdsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.0.1/src/ezdsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.0.1/src/ezdsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.0.1/src/ezdsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6157 2024-04-08 03:52:52.000000 ezdsp-1.0.1/src/ezdsp/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.0.1/src/ezdsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/src/ezdsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.0.1/src/ezdsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 ezdsp-1.0.1/src/ezdsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5906 2024-04-08 04:19:18.000000 ezdsp-1.0.1/src/ezdsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 ezdsp-1.0.1/src/ezdsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.0.1/src/ezdsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.0.1/src/ezdsp/nn/_ModulationIndex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.0.1/src/ezdsp/nn/_PAC.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.0.1/src/ezdsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5227 2024-04-08 04:18:54.000000 ezdsp-1.0.1/src/ezdsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.0.1/src/ezdsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      444 2024-04-08 04:06:39.000000 ezdsp-1.0.1/src/ezdsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.0.1/src/ezdsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:26:57.576150 ezdsp-1.0.1/src/ezdsp.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      824 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       67 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 04:26:57.000000 ezdsp-1.0.1/src/ezdsp.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:35:42.773217 ezdsp-1.0.2/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.0.2/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      705 2024-04-08 04:35:42.773217 ezdsp-1.0.2/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-1.0.2/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 04:35:42.773217 ezdsp-1.0.2/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.0.2/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:35:42.771217 ezdsp-1.0.2/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:35:42.772217 ezdsp-1.0.2/src/ezdsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.0.2/src/ezdsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 04:35:13.000000 ezdsp-1.0.2/src/ezdsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.0.2/src/ezdsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.0.2/src/ezdsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.0.2/src/ezdsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.0.2/src/ezdsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.0.2/src/ezdsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.0.2/src/ezdsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.0.2/src/ezdsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.0.2/src/ezdsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.0.2/src/ezdsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.0.2/src/ezdsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.0.2/src/ezdsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.0.2/src/ezdsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:35:42.773217 ezdsp-1.0.2/src/ezdsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.0.2/src/ezdsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1344 2024-04-08 04:33:01.000000 ezdsp-1.0.2/src/ezdsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5907 2024-04-08 04:34:25.000000 ezdsp-1.0.2/src/ezdsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 ezdsp-1.0.2/src/ezdsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.0.2/src/ezdsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.0.2/src/ezdsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.0.2/src/ezdsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.0.2/src/ezdsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5215 2024-04-08 04:34:47.000000 ezdsp-1.0.2/src/ezdsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.0.2/src/ezdsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      444 2024-04-08 04:06:39.000000 ezdsp-1.0.2/src/ezdsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.0.2/src/ezdsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:35:42.773217 ezdsp-1.0.2/src/ezdsp.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      705 2024-04-08 04:35:42.000000 ezdsp-1.0.2/src/ezdsp.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      803 2024-04-08 04:35:42.000000 ezdsp-1.0.2/src/ezdsp.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 04:35:42.000000 ezdsp-1.0.2/src/ezdsp.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       78 2024-04-08 04:35:42.000000 ezdsp-1.0.2/src/ezdsp.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 04:35:42.000000 ezdsp-1.0.2/src/ezdsp.egg-info/top_level.txt
```

### Comparing `ezdsp-1.0.1/LICENSE` & `ezdsp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/PKG-INFO` & `ezdsp-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch_fn
 Requires-Dist: numpy_fn
+Requires-Dist: matplotlib
 
 ## Installation
 ``` bash
 $ pip install ezdsp
 ```
 
 ## Usage
```

### Comparing `ezdsp-1.0.1/setup.py` & `ezdsp-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/PARAMS.py` & `ezdsp-1.0.2/src/ezdsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/__init__.py` & `ezdsp-1.0.2/src/ezdsp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from ._pac import pac
 from ._psd import psd
 from ._resample import resample
 from ._transform import to_segments, to_sktime_df
 from ._wavelet import wavelet
 
 __copyright__ = "Copyright (C) 2024 Yusuke Watanabe"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __license__ = "MIT"
 __author__ = "ywatanabe1989"
 __author_email__ = "ywata1989@gmail.com"
 __url__ = "https://github.com/ywatanabe1989/ezdsp"
```

### Comparing `ezdsp-1.0.1/src/ezdsp/_demo_sig.py` & `ezdsp-1.0.2/src/ezdsp/_demo_sig.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_hilbert.py` & `ezdsp-1.0.2/src/ezdsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_mne.py` & `ezdsp-1.0.2/src/ezdsp/_mne.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_modulation_index.py` & `ezdsp-1.0.2/src/ezdsp/_modulation_index.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_pac.py` & `ezdsp-1.0.2/src/ezdsp/_pac.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_psd.py` & `ezdsp-1.0.2/src/ezdsp/_psd.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_resample.py` & `ezdsp-1.0.2/src/ezdsp/_resample.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_transform.py` & `ezdsp-1.0.2/src/ezdsp/_transform.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/_wavelet.py` & `ezdsp-1.0.2/src/ezdsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/add_noise.py` & `ezdsp-1.0.2/src/ezdsp/add_noise.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/filt.py` & `ezdsp-1.0.2/src/ezdsp/filt.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_ChannelGainChanger.py` & `ezdsp-1.0.2/src/ezdsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_DropoutChannels.py` & `ezdsp-1.0.2/src/ezdsp/nn/_DropoutChannels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2023-05-04 21:50:22 (ywatanabe)"
+# Time-stamp: "2024-04-08 14:33:00 (ywatanabe)"
 
+import random
+
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torchsummary import summary
-import mngs
-import numpy as np
-import random
 
 
 class DropoutChannels(nn.Module):
-    def __init__(
-        self,
-        dropout=0.5
-    ):
+    def __init__(self, dropout=0.5):
         super().__init__()
         self.dropout = nn.Dropout(p=dropout)
 
     def forward(self, x):
         """x: [batch_size, n_chs, seq_len]"""
         if self.training:
             orig_chs = torch.arange(x.shape[1])
-            
+
             indi_orig = self.dropout(torch.ones(x.shape[1])).bool()
             chs_to_shuffle = orig_chs[~indi_orig]
 
-            x[:, chs_to_shuffle] = torch.randn(x[:, chs_to_shuffle].shape).to(x.device)
+            x[:, chs_to_shuffle] = torch.randn(x[:, chs_to_shuffle].shape).to(
+                x.device
+            )
 
             # rand_chs = random.sample(list(np.array(chs_to_shuffle)), len(chs_to_shuffle))
 
             # swapped_chs = orig_chs.clone()
             # swapped_chs[~indi_orig] = torch.LongTensor(rand_chs)
 
             # x = x[:, swapped_chs.long(), :]
```

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_Filters.py` & `ezdsp-1.0.2/src/ezdsp/nn/_Filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 14:19:17 (ywatanabe)"
+# Time-stamp: "2024-04-08 14:34:25 (ywatanabe)"
 
 import math
 import warnings
 
-import mngs
+import ezdsp
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch_fn import torch_fn
```

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_FreqGainChanger.py` & `ezdsp-1.0.2/src/ezdsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_Hilbert.py` & `ezdsp-1.0.2/src/ezdsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_ModulationIndex.py` & `ezdsp-1.0.2/src/ezdsp/nn/_ModulationIndex.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_PAC.py` & `ezdsp-1.0.2/src/ezdsp/nn/_PAC.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_PSD.py` & `ezdsp-1.0.2/src/ezdsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/_Wavelet.py` & `ezdsp-1.0.2/src/ezdsp/nn/_Wavelet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 14:18:53 (ywatanabe)"
+# Time-stamp: "2024-04-08 14:34:47 (ywatanabe)"
 
 
-import mngs
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 
 class Wavelet(nn.Module):
```

### Comparing `ezdsp-1.0.1/src/ezdsp/nn/__init__.py` & `ezdsp-1.0.2/src/ezdsp/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp/ref.py` & `ezdsp-1.0.2/src/ezdsp/ref.py`

 * *Files identical despite different names*

### Comparing `ezdsp-1.0.1/src/ezdsp.egg-info/PKG-INFO` & `ezdsp-1.0.2/src/ezdsp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdsp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easy digital signal processing
 Home-page: https://github.com/ywatanabe1989/ezdsp
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
 License: MIT
 Keywords: numpytorch,pandas,LFP,EEG,MEG
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: torch_fn
 Requires-Dist: numpy_fn
+Requires-Dist: matplotlib
 
 ## Installation
 ``` bash
 $ pip install ezdsp
 ```
 
 ## Usage
```

### Comparing `ezdsp-1.0.1/src/ezdsp.egg-info/SOURCES.txt` & `ezdsp-1.0.2/src/ezdsp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 src/ezdsp/_modulation_index.py
 src/ezdsp/_pac.py
 src/ezdsp/_psd.py
 src/ezdsp/_resample.py
 src/ezdsp/_transform.py
 src/ezdsp/_wavelet.py
 src/ezdsp/add_noise.py
-src/ezdsp/example.py
 src/ezdsp/filt.py
 src/ezdsp/norm.py
 src/ezdsp/ref.py
 src/ezdsp.egg-info/PKG-INFO
 src/ezdsp.egg-info/SOURCES.txt
 src/ezdsp.egg-info/dependency_links.txt
 src/ezdsp.egg-info/requires.txt
```

