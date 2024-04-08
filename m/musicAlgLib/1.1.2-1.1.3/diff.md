# Comparing `tmp/musicAlgLib-1.1.2.tar.gz` & `tmp/musicAlgLib-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicAlgLib-1.1.2.tar", last modified: Wed Apr  3 08:38:22 2024, max compression
+gzip compressed data, was "musicAlgLib-1.1.3.tar", last modified: Mon Apr  8 01:56:27 2024, max compression
```

## Comparing `musicAlgLib-1.1.2.tar` & `musicAlgLib-1.1.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.826007 musicAlgLib-1.1.2/
--rw-rw-rw-   0        0        0     4676 2024-04-03 08:38:22.826007 musicAlgLib-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.792775 musicAlgLib-1.1.2/musicAlgLib/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.797240 musicAlgLib-1.1.2/musicAlgLib/AGC_EVALUATION/
--rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/AGC_EVALUATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.797735 musicAlgLib-1.1.2/musicAlgLib/CLIPPING_DETECTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/CLIPPING_DETECTION/__init__.py
--rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.808647 musicAlgLib-1.1.2/musicAlgLib/DLLS/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/__init__.py
--rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/cygwin1.dll
--rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.dll
--rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.dylib
--rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.so
--rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.dll
--rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.dylib
--rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.so
--rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.dll
--rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.dylib
--rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.so
--rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/peaqb.exe
--rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/silero_vad.jit
--rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.dll
--rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.dylib
--rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.so
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.808647 musicAlgLib-1.1.2/musicAlgLib/DynmicRange/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.2/musicAlgLib/DynmicRange/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.809639 musicAlgLib-1.1.2/musicAlgLib/FUNCTION/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/FUNCTION/__init__.py
--rw-rw-rw-   0        0        0    19295 2024-04-03 08:34:31.000000 musicAlgLib-1.1.2/musicAlgLib/FUNCTION/audioFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.810135 musicAlgLib-1.1.2/musicAlgLib/FrequencyResponse/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.2/musicAlgLib/FrequencyResponse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.811624 musicAlgLib-1.1.2/musicAlgLib/Noise_Suppression/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/Noise_Suppression/__init__.py
--rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/Noise_Suppression/noiseFuction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.812616 musicAlgLib-1.1.2/musicAlgLib/PCC/
--rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PCC/Pearson_CC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PCC/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.813608 musicAlgLib-1.1.2/musicAlgLib/PEAQ/
--rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PEAQ/PEAQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PEAQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.814600 musicAlgLib-1.1.2/musicAlgLib/PESQ/
--rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PESQ/PESQ.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/PESQ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.814600 musicAlgLib-1.1.2/musicAlgLib/PLAY_DELAY/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.2/musicAlgLib/PLAY_DELAY/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.817079 musicAlgLib-1.1.2/musicAlgLib/POLQA/
--rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/POLQA.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/file_server.py
--rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/polqa_client.py
--rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/polqa_server.py
--rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/POLQA/socketClient.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.818568 musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/
--rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
--rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.819559 musicAlgLib-1.1.2/musicAlgLib/STI/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/STI/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/STI/cal_sti.py
--rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/STI/sti.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.820552 musicAlgLib-1.1.2/musicAlgLib/VAD_NN/
--rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.2/musicAlgLib/VAD_NN/__init__.py
--rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.2/musicAlgLib/VAD_NN/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.821048 musicAlgLib-1.1.2/musicAlgLib/VISQOL/
--rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.2/musicAlgLib/VISQOL/__init__.py
--rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.1.2/musicAlgLib/__init__.py
--rw-rw-rw-   0        0        0    15698 2024-04-03 08:38:04.000000 musicAlgLib-1.1.2/musicAlgLib/commFunction.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.821543 musicAlgLib-1.1.2/musicAlgLib/computeAudioQuality/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/computeAudioQuality/__init__.py
--rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.1.2/musicAlgLib/computeAudioQuality/mainProcess.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.823032 musicAlgLib-1.1.2/musicAlgLib/formatConvert/
--rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/formatConvert/__init__.py
--rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/formatConvert/wav_pcm.py
--rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.824024 musicAlgLib-1.1.2/musicAlgLib/resample/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/resample/__init__.py
--rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/resample/resampler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.824519 musicAlgLib-1.1.2/musicAlgLib/tests/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/tests/__init__.py
--rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.2/musicAlgLib/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.825511 musicAlgLib-1.1.2/musicAlgLib/timeAligment/
--rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.2/musicAlgLib/timeAligment/__init__.py
--rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.2/musicAlgLib/timeAligment/time_align.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:38:22.796248 musicAlgLib-1.1.2/musicAlgLib.egg-info/
--rw-rw-rw-   0        0        0     4676 2024-04-03 08:38:22.000000 musicAlgLib-1.1.2/musicAlgLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2024-04-03 08:38:22.000000 musicAlgLib-1.1.2/musicAlgLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:38:22.000000 musicAlgLib-1.1.2/musicAlgLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-03 08:38:22.000000 musicAlgLib-1.1.2/musicAlgLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 08:38:22.000000 musicAlgLib-1.1.2/musicAlgLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:38:22.826007 musicAlgLib-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     5839 2024-04-03 08:38:21.000000 musicAlgLib-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.920612 musicAlgLib-1.1.3/
+-rw-rw-rw-   0        0        0     4676 2024-04-08 01:56:27.920116 musicAlgLib-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.886883 musicAlgLib-1.1.3/musicAlgLib/
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.890852 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/
+-rw-rw-rw-   0        0        0     1825 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.891843 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/__init__.py
+-rw-rw-rw-   0        0        0     4933 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.902259 musicAlgLib-1.1.3/musicAlgLib/DLLS/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/__init__.py
+-rw-rw-rw-   0        0        0   971618 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/cygwin1.dll
+-rw-rw-rw-   0        0        0   138362 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dll
+-rw-rw-rw-   0        0        0    60432 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dylib
+-rw-rw-rw-   0        0        0    39288 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.so
+-rw-rw-rw-   0        0        0   105729 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dll
+-rw-rw-rw-   0        0        0   145136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dylib
+-rw-rw-rw-   0        0        0    27600 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.so
+-rw-rw-rw-   0        0        0    54552 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dll
+-rw-rw-rw-   0        0        0   134144 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dylib
+-rw-rw-rw-   0        0        0     8136 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.so
+-rwxrwxrwx   0        0        0   134032 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/peaqb.exe
+-rw-rw-rw-   0        0        0  1439299 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/silero_vad.jit
+-rw-rw-rw-   0        0        0    67194 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dll
+-rw-rw-rw-   0        0        0   140336 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dylib
+-rw-rw-rw-   0        0        0    18200 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.so
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.902756 musicAlgLib-1.1.3/musicAlgLib/DynmicRange/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:08.000000 musicAlgLib-1.1.3/musicAlgLib/DynmicRange/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.903748 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/__init__.py
+-rw-rw-rw-   0        0        0    19289 2024-04-08 01:55:50.000000 musicAlgLib-1.1.3/musicAlgLib/FUNCTION/audioFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.904244 musicAlgLib-1.1.3/musicAlgLib/FrequencyResponse/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:09:36.000000 musicAlgLib-1.1.3/musicAlgLib/FrequencyResponse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.904739 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/__init__.py
+-rw-rw-rw-   0        0        0    23703 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/noiseFuction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.905732 musicAlgLib-1.1.3/musicAlgLib/PCC/
+-rw-rw-rw-   0        0        0     3235 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PCC/Pearson_CC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PCC/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.906227 musicAlgLib-1.1.3/musicAlgLib/PEAQ/
+-rw-rw-rw-   0        0        0      346 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PEAQ/PEAQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PEAQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.908212 musicAlgLib-1.1.3/musicAlgLib/PESQ/
+-rw-rw-rw-   0        0        0     1106 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PESQ/PESQ.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/PESQ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.908708 musicAlgLib-1.1.3/musicAlgLib/PLAY_DELAY/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:23:36.000000 musicAlgLib-1.1.3/musicAlgLib/PLAY_DELAY/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.910692 musicAlgLib-1.1.3/musicAlgLib/POLQA/
+-rw-rw-rw-   0        0        0     4006 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/POLQA.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/file_server.py
+-rw-rw-rw-   0        0        0     4528 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_client.py
+-rw-rw-rw-   0        0        0     4213 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_server.py
+-rw-rw-rw-   0        0        0     1341 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/POLQA/socketClient.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.912180 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/
+-rw-rw-rw-   0        0        0     2548 2024-04-02 06:41:17.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py
+-rw-rw-rw-   0        0        0     1410 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.913172 musicAlgLib-1.1.3/musicAlgLib/STI/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/cal_sti.py
+-rw-rw-rw-   0        0        0    20320 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/STI/sti.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.914164 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/
+-rw-rw-rw-   0        0        0        0 2022-12-08 08:31:54.000000 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/__init__.py
+-rw-rw-rw-   0        0        0    25053 2023-09-01 10:34:35.000000 musicAlgLib-1.1.3/musicAlgLib/VAD_NN/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.914660 musicAlgLib-1.1.3/musicAlgLib/VISQOL/
+-rw-rw-rw-   0        0        0        0 2024-04-01 08:10:40.000000 musicAlgLib-1.1.3/musicAlgLib/VISQOL/__init__.py
+-rw-rw-rw-   0        0        0     4781 2024-04-03 07:50:07.000000 musicAlgLib-1.1.3/musicAlgLib/__init__.py
+-rw-rw-rw-   0        0        0    15692 2024-04-08 01:55:50.000000 musicAlgLib-1.1.3/musicAlgLib/commFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.915156 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/__init__.py
+-rw-rw-rw-   0        0        0    11334 2024-04-03 08:07:32.000000 musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/mainProcess.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.916643 musicAlgLib-1.1.3/musicAlgLib/formatConvert/
+-rw-rw-rw-   0        0        0       36 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/formatConvert/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/formatConvert/wav_pcm.py
+-rw-rw-rw-   0        0        0     9466 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.917636 musicAlgLib-1.1.3/musicAlgLib/resample/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/resample/__init__.py
+-rw-rw-rw-   0        0        0     1687 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/resample/resampler.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.919124 musicAlgLib-1.1.3/musicAlgLib/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/tests/__init__.py
+-rw-rw-rw-   0        0        0      525 2024-04-01 10:45:14.000000 musicAlgLib-1.1.3/musicAlgLib/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.919619 musicAlgLib-1.1.3/musicAlgLib/timeAligment/
+-rw-rw-rw-   0        0        0        0 2023-12-04 07:48:57.000000 musicAlgLib-1.1.3/musicAlgLib/timeAligment/__init__.py
+-rw-rw-rw-   0        0        0     8537 2024-04-02 12:07:22.000000 musicAlgLib-1.1.3/musicAlgLib/timeAligment/time_align.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:56:27.889860 musicAlgLib-1.1.3/musicAlgLib.egg-info/
+-rw-rw-rw-   0        0        0     4676 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 01:56:27.000000 musicAlgLib-1.1.3/musicAlgLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 01:56:27.920612 musicAlgLib-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     5839 2024-04-08 01:56:20.000000 musicAlgLib-1.1.3/setup.py
```

### Comparing `musicAlgLib-1.1.2/PKG-INFO` & `musicAlgLib-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.2
+Version: 1.1.3
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.2/README.md` & `musicAlgLib-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py` & `musicAlgLib-1.1.3/musicAlgLib/AGC_EVALUATION/CAL_MUSIC_STABILITY.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py` & `musicAlgLib-1.1.3/musicAlgLib/CLIPPING_DETECTION/audio_clip_detection.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/cygwin1.dll` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/cygwin1.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.dll` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.dylib` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/matchsig.so` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/matchsig.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.dll` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.dylib` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/musicStability.so` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/musicStability.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.dll` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.dylib` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/pcc.so` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/pcc.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/peaqb.exe` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/peaqb.exe`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/silero_vad.jit` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/silero_vad.jit`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.dll` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dll`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.dylib` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.dylib`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/DLLS/snr_music.so` & `musicAlgLib-1.1.3/musicAlgLib/DLLS/snr_music.so`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/FUNCTION/audioFunction.py` & `musicAlgLib-1.1.3/musicAlgLib/FUNCTION/audioFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,19 +147,19 @@
         testdata, fs, ch = get_data_array(wavFileName)
         curdata = np.array([])
         for eachSection in speechSection:
             curdata = np.concatenate(
                 (curdata, testdata[int(fs * eachSection[0]):int(fs * eachSection[1])]))
 
     if rmsMode == 'total':
-        return get_rms(curdata,fs)
+        return get_rms(curdata)
     if rmsMode == 'average':
         return get_ave_rms(curdata,fs)
     if rmsMode == 'peak':
-        return  get_peak_rms(curdata,fs)
+        return  get_peak_rms(curdata)
     if rmsMode == 'std':
         return  get_std_rms(curdata,fs)
     if rmsMode == 'max':
         return  get_max_rms(curdata,fs)
     if rmsMode == 'min':
         return  get_min_rms(curdata,fs)
     if rmsMode == 'dynmic':
```

### Comparing `musicAlgLib-1.1.2/musicAlgLib/Noise_Suppression/noiseFuction.py` & `musicAlgLib-1.1.3/musicAlgLib/Noise_Suppression/noiseFuction.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/PCC/Pearson_CC.py` & `musicAlgLib-1.1.3/musicAlgLib/PCC/Pearson_CC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/PESQ/PESQ.py` & `musicAlgLib-1.1.3/musicAlgLib/PESQ/PESQ.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/POLQA/POLQA.py` & `musicAlgLib-1.1.3/musicAlgLib/POLQA/POLQA.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/POLQA/file_server.py` & `musicAlgLib-1.1.3/musicAlgLib/POLQA/file_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/POLQA/polqa_client.py` & `musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_client.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/POLQA/polqa_server.py` & `musicAlgLib-1.1.3/musicAlgLib/POLQA/polqa_server.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/POLQA/socketClient.py` & `musicAlgLib-1.1.3/musicAlgLib/POLQA/socketClient.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py` & `musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/MATCH_SIG.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py` & `musicAlgLib-1.1.3/musicAlgLib/SNR_ESTIMATION/SNR_MUSIC.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/STI/cal_sti.py` & `musicAlgLib-1.1.3/musicAlgLib/STI/cal_sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/STI/sti.py` & `musicAlgLib-1.1.3/musicAlgLib/STI/sti.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/VAD_NN/hubconf.py` & `musicAlgLib-1.1.3/musicAlgLib/VAD_NN/hubconf.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/__init__.py` & `musicAlgLib-1.1.3/musicAlgLib/__init__.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/commFunction.py` & `musicAlgLib-1.1.3/musicAlgLib/commFunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
         maxcnt += 1
         curRms = get_rms(data[a*frameLen:(a+1)*frameLen])
         if curRms > threshold:
             validcnt += 1
 
     return validcnt/maxcnt
 
-def get_rms(records,fs):
+def get_rms(records):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
@@ -432,15 +432,15 @@
     if len(data) == 0:
         return -99.9
     rms = math.sqrt(sum([(x/32767) * (x/32767) for x in data])/len(data))
     dBrmsValue = 20*math.log10(rms + 1.0E-6)
     return dBrmsValue
 
 
-def get_peak_rms(records,fs):
+def get_peak_rms(records):
     '''
     Parameters
     ----------
     records
 
     Returns
     -------
```

### Comparing `musicAlgLib-1.1.2/musicAlgLib/computeAudioQuality/mainProcess.py` & `musicAlgLib-1.1.3/musicAlgLib/computeAudioQuality/mainProcess.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/formatConvert/wav_pcm.py` & `musicAlgLib-1.1.3/musicAlgLib/formatConvert/wav_pcm.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/main.py` & `musicAlgLib-1.1.3/musicAlgLib/main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/resample/resampler.py` & `musicAlgLib-1.1.3/musicAlgLib/resample/resampler.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/tests/test_main.py` & `musicAlgLib-1.1.3/musicAlgLib/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib/timeAligment/time_align.py` & `musicAlgLib-1.1.3/musicAlgLib/timeAligment/time_align.py`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/musicAlgLib.egg-info/PKG-INFO` & `musicAlgLib-1.1.3/musicAlgLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicAlgLib
-Version: 1.1.2
+Version: 1.1.3
 Summary: audio algorithms to compute and test music quality
 Home-page: https://github.com/pypa/sampleproject
 Author:  MA JIANLI
 Author-email: majianli@corp.netease.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `musicAlgLib-1.1.2/musicAlgLib.egg-info/SOURCES.txt` & `musicAlgLib-1.1.3/musicAlgLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicAlgLib-1.1.2/setup.py` & `musicAlgLib-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 setup(
     name='musicAlgLib',
-    version='1.1.2',
+    version='1.1.3',
     packages=setuptools.find_packages(),
     url='https://github.com/pypa/sampleproject',
     license='MIT',
     author=' MA JIANLI',
     author_email='majianli@corp.netease.com',
     description='audio algorithms to compute and test music quality',
     long_description="""
```

