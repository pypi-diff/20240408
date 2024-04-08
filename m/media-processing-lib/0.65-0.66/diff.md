# Comparing `tmp/media-processing-lib-0.65.tar.gz` & `tmp/media-processing-lib-0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-processing-lib-0.65.tar", last modified: Wed Jan 17 12:48:39 2024, max compression
+gzip compressed data, was "media-processing-lib-0.66.tar", last modified: Mon Apr  8 06:57:00 2024, max compression
```

## Comparing `media-processing-lib-0.65.tar` & `media-processing-lib-0.66.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2023-03-26 06:25:47.000000 media-processing-lib-0.65/LICENSE.TXT
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2023-03-26 06:25:47.000000 media-processing-lib-0.65/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-01-17 12:48:39.288281 media-processing-lib-0.65/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2023-03-26 06:25:47.000000 media-processing-lib-0.65/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/audio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/audio_reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/audio_resample.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/audio_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/audio/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/audio/libs/librosa/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/libs/librosa/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/libs/librosa/reader.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/audio/libs/soundfile/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/libs/soundfile/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/libs/soundfile/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib/audio/melspectrogram/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/melspectrogram/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/melspectrogram/melspectrogram.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/mpl_audio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/audio/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/collage_maker/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/collage_maker/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/collage_maker/collage_maker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5178 2024-01-11 21:08:01.000000 media-processing-lib-0.65/media_processing_lib/collage_maker/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      167 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      704 2023-05-28 17:34:43.000000 media-processing-lib-0.65/media_processing_lib/image/image_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/image_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/libs/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-28 17:34:43.000000 media-processing-lib-0.65/media_processing_lib/image/libs/opencv/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/opencv/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/libs/pil/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/pil/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-28 17:34:43.000000 media-processing-lib-0.65/media_processing_lib/image/libs/pil/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1357 2024-01-10 14:55:20.000000 media-processing-lib-0.65/media_processing_lib/image/libs/pil/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/pil/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/libs/skimage/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/skimage/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/skimage/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/skimage/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/libs/skimage/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/resize/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/resize/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3677 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/resize/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/resize/resize_black_bars.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/resize/resize_stretch.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/image/utils/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/utils/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/utils/text.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1473 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/image/utils/title.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1030 2023-05-28 19:19:53.000000 media-processing-lib-0.65/media_processing_lib/image/utils/to_image.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2916 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/image/utils/utils.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-28 17:34:43.000000 media-processing-lib-0.65/media_processing_lib/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.284281 media-processing-lib-0.65/media_processing_lib/video/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2023-03-26 06:25:47.000000 media-processing-lib-0.65/media_processing_lib/video/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/media_processing_lib/video/backends/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/backends/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/backends/decord.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4138 2024-01-10 14:55:35.000000 media-processing-lib-0.65/media_processing_lib/video/backends/disk_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/backends/imageio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-05 14:47:46.000000 media-processing-lib-0.65/media_processing_lib/video/backends/memory_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-05 14:47:46.000000 media-processing-lib-0.65/media_processing_lib/video/backends/mpl_video_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/backends/opencv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-05-31 16:16:07.000000 media-processing-lib-0.65/media_processing_lib/video/backends/pims.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-05 14:47:46.000000 media-processing-lib-0.65/media_processing_lib/video/mpl_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-05-29 09:32:03.000000 media-processing-lib-0.65/media_processing_lib/video/utils.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-05 14:47:46.000000 media-processing-lib-0.65/media_processing_lib/video/video_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/video_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/media_processing_lib/video/writer/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/writer/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/media_processing_lib/video/writer/imageio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/writer/imageio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/writer/imageio/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/media_processing_lib/video/writer/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/writer/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-04-21 08:08:14.000000 media-processing-lib-0.65/media_processing_lib/video/writer/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.280280 media-processing-lib-0.65/media_processing_lib.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-01-17 12:48:39.000000 media-processing-lib-0.65/media_processing_lib.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3173 2024-01-17 12:48:39.000000 media-processing-lib-0.65/media_processing_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-01-17 12:48:39.000000 media-processing-lib-0.65/media_processing_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-01-17 12:48:39.000000 media-processing-lib-0.65/media_processing_lib.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2024-01-17 12:48:39.000000 media-processing-lib-0.65/media_processing_lib.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-01-17 12:47:15.000000 media-processing-lib-0.65/requirements.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-01-17 12:48:39.288281 media-processing-lib-0.65/resources/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2023-03-26 06:25:47.000000 media-processing-lib-0.65/resources/OpenSans-Bold.ttf
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-01-17 12:48:39.288281 media-processing-lib-0.65/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1831 2024-01-17 12:47:54.000000 media-processing-lib-0.65/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2022-07-21 09:37:21.000000 media-processing-lib-0.66/LICENSE.TXT
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2022-07-21 09:37:21.000000 media-processing-lib-0.66/MANIFEST.in
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-04-08 06:57:00.604480 media-processing-lib-0.66/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2022-07-21 09:37:21.000000 media-processing-lib-0.66/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_resample.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/reader.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/melspectrogram.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/mpl_audio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/collage_maker/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/collage_maker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5179 2024-04-08 06:11:46.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      172 2024-04-08 06:38:44.000000 media-processing-lib-0.66/media_processing_lib/image/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2024-04-08 06:32:57.000000 media-processing-lib-0.66/media_processing_lib/image/image_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      589 2024-04-08 06:32:21.000000 media-processing-lib-0.66/media_processing_lib/image/image_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/pil/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1357 2024-01-14 11:25:57.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/writer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2958 2024-04-08 06:31:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs_builder.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/resize/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/resize/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3684 2024-04-08 06:34:08.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize_black_bars.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize_stretch.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/transforms/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      154 2024-04-08 06:33:07.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1729 2024-04-08 06:51:20.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/border.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/text.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1472 2024-04-08 06:16:27.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/title.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1029 2024-04-08 06:13:02.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/to_image.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/video/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/video/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/backends/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/decord.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4138 2024-01-14 11:25:57.000000 media-processing-lib-0.66/media_processing_lib/video/backends/disk_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/imageio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/backends/memory_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/backends/mpl_video_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/opencv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/backends/pims.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/mpl_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/utils.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/video_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/video_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3242 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-08 06:11:46.000000 media-processing-lib-0.66/requirements.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/resources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2022-07-21 09:37:21.000000 media-processing-lib-0.66/resources/OpenSans-Bold.ttf
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-04-08 06:57:00.604480 media-processing-lib-0.66/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1789 2024-04-08 06:54:05.000000 media-processing-lib-0.66/setup.py
```

### Comparing `media-processing-lib-0.65/media_processing_lib/audio/audio_reader.py` & `media-processing-lib-0.66/media_processing_lib/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/audio/audio_writer.py` & `media-processing-lib-0.66/media_processing_lib/audio/audio_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/audio/melspectrogram/melspectrogram.py` & `media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/melspectrogram.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/audio/mpl_audio.py` & `media-processing-lib-0.66/media_processing_lib/audio/mpl_audio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/audio/utils.py` & `media-processing-lib-0.66/media_processing_lib/audio/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/collage_maker/collage_maker.py` & `media-processing-lib-0.66/media_processing_lib/collage_maker/collage_maker.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/collage_maker/utils.py` & `media-processing-lib-0.66/media_processing_lib/collage_maker/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
     assert len(images) > 1, "Must give at least two images to the collage"
     if rows_cols is None:
         rows_cols = get_closest_square(len(images))
         logger.debug2(f"row_cols was not set. Setting automatically to {rows_cols} based on number of images")
     assert len(rows_cols) == 2, f"rows_cols must be a tuple with 2 numbers, got: {rows_cols}"
     if np.prod(rows_cols) > len(images):
-        logger.debug(f"rows_cols: {rows_cols} greater than n images: {len(images)}. Padding with black images!")
+        logger.debug2(f"rows_cols: {rows_cols} greater than n images: {len(images)}. Padding with black images!")
     assert not all(x is None for x in images), "All images are None"
 
     if pad_to_max:
         images = _pad_to_max(images)
 
     shapes = [x.shape for x in [img for img in images if img is not None]]
```

### Comparing `media-processing-lib-0.65/media_processing_lib/image/libs/opencv/resize.py` & `media-processing-lib-0.66/media_processing_lib/image/libs/opencv/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/libs/pil/resize.py` & `media-processing-lib-0.66/media_processing_lib/image/libs/pil/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/libs/skimage/resize.py` & `media-processing-lib-0.66/media_processing_lib/image/libs/skimage/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/resize/resize.py` & `media-processing-lib-0.66/media_processing_lib/image/resize/resize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Resize module for images"""
 import numpy as np
 from ...logger import logger
-from ..utils import build_resize_fn
+from ..libs_builder import build_resize_fn
 from .resize_stretch import image_resize_stretch
 from .resize_black_bars import image_resize_black_bars
 
 
 def build_resize_mode_fn(mode):
     """builds the resize mode fn"""
     assert mode in ("stretch", "black_bars")
```

### Comparing `media-processing-lib-0.65/media_processing_lib/image/resize/resize_black_bars.py` & `media-processing-lib-0.66/media_processing_lib/image/resize/resize_black_bars.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/resize/resize_stretch.py` & `media-processing-lib-0.66/media_processing_lib/image/resize/resize_stretch.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/utils/text.py` & `media-processing-lib-0.66/media_processing_lib/image/transforms/text.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/image/utils/title.py` & `media-processing-lib-0.66/media_processing_lib/image/transforms/title.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .text import get_default_font, image_add_text, StrOrColor
 from ...logger import logger
 
 def image_add_title(image: np.ndarray, text: str, font: str = None, font_color: str = "white",
                     background_color: StrOrColor = "black", top_padding: int = None, size_px: int = None) -> np.ndarray:
     """Calls image_add_text to add title on an updated image with padding on top for space and text centered"""
     assert len(image.shape) == 3, f"Wrong image shape: {image.shape}"
-    height, _ = image.shape[0 : 2]
+    height, _ = image.shape[0: 2]
     pil_image = Image.fromarray(image.astype(np.uint8))
     draw = ImageDraw.Draw(pil_image)
 
     if top_padding is None:
         top_padding = int(height * 0.15)
         logger.debug2(f"Top padding not provided. Giving 15% of the image = {top_padding}")
```

### Comparing `media-processing-lib-0.65/media_processing_lib/image/utils/to_image.py` & `media-processing-lib-0.66/media_processing_lib/image/transforms/to_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         x = np.expand_dims(x, axis=-1)
     assert len(x.shape) == 3, f"Got: {x.shape}."
     if x.shape[0] in (1, 3):
         x = x.transpose(1, 2, 0)
     if x.shape[-1] == 1:
         x = np.concatenate([x, x, x], axis=-1)
     if x.shape[-1] == 4:
-        x = x[..., 0 : 3]
+        x = x[..., 0: 3]
     x = np.clip(x, 0, 1) * 255
     x = x.astype(np.uint8)
     return x
```

### Comparing `media-processing-lib-0.65/media_processing_lib/image/utils/utils.py` & `media-processing-lib-0.66/media_processing_lib/image/libs_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,81 @@
-"""Utils module"""
-from typing import Set, Callable
+"""Libraries builder for the image module"""
+from __future__ import annotations
+from typing import Callable
 import os
-from ...logger import logger
-
-from ..libs.pil import image_read as image_read_pil, image_write as image_write_pil, image_resize as image_resize_pil
-from ..libs.opencv import (
-    image_read as image_read_opencv,
-    image_write as image_write_opencv,
-    image_resize as image_resize_opencv,
-)
-from ..libs.skimage import (
-    image_read as image_read_skimage,
-    image_write as image_write_skimage,
-    image_resize as image_resize_skimage,
-)
+from ..logger import logger
 
+from .libs.pil import image_read as image_read_pil, image_write as image_write_pil, image_resize as image_resize_pil
+from .libs.opencv import image_read as image_read_opencv, image_write as image_write_opencv, \
+    image_resize as image_resize_opencv
+from .libs.skimage import image_read as image_read_skimage, image_write as image_write_skimage, \
+    image_resize as image_resize_skimage
 
 # pylint: disable=import-outside-toplevel, unused-import
-def get_available_image_libs() -> Set[str]:
+def get_available_image_libs() -> set[str]:
     """Returns a set with all the available image libraries used for reading/writing"""
-
     res = set()
     try:
-        import PIL
-
+        import PIL # noqa
         res.add("PIL")
     except ModuleNotFoundError:
         pass
 
     try:
-        import cv2
-
+        import cv2 # noqa
         res.add("opencv")
     except ModuleNotFoundError:
         pass
 
     try:
-        import skimage
-
+        import skimage # noqa
         res.add("skimage")
     except ModuleNotFoundError:
         pass
 
     if len(res) == 0:
         logger.info("Warning! No image libraries available. Use 'pip install -r requirements.txt'")
     return res
 
-
 def build_image_reader_fn(img_lib: str) -> Callable:
     """Build the image reader function"""
     img_lib = get_default_img_lib() if img_lib is None else img_lib
     assert img_lib in get_available_image_libs(), f"Image library '{img_lib}' not in {get_available_image_libs()}"
     if img_lib == "opencv":
         return image_read_opencv
     if img_lib == "PIL":
         return image_read_pil
     if img_lib == "skimage":
         return image_read_skimage
     return None
 
-
 def build_image_writer_fn(img_lib: str) -> Callable:
     """build image writer function"""
     img_lib = get_default_img_lib() if img_lib is None else img_lib
     assert img_lib in get_available_image_libs(), f"Image library '{img_lib}' not in {get_available_image_libs()}"
     if img_lib == "opencv":
         return image_write_opencv
     if img_lib == "PIL":
         return image_write_pil
     if img_lib == "skimage":
         return image_write_skimage
     return None
 
-
 def build_resize_fn(resize_lib: str) -> Callable:
     """Builds the resize fn"""
     resize_lib = get_default_img_lib() if resize_lib is None else resize_lib
     assert resize_lib in get_available_image_libs(), f"Image library '{resize_lib}' not in {get_available_image_libs()}"
     if resize_lib == "skimage":
         return image_resize_skimage
     if resize_lib == "PIL":
         return image_resize_pil
     if resize_lib == "opencv":
         return image_resize_opencv
     return None
 
-
 def get_default_img_lib() -> str:
     """gets the default img lib from the env variable or set opencv if it is not set"""
     backend = os.getenv("MPL_IMAGE_BACKEND")
     if not backend:
         backend = "PIL"
         logger.debug(f"MPL_IMAGE_BACKEND not set. Defaulting to '{backend}' backend")
     return backend
```

### Comparing `media-processing-lib-0.65/media_processing_lib/logger.py` & `media-processing-lib-0.66/media_processing_lib/logger.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/decord.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/decord.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/disk_backend.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/disk_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/imageio.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/imageio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/memory_backend.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/memory_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/mpl_video_backend.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/mpl_video_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/opencv.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/opencv.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/backends/pims.py` & `media-processing-lib-0.66/media_processing_lib/video/backends/pims.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/mpl_video.py` & `media-processing-lib-0.66/media_processing_lib/video/mpl_video.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/utils.py` & `media-processing-lib-0.66/media_processing_lib/video/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/video_reader.py` & `media-processing-lib-0.66/media_processing_lib/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/video_writer.py` & `media-processing-lib-0.66/media_processing_lib/video/video_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib/video/writer/opencv/writer.py` & `media-processing-lib-0.66/media_processing_lib/video/writer/opencv/writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/media_processing_lib.egg-info/SOURCES.txt` & `media-processing-lib-0.66/media_processing_lib.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 media_processing_lib/audio/melspectrogram/melspectrogram.py
 media_processing_lib/collage_maker/__init__.py
 media_processing_lib/collage_maker/collage_maker.py
 media_processing_lib/collage_maker/utils.py
 media_processing_lib/image/__init__.py
 media_processing_lib/image/image_reader.py
 media_processing_lib/image/image_writer.py
+media_processing_lib/image/libs_builder.py
 media_processing_lib/image/libs/__init__.py
 media_processing_lib/image/libs/opencv/__init__.py
 media_processing_lib/image/libs/opencv/reader.py
 media_processing_lib/image/libs/opencv/resize.py
 media_processing_lib/image/libs/opencv/writer.py
 media_processing_lib/image/libs/pil/__init__.py
 media_processing_lib/image/libs/pil/reader.py
@@ -43,19 +44,19 @@
 media_processing_lib/image/libs/skimage/reader.py
 media_processing_lib/image/libs/skimage/resize.py
 media_processing_lib/image/libs/skimage/writer.py
 media_processing_lib/image/resize/__init__.py
 media_processing_lib/image/resize/resize.py
 media_processing_lib/image/resize/resize_black_bars.py
 media_processing_lib/image/resize/resize_stretch.py
-media_processing_lib/image/utils/__init__.py
-media_processing_lib/image/utils/text.py
-media_processing_lib/image/utils/title.py
-media_processing_lib/image/utils/to_image.py
-media_processing_lib/image/utils/utils.py
+media_processing_lib/image/transforms/__init__.py
+media_processing_lib/image/transforms/border.py
+media_processing_lib/image/transforms/text.py
+media_processing_lib/image/transforms/title.py
+media_processing_lib/image/transforms/to_image.py
 media_processing_lib/video/__init__.py
 media_processing_lib/video/mpl_video.py
 media_processing_lib/video/utils.py
 media_processing_lib/video/video_reader.py
 media_processing_lib/video/video_writer.py
 media_processing_lib/video/backends/__init__.py
 media_processing_lib/video/backends/decord.py
```

### Comparing `media-processing-lib-0.65/resources/OpenSans-Bold.ttf` & `media-processing-lib-0.66/resources/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.65/setup.py` & `media-processing-lib-0.66/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 
 
 def get_reqs(requirements):
     # Do not add to required lines pointing to Git repositories
     required, dependency_links = [], []
     EGG_MARK = "#egg="
     for line in requirements:
-        if (
-            line.startswith("-e git:")
-            or line.startswith("-e git+")
-            or line.startswith("git:")
-            or line.startswith("git+")
-        ):
+        if line.startswith("-e git:") or line.startswith("-e git+") or line.startswith("git:") \
+                or line.startswith("git+"):
             line = line.lstrip("-e ")  # in case that is using "-e"
             if EGG_MARK in line:
                 package_name = line[line.find(EGG_MARK) + len(EGG_MARK) :]
                 repository = line[: line.find(EGG_MARK)]
                 required.append(f"{package_name} @ {repository}")
                 dependency_links.append(line)
             else:
@@ -24,15 +20,15 @@
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
 
 name = "media-processing-lib"
-version = "0.65"
+version = "0.66"
 description = "Media processing library for video, audio and images."
 url = "https://gitlab.com/mihaicristianpirvu/media-processing-lib"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

