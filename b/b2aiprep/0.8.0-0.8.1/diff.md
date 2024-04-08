# Comparing `tmp/b2aiprep-0.8.0.tar.gz` & `tmp/b2aiprep-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2aiprep-0.8.0.tar", last modified: Mon Apr  1 02:29:50 2024, max compression
+gzip compressed data, was "b2aiprep-0.8.1.tar", last modified: Mon Apr  8 18:01:43 2024, max compression
```

## Comparing `b2aiprep-0.8.0.tar` & `b2aiprep-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:29:50.631483 b2aiprep-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:29:50.631483 b2aiprep-0.8.0/src/b2aiprep/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/src/b2aiprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/src/b2aiprep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/src/b2aiprep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/src/b2aiprep/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/src/b2aiprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 02:29:50.000000 b2aiprep-0.8.0/src/b2aiprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:29:50.635483 b2aiprep-0.8.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/src/tests/test_speech_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/src/tests/test_voice_converstion.py
--rw-r--r--   0 runner    (1001) docker     (127)    86892 2024-04-01 02:29:38.000000 b2aiprep-0.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.335659 b2aiprep-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.335659 b2aiprep-0.8.1/src/b2aiprep/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/b2aiprep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14787 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/b2aiprep/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/b2aiprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 18:01:43.000000 b2aiprep-0.8.1/src/b2aiprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 18:01:43.339659 b2aiprep-0.8.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/tests/test_speech_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/src/tests/test_voice_converstion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86892 2024-04-08 18:01:34.000000 b2aiprep-0.8.1/versioneer.py
```

### Comparing `b2aiprep-0.8.0/LICENSE` & `b2aiprep-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/PKG-INFO` & `b2aiprep-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2aiprep
-Version: 0.8.0
+Version: 0.8.1
 Summary: A small package to generate features from acoustic
 Author-email: Rahul Brito <rfbrito@mit.edu>, SenseIn Group <sensein-social@mit.edu>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `b2aiprep-0.8.0/README.md` & `b2aiprep-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/pyproject.toml` & `b2aiprep-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/src/b2aiprep/cli.py` & `b2aiprep-0.8.1/src/b2aiprep/cli.py`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/src/b2aiprep/process.py` & `b2aiprep-0.8.1/src/b2aiprep/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pathlib import Path
 from typing import Union
 
 import matplotlib.pyplot as plt
 import opensmile
 import speechbrain.processing.features as spf
 import torch
-import torchaudio
 from datasets import Dataset
 from scipy import signal
 from speechbrain.augment.time_domain import Resample
 from speechbrain.dataio.dataio import read_audio, read_audio_info
 from speechbrain.inference.speaker import EncoderClassifier
 from transformers import AutoModelForSpeechSeq2Seq, AutoProcessor, pipeline
 
@@ -103,21 +102,22 @@
     :param audio: Audio object
     :param n_fft: FFT window size
     :param win_length: Window length (ms)
     :param hop_length: Hop length (ms)
     :param toDb: If True, return the log of the power of the spectrogram
     :return: Spectrogram
     """
-    spectrogram = torchaudio.transforms.Spectrogram(
-        n_fft=n_fft,
-        win_length=int(audio.sample_rate * win_length / 1000),
-        hop_length=int(audio.sample_rate * hop_length / 1000),
-        power=2 if toDb else 1,
+    compute_STFT = spf.STFT(
+        sample_rate=audio.sample_rate,
+        win_length=win_length,
+        hop_length=hop_length,
+        n_fft=n_fft or int(400 * audio.sample_rate / 16000),
     )
-    spec = spectrogram(audio.signal.squeeze()).T
+    stft = compute_STFT(audio.signal.unsqueeze(0))
+    spec = spf.spectral_magnitude(stft.squeeze(), power=1)
     if toDb:
         log_spec = 10.0 * torch.log10(torch.maximum(spec, torch.tensor(1e-10)))
         log_spec = torch.maximum(log_spec, log_spec.max() - 80)
         return log_spec
     else:
         return spec
 
@@ -199,30 +199,38 @@
     save_figures: bool = False,
     n_mels: int = 20,
     n_coeff: int = 20,
     compute_deltas: bool = True,
     opensmile_feature_set: str = "eGeMAPSv02",
     opensmile_feature_level: str = "Functionals",
     return_features: bool = False,
+    mpl_backend: str = "Agg",
 ) -> ty.Tuple[ty.Dict, Path, ty.Optional[Path]]:
     """Compute features from audio file
 
     :param filename: Path to audio file
     :param subject: Subject ID
     :param task: Task ID
     :param outdir: Output directory
     :param save_figures: Whether to save figures
     :param n_mels: Number of Mel bands
     :param n_coeff: Number of MFCC coefficients
     :param compute_deltas: Whether to compute delta features
     :param opensmile_feature_set: OpenSmile feature set
     :param opensmile_feature_level: OpenSmile feature level
+    :param return_features: Whether to return features
+    :param mpl_backend: matplotlib backend
     :return: Features dictionary
     :return: Path to features
+    :return: Path to figures
     """
+    if mpl_backend is not None:
+        import matplotlib
+
+        matplotlib.use(mpl_backend)
     with open(filename, "rb") as f:
         md5sum = md5(f.read()).hexdigest()
     audio = Audio.from_file(str(filename))
     audio = audio.to_16khz()
     features_specgram = specgram(audio)
     features_melfilterbank = melfilterbank(features_specgram, n_mels=n_mels)
     features_mfcc = MFCC(features_melfilterbank, n_coeff=n_coeff, compute_deltas=compute_deltas)
```

### Comparing `b2aiprep-0.8.0/src/b2aiprep.egg-info/PKG-INFO` & `b2aiprep-0.8.1/src/b2aiprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2aiprep
-Version: 0.8.0
+Version: 0.8.1
 Summary: A small package to generate features from acoustic
 Author-email: Rahul Brito <rfbrito@mit.edu>, SenseIn Group <sensein-social@mit.edu>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `b2aiprep-0.8.0/src/tests/test_speech_to_text.py` & `b2aiprep-0.8.1/src/tests/test_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/src/tests/test_voice_converstion.py` & `b2aiprep-0.8.1/src/tests/test_voice_converstion.py`

 * *Files identical despite different names*

### Comparing `b2aiprep-0.8.0/versioneer.py` & `b2aiprep-0.8.1/versioneer.py`

 * *Files identical despite different names*

