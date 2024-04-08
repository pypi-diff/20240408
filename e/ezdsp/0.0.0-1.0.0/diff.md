# Comparing `tmp/ezdsp-0.0.0.tar.gz` & `tmp/ezdsp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezdsp-0.0.0.tar", last modified: Mon Apr  8 02:57:15 2024, max compression
+gzip compressed data, was "ezdsp-1.0.0.tar", last modified: Mon Apr  8 04:20:08 2024, max compression
```

## Comparing `ezdsp-0.0.0.tar` & `ezdsp-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,42 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 02:57:15.895588 ezdsp-0.0.0/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-0.0.0/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      577 2024-04-08 02:57:15.895588 ezdsp-0.0.0/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-0.0.0/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 02:57:15.895588 ezdsp-0.0.0/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1990 2024-04-08 02:56:09.000000 ezdsp-0.0.0/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 02:57:15.894589 ezdsp-0.0.0/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 02:57:15.894589 ezdsp-0.0.0/src/ezdsp/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      339 2024-04-08 02:56:48.000000 ezdsp-0.0.0/src/ezdsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      127 2024-04-08 02:48:56.000000 ezdsp-0.0.0/src/ezdsp/_ezdsp.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 02:57:15.895588 ezdsp-0.0.0/src/ezdsp.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      577 2024-04-08 02:57:15.000000 ezdsp-0.0.0/src/ezdsp.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      232 2024-04-08 02:57:15.000000 ezdsp-0.0.0/src/ezdsp.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 02:57:15.000000 ezdsp-0.0.0/src/ezdsp.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       43 2024-04-08 02:57:15.000000 ezdsp-0.0.0/src/ezdsp.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 02:57:15.000000 ezdsp-0.0.0/src/ezdsp.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.724807 ezdsp-1.0.0/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:45:34.000000 ezdsp-1.0.0/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:20:08.724807 ezdsp-1.0.0/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       59 2024-04-08 02:55:32.000000 ezdsp-1.0.0/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       38 2024-04-08 04:20:08.724807 ezdsp-1.0.0/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1984 2024-04-08 02:58:30.000000 ezdsp-1.0.0/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.721807 ezdsp-1.0.0/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.722807 ezdsp-1.0.0/src/ezdsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 ezdsp-1.0.0/src/ezdsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      615 2024-04-08 04:12:38.000000 ezdsp-1.0.0/src/ezdsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5954 2024-04-08 03:21:19.000000 ezdsp-1.0.0/src/ezdsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1454 2024-04-08 03:58:37.000000 ezdsp-1.0.0/src/ezdsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      334 2024-04-08 03:59:13.000000 ezdsp-1.0.0/src/ezdsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      728 2024-04-08 03:09:04.000000 ezdsp-1.0.0/src/ezdsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2924 2024-04-08 04:01:30.000000 ezdsp-1.0.0/src/ezdsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2837 2024-04-08 04:03:01.000000 ezdsp-1.0.0/src/ezdsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1667 2024-04-08 04:07:09.000000 ezdsp-1.0.0/src/ezdsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1641 2024-04-08 04:07:29.000000 ezdsp-1.0.0/src/ezdsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1656 2024-04-08 04:08:57.000000 ezdsp-1.0.0/src/ezdsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2846 2024-04-08 04:13:52.000000 ezdsp-1.0.0/src/ezdsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2681 2024-04-08 03:17:47.000000 ezdsp-1.0.0/src/ezdsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6157 2024-04-08 03:52:52.000000 ezdsp-1.0.0/src/ezdsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1976 2024-04-08 03:50:23.000000 ezdsp-1.0.0/src/ezdsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.723807 ezdsp-1.0.0/src/ezdsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1002 2024-04-08 04:14:27.000000 ezdsp-1.0.0/src/ezdsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 ezdsp-1.0.0/src/ezdsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5906 2024-04-08 04:19:18.000000 ezdsp-1.0.0/src/ezdsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 ezdsp-1.0.0/src/ezdsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 ezdsp-1.0.0/src/ezdsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5817 2024-04-08 04:09:13.000000 ezdsp-1.0.0/src/ezdsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9593 2024-04-08 03:09:29.000000 ezdsp-1.0.0/src/ezdsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 ezdsp-1.0.0/src/ezdsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5227 2024-04-08 04:18:54.000000 ezdsp-1.0.0/src/ezdsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      515 2024-04-08 04:12:12.000000 ezdsp-1.0.0/src/ezdsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      444 2024-04-08 04:06:39.000000 ezdsp-1.0.0/src/ezdsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1013 2024-04-08 04:09:05.000000 ezdsp-1.0.0/src/ezdsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 04:20:08.723807 ezdsp-1.0.0/src/ezdsp.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      679 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      824 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       67 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        6 2024-04-08 04:20:08.000000 ezdsp-1.0.0/src/ezdsp.egg-info/top_level.txt
```

### Comparing `ezdsp-0.0.0/LICENSE` & `ezdsp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezdsp-0.0.0/setup.py` & `ezdsp-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-08 12:56:09 (ywatanabe)"
+# Time-stamp: "2024-04-08 12:58:29 (ywatanabe)"
 
 import re
 from codecs import open
 from os import path
 
 from setuptools import find_packages, setup
 
 ################################################################################
 PACKAGE_NAME = "ezdsp"
 PACKAGES = find_packages(where="src")
-DESCRIPTION = "A digital signal processing tool box"
+DESCRIPTION = "Easy digital signal processing"
 KEYWORDS = ["numpy" "torch", "pandas", "LFP", "EEG", "MEG"]
 CLASSIFIERS = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 ################################################################################
```

