# Comparing `tmp/openwillis-2.1.2.tar.gz` & `tmp/openwillis-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-2.1.2.tar", last modified: Mon Apr  8 13:39:18 2024, max compression
+gzip compressed data, was "openwillis-2.1.3.tar", last modified: Mon Apr  8 14:29:46 2024, max compression
```

## Comparing `openwillis-2.1.2.tar` & `openwillis-2.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.681648 openwillis-2.1.2/
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-04-08 13:38:58.000000 openwillis-2.1.2/LICENSE.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-04-08 13:38:58.000000 openwillis-2.1.2/MANIFEST.in
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 13:39:18.682073 openwillis-2.1.2/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1063 2024-04-08 13:38:58.000000 openwillis-2.1.2/README.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-04-08 13:38:58.000000 openwillis-2.1.2/RELEASE.md
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.671765 openwillis-2.1.2/openwillis/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.672893 openwillis-2.1.2/openwillis/measures/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/api.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.674466 openwillis-2.1.2/openwillis/measures/audio/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/acoustic.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.674874 openwillis-2.1.2/openwillis/measures/audio/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/config/acoustic.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/config/speech.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_separation_labels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_separation_nlabels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     4055 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_cloud.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_vosk.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5004 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_whisper.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.676668 openwillis-2.1.2/openwillis/measures/audio/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/acoustic_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/disvoice_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/separation_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/transcribe_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5939 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/whisperx_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677193 openwillis-2.1.2/openwillis/measures/commons/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/commons/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/commons/common.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677599 openwillis-2.1.2/openwillis/measures/gps/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/geolocation_processing.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677977 openwillis-2.1.2/openwillis/measures/gps/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/util/gps_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.678507 openwillis-2.1.2/openwillis/measures/text/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.678789 openwillis-2.1.2/openwillis/measures/text/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/config/text.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/speech_attribute.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.679206 openwillis-2.1.2/openwillis/measures/text/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    70717 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/util/characteristics_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.680823 openwillis-2.1.2/openwillis/measures/video/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.681402 openwillis-2.1.2/openwillis/measures/video/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/config/eye.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/config/facial.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/eye_blink.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/face_landmark.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/facial_emotion.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/usability.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.672647 openwillis-2.1.2/openwillis.egg-info/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/SOURCES.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/dependency_links.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/not-zip-safe
--rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/requires.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/top_level.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-04-08 13:38:58.000000 openwillis-2.1.2/requirements.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-04-08 13:39:18.682314 openwillis-2.1.2/setup.cfg
--rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-04-08 13:38:58.000000 openwillis-2.1.2/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.706498 openwillis-2.1.3/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-04-08 14:29:33.000000 openwillis-2.1.3/LICENSE.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-04-08 14:29:33.000000 openwillis-2.1.3/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 14:29:46.706737 openwillis-2.1.3/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1063 2024-04-08 14:29:33.000000 openwillis-2.1.3/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-04-08 14:29:33.000000 openwillis-2.1.3/RELEASE.md
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.696499 openwillis-2.1.3/openwillis/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.698049 openwillis-2.1.3/openwillis/measures/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.699649 openwillis-2.1.3/openwillis/measures/audio/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/acoustic.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.700099 openwillis-2.1.3/openwillis/measures/audio/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/config/acoustic.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/config/speech.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/speech_separation_labels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/speech_separation_nlabels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     4055 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_cloud.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_vosk.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5004 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_whisper.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.701988 openwillis-2.1.3/openwillis/measures/audio/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/acoustic_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/disvoice_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/separation_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/transcribe_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5939 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/audio/util/whisperx_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.702525 openwillis-2.1.3/openwillis/measures/commons/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/commons/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/commons/common.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.702922 openwillis-2.1.3/openwillis/measures/gps/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/gps/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/gps/geolocation_processing.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.703301 openwillis-2.1.3/openwillis/measures/gps/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/gps/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/gps/util/gps_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.703761 openwillis-2.1.3/openwillis/measures/text/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/text/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.704135 openwillis-2.1.3/openwillis/measures/text/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/text/config/text.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/text/speech_attribute.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.704522 openwillis-2.1.3/openwillis/measures/text/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/text/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    70758 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/text/util/characteristics_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.705716 openwillis-2.1.3/openwillis/measures/video/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.706250 openwillis-2.1.3/openwillis/measures/video/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/config/eye.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/config/facial.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/eye_blink.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/face_landmark.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/measures/video/facial_emotion.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-04-08 14:29:33.000000 openwillis-2.1.3/openwillis/usability.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 14:29:46.697737 openwillis-2.1.3/openwillis.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-04-08 14:29:46.000000 openwillis-2.1.3/openwillis.egg-info/top_level.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-04-08 14:29:33.000000 openwillis-2.1.3/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-04-08 14:29:46.706971 openwillis-2.1.3/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-04-08 14:29:33.000000 openwillis-2.1.3/setup.py
```

### Comparing `openwillis-2.1.2/LICENSE.txt` & `openwillis-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/PKG-INFO` & `openwillis-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.2
+Version: 2.1.3
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-2.1.2/README.md` & `openwillis-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/__init__.py` & `openwillis-2.1.3/openwillis/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/api.py` & `openwillis-2.1.3/openwillis/measures/api.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/__init__.py` & `openwillis-2.1.3/openwillis/measures/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/acoustic.py` & `openwillis-2.1.3/openwillis/measures/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/config/acoustic.json` & `openwillis-2.1.3/openwillis/measures/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/config/speech.json` & `openwillis-2.1.3/openwillis/measures/audio/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/speech_separation_labels.py` & `openwillis-2.1.3/openwillis/measures/audio/speech_separation_labels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/speech_separation_nlabels.py` & `openwillis-2.1.3/openwillis/measures/audio/speech_separation_nlabels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_cloud.py` & `openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_cloud.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_vosk.py` & `openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_vosk.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_whisper.py` & `openwillis-2.1.3/openwillis/measures/audio/speech_transcribe_whisper.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/acoustic_util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/acoustic_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/disvoice_util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/disvoice_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/separation_util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/separation_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/transcribe_util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/transcribe_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/audio/util/whisperx_util.py` & `openwillis-2.1.3/openwillis/measures/audio/util/whisperx_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/commons/common.py` & `openwillis-2.1.3/openwillis/measures/commons/common.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/gps/geolocation_processing.py` & `openwillis-2.1.3/openwillis/measures/gps/geolocation_processing.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/gps/util/gps_util.py` & `openwillis-2.1.3/openwillis/measures/gps/util/gps_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/text/config/text.json` & `openwillis-2.1.3/openwillis/measures/text/config/text.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/text/speech_attribute.py` & `openwillis-2.1.3/openwillis/measures/text/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/text/util/characteristics_util.py` & `openwillis-2.1.3/openwillis/measures/text/util/characteristics_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -761,23 +761,23 @@
     """
     tag_list = nltk.pos_tag(word_list)
     
     tag_list_pos = [TAG_DICT[tag[1]] if tag[1] in TAG_DICT.keys() else "Other" for tag in tag_list]
     word_df[measures["part_of_speech"]] = tag_list_pos
 
     word_df[measures["first_person"]] = [word in FIRST_PERSON_PRONOUNS for word in word_list]
-    # make non pronouns None
-    word_df[measures["first_person"]] = word_df[measures["first_person"]].where(word_df[measures["part_of_speech"]] == "Pronoun", None)
+    # make non pronouns NaN
+    word_df[measures["first_person"]] = word_df[measures["first_person"]].where(word_df[measures["part_of_speech"]] == "Pronoun", np.nan)
 
     present_tense = ["VBP", "VBZ"]
     past_tense = ["VBD", "VBN"]
     tag_list_verb = ["Present" if tag[1] in present_tense else "Past" if tag[1] in past_tense else "Other" for tag in tag_list]
     word_df[measures["verb_tense"]] = tag_list_verb
-    # make non verbs None
-    word_df[measures["verb_tense"]] = word_df[measures["verb_tense"]].where(word_df[measures["part_of_speech"]] == "Verb", None)
+    # make non verbs NaN
+    word_df[measures["verb_tense"]] = word_df[measures["verb_tense"]].where(word_df[measures["part_of_speech"]] == "Verb", np.nan)
 
     return word_df
 
 def calculate_first_person_sentiment(df, measures):
     """
     ------------------------------------------------------------------------------------------------------
 
@@ -1334,16 +1334,16 @@
     float
         The calculated pseudo-perplexity of the input text.
 
     ------------------------------------------------------------------------------------------------------
     """
     # Tokenize input text
     clean_text = text.translate(str.maketrans('', '', string.punctuation))
-    clean_text = re.sub(r'\s+', ' ', clean_text)
-    if len(clean_text) == 0:
+    clean_text = re.sub(r'\s+', ' ', clean_text).strip()
+    if len(clean_text) == 0 or len(clean_text.split()) < 2:
         return np.nan
 
     tokens = tokenizer(clean_text, return_tensors='pt')
     input_ids = tokens.input_ids
     masked_input_ids = input_ids.clone()
 
     log_probs = []
@@ -1414,15 +1414,15 @@
     """
     if sentence_encoder is not None and len(phrases_texts) > 0:
         phrase_embeddings = sentence_encoder.encode(phrases_texts)
         similarity_matrix = cosine_similarity(phrase_embeddings)
 
         # calculate semantic similarity of each phrase to the immediately preceding phrase
         if len(phrases_texts) > 1:
-            sentence_tangeniality1 = np.mean([similarity_matrix[j, j-1] for j in range(1, len(phrases_texts))])
+            sentence_tangeniality1 = np.mean([similarity_matrix[j-1, j] for j in range(1, len(phrases_texts))])
         else:
             sentence_tangeniality1 = np.nan
 
         # calculate semantic similarity of each phrase to the phrase 2 turns before
         if len(phrases_texts) > 2:
             sentence_tangeniality2 = np.mean([similarity_matrix[j-2, j] for j in range(2, len(phrases_texts))])
         else:
```

### Comparing `openwillis-2.1.2/openwillis/measures/video/config/facial.json` & `openwillis-2.1.3/openwillis/measures/video/config/facial.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/video/eye_blink.py` & `openwillis-2.1.3/openwillis/measures/video/eye_blink.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/video/face_landmark.py` & `openwillis-2.1.3/openwillis/measures/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis/measures/video/facial_emotion.py` & `openwillis-2.1.3/openwillis/measures/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/openwillis.egg-info/PKG-INFO` & `openwillis-2.1.3/openwillis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.2
+Version: 2.1.3
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-2.1.2/openwillis.egg-info/SOURCES.txt` & `openwillis-2.1.3/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.2/setup.py` & `openwillis-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='2.1.2',
+                 version='2.1.3',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6',
                  install_requires=install_requires,
```

