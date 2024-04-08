# Comparing `tmp/musicAlgLib-1.1.3.tar.gz` & `tmp/musicAlgLib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.1.3.tar", last modified: Mon Apr  8 01:56:27 2024, max compression
+gzip compressed data, was "musicAlgLib-1.1.5.tar", last modified: Mon Apr  8 02:18:58 2024, max compression
```

## Comparing `musicAlgLib-1.1.3.tar` & `musicAlgLib-1.1.5.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.920612 musicAlgLib-1.1.3/
--rw-rw-rw-   0        0        0     4676 2024-04-08 01:56:27.920116 musicAlgLib-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.886883 musicAlgLib-1.1.3/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.890852 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.891843 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.902259 musicAlgLib-1.1.3/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.902756 musicAlgLib-1.1.3/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.3/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.903748 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19289 2024-04-08 01:55:50.000000 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.904244 musicAlgLib-1.1.3/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.3/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.904739 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.905732 musicAlgLib-1.1.3/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.906227 musicAlgLib-1.1.3/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.908212 musicAlgLib-1.1.3/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.908708 musicAlgLib-1.1.3/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.3/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.910692 musicAlgLib-1.1.3/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.912180 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.913172 musicAlgLib-1.1.3/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.914164 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.914660 musicAlgLib-1.1.3/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.3/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.1.3/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    15692 2024-04-08 01:55:50.000000 musicAlgLib-1.1.3/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.915156 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.916643 musicAlgLib-1.1.3/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.917636 musicAlgLib-1.1.3/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.919124 musicAlgLib-1.1.3/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.3/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.919619 musicAlgLib-1.1.3/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.3/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.889860 musicAlgLib-1.1.3/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 01:56:27.920612 musicAlgLib-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     5839 2024-04-08 01:56:20.000000 musicAlgLib-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.630877 musicAlgLib-1.1.5/
+-rw-rw-rw-   0        0        0     4676 2024-04-08 02:18:58.630877 musicAlgLib-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.596653 musicAlgLib-1.1.5/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.600621 musicAlgLib-1.1.5/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.601613 musicAlgLib-1.1.5/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.612028 musicAlgLib-1.1.5/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.612525 musicAlgLib-1.1.5/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.5/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.613516 musicAlgLib-1.1.5/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19719 2024-04-08 02:18:42.000000 musicAlgLib-1.1.5/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.613516 musicAlgLib-1.1.5/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.5/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.614508 musicAlgLib-1.1.5/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.615501 musicAlgLib-1.1.5/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.615996 musicAlgLib-1.1.5/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.617981 musicAlgLib-1.1.5/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.618476 musicAlgLib-1.1.5/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.5/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.620957 musicAlgLib-1.1.5/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.621949 musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.622941 musicAlgLib-1.1.5/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.623933 musicAlgLib-1.1.5/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.5/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.5/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.624429 musicAlgLib-1.1.5/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.5/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     5014 2024-04-08 02:18:42.000000 musicAlgLib-1.1.5/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    15970 2024-04-08 02:18:42.000000 musicAlgLib-1.1.5/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.625917 musicAlgLib-1.1.5/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0    12316 2024-04-08 02:18:42.000000 musicAlgLib-1.1.5/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.627405 musicAlgLib-1.1.5/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     6315 2024-04-08 02:18:42.000000 musicAlgLib-1.1.5/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.628397 musicAlgLib-1.1.5/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.629389 musicAlgLib-1.1.5/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.5/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.630381 musicAlgLib-1.1.5/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.5/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.5/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-08 02:18:58.600125 musicAlgLib-1.1.5/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-08 02:18:58.000000 musicAlgLib-1.1.5/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-08 02:18:58.000000 musicAlgLib-1.1.5/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 02:18:58.000000 musicAlgLib-1.1.5/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-08 02:18:58.000000 musicAlgLib-1.1.5/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 02:18:58.000000 musicAlgLib-1.1.5/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 02:18:58.631373 musicAlgLib-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     5839 2024-04-08 02:18:52.000000 musicAlgLib-1.1.5/setup.py
```

### Comparing `musicAlgLib-1.1.3/PKG-INFO` & `musicAlgLib-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.3
+Version: 1.1.5
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.3/README.md` & `musicAlgLib-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.1.5/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.1.5/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.1.5/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.1.5/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         raise TypeError('wrong format! not wav/mp4 file!' + str(suffix))
     if suffix == '.mp4':
         wavFileName = get_wav_from_mp4(wavFileName)
     wavf = wave.open(wavFileName, 'rb')
     refChannel,refsamWidth,refsamplerate,refframeCount = wavf.getnchannels(),wavf.getsampwidth(),wavf.getframerate(),wavf.getnframes()
     return refChannel,refsamWidth*8,refsamplerate,refframeCount
 
-def get_rms_level(wavFileName=None,rmsMode='total',section=None,speechOnly=False):
+def get_rms_level(wavFileName=None,rmsMode='total',section=None,speechOnly=False,frameDuration=0.05,shiftduration=0.05):
     """
     wavFileName：输入文件 wav，mp4
     Returns
     -------
     refChannel:通道数
     refsamWidth：比特位 2代表16bit
     refsamplerate：采样率
@@ -149,27 +149,27 @@
         for eachSection in speechSection:
             curdata = np.concatenate(
                 (curdata, testdata[int(fs * eachSection[0]):int(fs * eachSection[1])]))
 
     if rmsMode == 'total':
         return get_rms(curdata)
     if rmsMode == 'average':
-        return get_ave_rms(curdata,fs)
+        return get_ave_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     if rmsMode == 'peak':
         return  get_peak_rms(curdata)
     if rmsMode == 'std':
-        return  get_std_rms(curdata,fs)
+        return  get_std_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     if rmsMode == 'max':
-        return  get_max_rms(curdata,fs)
+        return  get_max_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     if rmsMode == 'min':
-        return  get_min_rms(curdata,fs)
+        return  get_min_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     if rmsMode == 'dynmic':
-        return  get_max_rms(curdata,fs) - get_min_rms(curdata,fs)
+        return  get_max_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration) - get_min_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     if rmsMode == 'duration':
-        return  get_duration_above_specific_rms(curdata,fs)
+        return  get_duration_above_specific_rms(curdata,fs,frameDuration=frameDuration,shiftduration=shiftduration)
     return None
 
 
 
 def calculate_band_energy(audio_signal, sample_rate, num_bands,freq_mode='upper'):
     # Perform FFT on audio signal
     fmin,fmax = 100,sample_rate/2 - 100
```

### Comparing `musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.1.5/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.1.5/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.1.5/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.1.5/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.1.5/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.1.5/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.1.5/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.1.5/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.1.5/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.1.5/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/STI/sti.py` & `musicAlgLib-1.1.5/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.1.5/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/__init__.py` & `musicAlgLib-1.1.5/musicAlgLib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .VAD_NN.hubconf import silero_vad
 from operator import methodcaller
 from .computeAudioQuality.mainProcess import computeAudioQuality
 
 from ctypes import  *
 
 def compute_music_quality(metrics,testFile=None,refFile=None,outFile=None,audioType=1,
-                         rmsCalsection=None,polqaMode=0,pitchLogMode=1,fineDelaySection=None,rmsSpeechOnly=False):
+                         rmsCalsection=None,polqaMode=0,pitchLogMode=1,fineDelaySection=None,rmsSpeechOnly=False,frameDuration=0.05,shiftduration=0.05):
     """
     :param metrics: ['ALL','POLQA','PEAQ','LOUDNESS','MUSIC','MATCH','MUSICSTA','SLIENCE','FORMAT','TOTALRMS','AVERMS','PEAKRMS','STDRMS','MAXRMS','MINRMS','DYNMIC','LRATE','CLIP','DELAY','SPEC','PITCH','EQ','MATCH2','MATCH3']
 
     #
     # POLQA 窄带模式  8k  超宽带模式 48k ；WAV/PCM输入 ；双端输入：ref、test；时长 < 20s；
     # PEAQ 无采样率限制；WAV/PCM输入 ；双端输入：ref、test；无时间长度要求；
     # MATCH 无采样率限制; WAV/PCM输入;三端输入：ref、test、out； 无时间长度要求；
@@ -48,25 +48,29 @@
     :param refFile:  参考文件，可选项，全参考指标必选，比如POLQA/PESQ/PEAQ
     :param outFile 输出文件，可选项，对齐文件可选
     :param audioType  输入音频的模式 0：语音 1：音乐 MATCH/GAINTABLE需要
     :param rmsCalsection 计算rms的区间 TRMS和ARMS需要，时间单位s，比如：[1,20]
     :param polqaMode 计算polqa的模式 0:默认模式  1: 理想模式：排除小声音的影响，把声音校准到理想点平 -26db
     :param pitchLogMode 计算pitch的模式 0：线性模式，用于SetLocalVoicePitch接口; 1：对数模式,用于SetAudioMixingPitch接口；默认为1
     :param fineDelaySection 精准计算延时(MTACH3)，需要手动标出语音块的位置，比如有三段：speech_section=[[2.423,4.846],[5.577,7.411],[8,10.303]]
+    :param frameDuration 计算rms的帧长度 默认50ms
+    :param shiftduration 计算rms的帧移 默认50ms
     :return:
     """
     paraDicts = {
         'metrics':metrics,
         'testFile':testFile,
         'refFile':refFile,
         'outFile':outFile,
         "audioType":audioType,
         'rmsCalsection':rmsCalsection,
         'polqaMode':polqaMode,
         "pitchLogMode":pitchLogMode,
         "fineDelaySection":fineDelaySection,
-        "rmsSpeechOnly":rmsSpeechOnly
+        "rmsSpeechOnly":rmsSpeechOnly,
+        'frameDuration' : frameDuration,
+        'shiftduration' : shiftduration
     }
     comAuQUA = computeAudioQuality(**paraDicts)
     return methodcaller(metrics)(comAuQUA)
```

### Comparing `musicAlgLib-1.1.3/musicAlgLib/commFunction.py` & `musicAlgLib-1.1.5/musicAlgLib/commFunction.py`

 * *Files 5% similar despite different names*

```diff
@@ -358,59 +358,61 @@
     wavfile = wave.open(tarFile, 'wb')
     wavfile.setnchannels(channel)
     wavfile.setsampwidth(databitnum)
     wavfile.setframerate(fs)
     wavfile.writeframes(outData.tobytes())
     wavfile.close()
 
-def get_ave_rms(data,fs):
+def get_ave_rms(data,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = windowLen * fs
-    frameshift = windowLen * fs / 2
+    frameLen = frameDuration * fs
+    frameshift = shiftduration * fs
     nFrames = int((len(data)-frameLen)//frameshift)
     totalRms,cnt = 0,0
     for a in range(nFrames):
         totalRms += get_rms(data[int(a*frameshift):int(a*frameshift+frameLen)])
         cnt += 1
     return totalRms/cnt
 
-def get_std_rms(data,fs):
+def get_std_rms(data,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = fs * windowLen * 2
+    frameLen = frameDuration * fs
+    frameshift = shiftduration * fs
     nFrames = len(data)//frameLen
     curRms = 0
     rms_list = []
     for a in range(nFrames):
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         rms_list.append(curRms)
     return np.std(rms_list, ddof=1)
-def get_duration_above_specific_rms(data,fs):
+def get_duration_above_specific_rms(data,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     data
 
     Returns
     -------
     '''
-    frameLen = fs * windowLen * 2
+    frameLen = frameDuration * fs
+    frameshift = shiftduration * fs
     nFrames = len(data)//frameLen
     threshold = -45
     maxcnt,validcnt = 0,0
     for a in range(nFrames):
         maxcnt += 1
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         if curRms > threshold:
@@ -447,47 +449,47 @@
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
 
     maxdata = max(records)
     maxRms = 20 * math.log10(maxdata/32767 + 1.0E-6)
     return maxRms
 
-def get_max_rms(records,fs):
+def get_max_rms(records,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = windowLen * fs
-    frameshift = windowLen * fs/2
+    frameLen = frameDuration * fs
+    frameshift = shiftduration * fs
     nFrames = int((len(records) - frameLen) // frameshift)
     maxRms = -99
     for a in range(nFrames):
         curRms = get_rms(records[int(a*frameshift):int(a*frameshift+frameLen)])
         if curRms > maxRms:
             maxRms = curRms
     return maxRms
 
 
-def get_min_rms(records,fs):
+def get_min_rms(records,fs,frameDuration=0.05,shiftduration=0.05):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
     '''
     #return math.sqrt(sum([x * x for x in records])/len(records))
-    frameLen = windowLen * fs
-    frameshift = windowLen * fs/2
+    frameLen = frameDuration * fs
+    frameshift = shiftduration * fs
     nFrames = int((len(records) - frameLen) // frameshift)
     minrms = 100
     for a in range(nFrames):
         curRms = get_rms(records[int(a*frameshift):int(a*frameshift+frameLen)])
         if curRms < minrms:
             minrms = curRms
     return minrms
```

### Comparing `musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.1.5/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self.outFile = kwargs['outFile']
         self.audioType = kwargs["audioType"]
         self.rmsCalsection = kwargs["rmsCalsection"]
         self.polqaMode = kwargs["polqaMode"]
         self.pitchLogMode = kwargs["pitchLogMode"]
         self.fineDelaySection = kwargs["fineDelaySection"]
         self.rmsSpeechOnly = kwargs["rmsSpeechOnly"]
+        self.rmsFrameDuration = kwargs["rmsFrameDuration"]
+        self.rmsShiftDuration = kwargs["rmsShiftDuration"]
 
         self.testFile_L,self.testFile_R = self.Extract_Mono(self.testFile)
 
         self.refFile_L, self.refFile_R = self.Extract_Mono(self.refFile)
         if self.outFile is not None:
             self.outFile_L, self.outFile_R = self.outFile[:-4] + '_L.wav',self.outFile[:-4] + '_R.wav'
         if self.refFile is not None:
@@ -230,67 +232,67 @@
 
     def PEAKRMS(self):
         """
         Returns
         -------
         # (wavFileName=None,rmsMode='total',startTime=0,endTime=1):
         """
-        return get_rms_level(wavFileName=self.testFile_L,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
+        return get_rms_level(wavFileName=self.testFile_L,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration),get_rms_level(wavFileName=self.testFile_R,rmsMode='peak',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
 
     def STDRMS(self):
         """
         Returns
         -------
         # (wavFileName=None,rmsMode='total',startTime=0,endTime=1):
         """
-        return get_rms_level(wavFileName=self.testFile_L,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
+        return get_rms_level(wavFileName=self.testFile_L,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration),get_rms_level(wavFileName=self.testFile_R,rmsMode='std',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
 
 
     def AVERMS(self):
         """
         Returns
         -------
 
         """
-        return get_rms_level(wavFileName=self.testFile_L,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly),get_rms_level(wavFileName=self.testFile_R,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly)
+        return get_rms_level(wavFileName=self.testFile_L,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration),get_rms_level(wavFileName=self.testFile_R,rmsMode='average',section=self.rmsCalsection,speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
 
     def MAXRMS(self):
         """
         Returns
         -------
 
         """
         return get_rms_level(wavFileName=self.testFile_L, rmsMode='max', section=self.rmsCalsection,
-                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                             speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration), get_rms_level(wavFileName=self.testFile_R,
                                                                            rmsMode='max',
                                                                            section=self.rmsCalsection,
-                                                                           speechOnly=self.rmsSpeechOnly)
+                                                                           speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
 
     def MINRMS(self):
         """
         Returns
         -------
 
         """
         return get_rms_level(wavFileName=self.testFile_L, rmsMode='min', section=self.rmsCalsection,
-                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                             speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration), get_rms_level(wavFileName=self.testFile_R,
                                                                            rmsMode='min',
                                                                            section=self.rmsCalsection,
-                                                                           speechOnly=self.rmsSpeechOnly)
+                                                                           speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
     def DYNMIC(self):
         """
         Returns
         -------
 
         """
         return get_rms_level(wavFileName=self.testFile_L, rmsMode='dynmic', section=self.rmsCalsection,
-                             speechOnly=self.rmsSpeechOnly), get_rms_level(wavFileName=self.testFile_R,
+                             speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration), get_rms_level(wavFileName=self.testFile_R,
                                                                            rmsMode='dynmic',
                                                                            section=self.rmsCalsection,
-                                                                           speechOnly=self.rmsSpeechOnly)
+                                                                           speechOnly=self.rmsSpeechOnly,frameDuration=self.rmsFrameDuration,shiftduration=self.rmsShiftDuration)
 
 
 
     def CLIP(self):
         """
         Returns
         -------
```

### Comparing `musicAlgLib-1.1.3/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.1.5/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.1.5/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.1.5/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.1.5/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.1.5/musicAlgLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.3
+Version: 1.1.5
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.3/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.1.5/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.3/setup.py` & `musicAlgLib-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.1.3',
+    version='1.1.5',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```

