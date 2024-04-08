# Comparing `tmp/mngs-1.2.2.tar.gz` & `tmp/mngs-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mngs-1.2.2.tar", last modified: Fri Apr  5 06:24:19 2024, max compression
+gzip compressed data, was "mngs-1.2.3.tar", last modified: Mon Apr  8 15:28:46 2024, max compression
```

## Comparing `mngs-1.2.2.tar` & `mngs-1.2.3.tar`

### file list

```diff
@@ -1,215 +1,226 @@
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)    35149 2024-02-03 10:31:02.000000 mngs-1.2.2/LICENSE
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.2/MANIFEST.in
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-05 06:24:19.371817 mngs-1.2.2/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.2/README.md
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-05 06:24:19.375817 mngs-1.2.2/setup.cfg
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.2/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.357818 mngs-1.2.2/src/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.359818 mngs-1.2.2/src/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      482 2024-04-05 06:24:14.000000 mngs-1.2.2/src/mngs/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.360818 mngs-1.2.2/src/mngs/dsp/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.2/src/mngs/dsp/PARAMS.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      365 2024-04-05 01:14:27.000000 mngs-1.2.2/src/mngs/dsp/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5064 2024-04-05 05:01:38.000000 mngs-1.2.2/src/mngs/dsp/_demo_sig.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.2/src/mngs/dsp/_hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.2.2/src/mngs/dsp/_misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.2/src/mngs/dsp/_mne.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.2/src/mngs/dsp/_psd.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1672 2024-04-04 21:38:57.000000 mngs-1.2.2/src/mngs/dsp/_resample.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1749 2024-04-04 02:34:34.000000 mngs-1.2.2/src/mngs/dsp/_transform.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.2/src/mngs/dsp/_wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2755 2024-04-05 03:19:19.000000 mngs-1.2.2/src/mngs/dsp/add_noise.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5938 2024-04-05 06:19:44.000000 mngs-1.2.2/src/mngs/dsp/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1909 2024-04-04 10:07:16.000000 mngs-1.2.2/src/mngs/dsp/filt.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.361817 mngs-1.2.2/src/mngs/dsp/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.2/src/mngs/dsp/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7079 2024-04-05 02:45:12.000000 mngs-1.2.2/src/mngs/dsp/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.2/src/mngs/dsp/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.2/src/mngs/dsp/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.2/src/mngs/dsp/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.2/src/mngs/dsp/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/dsp/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.2/src/mngs/dsp/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.2/src/mngs/dsp/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.2/src/mngs/dsp/nn/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.2.2/src/mngs/dsp/norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.2/src/mngs/dsp/ref.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/general/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1065 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/TimeStamper.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1478 2024-04-04 11:51:21.000000 mngs-1.2.2/src/mngs/general/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.2/src/mngs/general/_close.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8880 2024-04-04 02:22:41.000000 mngs-1.2.2/src/mngs/general/_converters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.2/src/mngs/general/_norm.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/_shell.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.2/src/mngs/general/_start.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/_xml2dict.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/cuda_collect_env.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2144 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/debug.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/email.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/latex.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.2/src/mngs/general/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/mat2py.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.2/src/mngs/general/misc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/pandas.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.2/src/mngs/general/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.2/src/mngs/general/repro.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.2/src/mngs/general/save.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/general/torch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/gists/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/_SigMacro_processFigure_S.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/_SigMacro_toBlue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/gists/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/io/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-02-04 02:18:33.000000 mngs-1.2.2/src/mngs/io/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9820 2024-03-08 21:41:35.000000 mngs-1.2.2/src/mngs/io/load.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.2/src/mngs/io/path.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.2/src/mngs/io/save.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.363818 mngs-1.2.2/src/mngs/linalg/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/linalg/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/linalg/_misc.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/ClassificationReporter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/ClassifierServer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.2/src/mngs/ml/EarlyStopping.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/LearningCurveLogger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/__Classifiers.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.2/src/mngs/ml/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/act/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/act/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/act/_define.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/clustering/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.2/src/mngs/ml/clustering/_UMAP.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.2/src/mngs/ml/clustering/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.2/src/mngs/ml/clustering/_umap.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.364817 mngs-1.2.2/src/mngs/ml/layer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/_Pass.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/layer/_switch.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/loss/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/MultiTaskLoss.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/_L1L2Losses.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/loss/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/metrics/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.2/src/mngs/ml/metrics/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.2/src/mngs/ml/metrics/_bACC.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/__init__.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/optim/_get_set.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.365817 mngs-1.2.2/src/mngs/ml/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.2/src/mngs/ml/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.2/src/mngs/ml/plt/_conf_mat.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.2/src/mngs/ml/plt/_learning_curve.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.2/src/mngs/ml/plt/_optuna_study.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.366817 mngs-1.2.2/src/mngs/ml/plt/aucs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/example.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/pre_rec_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/plt/aucs/roc_auc.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/silhoute_score_block.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.366817 mngs-1.2.2/src/mngs/ml/sk/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.2/src/mngs/ml/sk/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.2/src/mngs/ml/sk/_clf.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.2/src/mngs/ml/sk/_to_sktime.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.367817 mngs-1.2.2/src/mngs/ml/utils/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_DefaultDataset.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.2/src/mngs/ml/utils/_LabelEncoder.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.2/src/mngs/ml/utils/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.2/src/mngs/ml/utils/_check_params.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_format_samples_for_sktime.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.2/src/mngs/ml/utils/_merge_labels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_sliding_window_data_augmentation.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_under_sample.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/ml/utils/_verify_n_gpus.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.367817 mngs-1.2.2/src/mngs/mngs/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/mngs/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/mngs/setup.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.368817 mngs-1.2.2/src/mngs/nn/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.2/src/mngs/nn/_AxiswiseDropout.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_BNet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_BNet_Res.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_ChannelGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_DropoutChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7079 2024-04-05 02:45:12.000000 mngs-1.2.2/src/mngs/nn/_Filters.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_FreqGainChanger.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.2/src/mngs/nn/_GaussianFilter.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-02 12:48:08.000000 mngs-1.2.2/src/mngs/nn/_Hilbert.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_MNet_1000.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.2/src/mngs/nn/_PSD.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_ResNet1D.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_SpatialAttention.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.2/src/mngs/nn/_Spectrogram.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/nn/_SwapChannels.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.2/src/mngs/nn/_TransposeLayer.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.2/src/mngs/nn/_Wavelet.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      838 2024-04-02 13:16:20.000000 mngs-1.2.2/src/mngs/nn/__init__.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.368817 mngs-1.2.2/src/mngs/os/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.2/src/mngs/os/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1342 2024-03-02 10:35:45.000000 mngs-1.2.2/src/mngs/os/_mv.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.369817 mngs-1.2.2/src/mngs/plt/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.2/src/mngs/plt/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_add_hue.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_annotated_heatmap.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-05 06:07:27.000000 mngs-1.2.2/src/mngs/plt/_configure_mpl.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_draw_a_cube.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_get_RGBA_from_colormap.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_mk_colorbar.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/_mk_patches.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9875 2024-02-04 02:05:41.000000 mngs-1.2.2/src/mngs/plt/_subplots.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.2/src/mngs/plt/_tpl.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.369817 mngs-1.2.2/src/mngs/plt/ax/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      436 2024-03-07 12:38:36.000000 mngs-1.2.2/src/mngs/plt/ax/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_circular_hist.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_extend.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_fill_between.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.2/src/mngs/plt/ax/_hide_spines.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_map_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_panel.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_sci_note.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      389 2024-04-05 02:48:46.000000 mngs-1.2.2/src/mngs/plt/ax/_set_n_ticks.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.2/src/mngs/plt/ax/_set_pos.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/ax/_set_size.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/colors.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/plt/get_mpl_color.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.370817 mngs-1.2.2/src/mngs/resource/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/get.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/resource/limit_RAM.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.370817 mngs-1.2.2/src/mngs/stats/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.2/src/mngs/stats/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_bonferroni_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_brunner_munzel_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_calc_partial_corr.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_corr_test.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_fdr_correction.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.2/src/mngs/stats/_general.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_multicompair.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_nocorrelation_test.py
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_smirnov_grubbs.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.2/src/mngs/stats/_to_asterisks.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/src/mngs/torch/
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.2/src/mngs/torch/__init__.py
--rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.2/src/mngs/torch/_apply_to.py
-drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-05 06:24:19.371817 mngs-1.2.2/src/mngs.egg-info/
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1793 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/PKG-INFO
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5535 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/SOURCES.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/dependency_links.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      375 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/requires.txt
--rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-05 06:24:19.000000 mngs-1.2.2/src/mngs.egg-info/top_level.txt
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1084 2024-04-08 02:30:42.000000 mngs-1.2.3/LICENSE
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       64 2024-02-03 10:31:02.000000 mngs-1.2.3/MANIFEST.in
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1887 2024-04-08 15:28:46.887353 mngs-1.2.3/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      295 2024-02-03 10:31:02.000000 mngs-1.2.3/README.md
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      152 2024-04-08 15:28:46.887353 mngs-1.2.3/setup.cfg
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.3/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.859353 mngs-1.2.3/src/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.860353 mngs-1.2.3/src/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      586 2024-04-08 02:29:53.000000 mngs-1.2.3/src/mngs/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.862353 mngs-1.2.3/src/mngs/dsp/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      742 2024-04-04 08:25:32.000000 mngs-1.2.3/src/mngs/dsp/PARAMS.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      435 2024-04-08 01:51:33.000000 mngs-1.2.3/src/mngs/dsp/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6008 2024-04-08 00:35:43.000000 mngs-1.2.3/src/mngs/dsp/_demo_sig.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1455 2024-04-03 21:02:11.000000 mngs-1.2.3/src/mngs/dsp/_hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      539 2024-04-05 01:14:09.000000 mngs-1.2.3/src/mngs/dsp/_misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      731 2024-04-04 08:34:47.000000 mngs-1.2.3/src/mngs/dsp/_mne.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3483 2024-04-07 23:40:24.000000 mngs-1.2.3/src/mngs/dsp/_modulation_index.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5874 2024-04-08 02:24:40.000000 mngs-1.2.3/src/mngs/dsp/_pac.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1710 2024-04-04 08:07:31.000000 mngs-1.2.3/src/mngs/dsp/_psd.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1672 2024-04-04 21:38:57.000000 mngs-1.2.3/src/mngs/dsp/_resample.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1663 2024-04-08 02:41:59.000000 mngs-1.2.3/src/mngs/dsp/_transform.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2848 2024-04-03 20:26:59.000000 mngs-1.2.3/src/mngs/dsp/_wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2755 2024-04-05 03:19:19.000000 mngs-1.2.3/src/mngs/dsp/add_noise.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6150 2024-04-05 14:36:19.000000 mngs-1.2.3/src/mngs/dsp/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1909 2024-04-04 10:07:16.000000 mngs-1.2.3/src/mngs/dsp/filt.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.862353 mngs-1.2.3/src/mngs/dsp/fx/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       95 2024-04-05 06:28:18.000000 mngs-1.2.3/src/mngs/dsp/fx/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.863353 mngs-1.2.3/src/mngs/dsp/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.3/src/mngs/dsp/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7199 2024-04-07 17:06:51.000000 mngs-1.2.3/src/mngs/dsp/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.3/src/mngs/dsp/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 mngs-1.2.3/src/mngs/dsp/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-08 00:30:03.000000 mngs-1.2.3/src/mngs/dsp/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9591 2024-04-08 02:28:29.000000 mngs-1.2.3/src/mngs/dsp/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.2.3/src/mngs/dsp/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.3/src/mngs/dsp/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.3/src/mngs/dsp/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/dsp/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.3/src/mngs/dsp/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.3/src/mngs/dsp/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      962 2024-04-08 01:51:20.000000 mngs-1.2.3/src/mngs/dsp/nn/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      471 2024-04-05 01:15:43.000000 mngs-1.2.3/src/mngs/dsp/norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      974 2024-04-04 08:39:58.000000 mngs-1.2.3/src/mngs/dsp/ref.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.867353 mngs-1.2.3/src/mngs/general/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2042 2024-04-07 09:12:16.000000 mngs-1.2.3/src/mngs/general/_TimeStamper.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1520 2024-04-07 09:17:14.000000 mngs-1.2.3/src/mngs/general/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2146 2024-03-11 03:28:22.000000 mngs-1.2.3/src/mngs/general/_close.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     8718 2024-04-07 10:54:07.000000 mngs-1.2.3/src/mngs/general/_converters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15227 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_cuda_collect_env.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1582 2024-04-02 10:34:34.000000 mngs-1.2.3/src/mngs/general/_norm.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2061 2024-04-07 09:16:08.000000 mngs-1.2.3/src/mngs/general/_reload.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1317 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_shell.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3822 2024-03-25 01:12:15.000000 mngs-1.2.3/src/mngs/general/_start.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2882 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/_xml2dict.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5213 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/email.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      502 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/latex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9812 2024-04-05 21:59:08.000000 mngs-1.2.3/src/mngs/general/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2181 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/mat2py.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    22093 2024-04-01 10:51:59.000000 mngs-1.2.3/src/mngs/general/misc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5068 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/pandas.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.3/src/mngs/general/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3941 2024-02-17 20:51:51.000000 mngs-1.2.3/src/mngs/general/repro.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.3/src/mngs/general/save.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/general/torch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.867353 mngs-1.2.3/src/mngs/gists/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4678 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/_SigMacro_processFigure_S.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5297 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/_SigMacro_toBlue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      206 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/gists/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.868353 mngs-1.2.3/src/mngs/io/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-05 14:24:05.000000 mngs-1.2.3/src/mngs/io/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9812 2024-04-05 21:59:08.000000 mngs-1.2.3/src/mngs/io/load.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5671 2024-02-04 20:26:57.000000 mngs-1.2.3/src/mngs/io/path.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9974 2024-03-29 21:17:52.000000 mngs-1.2.3/src/mngs/io/save.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.868353 mngs-1.2.3/src/mngs/linalg/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      175 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/linalg/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1574 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/linalg/_misc.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.869353 mngs-1.2.3/src/mngs/ml/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    23162 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/ClassificationReporter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3454 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/ClassifierServer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4927 2024-03-25 03:52:32.000000 mngs-1.2.3/src/mngs/ml/EarlyStopping.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    15503 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/LearningCurveLogger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3447 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/__Classifiers.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      447 2024-03-04 09:20:04.000000 mngs-1.2.3/src/mngs/ml/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.870353 mngs-1.2.3/src/mngs/ml/act/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      124 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/act/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      220 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/act/_define.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.870353 mngs-1.2.3/src/mngs/ml/clustering/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2494 2024-02-11 11:10:10.000000 mngs-1.2.3/src/mngs/ml/clustering/_UMAP.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-03-02 12:20:15.000000 mngs-1.2.3/src/mngs/ml/clustering/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    13347 2024-03-02 15:12:27.000000 mngs-1.2.3/src/mngs/ml/clustering/_umap.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.871353 mngs-1.2.3/src/mngs/ml/layer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      141 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/_Pass.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       52 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      122 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/layer/_switch.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/loss/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1387 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/MultiTaskLoss.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      623 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/_L1L2Losses.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/loss/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/metrics/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      120 2024-02-26 05:15:47.000000 mngs-1.2.3/src/mngs/ml/metrics/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1110 2024-02-26 05:32:45.000000 mngs-1.2.3/src/mngs/ml/metrics/_bACC.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/optim/
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.872353 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.874353 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)       91 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     7915 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     9051 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     8568 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     6934 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      696 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/__init__.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      713 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/optim/_get_set.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.874353 mngs-1.2.3/src/mngs/ml/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      216 2024-03-08 21:27:15.000000 mngs-1.2.3/src/mngs/ml/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7774 2024-03-12 08:52:13.000000 mngs-1.2.3/src/mngs/ml/plt/_conf_mat.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6373 2024-03-12 08:52:52.000000 mngs-1.2.3/src/mngs/ml/plt/_learning_curve.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4234 2024-03-29 21:24:56.000000 mngs-1.2.3/src/mngs/ml/plt/_optuna_study.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.875353 mngs-1.2.3/src/mngs/ml/plt/aucs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       71 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1625 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/example.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7322 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/pre_rec_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7403 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/plt/aucs/roc_auc.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    17121 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/silhoute_score_block.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.876353 mngs-1.2.3/src/mngs/ml/sk/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      153 2024-03-05 02:17:18.000000 mngs-1.2.3/src/mngs/ml/sk/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1988 2024-03-23 06:36:06.000000 mngs-1.2.3/src/mngs/ml/sk/_clf.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3049 2024-03-05 02:17:08.000000 mngs-1.2.3/src/mngs/ml/sk/_to_sktime.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.877353 mngs-1.2.3/src/mngs/ml/utils/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1295 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_DefaultDataset.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4073 2024-03-01 22:52:34.000000 mngs-1.2.3/src/mngs/ml/utils/_LabelEncoder.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      392 2024-03-01 02:42:25.000000 mngs-1.2.3/src/mngs/ml/utils/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1450 2024-02-17 01:38:41.000000 mngs-1.2.3/src/mngs/ml/utils/_check_params.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      596 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_format_samples_for_sktime.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      629 2024-02-08 00:22:23.000000 mngs-1.2.3/src/mngs/ml/utils/_merge_labels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      294 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_sliding_window_data_augmentation.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1197 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_under_sample.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      437 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/ml/utils/_verify_n_gpus.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.878352 mngs-1.2.3/src/mngs/mngs/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       23 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/mngs/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2451 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/mngs/setup.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.879353 mngs-1.2.3/src/mngs/nn/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      812 2024-03-29 20:27:28.000000 mngs-1.2.3/src/mngs/nn/_AxiswiseDropout.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3448 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_BNet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_BNet_Res.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      998 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_ChannelGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1359 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_DropoutChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     7199 2024-04-07 17:06:51.000000 mngs-1.2.3/src/mngs/nn/_Filters.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3050 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_FreqGainChanger.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1326 2024-04-01 07:14:45.000000 mngs-1.2.3/src/mngs/nn/_GaussianFilter.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2616 2024-04-05 06:51:21.000000 mngs-1.2.3/src/mngs/nn/_Hilbert.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3914 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_MNet_1000.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-08 00:30:03.000000 mngs-1.2.3/src/mngs/nn/_ModulationIndex.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9591 2024-04-08 02:28:29.000000 mngs-1.2.3/src/mngs/nn/_PAC.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3271 2024-04-08 00:40:20.000000 mngs-1.2.3/src/mngs/nn/_PAC_working.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1151 2024-04-04 08:03:08.000000 mngs-1.2.3/src/mngs/nn/_PSD.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3138 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_ResNet1D.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      640 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_SpatialAttention.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4821 2024-04-01 22:21:12.000000 mngs-1.2.3/src/mngs/nn/_Spectrogram.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1245 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/nn/_SwapChannels.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      381 2024-03-29 20:26:35.000000 mngs-1.2.3/src/mngs/nn/_TransposeLayer.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     9524 2024-04-05 01:09:23.000000 mngs-1.2.3/src/mngs/nn/_Wavelet.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      962 2024-04-08 01:51:20.000000 mngs-1.2.3/src/mngs/nn/__init__.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.879353 mngs-1.2.3/src/mngs/os/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      116 2024-02-29 23:25:42.000000 mngs-1.2.3/src/mngs/os/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1379 2024-04-05 22:00:45.000000 mngs-1.2.3/src/mngs/os/_mv.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.881353 mngs-1.2.3/src/mngs/plt/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      417 2024-03-31 00:58:18.000000 mngs-1.2.3/src/mngs/plt/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      822 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_add_hue.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1308 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_annotated_heatmap.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     5827 2024-04-05 06:07:27.000000 mngs-1.2.3/src/mngs/plt/_configure_mpl.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      560 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_draw_a_cube.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      795 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_get_RGBA_from_colormap.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      607 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_mk_colorbar.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/_mk_patches.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)    14273 2024-04-08 14:14:38.000000 mngs-1.2.3/src/mngs/plt/_subplots.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      653 2024-03-31 00:58:28.000000 mngs-1.2.3/src/mngs/plt/_tpl.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.883353 mngs-1.2.3/src/mngs/plt/ax/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:34:39.000000 mngs-1.2.3/src/mngs/plt/ax/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2981 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_circular_hist.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     3502 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_extend.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      269 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_fill_between.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      538 2024-03-07 12:44:29.000000 mngs-1.2.3/src/mngs/plt/ax/_hide_spines.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     4420 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_map_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1343 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_panel.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1704 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_sci_note.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      470 2024-04-07 04:15:04.000000 mngs-1.2.3/src/mngs/plt/ax/_set_n_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2582 2024-02-16 10:52:35.000000 mngs-1.2.3/src/mngs/plt/ax/_set_pos.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      449 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/ax/_set_size.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      401 2024-04-07 04:39:32.000000 mngs-1.2.3/src/mngs/plt/ax/_set_ticks.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2364 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/colors.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1004 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/plt/get_mpl_color.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.884353 mngs-1.2.3/src/mngs/resource/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)       93 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     4702 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/get.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      745 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/resource/limit_RAM.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.886352 mngs-1.2.3/src/mngs/stats/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      533 2024-03-30 07:10:35.000000 mngs-1.2.3/src/mngs/stats/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2056 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_bonferroni_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2002 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_brunner_munzel_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      495 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_calc_partial_corr.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1394 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_corr_test.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     6941 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_fdr_correction.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     2237 2024-03-30 07:17:46.000000 mngs-1.2.3/src/mngs/stats/_general.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)     1153 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_multicompair.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      814 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_nocorrelation_test.py
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     2604 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_smirnov_grubbs.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      272 2024-02-03 10:31:02.000000 mngs-1.2.3/src/mngs/stats/_to_asterisks.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/src/mngs/torch/
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      128 2024-03-30 21:24:51.000000 mngs-1.2.3/src/mngs/torch/__init__.py
+-rwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)      905 2024-03-30 21:11:45.000000 mngs-1.2.3/src/mngs/torch/_apply_to.py
+drwxr-xr-x   0 ywatanabe  (1000) ywatanabe  (1000)        0 2024-04-08 15:28:46.887353 mngs-1.2.3/src/mngs.egg-info/
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     1887 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/PKG-INFO
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)     5824 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/SOURCES.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        1 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/dependency_links.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)      412 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/requires.txt
+-rw-r--r--   0 ywatanabe  (1000) ywatanabe  (1000)        5 2024-04-08 15:28:46.000000 mngs-1.2.3/src/mngs.egg-info/top_level.txt
```

### Comparing `mngs-1.2.2/PKG-INFO` & `mngs-1.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.2.2
+Version: 1.2.3
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
-License: GPL3.0
+License: MIT
 Keywords: utils,utilities,python,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython
@@ -50,14 +50,18 @@
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
 Requires-Dist: umap-learn
 Requires-Dist: wheel
 Requires-Dist: xmltodict
 Requires-Dist: sktime
+Requires-Dist: tensorpac
+Requires-Dist: ipython==8.0.0
+Requires-Dist: ipdb
+Requires-Dist: plotly
 
 ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
 
 ## Installation
 ``` bash
 $ pip install mngs
 ```
```

### Comparing `mngs-1.2.2/setup.py` & `mngs-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/PARAMS.py` & `mngs-1.2.3/src/mngs/dsp/PARAMS.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_demo_sig.py` & `mngs-1.2.3/src/mngs/dsp/_demo_sig.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,54 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 16:01:37 (ywatanabe)"
+# Time-stamp: "2024-04-08 11:35:43 (ywatanabe)"
 
 import random
 import warnings
 
 import mne
+import mngs
 import numpy as np
 from mne import Epochs, compute_covariance, find_events, make_ad_hoc_cov
 from mne.datasets import sample
 from mne.simulation import (
     add_ecg,
     add_eog,
     add_noise,
     simulate_raw,
     simulate_sparse_stc,
 )
 from ripple_detection.simulate import simulate_LFP, simulate_time
 from scipy.signal import chirp
+from tensorpac.signals import pac_signals_wavelet
+
+
+def _demo_sig_tensorpac(
+    batch_size=8,
+    n_chs=19,
+    t_sec=4,
+    fs=512,
+    f_pha=10,
+    f_amp=100,
+    noise=0.8,
+    n_segments=20,
+    verbose=False,
+):
+    n_times = int(t_sec * fs)
+    x_2d, tt = pac_signals_wavelet(
+        sf=fs,
+        f_pha=f_pha,
+        f_amp=f_amp,
+        noise=noise,
+        n_epochs=n_segments,
+        n_times=n_times,
+    )
+    x_3d = np.stack([x_2d for _ in range(batch_size)], axis=0)
+    x_4d = np.stack([x_3d for _ in range(n_chs)], axis=1)
+    return x_4d, tt
 
 
 def demo_sig(
     batch_size=8,
     n_chs=19,
     t_sec=4,
     fs=512,
@@ -33,27 +60,28 @@
     assert sig_type in [
         "uniform",
         "gauss",
         "periodic",
         "chirp",
         "ripple",
         "meg",
+        "tensorpac",
     ]
     tt = np.linspace(0, t_sec, int(t_sec * fs), endpoint=False)
 
     if sig_type == "uniform":
         return (
             np.random.uniform(
                 low=-0.5, high=0.5, size=(batch_size, n_chs, len(tt))
             ),
             tt,
             fs,
         )
 
-    if sig_type == "gauss":
+    elif sig_type == "gauss":
         return np.random.randn(batch_size, n_chs, len(tt)), tt, fs
 
     elif sig_type == "meg":
         return (
             _demo_sig_meg(
                 batch_size=batch_size,
                 n_chs=n_chs,
@@ -61,14 +89,23 @@
                 fs=fs,
                 verbose=verbose,
             ).astype(np.float32)[..., : len(tt)],
             tt,
             fs,
         )
 
+    elif sig_type == "tensorpac":
+        xx, tt = _demo_sig_tensorpac(
+            batch_size=batch_size,
+            n_chs=n_chs,
+            t_sec=t_sec,
+            fs=fs,
+        )
+        return xx.astype(np.float32)[..., : len(tt)], tt, fs
+
     else:
         fn_1d = {
             "periodic": _demo_sig_periodic_1d,
             "chirp": _demo_sig_chirp_1d,
             "ripple": _demo_sig_ripple_1d,
         }.get(sig_type)
 
@@ -167,19 +204,21 @@
 if __name__ == "__main__":
     uu, tt, fs = demo_sig(sig_type="uniform")
     gg, tt, fs = demo_sig(sig_type="gauss")
     mm, tt, fs = demo_sig(sig_type="meg")
     pp, tt, fs = demo_sig(sig_type="periodic")
     cc, tt, fs = demo_sig(sig_type="chirp")
     rr, tt, fs = demo_sig(sig_type="ripple")
+    tp, tt, fs = demo_sig(sig_type="tensorpac")
 
-    fig, axes = mngs.plt.subplots(nrows=6)
+    fig, axes = mngs.plt.subplots(nrows=7)
     axes[0].plot(uu[0, 0], label="uniform")
     axes[1].plot(gg[0, 0], label="gauss")
     axes[2].plot(mm[0, 0], label="meg")
     axes[3].plot(pp[0, 0], label="periodic")
     axes[4].plot(cc[0, 0], label="chirp")
     axes[5].plot(rr[0, 0], label="ripple")
+    axes[6].plot(tp[0, 0, 0], label="tensorpac")
     for ax in axes:
         ax.legend(loc="upper right")
 
     plt.show()
```

### Comparing `mngs-1.2.2/src/mngs/dsp/_hilbert.py` & `mngs-1.2.3/src/mngs/dsp/_hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_misc.py` & `mngs-1.2.3/src/mngs/dsp/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_mne.py` & `mngs-1.2.3/src/mngs/dsp/_mne.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_psd.py` & `mngs-1.2.3/src/mngs/dsp/_psd.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_resample.py` & `mngs-1.2.3/src/mngs/dsp/_resample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/_transform.py` & `mngs-1.2.3/src/mngs/dsp/_transform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 13:34:33 (ywatanabe)"#!/usr/bin/env python3
+# Time-stamp: "2024-04-08 12:41:59 (ywatanabe)"#!/usr/bin/env python3
 
 
 import warnings
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import skimage
 import torch
 from mngs.general import torch_fn
-from obspy.signal.tf_misfit import cwt
 
 
 def to_sktime_df(arr):
     """
     Convert a 3D numpy array into a DataFrame suitable for sktime.
 
     Parameters:
```

### Comparing `mngs-1.2.2/src/mngs/dsp/_wavelet.py` & `mngs-1.2.3/src/mngs/dsp/_wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/add_noise.py` & `mngs-1.2.3/src/mngs/dsp/add_noise.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/example.py` & `mngs-1.2.3/src/mngs/dsp/example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 17:19:43 (ywatanabe)"
+# Time-stamp: "2024-04-06 01:36:18 (ywatanabe)"
 
 import matplotlib
 
-# try:
-#     import mngs
-# except ImportError:
-#     !pip uninstall mngs -y
-#     !pip install -U git+https://github.com/ywatanabe1989/mngs.git@develop
-# finally:
-#     import mngs
-import mngs
-
 matplotlib.use("Agg")
 import matplotlib.pyplot as plt
 import pandas as pd
 
 
 # Functions
 def calc_norm_resample_filt_hilbert(xx, tt, fs, sig_type, verbose=True):
     sigs = {"index": ("signal", "time", "fs")}  # Collector
+
+    if sig_type == "tensorpac":
+        xx = xx[:, :, 0]
+
     sigs[f"orig"] = (xx, tt, fs)
 
     # Normalization
     sigs["z_normed"] = (mngs.dsp.norm.z(xx), tt, fs)
     sigs["minmax_normed"] = (mngs.dsp.norm.minmax(xx), tt, fs)
 
     # Resampling
@@ -86,14 +81,17 @@
                 _tt,
                 _fs,
             ) = sigs[_col]
             ax.plot(_tt, _xx[i_batch, i_ch], label=_col, c=CC["blue"])
 
         # Main
         xx, tt, fs = sigs[col]
+        # if sig_type == "tensorpac":
+        #     xx = xx[:, :, 0]
+
         try:
             ax.plot(
                 tt,
                 xx[i_batch, i_ch],
                 label=col,
                 c=CC["red"] if col == "hilbert_amp" else CC["blue"],
             )
@@ -114,14 +112,16 @@
     fig.suptitle(sig_type)
     return fig
 
 
 def plot_wavelet(plt, sigs, sig_col, sig_type):
 
     xx, tt, fs = sigs[sig_col]
+    # if sig_type == "tensorpac":
+    #     xx = xx[:, :, 0]
 
     # Wavelet Transformation
     wavelet_coef, ff_ww = mngs.dsp.wavelet(xx, fs)
 
     i_batch = 0
     i_ch = 0
 
@@ -158,14 +158,17 @@
     return fig
 
 
 def plot_psd(plt, sigs, sig_col, sig_type):
 
     xx, tt, fs = sigs[sig_col]
 
+    # if sig_type == "tensorpac":
+    #     xx = xx[:, :, 0]
+
     # Power Spetrum Density
     psd, ff_pp = mngs.dsp.psd(xx, fs)
 
     # Main
     i_batch = 0
     i_ch = 0
     fig, axes = plt.subplots(nrows=2, sharex=False)
@@ -192,49 +195,60 @@
 
     fig.suptitle(sig_type)
 
     return fig
 
 
 if __name__ == "__main__":
+    import mngs
+
     # Parameters
     T_SEC = 4
-    SIG_TYPES = ["uniform", "gauss", "periodic", "chirp", "ripple", "meg"]
+    SIG_TYPES = [
+        # "uniform",
+        # "gauss",
+        # "periodic",
+        # "chirp",
+        # "ripple",
+        # "meg",
+        "tensorpac",
+    ]
     SRC_FS = 1024
     TGT_FS = 512
     FREQS_HZ = [10, 30, 100]
     LOW_HZ = 20
     HIGH_HZ = 50
     SIGMA = 10
 
     plt, CC = mngs.plt.configure_mpl(plt, fig_scale=10)
+    sdir = "/home/ywatanabe/proj/entrance/mngs/dsp/example/"
 
     for sig_type in SIG_TYPES:
         # Demo Signal
         xx, tt, fs = mngs.dsp.demo_sig(
             t_sec=T_SEC, fs=SRC_FS, freqs_hz=FREQS_HZ, sig_type=sig_type
         )
 
         # Apply calculations on the original signal
         sigs = calc_norm_resample_filt_hilbert(xx, tt, fs, sig_type)
 
         # Plots signals
         fig = plot_signals(plt, sigs, sig_type)
-        mngs.io.save(fig, f"{sig_type}_1_signals.png")
+        mngs.io.save(fig, sdir + f"{sig_type}/1_signals.png")
 
         # Plots wavelet coefficients and PSD
         for sig_col in sigs.columns:
 
             if "hilbert" in sig_col:
                 continue
 
             fig = plot_wavelet(plt, sigs, sig_col, sig_type)
-            mngs.io.save(fig, f"{sig_type}_2_wavelet_{sig_col}.png")
+            mngs.io.save(fig, sdir + f"{sig_type}/2_wavelet_{sig_col}.png")
 
             fig = plot_psd(plt, sigs, sig_col, sig_type)
-            mngs.io.save(fig, f"{sig_type}_3_psd_{sig_col}.png")
+            mngs.io.save(fig, sdir + f"{sig_type}/3_psd_{sig_col}.png")
 
     # plt.show()
 
     """
-    python /home/ywatanabe/proj/entrance/mngs/dsp/example.py
+    python ./dsp/example.py
     """
```

### Comparing `mngs-1.2.2/src/mngs/dsp/filt.py` & `mngs-1.2.3/src/mngs/dsp/filt.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_AxiswiseDropout.py` & `mngs-1.2.3/src/mngs/dsp/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_BNet.py` & `mngs-1.2.3/src/mngs/dsp/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_BNet_Res.py` & `mngs-1.2.3/src/mngs/dsp/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_ChannelGainChanger.py` & `mngs-1.2.3/src/mngs/dsp/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_DropoutChannels.py` & `mngs-1.2.3/src/mngs/dsp/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_Filters.py` & `mngs-1.2.3/src/mngs/dsp/nn/_Filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 13:45:11 (ywatanabe)"
+# Time-stamp: "2024-04-08 04:06:50 (ywatanabe)"
 
 import math
 import warnings
 
 import mngs
 import numpy as np
-import pywt
 import seaborn as sns
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mngs.general import torch_fn
 
 
@@ -62,18 +61,20 @@
 
         x_filted_extended = F.conv1d(
             extended_x, kernel, padding=0, groups=channels
         )[..., :seq_len]
 
         assert x.shape == x_filted_extended.shape
 
-        # Remove edges
-        x_filted_extended[..., : self.radius] *= 0
-        x_filted_extended[..., -self.radius :] *= 0
+        # # Remove edges
+        # x_filted_extended[..., : self.radius] *= 0
+        # x_filted_extended[..., -self.radius :] *= 0
 
+        nn_remove = x_filted_extended.shape[-1] // 4
+        x_filted_extended = x_filted_extended[..., nn_remove:-nn_remove]
         return x_filted_extended
 
 
 class GaussianFilter(BaseFilter1D):
     def __init__(self, sigma):
         super().__init__()
         self.sigma = mngs.gen.to_even(sigma)
```

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_FreqGainChanger.py` & `mngs-1.2.3/src/mngs/dsp/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_GaussianFilter.py` & `mngs-1.2.3/src/mngs/dsp/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_Hilbert.py` & `mngs-1.2.3/src/mngs/dsp/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_MNet_1000.py` & `mngs-1.2.3/src/mngs/dsp/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_PSD.py` & `mngs-1.2.3/src/mngs/dsp/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_ResNet1D.py` & `mngs-1.2.3/src/mngs/dsp/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_SpatialAttention.py` & `mngs-1.2.3/src/mngs/dsp/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_Spectrogram.py` & `mngs-1.2.3/src/mngs/dsp/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_SwapChannels.py` & `mngs-1.2.3/src/mngs/dsp/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/_Wavelet.py` & `mngs-1.2.3/src/mngs/dsp/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/dsp/nn/__init__.py` & `mngs-1.2.3/src/mngs/dsp/nn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-03 00:16:20 (ywatanabe)"
+# Time-stamp: "2024-04-08 12:51:19 (ywatanabe)"
 
 from ._AxiswiseDropout import AxiswiseDropout
 
 # from ._BandPassFilter import BandPassFilter
 from ._BNet import BNet, BNet_config
 from ._ChannelGainChanger import ChannelGainChanger
 from ._DropoutChannels import DropoutChannels
 
 # from ._GaussianFilter import GaussianFilter
-from ._Filters import BandPassFilter, BandStopFilter, GaussianFilter
+from ._Filters import (
+    BandPassFilter,
+    BandStopFilter,
+    GaussianFilter,
+    HighPassFilter,
+    LowPassFilter,
+)
 from ._FreqGainChanger import FreqGainChanger
 from ._Hilbert import Hilbert
 
 # from ._FreqDropout import FreqDropout
 from ._MNet_1000 import MNet_1000, MNet_config
+from ._ModulationIndex import ModulationIndex
+from ._PAC import PAC
 from ._PSD import PSD
 from ._ResNet1D import ResNet1D, ResNetBasicBlock
 from ._SpatialAttention import SpatialAttention
 from ._SwapChannels import SwapChannels
 from ._TransposeLayer import TransposeLayer
 from ._Wavelet import Wavelet
```

### Comparing `mngs-1.2.2/src/mngs/dsp/ref.py` & `mngs-1.2.3/src/mngs/dsp/ref.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/__init__.py` & `mngs-1.2.3/src/mngs/general/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #!/usr/bin/env python3
 
 # from .path import find_the_git_root_dir, get_this_fpath, mk_spath, split_fpath
 # from .load import get_data_path_from_a_package, load
 # from .save import is_listed_X, save, save_listed_dfs_as_csv, save_listed_scalars_as_csv
+# from .debug import *
 from ..io.__init__ import *
 from ._close import close
 from ._converters import (
     numpy_fn,
     squeeze_if,
     to_numpy,
     to_torch,
     torch_fn,
     unsqueeze_if,
 )
+from ._cuda_collect_env import main as cuda_collect_env
 from ._norm import to_z
+from ._reload import reload
 from ._shell import run_shellcommand, run_shellscript
 from ._start import start
-from .cuda_collect_env import main as cuda_collect_env
-from .debug import *
+from ._TimeStamper import TimeStamper
 from .email import notify, send_gmail
 from .latex import add_hat_in_the_latex_style, to_the_latex_style
 from .mat2py import *
 from .misc import (
     _return_counting_process,
     color_text,
     connect_nums,
@@ -59,9 +61,8 @@
     col_to_last,
     col_to_top,
     force_dataframe,
     ignore_SettingWithCopyWarning,
     merge_columns,
 )
 from .repro import *
-from .TimeStamper import *
 from .torch import *
```

### Comparing `mngs-1.2.2/src/mngs/general/_close.py` & `mngs-1.2.3/src/mngs/general/_close.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/_converters.py` & `mngs-1.2.3/src/mngs/general/_converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-04 13:22:40 (ywatanabe)"#!/usr/bin/env python3
+# Time-stamp: "2024-04-07 21:54:06 (ywatanabe)"#!/usr/bin/env python3
 
 import warnings
 from functools import wraps
 
 import numpy as np
 import pandas as pd
 import torch
@@ -210,19 +210,16 @@
         # Runs the func
         c_args, c_kwargs = to_numpy(*args, return_fn=return_always, **kwargs)
         results = func(*c_args, **c_kwargs)
 
         # Reverts to the original data type
         if not is_torch_input:
             return results
-        elif is_torch_input:
-            if not is_cuda_input:
-                return to_torch(results, return_fn=return_if, device=device)[0]
-            elif is_cuda_input:
-                return to_torch(results, return_fn=return_if, device=device)[0]
+        else:
+            return to_torch(results, return_fn=return_if, device=device)[0][0]
 
     return wrapper
 
 
 if __name__ == "__main__":
     import scipy
     import torch.nn.functional as F
```

### Comparing `mngs-1.2.2/src/mngs/general/_norm.py` & `mngs-1.2.3/src/mngs/general/_norm.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/_shell.py` & `mngs-1.2.3/src/mngs/general/_shell.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/_start.py` & `mngs-1.2.3/src/mngs/general/_start.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/_xml2dict.py` & `mngs-1.2.3/src/mngs/general/_xml2dict.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/cuda_collect_env.py` & `mngs-1.2.3/src/mngs/general/_cuda_collect_env.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/email.py` & `mngs-1.2.3/src/mngs/general/email.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/load.py` & `mngs-1.2.3/src/mngs/general/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 import json
-import logging
 import os
 import pickle
 import warnings
 from glob import glob
 
 import h5py
-import joblib  # [REVISED]
+import joblib
 import mne
 import mngs
 import numpy as np
 import pandas as pd
 import torch
 import yaml
 
@@ -23,14 +22,16 @@
             '\n"mngs.general.load" will be removed. '
             'Please use "mngs.io.load" instead.',
             PendingDeprecationWarning,
         )
 
 
 def load(lpath, show=False, **kwargs):
+    import logging
+
     try:
         extension = "." + lpath.split(".")[-1]  # [REVISED]
 
         # csv
         if extension == ".csv":
             obj = pd.read_csv(lpath, **kwargs)
             obj = obj.loc[
```

### Comparing `mngs-1.2.2/src/mngs/general/mat2py.py` & `mngs-1.2.3/src/mngs/general/mat2py.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/misc.py` & `mngs-1.2.3/src/mngs/general/misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/pandas.py` & `mngs-1.2.3/src/mngs/general/pandas.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/path.py` & `mngs-1.2.3/src/mngs/general/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/repro.py` & `mngs-1.2.3/src/mngs/general/repro.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/save.py` & `mngs-1.2.3/src/mngs/general/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/general/torch.py` & `mngs-1.2.3/src/mngs/general/torch.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/gists/_SigMacro_processFigure_S.py` & `mngs-1.2.3/src/mngs/gists/_SigMacro_processFigure_S.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/gists/_SigMacro_toBlue.py` & `mngs-1.2.3/src/mngs/gists/_SigMacro_toBlue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/io/load.py` & `mngs-1.2.3/src/mngs/io/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 import json
-import logging
 import os
 import pickle
 import warnings
 from glob import glob
 
 import h5py
-import joblib  # [REVISED]
+import joblib
 import mne
 import mngs
 import numpy as np
 import pandas as pd
 import torch
 import yaml
 
@@ -23,14 +22,16 @@
             '\n"mngs.general.load" will be removed. '
             'Please use "mngs.io.load" instead.',
             PendingDeprecationWarning,
         )
 
 
 def load(lpath, show=False, **kwargs):
+    import logging
+
     try:
         extension = "." + lpath.split(".")[-1]  # [REVISED]
 
         # csv
         if extension == ".csv":
             obj = pd.read_csv(lpath, **kwargs)
             obj = obj.loc[
```

### Comparing `mngs-1.2.2/src/mngs/io/path.py` & `mngs-1.2.3/src/mngs/io/path.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/io/save.py` & `mngs-1.2.3/src/mngs/io/save.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/linalg/_misc.py` & `mngs-1.2.3/src/mngs/linalg/_misc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/ClassificationReporter.py` & `mngs-1.2.3/src/mngs/ml/ClassificationReporter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/ClassifierServer.py` & `mngs-1.2.3/src/mngs/ml/ClassifierServer.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/EarlyStopping.py` & `mngs-1.2.3/src/mngs/ml/EarlyStopping.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/LearningCurveLogger.py` & `mngs-1.2.3/src/mngs/ml/LearningCurveLogger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/__Classifiers.py` & `mngs-1.2.3/src/mngs/ml/__Classifiers.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/clustering/_UMAP.py` & `mngs-1.2.3/src/mngs/ml/clustering/_UMAP.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/clustering/_umap.py` & `mngs-1.2.3/src/mngs/ml/clustering/_umap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/loss/MultiTaskLoss.py` & `mngs-1.2.3/src/mngs/ml/loss/MultiTaskLoss.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/loss/_L1L2Losses.py` & `mngs-1.2.3/src/mngs/ml/loss/_L1L2Losses.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/metrics/_bACC.py` & `mngs-1.2.3/src/mngs/ml/metrics/_bACC.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py` & `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py` & `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger2020.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py` & `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/ranger913A.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py` & `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/ranger/rangerqh.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py` & `mngs-1.2.3/src/mngs/ml/optim/Ranger_Deep_Learning_Optimizer/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/optim/_get_set.py` & `mngs-1.2.3/src/mngs/ml/optim/_get_set.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/_conf_mat.py` & `mngs-1.2.3/src/mngs/ml/plt/_conf_mat.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/_learning_curve.py` & `mngs-1.2.3/src/mngs/ml/plt/_learning_curve.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/_optuna_study.py` & `mngs-1.2.3/src/mngs/ml/plt/_optuna_study.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/aucs/example.py` & `mngs-1.2.3/src/mngs/ml/plt/aucs/example.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/aucs/pre_rec_auc.py` & `mngs-1.2.3/src/mngs/ml/plt/aucs/pre_rec_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/plt/aucs/roc_auc.py` & `mngs-1.2.3/src/mngs/ml/plt/aucs/roc_auc.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/silhoute_score_block.py` & `mngs-1.2.3/src/mngs/ml/silhoute_score_block.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/sk/_clf.py` & `mngs-1.2.3/src/mngs/ml/sk/_clf.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/sk/_to_sktime.py` & `mngs-1.2.3/src/mngs/ml/sk/_to_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_DefaultDataset.py` & `mngs-1.2.3/src/mngs/ml/utils/_DefaultDataset.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_LabelEncoder.py` & `mngs-1.2.3/src/mngs/ml/utils/_LabelEncoder.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_check_params.py` & `mngs-1.2.3/src/mngs/ml/utils/_check_params.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_format_samples_for_sktime.py` & `mngs-1.2.3/src/mngs/ml/utils/_format_samples_for_sktime.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_merge_labels.py` & `mngs-1.2.3/src/mngs/ml/utils/_merge_labels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/ml/utils/_under_sample.py` & `mngs-1.2.3/src/mngs/ml/utils/_under_sample.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/mngs/setup.py` & `mngs-1.2.3/src/mngs/mngs/setup.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_AxiswiseDropout.py` & `mngs-1.2.3/src/mngs/nn/_AxiswiseDropout.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_BNet.py` & `mngs-1.2.3/src/mngs/nn/_BNet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_BNet_Res.py` & `mngs-1.2.3/src/mngs/nn/_BNet_Res.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_ChannelGainChanger.py` & `mngs-1.2.3/src/mngs/nn/_ChannelGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_DropoutChannels.py` & `mngs-1.2.3/src/mngs/nn/_DropoutChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_Filters.py` & `mngs-1.2.3/src/mngs/nn/_Filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-05 13:45:11 (ywatanabe)"
+# Time-stamp: "2024-04-08 04:06:50 (ywatanabe)"
 
 import math
 import warnings
 
 import mngs
 import numpy as np
-import pywt
 import seaborn as sns
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from mngs.general import torch_fn
 
 
@@ -62,18 +61,20 @@
 
         x_filted_extended = F.conv1d(
             extended_x, kernel, padding=0, groups=channels
         )[..., :seq_len]
 
         assert x.shape == x_filted_extended.shape
 
-        # Remove edges
-        x_filted_extended[..., : self.radius] *= 0
-        x_filted_extended[..., -self.radius :] *= 0
+        # # Remove edges
+        # x_filted_extended[..., : self.radius] *= 0
+        # x_filted_extended[..., -self.radius :] *= 0
 
+        nn_remove = x_filted_extended.shape[-1] // 4
+        x_filted_extended = x_filted_extended[..., nn_remove:-nn_remove]
         return x_filted_extended
 
 
 class GaussianFilter(BaseFilter1D):
     def __init__(self, sigma):
         super().__init__()
         self.sigma = mngs.gen.to_even(sigma)
```

### Comparing `mngs-1.2.2/src/mngs/nn/_FreqGainChanger.py` & `mngs-1.2.3/src/mngs/nn/_FreqGainChanger.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_GaussianFilter.py` & `mngs-1.2.3/src/mngs/nn/_GaussianFilter.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_Hilbert.py` & `mngs-1.2.3/src/mngs/nn/_Hilbert.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_MNet_1000.py` & `mngs-1.2.3/src/mngs/nn/_MNet_1000.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_PSD.py` & `mngs-1.2.3/src/mngs/nn/_PSD.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_ResNet1D.py` & `mngs-1.2.3/src/mngs/nn/_ResNet1D.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_SpatialAttention.py` & `mngs-1.2.3/src/mngs/nn/_SpatialAttention.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_Spectrogram.py` & `mngs-1.2.3/src/mngs/nn/_Spectrogram.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_SwapChannels.py` & `mngs-1.2.3/src/mngs/nn/_SwapChannels.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/_Wavelet.py` & `mngs-1.2.3/src/mngs/nn/_Wavelet.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/nn/__init__.py` & `mngs-1.2.3/src/mngs/nn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-04-03 00:16:20 (ywatanabe)"
+# Time-stamp: "2024-04-08 12:51:19 (ywatanabe)"
 
 from ._AxiswiseDropout import AxiswiseDropout
 
 # from ._BandPassFilter import BandPassFilter
 from ._BNet import BNet, BNet_config
 from ._ChannelGainChanger import ChannelGainChanger
 from ._DropoutChannels import DropoutChannels
 
 # from ._GaussianFilter import GaussianFilter
-from ._Filters import BandPassFilter, BandStopFilter, GaussianFilter
+from ._Filters import (
+    BandPassFilter,
+    BandStopFilter,
+    GaussianFilter,
+    HighPassFilter,
+    LowPassFilter,
+)
 from ._FreqGainChanger import FreqGainChanger
 from ._Hilbert import Hilbert
 
 # from ._FreqDropout import FreqDropout
 from ._MNet_1000 import MNet_1000, MNet_config
+from ._ModulationIndex import ModulationIndex
+from ._PAC import PAC
 from ._PSD import PSD
 from ._ResNet1D import ResNet1D, ResNetBasicBlock
 from ._SpatialAttention import SpatialAttention
 from ._SwapChannels import SwapChannels
 from ._TransposeLayer import TransposeLayer
 from ._Wavelet import Wavelet
```

### Comparing `mngs-1.2.2/src/mngs/os/_mv.py` & `mngs-1.2.3/src/mngs/os/_mv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# Time-stamp: "2024-03-02 21:35:41 (ywatanabe)"
+# Time-stamp: "2024-04-06 09:00:45 (ywatanabe)"
 
-import os
-import shutil
+# import os
+# import shutil
 
 # def mv(src, tgt):
 #     successful = True
 #     os.makedirs(tgt, exist_ok=True)
 
 #     if os.path.isdir(src):
 #         # Iterate over the items in the directory
@@ -32,14 +32,17 @@
 #             print(f"\nError: {e}")
 #             successful = False
 
 #     return successful
 
 
 def mv(src, tgt):
+    import os
+    import shutil
+
     successful = True
     os.makedirs(tgt, exist_ok=True)
 
     try:
         shutil.move(src, tgt)
         print(f"\nMoved from {src} to {tgt}")
     except OSError as e:
```

### Comparing `mngs-1.2.2/src/mngs/plt/_add_hue.py` & `mngs-1.2.3/src/mngs/plt/_add_hue.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_annotated_heatmap.py` & `mngs-1.2.3/src/mngs/plt/_annotated_heatmap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_configure_mpl.py` & `mngs-1.2.3/src/mngs/plt/_configure_mpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_draw_a_cube.py` & `mngs-1.2.3/src/mngs/plt/_draw_a_cube.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_get_RGBA_from_colormap.py` & `mngs-1.2.3/src/mngs/plt/_get_RGBA_from_colormap.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_mk_colorbar.py` & `mngs-1.2.3/src/mngs/plt/_mk_colorbar.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/_tpl.py` & `mngs-1.2.3/src/mngs/plt/_tpl.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_circular_hist.py` & `mngs-1.2.3/src/mngs/plt/ax/_circular_hist.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_extend.py` & `mngs-1.2.3/src/mngs/plt/ax/_extend.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_hide_spines.py` & `mngs-1.2.3/src/mngs/plt/ax/_hide_spines.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_map_ticks.py` & `mngs-1.2.3/src/mngs/plt/ax/_map_ticks.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_panel.py` & `mngs-1.2.3/src/mngs/plt/ax/_panel.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_sci_note.py` & `mngs-1.2.3/src/mngs/plt/ax/_sci_note.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/ax/_set_pos.py` & `mngs-1.2.3/src/mngs/plt/ax/_set_pos.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/colors.py` & `mngs-1.2.3/src/mngs/plt/colors.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/plt/get_mpl_color.py` & `mngs-1.2.3/src/mngs/plt/get_mpl_color.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/resource/get.py` & `mngs-1.2.3/src/mngs/resource/get.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/resource/limit_RAM.py` & `mngs-1.2.3/src/mngs/resource/limit_RAM.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/__init__.py` & `mngs-1.2.3/src/mngs/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_bonferroni_correction.py` & `mngs-1.2.3/src/mngs/stats/_bonferroni_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_brunner_munzel_test.py` & `mngs-1.2.3/src/mngs/stats/_brunner_munzel_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_corr_test.py` & `mngs-1.2.3/src/mngs/stats/_corr_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_fdr_correction.py` & `mngs-1.2.3/src/mngs/stats/_fdr_correction.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_general.py` & `mngs-1.2.3/src/mngs/stats/_general.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_multicompair.py` & `mngs-1.2.3/src/mngs/stats/_multicompair.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_nocorrelation_test.py` & `mngs-1.2.3/src/mngs/stats/_nocorrelation_test.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/stats/_smirnov_grubbs.py` & `mngs-1.2.3/src/mngs/stats/_smirnov_grubbs.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs/torch/_apply_to.py` & `mngs-1.2.3/src/mngs/torch/_apply_to.py`

 * *Files identical despite different names*

### Comparing `mngs-1.2.2/src/mngs.egg-info/PKG-INFO` & `mngs-1.2.3/src/mngs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mngs
-Version: 1.2.2
+Version: 1.2.3
 Summary: For lazy python users (monogusa people in Japanse), especially in ML/DSP fields
 Home-page: https://github.com/ywatanabe1989/mngs
 Author: ywatanabe1989
 Author-email: ywata1989@gmail.com
-License: GPL3.0
+License: MIT
 Keywords: utils,utilities,python,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: GitPython
@@ -50,14 +50,18 @@
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchsummary
 Requires-Dist: umap-learn
 Requires-Dist: wheel
 Requires-Dist: xmltodict
 Requires-Dist: sktime
+Requires-Dist: tensorpac
+Requires-Dist: ipython==8.0.0
+Requires-Dist: ipdb
+Requires-Dist: plotly
 
 ![CI](https://github.com/ywatanabe1989/mngs/actions/workflows/pip_install.yml/badge.svg)
 
 ## Installation
 ``` bash
 $ pip install mngs
 ```
```

### Comparing `mngs-1.2.2/src/mngs.egg-info/SOURCES.txt` & `mngs-1.2.3/src/mngs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,51 +11,57 @@
 src/mngs.egg-info/top_level.txt
 src/mngs/dsp/PARAMS.py
 src/mngs/dsp/__init__.py
 src/mngs/dsp/_demo_sig.py
 src/mngs/dsp/_hilbert.py
 src/mngs/dsp/_misc.py
 src/mngs/dsp/_mne.py
+src/mngs/dsp/_modulation_index.py
+src/mngs/dsp/_pac.py
 src/mngs/dsp/_psd.py
 src/mngs/dsp/_resample.py
 src/mngs/dsp/_transform.py
 src/mngs/dsp/_wavelet.py
 src/mngs/dsp/add_noise.py
 src/mngs/dsp/example.py
 src/mngs/dsp/filt.py
 src/mngs/dsp/norm.py
 src/mngs/dsp/ref.py
+src/mngs/dsp/fx/__init__.py
 src/mngs/dsp/nn/_AxiswiseDropout.py
 src/mngs/dsp/nn/_BNet.py
 src/mngs/dsp/nn/_BNet_Res.py
 src/mngs/dsp/nn/_ChannelGainChanger.py
 src/mngs/dsp/nn/_DropoutChannels.py
 src/mngs/dsp/nn/_Filters.py
 src/mngs/dsp/nn/_FreqGainChanger.py
 src/mngs/dsp/nn/_GaussianFilter.py
 src/mngs/dsp/nn/_Hilbert.py
 src/mngs/dsp/nn/_MNet_1000.py
+src/mngs/dsp/nn/_ModulationIndex.py
+src/mngs/dsp/nn/_PAC.py
+src/mngs/dsp/nn/_PAC_working.py
 src/mngs/dsp/nn/_PSD.py
 src/mngs/dsp/nn/_ResNet1D.py
 src/mngs/dsp/nn/_SpatialAttention.py
 src/mngs/dsp/nn/_Spectrogram.py
 src/mngs/dsp/nn/_SwapChannels.py
 src/mngs/dsp/nn/_TransposeLayer.py
 src/mngs/dsp/nn/_Wavelet.py
 src/mngs/dsp/nn/__init__.py
-src/mngs/general/TimeStamper.py
+src/mngs/general/_TimeStamper.py
 src/mngs/general/__init__.py
 src/mngs/general/_close.py
 src/mngs/general/_converters.py
+src/mngs/general/_cuda_collect_env.py
 src/mngs/general/_norm.py
+src/mngs/general/_reload.py
 src/mngs/general/_shell.py
 src/mngs/general/_start.py
 src/mngs/general/_xml2dict.py
-src/mngs/general/cuda_collect_env.py
-src/mngs/general/debug.py
 src/mngs/general/email.py
 src/mngs/general/latex.py
 src/mngs/general/load.py
 src/mngs/general/mat2py.py
 src/mngs/general/misc.py
 src/mngs/general/pandas.py
 src/mngs/general/path.py
@@ -128,14 +134,17 @@
 src/mngs/nn/_ChannelGainChanger.py
 src/mngs/nn/_DropoutChannels.py
 src/mngs/nn/_Filters.py
 src/mngs/nn/_FreqGainChanger.py
 src/mngs/nn/_GaussianFilter.py
 src/mngs/nn/_Hilbert.py
 src/mngs/nn/_MNet_1000.py
+src/mngs/nn/_ModulationIndex.py
+src/mngs/nn/_PAC.py
+src/mngs/nn/_PAC_working.py
 src/mngs/nn/_PSD.py
 src/mngs/nn/_ResNet1D.py
 src/mngs/nn/_SpatialAttention.py
 src/mngs/nn/_Spectrogram.py
 src/mngs/nn/_SwapChannels.py
 src/mngs/nn/_TransposeLayer.py
 src/mngs/nn/_Wavelet.py
@@ -161,14 +170,15 @@
 src/mngs/plt/ax/_hide_spines.py
 src/mngs/plt/ax/_map_ticks.py
 src/mngs/plt/ax/_panel.py
 src/mngs/plt/ax/_sci_note.py
 src/mngs/plt/ax/_set_n_ticks.py
 src/mngs/plt/ax/_set_pos.py
 src/mngs/plt/ax/_set_size.py
+src/mngs/plt/ax/_set_ticks.py
 src/mngs/resource/__init__.py
 src/mngs/resource/get.py
 src/mngs/resource/limit_RAM.py
 src/mngs/stats/__init__.py
 src/mngs/stats/_bonferroni_correction.py
 src/mngs/stats/_brunner_munzel_test.py
 src/mngs/stats/_calc_partial_corr.py
```

