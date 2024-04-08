# Comparing `tmp/openwillis-2.1.1.tar.gz` & `tmp/openwillis-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-2.1.1.tar", last modified: Fri Mar 22 13:15:06 2024, max compression
+gzip compressed data, was "openwillis-2.1.2.tar", last modified: Mon Apr  8 13:39:18 2024, max compression
```

## Comparing `openwillis-2.1.1.tar` & `openwillis-2.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.653932 openwillis-2.1.1/
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-03-22 13:14:53.000000 openwillis-2.1.1/LICENSE.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-03-22 13:14:53.000000 openwillis-2.1.1/MANIFEST.in
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1255 2024-03-22 13:15:06.654000 openwillis-2.1.1/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)      956 2024-03-22 13:14:53.000000 openwillis-2.1.1/README.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-03-22 13:14:53.000000 openwillis-2.1.1/RELEASE.md
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.647972 openwillis-2.1.1/openwillis/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.648969 openwillis-2.1.1/openwillis/measures/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/api.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.649959 openwillis-2.1.1/openwillis/measures/audio/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/acoustic.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.650328 openwillis-2.1.1/openwillis/measures/audio/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/config/acoustic.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/config/speech.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/speech_separation_labels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/speech_separation_nlabels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     4055 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_cloud.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_vosk.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5004 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_whisper.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.651403 openwillis-2.1.1/openwillis/measures/audio/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/acoustic_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/disvoice_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/separation_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/transcribe_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5939 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/audio/util/whisperx_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.651643 openwillis-2.1.1/openwillis/measures/commons/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/commons/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/commons/common.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.651866 openwillis-2.1.1/openwillis/measures/gps/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/gps/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/gps/geolocation_processing.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.652082 openwillis-2.1.1/openwillis/measures/gps/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/gps/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/gps/util/gps_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.652327 openwillis-2.1.1/openwillis/measures/text/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/text/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.652483 openwillis-2.1.1/openwillis/measures/text/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/text/config/text.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/text/speech_attribute.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.652804 openwillis-2.1.1/openwillis/measures/text/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/text/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    70393 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/text/util/characteristics_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.653371 openwillis-2.1.1/openwillis/measures/video/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.653740 openwillis-2.1.1/openwillis/measures/video/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/config/eye.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/config/facial.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/eye_blink.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/face_landmark.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/measures/video/facial_emotion.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-03-22 13:14:53.000000 openwillis-2.1.1/openwillis/usability.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-03-22 13:15:06.648737 openwillis-2.1.1/openwillis.egg-info/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1255 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/SOURCES.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/dependency_links.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/not-zip-safe
--rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/requires.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-03-22 13:15:06.000000 openwillis-2.1.1/openwillis.egg-info/top_level.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-03-22 13:14:53.000000 openwillis-2.1.1/requirements.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-03-22 13:15:06.654188 openwillis-2.1.1/setup.cfg
--rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-03-22 13:14:54.000000 openwillis-2.1.1/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.681648 openwillis-2.1.2/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-04-08 13:38:58.000000 openwillis-2.1.2/LICENSE.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-04-08 13:38:58.000000 openwillis-2.1.2/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 13:39:18.682073 openwillis-2.1.2/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1063 2024-04-08 13:38:58.000000 openwillis-2.1.2/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-04-08 13:38:58.000000 openwillis-2.1.2/RELEASE.md
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.671765 openwillis-2.1.2/openwillis/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.672893 openwillis-2.1.2/openwillis/measures/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.674466 openwillis-2.1.2/openwillis/measures/audio/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/acoustic.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.674874 openwillis-2.1.2/openwillis/measures/audio/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/config/acoustic.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/config/speech.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_separation_labels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_separation_nlabels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     4055 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_cloud.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_vosk.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5004 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_whisper.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.676668 openwillis-2.1.2/openwillis/measures/audio/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/acoustic_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/disvoice_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/separation_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/transcribe_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5939 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/audio/util/whisperx_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677193 openwillis-2.1.2/openwillis/measures/commons/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/commons/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/commons/common.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677599 openwillis-2.1.2/openwillis/measures/gps/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/geolocation_processing.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.677977 openwillis-2.1.2/openwillis/measures/gps/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/gps/util/gps_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.678507 openwillis-2.1.2/openwillis/measures/text/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.678789 openwillis-2.1.2/openwillis/measures/text/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/config/text.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/speech_attribute.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.679206 openwillis-2.1.2/openwillis/measures/text/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    70717 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/text/util/characteristics_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.680823 openwillis-2.1.2/openwillis/measures/video/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.681402 openwillis-2.1.2/openwillis/measures/video/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/config/eye.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/config/facial.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/eye_blink.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/face_landmark.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/measures/video/facial_emotion.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-04-08 13:38:58.000000 openwillis-2.1.2/openwillis/usability.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 13:39:18.672647 openwillis-2.1.2/openwillis.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-04-08 13:39:18.000000 openwillis-2.1.2/openwillis.egg-info/top_level.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-04-08 13:38:58.000000 openwillis-2.1.2/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-04-08 13:39:18.682314 openwillis-2.1.2/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-04-08 13:38:58.000000 openwillis-2.1.2/setup.py
```

### Comparing `openwillis-2.1.1/LICENSE.txt` & `openwillis-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/PKG-INFO` & `openwillis-2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.1
+Version: 2.1.2
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<img src="https://github.com/bklynhlth/openwillis/blob/main/resources/willis-openwillis.png" width="150">
+
 OpenWillis is a python library for digital health measurement.
 
 It was developed by [Brooklyn Health](https://brooklyn.health/openwillis) to establish standardized methods in digital phenotyping and make them open and accessible to the scientific community.
 
 It is freely available for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
```

### Comparing `openwillis-2.1.1/README.md` & `openwillis-2.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<img src="https://github.com/bklynhlth/openwillis/blob/main/resources/willis-openwillis.png" width="150">
+
 OpenWillis is a python library for digital health measurement.
 
 It was developed by [Brooklyn Health](https://brooklyn.health/openwillis) to establish standardized methods in digital phenotyping and make them open and accessible to the scientific community.
 
 It is freely available for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
```

### Comparing `openwillis-2.1.1/openwillis/__init__.py` & `openwillis-2.1.2/openwillis/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/api.py` & `openwillis-2.1.2/openwillis/measures/api.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/__init__.py` & `openwillis-2.1.2/openwillis/measures/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/acoustic.py` & `openwillis-2.1.2/openwillis/measures/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/config/acoustic.json` & `openwillis-2.1.2/openwillis/measures/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/config/speech.json` & `openwillis-2.1.2/openwillis/measures/audio/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/speech_separation_labels.py` & `openwillis-2.1.2/openwillis/measures/audio/speech_separation_labels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/speech_separation_nlabels.py` & `openwillis-2.1.2/openwillis/measures/audio/speech_separation_nlabels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_cloud.py` & `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_cloud.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_vosk.py` & `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_vosk.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/speech_transcribe_whisper.py` & `openwillis-2.1.2/openwillis/measures/audio/speech_transcribe_whisper.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/acoustic_util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/acoustic_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/disvoice_util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/disvoice_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/separation_util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/separation_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/transcribe_util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/transcribe_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/audio/util/whisperx_util.py` & `openwillis-2.1.2/openwillis/measures/audio/util/whisperx_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/commons/common.py` & `openwillis-2.1.2/openwillis/measures/commons/common.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/gps/geolocation_processing.py` & `openwillis-2.1.2/openwillis/measures/gps/geolocation_processing.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/gps/util/gps_util.py` & `openwillis-2.1.2/openwillis/measures/gps/util/gps_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/text/config/text.json` & `openwillis-2.1.2/openwillis/measures/text/config/text.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/text/speech_attribute.py` & `openwillis-2.1.2/openwillis/measures/text/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/text/util/characteristics_util.py` & `openwillis-2.1.2/openwillis/measures/text/util/characteristics_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1134,15 +1134,14 @@
         word_embeddings = []
         for chunk in word_list:
             inputs = tokenizer(chunk, return_tensors='pt', padding=True)
             outputs = model(**inputs)
             word_embeddings.append(outputs.last_hidden_state.mean(1).detach().numpy())
         word_embeddings = np.concatenate(word_embeddings, axis=0)
     else:
-
         inputs = tokenizer(word_list, return_tensors='pt', padding=True)
         outputs = model(**inputs)
         # Average pooling of the hidden states
         word_embeddings = outputs.last_hidden_state.mean(1).detach().numpy()
     return word_embeddings
 
 def get_word_coherence_utterance(row, tokenizer, model, measures):
@@ -1172,14 +1171,18 @@
         A list containing the calculated semantic similarity of each word in 10-words window.
     word_word_variability: dict
         A dictionary containing the calculated word-to-word variability at k inter-word distances.
 
     ------------------------------------------------------------------------------------------------------
     """
     words_texts = row[measures['words_texts']]
+    if len(words_texts) == 0:
+        # return empty lists if no words in the utterance
+        return [np.nan]*len(words_texts), [np.nan]*len(words_texts), [np.nan]*len(words_texts), {k: [np.nan]*len(words_texts) for k in range(2, 11)}
+
     word_embeddings = get_word_embeddings(words_texts, tokenizer, model)
     similarity_matrix = cosine_similarity(word_embeddings)
 
     # calculate semantic similarity of each word to the immediately preceding word
     if len(words_texts) > 1:
         word_coherence = [np.nan] + [similarity_matrix[j, j-1] for j in range(1, len(words_texts))]
     else:
@@ -1332,14 +1335,16 @@
         The calculated pseudo-perplexity of the input text.
 
     ------------------------------------------------------------------------------------------------------
     """
     # Tokenize input text
     clean_text = text.translate(str.maketrans('', '', string.punctuation))
     clean_text = re.sub(r'\s+', ' ', clean_text)
+    if len(clean_text) == 0:
+        return np.nan
 
     tokens = tokenizer(clean_text, return_tensors='pt')
     input_ids = tokens.input_ids
     masked_input_ids = input_ids.clone()
 
     log_probs = []
     # Iterate over each token in the input
@@ -1351,29 +1356,31 @@
             start = i - 256
         if i > input_ids.size(1) - 256:
             end = input_ids.size(1)
         else:
             end = i + 256
 
         masked_input_ids[0, i] = tokenizer.mask_token_id
-        
-        input_ids2 = input_ids[:, start:end]
-        masked_input_ids2 = masked_input_ids[:, start:end]
+
+        input_ids2 = input_ids[:, start:(end+1)]
+        masked_input_ids2 = masked_input_ids[:, start:(end+1)]
+        # get new i from that
+        idx = i - start
 
         with torch.no_grad():
             outputs = model(input_ids=masked_input_ids2, labels=input_ids2)
-        
+
         # Calculate log probability of the original token
-        logit_prob = outputs.logits[0, i].softmax(dim=0)
+        logit_prob = outputs.logits[0, idx].softmax(dim=0)
         true_log_prob = logit_prob[input_ids[0, i]].log().item()
         log_probs.append(true_log_prob)
-        
+
         # Unmask the token for the next iteration
         masked_input_ids[0, i] = input_ids[0, i]
-    
+
     # Calculate perplexity
     perplexity = np.exp(-np.mean(log_probs))
     return perplexity
 
 def calculate_phrase_tangeniality(phrases_texts, utterance_text, sentence_encoder, bert, tokenizer):
     """
     ------------------------------------------------------------------------------------------------------
```

### Comparing `openwillis-2.1.1/openwillis/measures/video/config/facial.json` & `openwillis-2.1.2/openwillis/measures/video/config/facial.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/video/eye_blink.py` & `openwillis-2.1.2/openwillis/measures/video/eye_blink.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/video/face_landmark.py` & `openwillis-2.1.2/openwillis/measures/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis/measures/video/facial_emotion.py` & `openwillis-2.1.2/openwillis/measures/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/openwillis.egg-info/PKG-INFO` & `openwillis-2.1.2/openwillis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.1
+Version: 2.1.2
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+<img src="https://github.com/bklynhlth/openwillis/blob/main/resources/willis-openwillis.png" width="150">
+
 OpenWillis is a python library for digital health measurement.
 
 It was developed by [Brooklyn Health](https://brooklyn.health/openwillis) to establish standardized methods in digital phenotyping and make them open and accessible to the scientific community.
 
 It is freely available for non-commercial use ([see license](https://github.com/bklynhlth/openwillis/blob/main/LICENSE.txt)).
```

### Comparing `openwillis-2.1.1/openwillis.egg-info/SOURCES.txt` & `openwillis-2.1.2/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.1/setup.py` & `openwillis-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='2.1.1',
+                 version='2.1.2',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6',
                  install_requires=install_requires,
```

