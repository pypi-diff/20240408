# Comparing `tmp/mediagrains-5.0.0.tar.gz` & `tmp/mediagrains-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediagrains-5.0.0.tar", last modified: Tue Jan 30 14:47:08 2024, max compression
+gzip compressed data, was "mediagrains-5.1.0.tar", last modified: Mon Apr  8 15:40:27 2024, max compression
```

## Comparing `mediagrains-5.0.0.tar` & `mediagrains-5.1.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.365681 mediagrains-5.0.0/
--rw-r--r--   0 root         (0) root         (0)      573 2024-01-30 14:43:30.000000 mediagrains-5.0.0/COPYING
--rw-r--r--   0 root         (0) root         (0)     6607 2024-01-30 14:43:30.000000 mediagrains-5.0.0/ICLA.md
--rw-r--r--   0 root         (0) root         (0)    11362 2024-01-30 14:43:30.000000 mediagrains-5.0.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-30 14:43:30.000000 mediagrains-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      552 2024-01-30 14:47:08.365681 mediagrains-5.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10358 2024-01-30 14:43:30.000000 mediagrains-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.341681 mediagrains-5.0.0/examples/
--rw-r--r--   0 root         (0) root         (0)    62845 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/audio_7.gsf
--rw-r--r--   0 root         (0) root         (0)    62705 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/audio_8.gsf
--rw-r--r--   0 root         (0) root         (0)     8295 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/coded_audio_7.gsf
--rw-r--r--   0 root         (0) root         (0)     8155 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/coded_audio_8.gsf
--rw-r--r--   0 root         (0) root         (0)    68457 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/coded_video_7.gsf
--rw-r--r--   0 root         (0) root         (0)    68317 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/coded_video_8.gsf
--rw-r--r--   0 root         (0) root         (0)    68317 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/coded_video_9.gsf
--rw-r--r--   0 root         (0) root         (0)    37610 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/event_7.gsf
--rw-r--r--   0 root         (0) root         (0)    37570 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/event_8.gsf
--rw-r--r--   0 root         (0) root         (0) 25011059 2024-01-30 14:43:30.000000 mediagrains-5.0.0/examples/interleaved_7.gsf
--rw-r--r--   0 root         (0) root         (0) 25010569 2024-01-30 14:43:31.000000 mediagrains-5.0.0/examples/interleaved_8.gsf
--rw-r--r--   0 root         (0) root         (0)  1946205 2024-01-30 14:43:31.000000 mediagrains-5.0.0/examples/video_7.gsf
--rw-r--r--   0 root         (0) root         (0)  1946635 2024-01-30 14:43:31.000000 mediagrains-5.0.0/examples/video_8.gsf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.345681 mediagrains-5.0.0/mediagrains/
--rw-r--r--   0 root         (0) root         (0)     1820 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/__init__.py
--rw-r--r--   0 root         (0) root         (0)      100 2024-01-30 14:46:59.000000 mediagrains-5.0.0/mediagrains/_version.py
--rw-r--r--   0 root         (0) root         (0)     5644 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/cogenums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.349681 mediagrains-5.0.0/mediagrains/comparison/
--rw-r--r--   0 root         (0) root         (0)     2321 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1435 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/__main__.py
--rw-r--r--   0 root         (0) root         (0)    42508 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/_internal.py
--rw-r--r--   0 root         (0) root         (0)     8221 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/options.py
--rw-r--r--   0 root         (0) root         (0)     5699 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/psnr.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/comparison/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.349681 mediagrains-5.0.0/mediagrains/grains/
--rw-r--r--   0 root         (0) root         (0)     8158 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/AudioGrain.py
--rw-r--r--   0 root         (0) root         (0)     8807 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/CodedAudioGrain.py
--rw-r--r--   0 root         (0) root         (0)    16479 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/CodedVideoGrain.py
--rw-r--r--   0 root         (0) root         (0)    11074 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/EventGrain.py
--rw-r--r--   0 root         (0) root         (0)    27612 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/Grain.py
--rw-r--r--   0 root         (0) root         (0)    20331 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/VideoGrain.py
--rw-r--r--   0 root         (0) root         (0)      530 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/grains/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97541 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/gsf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.349681 mediagrains-5.0.0/mediagrains/hypothesis/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/hypothesis/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/hypothesis/py.typed
--rw-r--r--   0 root         (0) root         (0)    36636 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/hypothesis/strategies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.353681 mediagrains-5.0.0/mediagrains/numpy/
--rw-r--r--   0 root         (0) root         (0)      830 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21960 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/convert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.353681 mediagrains-5.0.0/mediagrains/numpy/numpy_grains/
--rw-r--r--   0 root         (0) root         (0)     8748 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/numpy_grains/AudioGrain.py
--rw-r--r--   0 root         (0) root         (0)    18875 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/numpy_grains/VideoGrain.py
--rw-r--r--   0 root         (0) root         (0)      110 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/numpy_grains/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/numpy/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.353681 mediagrains-5.0.0/mediagrains/patterngenerators/
--rw-r--r--   0 root         (0) root         (0)      881 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4538 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.353681 mediagrains-5.0.0/mediagrains/patterngenerators/audio/
--rw-r--r--   0 root         (0) root         (0)      747 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/audio/abc.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/audio/py.typed
--rw-r--r--   0 root         (0) root         (0)     8580 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/audio/tone.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.357681 mediagrains-5.0.0/mediagrains/patterngenerators/video/
--rw-r--r--   0 root         (0) root         (0)      905 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1626 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/abc.py
--rw-r--r--   0 root         (0) root         (0)     3153 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/colourbars.py
--rw-r--r--   0 root         (0) root         (0)     1839 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/constants.py
--rw-r--r--   0 root         (0) root         (0)     3302 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/lumasteps.py
--rw-r--r--   0 root         (0) root         (0)     4773 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/movingbaroverlay.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/py.typed
--rw-r--r--   0 root         (0) root         (0)     1650 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/patterngenerators/video/still.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.357681 mediagrains-5.0.0/mediagrains/tools/
--rw-r--r--   0 root         (0) root         (0)      866 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/tools/_file_or_pipe.py
--rw-r--r--   0 root         (0) root         (0)     4115 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/tools/extract_from_gsf.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/tools/py.typed
--rw-r--r--   0 root         (0) root         (0)     7917 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/tools/wrap_in_gsf.py
--rw-r--r--   0 root         (0) root         (0)     8851 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.361681 mediagrains-5.0.0/mediagrains/utils/
--rw-r--r--   0 root         (0) root         (0)      855 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4376 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/adts_aac_grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2685 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/adts_aac_parser.py
--rw-r--r--   0 root         (0) root         (0)    12766 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/asyncbinaryio.py
--rw-r--r--   0 root         (0) root         (0)     2416 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     6988 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/h264_grain_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    31694 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/h264_parser.py
--rw-r--r--   0 root         (0) root         (0)     6642 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/iobytes.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/mediagrains/utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.361681 mediagrains-5.0.0/mediagrains.egg-info/
--rw-r--r--   0 root         (0) root         (0)      552 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2960 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-01-30 14:47:08.000000 mediagrains-5.0.0/mediagrains.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-30 14:47:08.365681 mediagrains-5.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2547 2024-01-30 14:43:31.000000 mediagrains-5.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:47:08.361681 mediagrains-5.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4625 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/audio_utils.py
--rw-r--r--   0 root         (0) root         (0)     4586 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     1812 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_adts_aac_parser.py
--rw-r--r--   0 root         (0) root         (0)     7043 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_audio_psnr.py
--rw-r--r--   0 root         (0) root         (0)    11132 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_comparison.py
--rw-r--r--   0 root         (0) root         (0)    84610 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_grain.py
--rw-r--r--   0 root         (0) root         (0)   128793 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_gsf.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_iobytes.py
--rw-r--r--   0 root         (0) root         (0)     8694 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_numpy_audiograin.py
--rw-r--r--   0 root         (0) root         (0)    41583 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_numpy_videograin.py
--rw-r--r--   0 root         (0) root         (0)    29864 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_patterngenerators.py
--rw-r--r--   0 root         (0) root         (0)     8283 2024-01-30 14:43:31.000000 mediagrains-5.0.0/tests/test_video_psnr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.825195 mediagrains-5.1.0/
+-rw-r--r--   0 root         (0) root         (0)      573 2024-04-08 15:36:56.000000 mediagrains-5.1.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)     6607 2024-04-08 15:36:56.000000 mediagrains-5.1.0/ICLA.md
+-rw-r--r--   0 root         (0) root         (0)    11362 2024-04-08 15:36:56.000000 mediagrains-5.1.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-08 15:36:56.000000 mediagrains-5.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-08 15:40:27.825195 mediagrains-5.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10358 2024-04-08 15:36:56.000000 mediagrains-5.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.805195 mediagrains-5.1.0/examples/
+-rw-r--r--   0 root         (0) root         (0)    62845 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/audio_7.gsf
+-rw-r--r--   0 root         (0) root         (0)    62705 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/audio_8.gsf
+-rw-r--r--   0 root         (0) root         (0)     8295 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/coded_audio_7.gsf
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/coded_audio_8.gsf
+-rw-r--r--   0 root         (0) root         (0)    68457 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/coded_video_7.gsf
+-rw-r--r--   0 root         (0) root         (0)    68317 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/coded_video_8.gsf
+-rw-r--r--   0 root         (0) root         (0)    68317 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/coded_video_9.gsf
+-rw-r--r--   0 root         (0) root         (0)    37610 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/event_7.gsf
+-rw-r--r--   0 root         (0) root         (0)    37570 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/event_8.gsf
+-rw-r--r--   0 root         (0) root         (0) 25011059 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/interleaved_7.gsf
+-rw-r--r--   0 root         (0) root         (0) 25010569 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/interleaved_8.gsf
+-rw-r--r--   0 root         (0) root         (0)  1946205 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/video_7.gsf
+-rw-r--r--   0 root         (0) root         (0)  1946635 2024-04-08 15:36:56.000000 mediagrains-5.1.0/examples/video_8.gsf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.809195 mediagrains-5.1.0/mediagrains/
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-08 15:40:18.000000 mediagrains-5.1.0/mediagrains/_version.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/cogenums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.809195 mediagrains-5.1.0/mediagrains/comparison/
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42508 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/_internal.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/options.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/psnr.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/comparison/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.813195 mediagrains-5.1.0/mediagrains/grains/
+-rw-r--r--   0 root         (0) root         (0)     8158 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/AudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)     8807 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/CodedAudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)    17739 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/CodedVideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)    11074 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/EventGrain.py
+-rw-r--r--   0 root         (0) root         (0)    28354 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/Grain.py
+-rw-r--r--   0 root         (0) root         (0)    20331 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/VideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)      530 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/grains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97541 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/gsf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.813195 mediagrains-5.1.0/mediagrains/hypothesis/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/hypothesis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/hypothesis/py.typed
+-rw-r--r--   0 root         (0) root         (0)    36910 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/hypothesis/strategies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.813195 mediagrains-5.1.0/mediagrains/numpy/
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21960 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/convert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.813195 mediagrains-5.1.0/mediagrains/numpy/numpy_grains/
+-rw-r--r--   0 root         (0) root         (0)     8748 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/numpy_grains/AudioGrain.py
+-rw-r--r--   0 root         (0) root         (0)    18875 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/numpy_grains/VideoGrain.py
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/numpy_grains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/numpy/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.817195 mediagrains-5.1.0/mediagrains/patterngenerators/
+-rw-r--r--   0 root         (0) root         (0)      881 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4538 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.817195 mediagrains-5.1.0/mediagrains/patterngenerators/audio/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/audio/abc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/audio/py.typed
+-rw-r--r--   0 root         (0) root         (0)     8580 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/audio/tone.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.817195 mediagrains-5.1.0/mediagrains/patterngenerators/video/
+-rw-r--r--   0 root         (0) root         (0)      905 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/abc.py
+-rw-r--r--   0 root         (0) root         (0)     3153 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/colourbars.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/lumasteps.py
+-rw-r--r--   0 root         (0) root         (0)     4773 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/movingbaroverlay.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/patterngenerators/video/still.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.821195 mediagrains-5.1.0/mediagrains/tools/
+-rw-r--r--   0 root         (0) root         (0)      866 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/tools/_file_or_pipe.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/tools/extract_from_gsf.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/tools/py.typed
+-rw-r--r--   0 root         (0) root         (0)     7917 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/tools/wrap_in_gsf.py
+-rw-r--r--   0 root         (0) root         (0)     8851 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.821195 mediagrains-5.1.0/mediagrains/utils/
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/adts_aac_grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/adts_aac_parser.py
+-rw-r--r--   0 root         (0) root         (0)    12766 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/asyncbinaryio.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     6988 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/h264_grain_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    31694 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/h264_parser.py
+-rw-r--r--   0 root         (0) root         (0)     6642 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/iobytes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/mediagrains/utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.825195 mediagrains-5.1.0/mediagrains.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-08 15:40:27.000000 mediagrains-5.1.0/mediagrains.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 15:40:27.825195 mediagrains-5.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2547 2024-04-08 15:36:56.000000 mediagrains-5.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 15:40:27.825195 mediagrains-5.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/audio_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_adts_aac_parser.py
+-rw-r--r--   0 root         (0) root         (0)     7043 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_audio_psnr.py
+-rw-r--r--   0 root         (0) root         (0)    11132 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_comparison.py
+-rw-r--r--   0 root         (0) root         (0)    84610 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_grain.py
+-rw-r--r--   0 root         (0) root         (0)   128793 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_gsf.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_iobytes.py
+-rw-r--r--   0 root         (0) root         (0)     8694 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_numpy_audiograin.py
+-rw-r--r--   0 root         (0) root         (0)    41583 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_numpy_videograin.py
+-rw-r--r--   0 root         (0) root         (0)    29864 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_patterngenerators.py
+-rw-r--r--   0 root         (0) root         (0)     8283 2024-04-08 15:36:56.000000 mediagrains-5.1.0/tests/test_video_psnr.py
```

### Comparing `mediagrains-5.0.0/COPYING` & `mediagrains-5.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/ICLA.md` & `mediagrains-5.1.0/ICLA.md`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/LICENSE.md` & `mediagrains-5.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/PKG-INFO` & `mediagrains-5.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediagrains
-Version: 5.0.0
+Version: 5.1.0
 Summary: Simple utility for grain-based media
 Home-page: https://github.com/bbc/rd-apmm-python-lib-mediagrains
 Author: BBC R&D
 Author-email: cloudfit-opensource@rd.bbc.co.uk
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE.md
```

### Comparing `mediagrains-5.0.0/README.md` & `mediagrains-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/audio_7.gsf` & `mediagrains-5.1.0/examples/audio_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/audio_8.gsf` & `mediagrains-5.1.0/examples/audio_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/coded_audio_7.gsf` & `mediagrains-5.1.0/examples/coded_audio_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/coded_audio_8.gsf` & `mediagrains-5.1.0/examples/coded_audio_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/coded_video_7.gsf` & `mediagrains-5.1.0/examples/coded_video_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/coded_video_8.gsf` & `mediagrains-5.1.0/examples/coded_video_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/coded_video_9.gsf` & `mediagrains-5.1.0/examples/coded_video_9.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/event_7.gsf` & `mediagrains-5.1.0/examples/event_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/event_8.gsf` & `mediagrains-5.1.0/examples/event_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/interleaved_7.gsf` & `mediagrains-5.1.0/examples/interleaved_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/interleaved_8.gsf` & `mediagrains-5.1.0/examples/interleaved_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/video_7.gsf` & `mediagrains-5.1.0/examples/video_7.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/examples/video_8.gsf` & `mediagrains-5.1.0/examples/video_8.gsf`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/__init__.py` & `mediagrains-5.1.0/mediagrains/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/cogenums.py` & `mediagrains-5.1.0/mediagrains/cogenums.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/comparison/__init__.py` & `mediagrains-5.1.0/mediagrains/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/comparison/__main__.py` & `mediagrains-5.1.0/mediagrains/comparison/__main__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/comparison/_internal.py` & `mediagrains-5.1.0/mediagrains/comparison/_internal.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/comparison/options.py` & `mediagrains-5.1.0/mediagrains/comparison/options.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/comparison/psnr.py` & `mediagrains-5.1.0/mediagrains/comparison/psnr.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/grains/AudioGrain.py` & `mediagrains-5.1.0/mediagrains/grains/AudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/grains/CodedAudioGrain.py` & `mediagrains-5.1.0/mediagrains/grains/CodedAudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/grains/CodedVideoGrain.py` & `mediagrains-5.1.0/mediagrains/grains/CodedVideoGrain.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Union,
     Optional,
     overload,
     cast,
     Sized,
     Iterable)
 from uuid import UUID
-from mediatimestamp.immutable import Timestamp, SupportsMediaTimestamp, mediatimestamp
+from mediatimestamp.immutable import Timestamp, TimeRange, SupportsMediaTimestamp, mediatimestamp
 from ..typing import (
     CodedVideoGrainMetadataDict,
     FractionDict,
     GrainDataParameterType,
     RationalTypes)
 
 from ..cogenums import CogFrameFormat, CogFrameLayout
@@ -408,7 +408,37 @@
 
     @property
     def media_rate(self) -> Optional[Fraction]:
         if self.rate:
             return self.rate
         else:
             return None
+
+    @property
+    def presentation_origin_timestamp(self) -> Timestamp:
+        if self.rate is not None and self.temporal_offset is not None:
+            return self.origin_timestamp + Timestamp.from_count(self.temporal_offset, self.rate)
+        else:
+            return self.origin_timestamp
+
+    def final_presentation_origin_timestamp(self) -> Timestamp:
+        if self.rate is not None and self.temporal_offset is not None:
+            return self.final_origin_timestamp() + Timestamp.from_count(self.temporal_offset, self.rate)
+        else:
+            return self.final_origin_timestamp()
+
+    def presentation_origin_timerange(self) -> TimeRange:
+        origin_tr = self.origin_timerange()
+        if self.rate is not None and self.temporal_offset is not None:
+            if origin_tr.start is not None:
+                start = origin_tr.start + Timestamp.from_count(self.temporal_offset, self.rate)
+            else:
+                start = None
+
+            if origin_tr.end is not None:
+                end = origin_tr.end + Timestamp.from_count(self.temporal_offset, self.rate)
+            else:
+                end = None
+
+            return TimeRange(start, end, origin_tr.inclusivity)
+        else:
+            return origin_tr
```

### Comparing `mediagrains-5.0.0/mediagrains/grains/EventGrain.py` & `mediagrains-5.1.0/mediagrains/grains/EventGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/grains/Grain.py` & `mediagrains-5.1.0/mediagrains/grains/Grain.py`

 * *Files 3% similar despite different names*

```diff
@@ -247,14 +247,24 @@
 final_origin_timestamp()
     The origin timestamp of the final sample in the grain. For most grain types this is the same as
     origin_timestamp, but not for audio grains.
 
 origin_timerange()
     The origin time range covered by the samples in the grain.
 
+presentation_origin_timestamp
+    The presentation timeline origin timestamp for the grain.
+
+final_presentation_origin_timestamp()
+    The presentation origin timestamp of the final sample in the grain. For most grain types this is the same as
+    presentation_origin_timestamp, but not for audio grains.
+
+presentation_origin_timerange()
+    The presentation timeline origin time range covered by the samples in the grain.
+
 normalise_time(value)
     Returns a normalised Timestamp, TimeOffset or TimeRange using the media rate.
 
 media_rate
     The video frame rate or audio sample rate as a Fraction or None. Returns None if there is no media
     rate or the media rate == 0.
 
@@ -445,14 +455,24 @@
 
     def final_origin_timestamp(self) -> Timestamp:
         return self.origin_timestamp
 
     def origin_timerange(self) -> TimeRange:
         return TimeRange(self.origin_timestamp, self.final_origin_timestamp(), TimeRange.INCLUSIVE)
 
+    @property
+    def presentation_origin_timestamp(self) -> Timestamp:
+        return self.origin_timestamp
+
+    def final_presentation_origin_timestamp(self) -> Timestamp:
+        return self.final_origin_timestamp()
+
+    def presentation_origin_timerange(self) -> TimeRange:
+        return self.origin_timerange()
+
     @overload
     def normalise_time(self, value: TimeOffset) -> TimeOffset: ...
 
     @overload
     def normalise_time(self, value: TimeRange) -> TimeRange: ...
 
     def normalise_time(self, value):
```

### Comparing `mediagrains-5.0.0/mediagrains/grains/VideoGrain.py` & `mediagrains-5.1.0/mediagrains/grains/VideoGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/grains/__init__.py` & `mediagrains-5.1.0/mediagrains/grains/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/gsf.py` & `mediagrains-5.1.0/mediagrains/gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/hypothesis/strategies.py` & `mediagrains-5.1.0/mediagrains/hypothesis/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,15 +479,19 @@
     raise ValueError("Cannot find a strategy to generate grains of type: {}".format(grain_type))
 
 
 def grains_with_data(grain_type):
     """Strategy giving grains which have data payloads filled out using an appropriate strategy for the grain type.
 
     :param grain_type: The type of grains to generate"""
-    if grain_type in ("audio", "video", "coded_audio", "coded_video"):
+    if grain_type == "video":
+        return grains(grain_type, width=16, height=9).flatmap(lambda g: grains_from_template_with_data(g))
+    elif grain_type == "coded_video":
+        return grains(grain_type, origin_width=16, origin_height=9).flatmap(lambda g: grains_from_template_with_data(g))
+    elif grain_type in ("audio", "coded_audio"):
         return grains(grain_type).flatmap(lambda g: grains_from_template_with_data(g))
     else:
         return grains(grain_type)
 
 
 def grains_from_template_with_data(grain, data=None):
     """A strategy that produces grains which are identical to the input grain but with randomised data based on the
```

### Comparing `mediagrains-5.0.0/mediagrains/numpy/__init__.py` & `mediagrains-5.1.0/mediagrains/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/numpy/convert.py` & `mediagrains-5.1.0/mediagrains/numpy/convert.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/numpy/numpy_grains/AudioGrain.py` & `mediagrains-5.1.0/mediagrains/numpy/numpy_grains/AudioGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/numpy/numpy_grains/VideoGrain.py` & `mediagrains-5.1.0/mediagrains/numpy/numpy_grains/VideoGrain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/__init__.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/abc.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/audio/__init__.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/audio/abc.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/audio/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/audio/tone.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/audio/tone.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/__init__.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/abc.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/abc.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/colourbars.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/colourbars.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/constants.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/constants.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/lumasteps.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/lumasteps.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/movingbaroverlay.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/movingbaroverlay.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/patterngenerators/video/still.py` & `mediagrains-5.1.0/mediagrains/patterngenerators/video/still.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/tools/__init__.py` & `mediagrains-5.1.0/mediagrains/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/tools/_file_or_pipe.py` & `mediagrains-5.1.0/mediagrains/tools/_file_or_pipe.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/tools/extract_from_gsf.py` & `mediagrains-5.1.0/mediagrains/tools/extract_from_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/tools/wrap_in_gsf.py` & `mediagrains-5.1.0/mediagrains/tools/wrap_in_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/typing.py` & `mediagrains-5.1.0/mediagrains/typing.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/__init__.py` & `mediagrains-5.1.0/mediagrains/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/adts_aac_grain_wrapper.py` & `mediagrains-5.1.0/mediagrains/utils/adts_aac_grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/adts_aac_parser.py` & `mediagrains-5.1.0/mediagrains/utils/adts_aac_parser.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/asyncbinaryio.py` & `mediagrains-5.1.0/mediagrains/utils/asyncbinaryio.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/grain_wrapper.py` & `mediagrains-5.1.0/mediagrains/utils/grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/h264_grain_wrapper.py` & `mediagrains-5.1.0/mediagrains/utils/h264_grain_wrapper.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/h264_parser.py` & `mediagrains-5.1.0/mediagrains/utils/h264_parser.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains/utils/iobytes.py` & `mediagrains-5.1.0/mediagrains/utils/iobytes.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/mediagrains.egg-info/PKG-INFO` & `mediagrains-5.1.0/mediagrains.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediagrains
-Version: 5.0.0
+Version: 5.1.0
 Summary: Simple utility for grain-based media
 Home-page: https://github.com/bbc/rd-apmm-python-lib-mediagrains
 Author: BBC R&D
 Author-email: cloudfit-opensource@rd.bbc.co.uk
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE.md
```

### Comparing `mediagrains-5.0.0/mediagrains.egg-info/SOURCES.txt` & `mediagrains-5.1.0/mediagrains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/setup.py` & `mediagrains-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/audio_utils.py` & `mediagrains-5.1.0/tests/audio_utils.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/fixtures.py` & `mediagrains-5.1.0/tests/fixtures.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,15 +68,23 @@
     attr_strat = attributes_for_grain_type(grain_type, new=True)
     grain_strat = sampled_from(attr_strat).flatmap(
         lambda attr: tuples(
             just(attr),
             pairs_of_grains_of_type_differing_only_at_specified_attribute(
                 grain_type, attr)))
 
-    if grain_type in ("audio", "video", "coded_audio", "coded_video"):
+    if grain_type == "video":
+        return grain_strat | grains(grain_type, width=16, height=9).flatmap(
+            lambda g: tuples(
+                just("data"), pairs_of(grains_from_template_with_data(g))))
+    elif grain_type == "coded_video":
+        return grain_strat | grains(grain_type, origin_width=16, origin_height=9).flatmap(
+            lambda g: tuples(
+                just("data"), pairs_of(grains_from_template_with_data(g))))
+    elif grain_type in ("audio", "coded_audio"):
         return grain_strat | grains(grain_type).flatmap(
             lambda g: tuples(
                 just("data"), pairs_of(grains_from_template_with_data(g))))
     else:
         return grain_strat
```

### Comparing `mediagrains-5.0.0/tests/test_adts_aac_parser.py` & `mediagrains-5.1.0/tests/test_adts_aac_parser.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_audio_psnr.py` & `mediagrains-5.1.0/tests/test_audio_psnr.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_comparison.py` & `mediagrains-5.1.0/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_grain.py` & `mediagrains-5.1.0/tests/test_grain.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_gsf.py` & `mediagrains-5.1.0/tests/test_gsf.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_iobytes.py` & `mediagrains-5.1.0/tests/test_iobytes.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_numpy_audiograin.py` & `mediagrains-5.1.0/tests/test_numpy_audiograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_numpy_videograin.py` & `mediagrains-5.1.0/tests/test_numpy_videograin.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_patterngenerators.py` & `mediagrains-5.1.0/tests/test_patterngenerators.py`

 * *Files identical despite different names*

### Comparing `mediagrains-5.0.0/tests/test_video_psnr.py` & `mediagrains-5.1.0/tests/test_video_psnr.py`

 * *Files identical despite different names*

