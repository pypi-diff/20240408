# Comparing `tmp/SightTraining-0.1.21.tar.gz` & `tmp/SightTraining-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SightTraining-0.1.21.tar", last modified: Mon Apr  8 06:06:48 2024, max compression
+gzip compressed data, was "SightTraining-0.1.22.tar", last modified: Mon Apr  8 09:44:08 2024, max compression
```

## Comparing `SightTraining-0.1.21.tar` & `SightTraining-0.1.22.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.581472 SightTraining-0.1.21/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.21/LICENSE
--rw-r--r--   0 wangjuntao   (501) staff       (20)       58 2024-04-01 09:37:31.000000 SightTraining-0.1.21/MANIFEST.in
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 06:06:48.581206 SightTraining-0.1.21/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.21/Readme.md
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.580823 SightTraining-0.1.21/SightTraining.egg-info/
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2932 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/SOURCES.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/dependency_links.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/entry_points.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/requires.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-08 06:06:48.000000 SightTraining-0.1.21/SightTraining.egg-info/top_level.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-08 06:06:48.581528 SightTraining-0.1.21/setup.cfg
--rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-08 06:06:20.000000 SightTraining-0.1.21/setup.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.555155 SightTraining-0.1.21/spacedefense/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1261 2024-04-07 13:38:55.000000 SightTraining-0.1.21/spacedefense/__init__.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    19908 2024-04-08 05:52:08.000000 SightTraining-0.1.21/spacedefense/actors.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.555303 SightTraining-0.1.21/spacedefense/assets/
--rw-r--r--   0 wangjuntao   (501) staff       (20)    10244 2024-04-08 03:01:25.000000 SightTraining-0.1.21/spacedefense/assets/.DS_Store
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.561484 SightTraining-0.1.21/spacedefense/assets/images/
--rw-r--r--   0 wangjuntao   (501) staff       (20)    18436 2024-04-08 03:03:21.000000 SightTraining-0.1.21/spacedefense/assets/images/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)    93950 2024-04-08 02:52:13.000000 SightTraining-0.1.21/spacedefense/assets/images/game_cover.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   115516 2024-04-08 02:53:25.000000 SightTraining-0.1.21/spacedefense/assets/images/game_cover_loss.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   129152 2024-04-08 02:53:06.000000 SightTraining-0.1.21/spacedefense/assets/images/game_cover_win.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)    31179 2024-04-01 06:54:20.000000 SightTraining-0.1.21/spacedefense/assets/images/icon.png
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6772 2024-04-07 13:57:36.000000 SightTraining-0.1.21/spacedefense/assets/images/my_slave_fighter1.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6578 2024-04-07 13:59:55.000000 SightTraining-0.1.21/spacedefense/assets/images/my_slave_fighter2.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.562577 SightTraining-0.1.21/spacedefense/assets/images/myf_master/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:42:44.000000 SightTraining-0.1.21/spacedefense/assets/images/myf_master/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7568 2024-04-07 13:41:47.000000 SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7358 2024-04-07 13:41:55.000000 SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7442 2024-04-07 13:42:06.000000 SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6916 2024-04-07 13:42:17.000000 SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_004.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)    95336 2024-04-07 14:00:31.000000 SightTraining-0.1.21/spacedefense/assets/images/scale_cambg1.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5298 2024-04-08 01:24:57.000000 SightTraining-0.1.21/spacedefense/assets/images/super_bullet.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.563952 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:00.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     8908 2024-04-07 13:49:06.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9406 2024-04-07 13:49:20.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9166 2024-04-07 13:49:28.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9482 2024-04-07 13:49:58.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_004.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.565065 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:40.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5838 2024-04-07 13:52:06.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5676 2024-04-07 13:52:20.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5802 2024-04-07 13:52:28.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5682 2024-04-07 13:52:42.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6584 2024-04-08 05:42:47.000000 SightTraining-0.1.21/spacedefense/assets/images/ufo_super_bullet.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.566454 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:18:10.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   323000 2024-04-07 13:16:38.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   262066 2024-04-07 13:16:50.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   322282 2024-04-07 13:17:12.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_003.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.568333 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:27:10.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   212520 2024-04-07 13:24:30.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   210670 2024-04-07 13:24:44.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   221782 2024-04-07 13:25:46.000000 SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_003.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 06:06:48.580540 SightTraining-0.1.21/spacedefense/assets/sounds/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-08 03:00:49.000000 SightTraining-0.1.21/spacedefense/assets/sounds/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   613595 2024-04-01 06:38:42.000000 SightTraining-0.1.21/spacedefense/assets/sounds/bgm.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    19873 2024-03-29 14:26:24.000000 SightTraining-0.1.21/spacedefense/assets/sounds/fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    18471 2024-03-29 14:25:00.000000 SightTraining-0.1.21/spacedefense/assets/sounds/fire_blast.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    26919 2024-03-29 14:24:28.000000 SightTraining-0.1.21/spacedefense/assets/sounds/firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    40320 2024-03-31 18:25:38.000000 SightTraining-0.1.21/spacedefense/assets/sounds/smyf_join.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   265674 2024-03-29 14:22:39.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_angry.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   214184 2024-03-29 14:21:15.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_end_loss.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   128369 2024-03-29 14:21:54.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_end_win.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   213937 2024-03-29 14:22:18.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_mid.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   295241 2024-03-29 14:22:58.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_pre.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   224144 2024-03-29 14:23:21.000000 SightTraining-0.1.21/spacedefense/assets/sounds/stage_start.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    49560 2024-03-31 18:25:08.000000 SightTraining-0.1.21/spacedefense/assets/sounds/sufo_join.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    24129 2024-03-29 18:13:37.000000 SightTraining-0.1.21/spacedefense/assets/sounds/super_fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    56632 2024-03-29 18:24:26.000000 SightTraining-0.1.21/spacedefense/assets/sounds/super_firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    10368 2024-03-29 14:23:49.000000 SightTraining-0.1.21/spacedefense/assets/sounds/ufo_fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    12270 2024-03-29 14:24:06.000000 SightTraining-0.1.21/spacedefense/assets/sounds/ufo_firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)     3705 2024-04-07 13:21:07.000000 SightTraining-0.1.21/spacedefense/common.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5577 2024-04-08 06:04:11.000000 SightTraining-0.1.21/spacedefense/config.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    12913 2024-04-08 04:51:36.000000 SightTraining-0.1.21/spacedefense/flight_unit.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2064 2024-04-07 14:10:18.000000 SightTraining-0.1.21/spacedefense/game.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9669 2024-04-08 04:39:32.000000 SightTraining-0.1.21/spacedefense/my_master.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    29841 2024-04-08 06:01:57.000000 SightTraining-0.1.21/spacedefense/scene_main.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     3653 2024-04-01 17:56:03.000000 SightTraining-0.1.21/spacedefense/scenes.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.050387 SightTraining-0.1.22/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.22/LICENSE
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       58 2024-04-01 09:37:31.000000 SightTraining-0.1.22/MANIFEST.in
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 09:44:08.050131 SightTraining-0.1.22/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.22/Readme.md
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.049833 SightTraining-0.1.22/SightTraining.egg-info/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2932 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/entry_points.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/requires.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-08 09:44:07.000000 SightTraining-0.1.22/SightTraining.egg-info/top_level.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-08 09:44:08.050439 SightTraining-0.1.22/setup.cfg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-08 09:44:04.000000 SightTraining-0.1.22/setup.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.007312 SightTraining-0.1.22/spacedefense/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1261 2024-04-07 13:38:55.000000 SightTraining-0.1.22/spacedefense/__init__.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    19909 2024-04-08 06:47:13.000000 SightTraining-0.1.22/spacedefense/actors.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.007787 SightTraining-0.1.22/spacedefense/assets/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10244 2024-04-08 03:01:25.000000 SightTraining-0.1.22/spacedefense/assets/.DS_Store
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.017080 SightTraining-0.1.22/spacedefense/assets/images/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18436 2024-04-08 03:03:21.000000 SightTraining-0.1.22/spacedefense/assets/images/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    93950 2024-04-08 02:52:13.000000 SightTraining-0.1.22/spacedefense/assets/images/game_cover.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   115516 2024-04-08 02:53:25.000000 SightTraining-0.1.22/spacedefense/assets/images/game_cover_loss.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   129152 2024-04-08 02:53:06.000000 SightTraining-0.1.22/spacedefense/assets/images/game_cover_win.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    31179 2024-04-01 06:54:20.000000 SightTraining-0.1.22/spacedefense/assets/images/icon.png
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6772 2024-04-07 13:57:36.000000 SightTraining-0.1.22/spacedefense/assets/images/my_slave_fighter1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6578 2024-04-07 13:59:55.000000 SightTraining-0.1.22/spacedefense/assets/images/my_slave_fighter2.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.020079 SightTraining-0.1.22/spacedefense/assets/images/myf_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:42:44.000000 SightTraining-0.1.22/spacedefense/assets/images/myf_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7568 2024-04-07 13:41:47.000000 SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7358 2024-04-07 13:41:55.000000 SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7442 2024-04-07 13:42:06.000000 SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6916 2024-04-07 13:42:17.000000 SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_004.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    95336 2024-04-07 14:00:31.000000 SightTraining-0.1.22/spacedefense/assets/images/scale_cambg1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5298 2024-04-08 01:24:57.000000 SightTraining-0.1.22/spacedefense/assets/images/super_bullet.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.022295 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:00.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     8908 2024-04-07 13:49:06.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9406 2024-04-07 13:49:20.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9166 2024-04-07 13:49:28.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9482 2024-04-07 13:49:58.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_004.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.023913 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:40.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5838 2024-04-07 13:52:06.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5676 2024-04-07 13:52:20.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5802 2024-04-07 13:52:28.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5682 2024-04-07 13:52:42.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6290 2024-04-08 06:43:52.000000 SightTraining-0.1.22/spacedefense/assets/images/ufo_super_bullet.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.027210 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:18:10.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   323000 2024-04-07 13:16:38.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   262066 2024-04-07 13:16:50.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   322282 2024-04-07 13:17:12.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.032960 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:27:10.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   212520 2024-04-07 13:24:30.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   210670 2024-04-07 13:24:44.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   221782 2024-04-07 13:25:46.000000 SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 09:44:08.049465 SightTraining-0.1.22/spacedefense/assets/sounds/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-08 03:00:49.000000 SightTraining-0.1.22/spacedefense/assets/sounds/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   613595 2024-04-01 06:38:42.000000 SightTraining-0.1.22/spacedefense/assets/sounds/bgm.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    19873 2024-03-29 14:26:24.000000 SightTraining-0.1.22/spacedefense/assets/sounds/fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18471 2024-03-29 14:25:00.000000 SightTraining-0.1.22/spacedefense/assets/sounds/fire_blast.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    26919 2024-03-29 14:24:28.000000 SightTraining-0.1.22/spacedefense/assets/sounds/firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    40320 2024-03-31 18:25:38.000000 SightTraining-0.1.22/spacedefense/assets/sounds/smyf_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   265674 2024-03-29 14:22:39.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_angry.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   214184 2024-03-29 14:21:15.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_end_loss.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   128369 2024-03-29 14:21:54.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_end_win.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   213937 2024-03-29 14:22:18.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_mid.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   295241 2024-03-29 14:22:58.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_pre.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   224144 2024-03-29 14:23:21.000000 SightTraining-0.1.22/spacedefense/assets/sounds/stage_start.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    49560 2024-03-31 18:25:08.000000 SightTraining-0.1.22/spacedefense/assets/sounds/sufo_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    24129 2024-03-29 18:13:37.000000 SightTraining-0.1.22/spacedefense/assets/sounds/super_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    56632 2024-03-29 18:24:26.000000 SightTraining-0.1.22/spacedefense/assets/sounds/super_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10368 2024-03-29 14:23:49.000000 SightTraining-0.1.22/spacedefense/assets/sounds/ufo_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    12270 2024-03-29 14:24:06.000000 SightTraining-0.1.22/spacedefense/assets/sounds/ufo_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3705 2024-04-07 13:21:07.000000 SightTraining-0.1.22/spacedefense/common.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5576 2024-04-08 07:42:36.000000 SightTraining-0.1.22/spacedefense/config.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    12911 2024-04-08 09:43:36.000000 SightTraining-0.1.22/spacedefense/flight_unit.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2064 2024-04-07 14:10:18.000000 SightTraining-0.1.22/spacedefense/game.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9758 2024-04-08 07:28:14.000000 SightTraining-0.1.22/spacedefense/my_master.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    30164 2024-04-08 07:17:26.000000 SightTraining-0.1.22/spacedefense/scene_main.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3653 2024-04-01 17:56:03.000000 SightTraining-0.1.22/spacedefense/scenes.py
```

### Comparing `SightTraining-0.1.21/LICENSE` & `SightTraining-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/PKG-INFO` & `SightTraining-0.1.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.21
+Version: 0.1.22
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.21/SightTraining.egg-info/PKG-INFO` & `SightTraining-0.1.22/SightTraining.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.21
+Version: 0.1.22
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.21/SightTraining.egg-info/SOURCES.txt` & `SightTraining-0.1.22/SightTraining.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/setup.py` & `SightTraining-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 readme = """
 SightTraining  is a game for children's amblyopia training
 """
 
 setup(
     name="SightTraining",
-    version="0.1.21",
+    version="0.1.22",
     author="jett.wang",
     author_email="jamiesun.net@gmail.com",
     description="SightTraining  is a game for children's amblyopia training",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `SightTraining-0.1.21/spacedefense/__init__.py` & `SightTraining-0.1.22/spacedefense/__init__.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/actors.py` & `SightTraining-0.1.22/spacedefense/actors.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
         self.rect = self.image.get_rect(center=(self.x, self.y))
         self.life_value = self.config["life_value"]
         self.rotation_angle = 0  # Initial rotation angle
 
     def attack(self):
         for _ in range(4):  # Generate two particles
             self.particle_group.add(
-                Particle(self.rect.centerx, self.rect.centery, Colors.white)
+                Particle(self.rect.centerx, self.rect.centery, Colors.orange)
             )
 
         # Calculate distance and angle to target
         dx = self.target.rect.centerx - self.rect.centerx
         dy = self.target.rect.centery - self.rect.centery
         dist = math.hypot(dx, dy)
         angle = math.atan2(dy, dx)
@@ -451,15 +451,15 @@
             self.speed *= 1.2
 
         # Adjust bullet position
         self.rect.x += self.speed * math.cos(angle)
         self.rect.y += self.speed * math.sin(angle)
 
         # Rotation for visual effect (since it's a circular bullet, rotation doesn't affect its direction)
-        self.rotation_angle = (self.rotation_angle + self.speed * 10) % 360  # Add 5 degrees each update
+        self.rotation_angle = (self.rotation_angle + self.speed * 15) % 360  # Add 5 degrees each update
         self.image = pygame.transform.rotate(self.original_image, self.rotation_angle)
         self.rect = self.image.get_rect(center=self.rect.center)  # Update rect to keep center position unchanged
 
         # Boundary check
         if (self.rect.top < 0 or self.rect.bottom > DISPLAY_HEIGHT or self.rect.left < 0 or self.rect.right > DISPLAY_WIDTH):
             self.kill()
```

### Comparing `SightTraining-0.1.21/spacedefense/assets/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/game_cover.webp` & `SightTraining-0.1.22/spacedefense/assets/images/game_cover.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/game_cover_loss.webp` & `SightTraining-0.1.22/spacedefense/assets/images/game_cover_loss.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/game_cover_win.webp` & `SightTraining-0.1.22/spacedefense/assets/images/game_cover_win.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/icon.png` & `SightTraining-0.1.22/spacedefense/assets/images/icon.png`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/my_slave_fighter1.webp` & `SightTraining-0.1.22/spacedefense/assets/images/my_slave_fighter1.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/my_slave_fighter2.webp` & `SightTraining-0.1.22/spacedefense/assets/images/my_slave_fighter2.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/myf_master/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/myf_master/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_001.webp` & `SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_002.webp` & `SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_003.webp` & `SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/myf_master/myf_master_004.webp` & `SightTraining-0.1.22/spacedefense/assets/images/myf_master/myf_master_004.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/scale_cambg1.webp` & `SightTraining-0.1.22/spacedefense/assets/images/scale_cambg1.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/super_bullet.webp` & `SightTraining-0.1.22/spacedefense/assets/images/super_bullet.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_master/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_master/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_001.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_002.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_003.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_master/ufo_master_004.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_master/ufo_master_004.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/ufo_super_bullet.webp` & `SightTraining-0.1.22/spacedefense/assets/images/ufo_super_bullet.webp`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 5249 4646 b019 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
+00000000: 5249 4646 8a18 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
 00000010: 0a00 0000 3400 0000 2f00 0030 0000 4943  ....4.../..0..IC
 00000020: 4350 480c 0000 0000 0c48 4c69 6e6f 0210  CPH......HLino..
 00000030: 0000 6d6e 7472 5247 4220 5859 5a20 07ce  ..mntrRGB XYZ ..
 00000040: 0002 0009 0006 0031 0000 6163 7370 4d53  .......1..acspMS
 00000050: 4654 0000 0000 4945 4320 7352 4742 0000  FT....IEC sRGB..
 00000060: 0000 0000 0000 0000 0000 0000 f6d6 0001  ................
 00000070: 0000 0000 d32d 4850 2020 0000 0000 0000  .....-HP  ......
@@ -193,220 +193,202 @@
 00000c00: e253 e2db e363 e3eb e473 e4fc e584 e60d  .S...c...s......
 00000c10: e696 e71f e7a9 e832 e8bc e946 e9d0 ea5b  .......2...F...[
 00000c20: eae5 eb70 ebfb ec86 ed11 ed9c ee28 eeb4  ...p.........(..
 00000c30: ef40 efcc f058 f0e5 f172 f1ff f28c f319  .@...X...r......
 00000c40: f3a7 f434 f4c2 f550 f5de f66d f6fb f78a  ...4...P...m....
 00000c50: f819 f8a8 f938 f9c7 fa57 fae7 fb77 fc07  .....8...W...w..
 00000c60: fc98 fd29 fdba fe4b fedc ff6d ffff 414c  ...)...K...m..AL
-00000c70: 5048 5004 0000 01a0 b06d dbd9 48df d1fd  PHP......m..H...
-00000c80: 46d5 d89e dd1d cfda b66d db3b 58db b66d  F........m.;X..m
-00000c90: dbb6 6ddb b6b7 335b 26cf 87cc 6cb3 1131  ..m...3[&...l..1
-00000ca0: 01d0 9231 fc9d f1e5 f480 2802 b55a 4b9a  ...1......(..ZK.
-00000cb0: 3101 4089 8bcd 8176 9d19 aadd 8903 c098  1.@....v........
-00000cc0: 1611 5372 00a6 edf3 180a 1486 efa2 5b59  ..Sr..........[Y
-00000cd0: 3d45 946e ce69 6058 b490 17fa 7e69 05f8  =E.n.i`X....~i..
-00000ce0: 0520 c9da 4f4a caca 1a1c 74d3 20ee f40a  . ..OJ....t. ...
-00000cf0: 21ec c1e7 623c 5207 b154 c796 2c6e fe7d  !...b<R..T..,n.}
-00000d00: 2e4e 175d c154 8c9b ccb5 1072 57be bca4  .N.].T.....rW...
-00000d10: 4e58 3022 6ec9 ab8c fd7f 8ef1 830b fd86  NX0"n...........
-00000d20: 54e3 0104 deb1 8e2d 14d8 fd83 4c5f eab0  T......-....L_..
-00000d30: f8fe 6fe8 4ed8 d6af c501 80c1 1425 6482  ..o.N........%d.
-00000d40: b977 bf98 050c ba25 4ec7 f7a3 f9f3 af55  .w.....%N......U
-00000d50: 684d ec65 999c 2b8d 4996 43e1 603c b801  hM.e..+.I.C.`<..
-00000d60: 2b3d 3272 6f6e 8cbd 5518 828e 8574 3fec  +=2ron..U....t?.
-00000d70: 5496 ba0d 72d2 8b35 0ea2 6391 e129 6667  T...r..5..c..)fg
-00000d80: 3298 c41b f6a4 2263 5d1e 31ee e5e1 31eb  2....."c].1...1.
-00000d90: 76b6 3570 f5d3 e8d0 80ef a47e 3ff9 9a85  v.5p.......~?...
-00000da0: 1c1d dd92 772c 5ef0 ad0f 78a6 06c0 3833  ....w,^...x...83
-00000db0: cd6e a79f 0df3 dd51 e8e3 67ca 50b1 10d1  .n.....Q..g.P...
-00000dc0: eee0 a474 c56e 7f50 50d7 3fb7 8aae 455d  ...t.n.PP.?...E]
-00000dd0: 1d3c 2a35 48fe 4ab3 fb2a f4e7 fbc3 77d3  .<*5H.J..*....w.
-00000de0: f5a6 0d13 39b1 59b4 5afb 1b25 2105 18a3  ....9.Y.Z..%!...
-00000df0: 5fd2 b393 e442 ebda f7b4 5ef2 0910 e026  _....B....^....&
-00000e00: a840 bf6f 49e5 45b7 b754 7b4a ae5f ddee  .@.oI.E..T{J._..
-00000e10: e2ed f105 17e7 54e3 46a6 9bd3 6465 e110  ......T.F...de..
-00000e20: b3cb 1e26 bfa4 cfd7 2fae f263 2af0 6e91  ...&..../..c*.n.
-00000e30: 5afd 127d 58ff dd65 b74f caf6 a480 2cee  Z..}X..e.O....,.
-00000e40: 6263 5f15 00d2 36d2 f877 65f8 c6f3 31fa  bc_...6..we...1.
-00000e50: 8c58 c397 b216 4afa ce00 d498 a743 c652  .X....J......C.R
-00000e60: c9fa ad5e 6991 3e30 5bb0 9b29 d0a3 4d1d  ...^i.>0[..)..M.
-00000e70: 1e86 209e d599 f3cc fcc1 a185 f2f4 c4bd  .. .............
-00000e80: 7d05 d0f9 5c5d 1e15 8f36 6365 4754 5949  }...\]...6ceGTYI
-00000e90: 9a2b a7eb 9d1a 0140 3fe0 6070 5461 df24  .+.....@?.`pTa.$
-00000ea0: 5933 8bcd 6a6e 0200 8d7e 5e7b fefd ec7d  Y3..jn...~^{...}
-00000eb0: d25a 1ed5 6141 47d3 ff7c 67de 782a 93f6  .Z..aAG..|g.x*..
-00000ec0: cff2 8163 5e02 c020 f995 fcf4 17ec 2e53  ...c^.. .......S
-00000ed0: 3387 be43 08dc 5b99 1243 bcf6 2bda 39cd  3..C..[..C..+.9.
-00000ee0: d617 758d 1ca4 04c3 c406 c879 50d6 8c94  ..u........yP...
-00000ef0: 7be7 f707 3000 f034 e807 bf57 34b3 1cca  {...0..4...W4...
-00000f00: 9f6d cf34 2300 16d7 79f1 2fd2 fee7 0813  .m.4#...y./.....
-00000f10: 0b8c e000 c45e fe6c a1bf f167 9bd8 3c6e  .....^.l...g..<n
-00000f20: 00d0 ec62 b13e 3fb4 5388 be3f 7e31 4502  ...b.>?.S..?~1E.
-00000f30: a256 cee1 f58d 674d 79a4 8d79 e2d2 0f0f  .V....gMy..y....
-00000f40: 3a36 b9d6 4440 fe21 5100 c422 a734 9a9c  :6..D@.!Q..".4..
-00000f50: 2f47 565e 6cd4 4a04 0043 e1b8 32af 156d  /GV^l.J..C..2..m
-00000f60: 48d9 a4d7 e9a1 eede f7ca d53b 0a39 650d  H..........;.9e.
-00000f70: ec0a 7d1c b371 4b21 15d6 e168 9154 337d  ..}..qK!...h.T3}
-00000f80: 1971 c575 b669 c715 fa36 72f4 64fe 7ff0  .q.u.i...6r.d...
-00000f90: 0ee1 4ccd a6d4 abf4 cd75 343f 6ed4 9cfa  ..L......u4?n...
-00000fa0: 7a53 2854 3977 0630 3477 90e5 a52b 6eef  zS(T9w.04w...+n.
-00000fb0: 77d0 e542 a112 60e2 d5b2 2d09 66c1 7913  w..B..`...-.f.y.
-00000fc0: a6ca 747e 98ec 824b a59f 91fc e9fe 2877  ..t~...K......(w
-00000fd0: d3ac 226a a6a2 fa84 c337 5f5a deac 2a97  .."j.....7_Z..*.
-00000fe0: ef3d bd7e 9f29 ebae 476f b377 befb e2e4  .=.~.)..Go.w....
-00000ff0: 99ef f5f8 22fe 6a00 3a6d 4c68 d9a3 80c9  ....".j.:mLh....
-00001000: 54fc ebed c6a7 89e4 3427 9172 e51b 7dc8  T.......4'.r..}.
-00001010: d5e1 61b9 80b0 28cf d04b 29c8 7454 5e00  ..a...(..K).tT^.
-00001020: 486c 58f1 7525 ef33 44d7 2bcf 93c9 de76  HlX.u%.3D.+....v
-00001030: 96d5 b2b0 ca82 634d 1907 fdee 01fa 4ca9  ......cM......L.
-00001040: 8b06 9f55 338d 7d64 ba13 324c b6ed 09f3  ...U3.}d..2L....
-00001050: 693e 72dd 892c fe3a c683 d5d9 9cc7 0590  i>r..,.:........
-00001060: 4a47 c547 ad54 e86a 96c3 f254 7f24 e645  JG.G.T.j...T.$.E
-00001070: ce8b 7150 656e 822b 3ce7 e68e 38fa e6d1  ..qPen.+<...8...
-00001080: 995a d21c c724 23da f762 7992 0c4c c5c5  .Z...$#..by..L..
-00001090: ccc4 373f 9b2f cc87 6311 339e b467 3a03  ..7?./..c.3..g:.
-000010a0: c7b8 aa09 5a00 a8b4 d90d c85f 1ee2 a055  ....Z......_...U
-000010b0: 3c82 9bf3 08f7 d248 1723 00be c1d0 4d6a  <......H.#....Mj
-000010c0: ce60 8862 f863 5650 3820 4805 0000 1017  .`.b.cVP8 H.....
-000010d0: 009d 012a 3000 3100 3e85 3292 4825 22a1  ...*0.1.>.2.H%".
-000010e0: a137 e800 a010 896c 009d 32e3 7a0f c3f9  .7.....l..2.z...
-000010f0: 9656 bfb6 6ced d21e 5343 1fe6 01fa 97d2  .V..l...SC......
-00001100: 03cc 0794 a7a8 9f40 0fec dfe0 3d5a fd45  .......@....=Z.E
-00001110: bd00 3f60 3d36 3d8a 3fb7 ffd2 f4a7 bb83  ..?`=6=.?.......
-00001120: c45f 24be 948e 9d27 786d de0e d43b a0f0  ._$....'xm...;..
-00001130: 03ea af41 1fe6 7c0d e3e3 d09f 3a9f 517b  ...A..|.....:.Q{
-00001140: 04fe b4f5 93f4 55fd 6b2b 4eca 5b51 dd73  ......U.k+N.[Q.s
-00001150: e027 e0cc d09b 9368 c796 619f dadf ecac  .'.....h..a.....
-00001160: 4a87 ca67 e290 7343 a631 7e9b 361f cdd2  J..g..sC.1~.6...
-00001170: 1db0 3724 f4f5 cbfa e689 19b7 ae05 a3b7  ..7$............
-00001180: eb54 4836 7041 8355 c9c0 d48e 9cf8 0000  .TH6pA.U........
-00001190: fef8 4e96 aebb 96d1 89af 9242 e3ae 24e5  ..N........B..$.
-000011a0: 41dc a631 dbad 843b 97e1 32ba f361 b2fb  A..1...;..2..a..
-000011b0: f203 13fa cff2 3eff 625d 0294 db38 dc96  ......>.b]...8..
-000011c0: ee28 06a9 cbc3 7250 adb4 df43 4d75 7c98  .(....rP...CMu|.
-000011d0: f654 8f18 f694 0d6a f28c 1fda 6bd6 de00  .T.....j....k...
-000011e0: 568e 0a71 b8fe f89e 032d 5afa 232a 3f28  V..q.....-Z.#*?(
-000011f0: e302 fc87 b57d f633 4e85 d8f0 ab92 c565  .....}.3N......e
-00001200: 5b42 dcdc 7dab 96e3 dda0 e37b a5d4 88a7  [B..}......{....
-00001210: 2bd7 2e19 5762 05b8 fff5 bd2f efdd 1e96  +...Wb...../....
-00001220: 87d4 08ef c4fb 468a e1ac 5bbf cbe7 31df  ......F...[...1.
-00001230: a846 6966 aa0e 3e04 0b93 28bf 4625 7e33  .Fif..>...(.F%~3
-00001240: bd89 61c9 1c33 dbd7 df3e 548c 4a63 783a  ..a..3...>T.Jcx:
-00001250: 1e4d 6d35 b5f5 55fe 21d9 86a5 1cb3 d073  .Mm5..U.!......s
-00001260: 6ad2 dcbb 35f9 70ba 20e6 8e23 deae bbf7  j...5.p. ..#....
-00001270: db58 0bb7 0d40 728c b182 1b86 d635 ba3f  .X...@r......5.?
-00001280: 29f5 9411 6a73 736d 59e9 af02 5725 9fc0  )...jssmY...W%..
-00001290: 12b8 5d7d 1ddd 3518 f753 cdbf 5a4f 2526  ..]}..5..S..ZO%&
-000012a0: c1e3 674e ea34 b23d bdb2 de18 edb6 d27c  ..gN.4.=.......|
-000012b0: cbc7 cba4 d1ea e690 44f1 800a af0b e952  ........D......R
-000012c0: 30fe 40fd c704 a322 3026 92c8 88fa 84d3  0.@...."0&......
-000012d0: 4f6f 334a 2ef6 4016 ad38 ea9b 93b1 b31b  Oo3J..@..8......
-000012e0: 1f94 cad5 b445 f152 dfb4 1dbf ee3b 70f9  .....E.R.....;p.
-000012f0: 8060 ff5f dbf7 e297 0b1a f7dc 494d 2873  .`._........IM(s
-00001300: 73ec 8b4c b01b 057c 3d5a a4fa fed1 6bf3  s..L...|=Z....k.
-00001310: e1d5 7931 62b9 e9b2 adfd 5c92 11a7 4291  ..y1b.....\...B.
-00001320: 5279 679b d797 d28b 3fa6 6753 b543 6790  Ryg.....?.gS.Cg.
-00001330: 194a a535 0eea 8237 c9ff d71a 9dc0 ff60  .J.5...7.......`
-00001340: 1f0d 6371 819e b4a5 0945 d71e 6600 2856  ..cq.....E..f.(V
-00001350: c676 8206 24ed 6372 bc4c 3377 00ea f00b  .v..$.cr.L3w....
-00001360: 1f95 0fca 8963 5b44 af24 00f1 484b f920  .....c[D.$..HK. 
-00001370: e3c7 6579 dda8 66ce ffca a349 b600 27b0  ..ey..f....I..'.
-00001380: af70 26de e1b0 876d e629 4aa4 d125 8ac7  .p&....m.)J..%..
-00001390: fc75 9db0 cfb6 1b18 ebc1 649e 48e3 a353  .u........d.H..S
-000013a0: 9f6d eafd 9cc9 e7ce 148b 5447 5a0b af23  .m........TGZ..#
-000013b0: 44ee ef0b 23c1 8b4a fdac 46d4 b786 0c6e  D...#..J..F....n
-000013c0: cc93 09d6 28f5 67b9 d731 c496 6de1 db06  ....(.g..1..m...
-000013d0: c827 202a a7f6 e829 dfdc 3725 bc25 e08e  .' *...)..7%.%..
-000013e0: fcf9 3b6b f524 515c a393 820e 78af 47af  ..;k.$Q\....x.G.
-000013f0: 84d1 4a8a f66b 251b d0ec e397 912b 93ca  ..J..k%......+..
-00001400: b614 08cb 1afc 9971 dffd 093a a0bf 8852  .......q...:...R
-00001410: 788f 6257 6811 9d76 3d3b 6aa3 cf71 74ba  x.bWh..v=;j..qt.
-00001420: 5cd3 7fbe 75d7 2131 6470 d644 a908 11be  \...u.!1dp.D....
-00001430: 0e73 d5d5 2307 9da8 1be1 5f11 9463 a802  .s..#....._..c..
-00001440: c6c5 42bd 7665 9174 2ce0 ffc2 cf5e 2c7e  ..B.ve.t,....^,~
-00001450: 0cd3 175b 47ba 443c 796d dc5d 761d 5673  ...[G.D<ym.]v.Vs
-00001460: 04a5 7770 22bc 44ec 333b f8df e8e9 8c62  ..wp".D.3;.....b
-00001470: 40df 0df5 8e72 34ef 9132 7793 e35f 21cb  @....r4..2w.._!.
-00001480: 8426 7166 940f d705 5410 d818 37dd 3ddf  .&qf....T...7.=.
-00001490: 2807 0879 d391 1c16 9c8e de68 f7ba 116a  (..y.......h...j
-000014a0: 1ddc 5f4d 15a6 bf6f 3fc9 8fbf ce45 ba9c  .._M...o?....E..
-000014b0: 4ff4 a1f2 4e0d 5e2e 3404 ac66 4cc0 0bf8  O...N.^.4..fL...
-000014c0: f49e 3be9 b836 825b 26f2 4fec c438 6d3e  ..;..6.[&.O..8m>
-000014d0: 1b88 2855 9b9c 98f9 7d2e b331 98a3 f62d  ..(U....}..1...-
-000014e0: a402 8e74 fcf9 a087 a526 ce89 ae22 e6c0  ...t.....&..."..
-000014f0: 62c2 234a 5fbe 170b 9abd 8b57 dc03 4d58  b.#J_......W..MX
-00001500: d0ca 6a00 fb25 9224 3093 6ef9 b364 6732  ..j..%.$0.n..dg2
-00001510: 1864 df56 b02e 8961 fabe abb5 33da d460  .d.V...a....3..`
-00001520: ed10 75ef 1fa4 6009 05bb 86f5 4c9d 1ade  ..u...`.....L...
-00001530: b1c2 d358 1f90 6d99 3b0f d3ef af96 ffca  ...X..m.;.......
-00001540: 5a9e 6e50 7e04 bb0f 4781 f5e4 f566 3577  Z.nP~...G....f5w
-00001550: 6291 4078 f3cb bc07 06dd e59b 37ad 309b  b.@x........7.0.
-00001560: d595 b1f4 eaa8 e1f1 c3bc 5ec7 680e 6ffa  ..........^.h.o.
-00001570: e3f2 9695 29d8 4e59 2d79 585c 804e 3406  ....).NY-yX\.N4.
-00001580: 4b1a d6f8 053f 994e 3291 9bb6 266d 95a0  K....?.N2...&m..
-00001590: 9dbd 557e 3775 e857 2b54 5bf7 5abd 745f  ..U~7u.W+T[.Z.t_
-000015a0: 9b92 c928 b7ad 1f89 6d94 6116 6c73 0d30  ...(....m.a.ls.0
-000015b0: 7ee0 d59c d317 1552 0a91 2bb8 bec5 999d  ~......R..+.....
-000015c0: 18f0 64c9 70c8 abee cc63 0673 a1e9 7591  ..d.p....c.s..u.
-000015d0: 52a4 a02c 46fe 3740 e385 7bfe c34d e069  R..,F.7@..{..M.i
-000015e0: 594b 37fa dd8a e682 d775 09ed e01a b3d4  YK7......u......
-000015f0: dabd 9940 9f06 7f31 dbf1 9fcc 7e5d cdfe  ...@...1....~]..
-00001600: 189e f502 8254 7ffe d20a 886a e8a4 299a  .....T.....j..).
-00001610: f2aa 393e 0000 584d 5020 9a03 0000 3c78  ..9>..XMP ....<x
-00001620: 3a78 6d70 6d65 7461 2078 6d6c 6e73 3a78  :xmpmeta xmlns:x
-00001630: 3d22 6164 6f62 653a 6e73 3a6d 6574 612f  ="adobe:ns:meta/
-00001640: 2220 783a 786d 7074 6b3d 2258 4d50 2043  " x:xmptk="XMP C
-00001650: 6f72 6520 362e 302e 3022 3e0a 2020 203c  ore 6.0.0">.   <
-00001660: 7264 663a 5244 4620 786d 6c6e 733a 7264  rdf:RDF xmlns:rd
-00001670: 663d 2268 7474 703a 2f2f 7777 772e 7733  f="http://www.w3
-00001680: 2e6f 7267 2f31 3939 392f 3032 2f32 322d  .org/1999/02/22-
-00001690: 7264 662d 7379 6e74 6178 2d6e 7323 223e  rdf-syntax-ns#">
-000016a0: 0a20 2020 2020 203c 7264 663a 4465 7363  .      <rdf:Desc
-000016b0: 7269 7074 696f 6e20 7264 663a 6162 6f75  ription rdf:abou
-000016c0: 743d 2222 0a20 2020 2020 2020 2020 2020  t="".           
-000016d0: 2078 6d6c 6e73 3a74 6966 663d 2268 7474   xmlns:tiff="htt
-000016e0: 703a 2f2f 6e73 2e61 646f 6265 2e63 6f6d  p://ns.adobe.com
-000016f0: 2f74 6966 662f 312e 302f 220a 2020 2020  /tiff/1.0/".    
-00001700: 2020 2020 2020 2020 786d 6c6e 733a 6578          xmlns:ex
-00001710: 6966 3d22 6874 7470 3a2f 2f6e 732e 6164  if="http://ns.ad
-00001720: 6f62 652e 636f 6d2f 6578 6966 2f31 2e30  obe.com/exif/1.0
-00001730: 2f22 0a20 2020 2020 2020 2020 2020 2078  /".            x
-00001740: 6d6c 6e73 3a78 6d70 3d22 6874 7470 3a2f  mlns:xmp="http:/
-00001750: 2f6e 732e 6164 6f62 652e 636f 6d2f 7861  /ns.adobe.com/xa
-00001760: 702f 312e 302f 223e 0a20 2020 2020 2020  p/1.0/">.       
-00001770: 2020 3c74 6966 663a 5952 6573 6f6c 7574    <tiff:YResolut
-00001780: 696f 6e3e 3732 3030 3030 2f31 3030 3030  ion>720000/10000
-00001790: 3c2f 7469 6666 3a59 5265 736f 6c75 7469  </tiff:YResoluti
-000017a0: 6f6e 3e0a 2020 2020 2020 2020 203c 7469  on>.         <ti
-000017b0: 6666 3a52 6573 6f6c 7574 696f 6e55 6e69  ff:ResolutionUni
-000017c0: 743e 323c 2f74 6966 663a 5265 736f 6c75  t>2</tiff:Resolu
-000017d0: 7469 6f6e 556e 6974 3e0a 2020 2020 2020  tionUnit>.      
-000017e0: 2020 203c 7469 6666 3a58 5265 736f 6c75     <tiff:XResolu
-000017f0: 7469 6f6e 3e37 3230 3030 302f 3130 3030  tion>720000/1000
-00001800: 303c 2f74 6966 663a 5852 6573 6f6c 7574  0</tiff:XResolut
-00001810: 696f 6e3e 0a20 2020 2020 2020 2020 3c74  ion>.         <t
-00001820: 6966 663a 4f72 6965 6e74 6174 696f 6e3e  iff:Orientation>
-00001830: 313c 2f74 6966 663a 4f72 6965 6e74 6174  1</tiff:Orientat
-00001840: 696f 6e3e 0a20 2020 2020 2020 2020 3c65  ion>.         <e
-00001850: 7869 663a 5069 7865 6c58 4469 6d65 6e73  xif:PixelXDimens
-00001860: 696f 6e3e 3438 3c2f 6578 6966 3a50 6978  ion>48</exif:Pix
-00001870: 656c 5844 696d 656e 7369 6f6e 3e0a 2020  elXDimension>.  
-00001880: 2020 2020 2020 203c 6578 6966 3a50 6978         <exif:Pix
-00001890: 656c 5944 696d 656e 7369 6f6e 3e34 393c  elYDimension>49<
-000018a0: 2f65 7869 663a 5069 7865 6c59 4469 6d65  /exif:PixelYDime
-000018b0: 6e73 696f 6e3e 0a20 2020 2020 2020 2020  nsion>.         
-000018c0: 3c78 6d70 3a43 7265 6174 6f72 546f 6f6c  <xmp:CreatorTool
-000018d0: 3e50 6978 656c 6d61 746f 7220 5072 6f20  >Pixelmator Pro 
-000018e0: 332e 352e 373c 2f78 6d70 3a43 7265 6174  3.5.7</xmp:Creat
-000018f0: 6f72 546f 6f6c 3e0a 2020 2020 2020 2020  orTool>.        
-00001900: 203c 786d 703a 4372 6561 7465 4461 7465   <xmp:CreateDate
-00001910: 3e32 3032 342d 3034 2d30 3854 3133 3a34  >2024-04-08T13:4
-00001920: 313a 3134 2b30 383a 3030 3c2f 786d 703a  1:14+08:00</xmp:
-00001930: 4372 6561 7465 4461 7465 3e0a 2020 2020  CreateDate>.    
-00001940: 2020 2020 203c 786d 703a 4d65 7461 6461       <xmp:Metada
-00001950: 7461 4461 7465 3e32 3032 342d 3034 2d30  taDate>2024-04-0
-00001960: 3854 3133 3a34 323a 3437 2b30 383a 3030  8T13:42:47+08:00
-00001970: 3c2f 786d 703a 4d65 7461 6461 7461 4461  </xmp:MetadataDa
-00001980: 7465 3e0a 2020 2020 2020 3c2f 7264 663a  te>.      </rdf:
-00001990: 4465 7363 7269 7074 696f 6e3e 0a20 2020  Description>.   
-000019a0: 3c2f 7264 663a 5244 463e 0a3c 2f78 3a78  </rdf:RDF>.</x:x
-000019b0: 6d70 6d65 7461 3e0a                      mpmeta>.
+00000c70: 5048 e003 0000 0190 b66d dbd9 c813 badf  PH.......m......
+00000c80: 7a6c 9b6b dbb6 6d73 b0b6 6ddb b66d 7bc7  zl.k..ms..m..m{.
+00000c90: e6da 6667 b64c 9e0f cd74 9389 8809 8094  ..fg.L...t......
+00000ca0: 8ca1 7896 6cac 116a 3f40 2519 5300 a81b  ..x.l..j?@%.S...
+00000cb0: d747 a875 6609 008c 4911 b8b2 2c60 7766  .G.uf...I...,`wf
+00000cc0: 33b3 70db 9e1e 0ca0 411f 9904 36db b7c9  3.p.....A...6...
+00000cd0: 1593 bef7 8765 947e b20c 605d afd9 4b50  .....e.~..`]..KP
+00000ce0: e2c1 5e85 7fee b7da 728b 58d3 c960 b84c  ..^.....r.X..`.L
+00000cf0: 8c5b a314 8309 d81e d7b6 876f 1697 b0b3  .[.........o....
+00000d00: a30a 084c e7f6 db4e f9b3 d01d 22ba cf6c  ...L...N...."..l
+00000d10: 2d07 e095 a95f 54dd 6bcc 678e be77 6425  -...._T.k.g..wd%
+00000d20: a7bc a74c ff53 3fea 0000 835d 98c2 1a87  ...L.S?....]....
+00000d30: 3171 c160 50ef 349b 7edd aa52 e510 4f07  1q.`P.4.~..R..O.
+00000d40: 2313 3832 efb3 8dd2 5d0f 0000 d9d4 7d8e  #.82....].....}.
+00000d50: d620 32bd 0614 6ae6 3be6 8699 df65 3fdd  . 2...j.;....e?.
+00000d60: 4caf 0f9a 886e 0705 c468 cdd1 602a b9cd  L....n...h..`*..
+00000d70: c558 585d e2cd 8d85 87cf 0db2 9175 29a0  .XX].........u).
+00000d80: eb53 7f91 704e 74b2 8e4c c3ec a3cf eed8  .S..pNt..L......
+00000d90: fa73 a275 b6eb 0a8c 46fa d3ad 7226 4f5f  .s.u....F...r&O_
+00000da0: be51 91bc 8e88 2ef8 4415 f246 636e 3530  .Q......D..Fcn50
+00000db0: 2175 df4e 6a38 36ef 1afd 8336 4ce2 e9ff  !u.Nj86....6L...
+00000dc0: af04 5ca0 945e dd4a cb50 a47a 486a 3da8  ..\..^.J.P.zHj=.
+00000dd0: 3c6d c3df d0cb 7b24 a2fe d027 3aa2 72f5  <m....{$...':.r.
+00000de0: 54c0 5e21 00cd e59d 2db6 679c 6cfd 82c4  T.^!....-.g.l...
+00000df0: 3f30 382e 6349 b51d e584 64f3 0ab5 051c  ?08.cI....d.....
+00000e00: bf6d a656 b4bc e837 f42d 256e bfbb 105c  .m.V...7.-%n...\
+00000e10: fac6 b689 a7cf 477e 8996 718f 3346 7906  ......G~..q.3Fy.
+00000e20: 3bc0 5ad5 6992 f85f 0bfc 27eb f686 9382  ;.Z.i.._..'.....
+00000e30: 2f3c e7f9 1faa 7a5d fabf 95a2 705a a88f  /<....z]....pZ..
+00000e40: 3de0 38b0 a31c 36de 72d6 71e3 4bed 6793  =.8...6.r.q.K.g.
+00000e50: 14fc 8bbb d997 ab62 c4e3 4e72 34bb d59b  .......b..Nr4...
+00000e60: 359a db72 1f49 ce3f e87c 7f2e 00cd d46b  5..r.I.?.|.....k
+00000e70: 3e61 35dc a238 c974 06bd b627 0074 ff93  >a5..8.t...'.t..
+00000e80: fcea d7a3 1c92 9a9b 3f74 eb30 3b0b b775  ........?t.0;..u
+00000e90: a92f 3892 fe65 65c8 20ac 72af f7b5 185c  ./8..ee. .r....\
+00000ea0: 68d8 aeac 4208 70be c24b 67d6 ea5f 7762  h...B.p..Kg.._wb
+00000eb0: 45a0 dc35 4e32 e2b3 9f5c f164 429a 199f  E..5N2...\.dB...
+00000ec0: 78c9 74d7 ab84 5e5c 6d0b 8095 18b1 e32f  x.t...^\m....../
+00000ed0: 49ff 67ae 1df3 0a94 0188 4cf8 a6a3 e2f8  I.g.......L.....
+00000ee0: 6760 6445 7b00 e81d 577b e26f e978 a25f  g`dE{...W{.o.x._
+00000ef0: cf5e af54 0161 fb36 ca35 3dd6 afcc 9746  .^.T.a.6.5=....F
+00000f00: bb6c d7e7 dc61 3d93 7b2a 5065 6618 0065  .l...a=.{*Pef..e
+00000f10: cdfb 12ad a85c 3644 aeec de5f 0900 3635  .....\6D..._..65
+00000f20: 4a34 7cc7 4b43 fc71 8d5a 0361 8749 8949  J4|.KC.q.Z.a.I.I
+00000f30: 993c 9939 098c 3c7d 5978 ec64 7501 36f4  .<.9..<}Yx.du.6.
+00000f40: 56cd 582d 7d9f 9b28 9e61 f51d 9e7e ce5b  V.X-}..(.a...~.[
+00000f50: b042 6e01 175f 995d ef95 9d9b ff14 8fb6  .Bn.._.]........
+00000f60: 9498 bfb1 8bc6 ce0f d632 f431 91ee 8d18  .........2.1....
+00000f70: 1957 4c94 50dd 4f05 eb99 4fa5 52ab 387a  .WL.P.O...O.R.8z
+00000f80: 329b 1321 bec1 4be2 bee6 cc77 b0ae d48d  2..!..K....w....
+00000f90: b437 baf7 fb1b 57fe 44ef 3e59 a53f 9fff  .7....W.D.>Y.?..
+00000fa0: a1cc 88ac d7f7 1efe ea6c ddf0 63a5 fa8d  .........l..c...
+00000fb0: adaa 449d 1f19 3d1e 1071 0566 223e f127  ..D...=..q.f">.'
+00000fc0: 7d2e 3f34 afb1 a77f 9893 5f7c 8c75 6195  }.?4......_|.ua.
+00000fd0: 20d8 f45d 7397 8744 292d 3673 641c b45e   ..]s..D)-6sd..^
+00000fe0: afdb d672 ebed 5e00 3417 a66a ac2a da75  ...r..^.4..j.*.u
+00000ff0: ff3a db89 1c65 face e60c 17fd 5dfb cc3b  .:...e......]..;
+00001000: 7c37 d843 0d80 753c 5151 14b8 940c dbc7  |7.C..u<QQ......
+00001010: 5352 f00d 6e95 0700 948b 2b01 4166 af10  SR..n.....+.Af..
+00001020: 0781 b7de e73f 6caf da68 5a6e 6b51 314a  .....?l..hZnkQ1J
+00001030: 2324 7e9f 4795 fd5d 1902 d73e 1fc2 0030  #$~.G..]...>...0
+00001040: 06a9 9b9f b087 a572 fa7e 398a a53a 4221  .......r.~9..:B!
+00001050: a05e de87 8903 5650 3820 9204 0000 3016  .^....VP8 ....0.
+00001060: 009d 012a 3000 3100 3e85 3091 4825 22a1  ...*0.1.>.0.H%".
+00001070: a137 e800 a010 896c 00a9 2734 3e37 c779  .7.....l..'4>7.y
+00001080: a2d5 3fca ff2e df87 205d b84e 3fcc 03f5  ..?..... ].N?...
+00001090: 57a4 0798 0fda 0f57 4fef 1ea2 bfc7 7a80  W......WO.....z.
+000010a0: 7f51 feed eaeb ea33 e81b fb3b e9bf ec51  .Q.....3...;...Q
+000010b0: fdb7 fdff ee67 b555 cb3f 08fb fa7a 2cfe  .....g.U.?...z,.
+000010c0: 6881 5a6f 787e 07e9 1a99 ef8e bfad 3d83  h.Zox~........=.
+000010d0: 3f5b 3ad4 7ed1 94a1 6e86 f2b3 4a3f 9a78  ?[:.~...n...J?.x
+000010e0: b987 dcf1 9419 361a c6e1 4cad 15a0 11ac  ......6...L.....
+000010f0: 1058 73e6 b14c 9dd2 dce0 8887 86f6 41b1  .Xs..L........A.
+00001100: 33bf f1b5 2182 ecdc 8d73 ead6 3bce 2eaa  3...!....s..;...
+00001110: 3eff dc65 a1fa 2080 00fe f84e 96ac 5409  >..e.. ....N..T.
+00001120: c377 90a8 75e0 792c 9246 0293 df92 f8c0  .w..u.y,.F......
+00001130: 121a 453e 0a04 6eaf 10e9 ecfa 9fa2 1c80  ..E>..n.........
+00001140: 12ba dbea 2e3c 03ff 0fa1 662f ee93 4152  .....<....f/..AR
+00001150: ec0a 762e e5a8 c56b 3fda 40b0 d7e8 2ba2  ..v....k?.@...+.
+00001160: b04f 65bc e1bc 6ab7 be7e f6b4 f7ac 68cd  .Oe...j..~....h.
+00001170: fc09 6e26 3d37 66a9 7fe0 a97c caa6 26a2  ..n&=7f....|..&.
+00001180: 0aa6 0572 10c8 ff1f 6649 eab0 e029 b863  ...r....fI...).c
+00001190: 393e 8c76 7222 67fa 2e7b 3bc0 ef51 eb72  9>.vr"g..{;..Q.r
+000011a0: 20fe 4608 baf2 a938 1bcf ebb0 4dd3 8213   .F....8....M...
+000011b0: e29c a4c8 1475 df1d f3e7 4c28 3cd9 22ab  .....u....L(<.".
+000011c0: 7d5c 079a 742d c0e9 ba9f fc45 8a6a ab18  }\..t-.....E.j..
+000011d0: be05 8daf b0f2 8ef9 725d 27ce 2633 505d  ........r]'.&3P]
+000011e0: 79ab bacc bd03 f3a5 315d 90c5 195d d5ba  y.......1]...]..
+000011f0: 020e 08c6 53f2 06b5 2a0f f034 f0fd 5f80  ....S...*..4.._.
+00001200: b5d2 7378 df50 86bd 67d9 0f81 01cd eaf4  ..sx.P..g.......
+00001210: faac f704 90dd 2f1e 7ed6 9ac5 648f 99f8  ....../.~...d...
+00001220: e476 00bb 3350 c867 8c4d 6fa8 d5ff 293d  .v..3P.g.Mo...)=
+00001230: 7566 5dc9 02ae 853c 5a77 e0d3 fdc4 cd02  uf]....<Zw......
+00001240: 4027 f899 a973 00f4 5b1a 2c5d dce5 1164  @'...s..[.,]...d
+00001250: f052 cb3a ac8b 8bb3 ea18 5523 6098 0ea6  .R.:......U#`...
+00001260: c8fb a584 e0a5 98aa 8066 110b 91d1 e8f2  .........f......
+00001270: df31 b812 e3a0 3104 7bda a7b3 79e3 5fdd  .1....1.{...y._.
+00001280: b057 682c 11c2 09d8 6ac9 aa5e d507 4529  .Wh,....j..^..E)
+00001290: 6024 9225 e22e eb68 322d 5104 0f6f a310  `$.%...h2-Q..o..
+000012a0: f3a8 5350 ce4c 0ade 767d 012e 3fa9 bf21  ..SP.L..v}..?..!
+000012b0: 3d5b 19fb c7e2 731d cb22 89b7 f8de 1cfe  =[....s.."......
+000012c0: fc0a c549 b38f b43f 3ae7 d6b0 5aa3 799b  ...I...?:...Z.y.
+000012d0: 333e 2e92 bc4a 57e0 ee65 2955 c216 2ea0  3>...JW..e)U....
+000012e0: f5cc 1020 416a 3f83 cfc8 ae51 77ce a5be  ... Aj?....Qw...
+000012f0: c205 ebe3 52a1 695f 64fb 5916 f02e aeb7  ....R.i_d.Y.....
+00001300: 5a37 eed7 7b3c 3ed2 b581 6e6b f68b c4ab  Z7..{<>...nk....
+00001310: b677 5093 2ae1 b1c7 12ae 7bd4 5266 a279  .wP.*.....{.Rf.y
+00001320: ae09 eba5 d258 42b5 f037 7919 e823 ace6  .....XB..7y..#..
+00001330: f03b 6c50 8bf7 9baf 33be 1348 f81a 0b39  .;lP....3..H...9
+00001340: 39ce 8983 59cf b010 b0cf 40d0 b29f e975  9...Y.....@....u
+00001350: e2e3 4db6 655e 256d 8ff4 8bd8 1f63 0375  ..M.e^%m.....c.u
+00001360: 4b0e 7929 b860 a2f7 6092 9ff7 4084 6291  K.y).`..`...@.b.
+00001370: 93af d6b5 35f2 7082 f5d7 de97 723e a7c0  ....5.p.....r>..
+00001380: 9d11 0536 2800 f401 e702 fcb8 c0a5 6f6a  ...6(.........oj
+00001390: 7da9 2669 81d5 6f7e ea13 388f c2ae 96a8  }.&i..o~..8.....
+000013a0: 2ca8 093c 60cc 1539 9982 c141 47e7 8e3d  ,..<`..9...AG..=
+000013b0: 1acd cb3a 056a 7516 f827 ae22 5c1a 6076  ...:.ju..'."\.`v
+000013c0: 620d d0cf bf81 a189 03c8 d48a 7137 828b  b...........q7..
+000013d0: bdee 48af 314c fde1 0618 e17b faf5 7320  ..H.1L.....{..s 
+000013e0: 286d e910 fc2d 591a 9be7 485d 23f7 d12c  (m...-Y...H]#..,
+000013f0: 66b2 96d5 3ef8 0589 ec46 45de 3608 0f4e  f...>....FE.6..N
+00001400: b711 b85b 85fc 629a b9c3 37d8 b5d6 e888  ...[..b...7.....
+00001410: 21bd 3c1a 6d67 9f6a dd05 ccfc 8403 9b95  !.<.mg.j........
+00001420: cead b8b0 82b1 a843 d7bc 1319 4580 2e83  .......C....E...
+00001430: 7219 6515 72d9 cf67 71bf 62ec 1039 c806  r.e.r..gq.b..9..
+00001440: c27b e383 2d9e 2a01 9b1a 953d 0590 4429  .{..-.*....=..D)
+00001450: 5b53 edb5 317e fdd8 6e43 a446 15b2 f5f2  [S..1~..nC.F....
+00001460: 57e9 87ed 58f3 8e4b 84d2 1b68 4ec8 97dc  W...X..K...hN...
+00001470: 5aa1 e978 e8eb 541b 19eb 16e8 7ccb b1e1  Z..x..T.....|...
+00001480: 77be 85c2 bc79 195e 2c31 6801 412b a156  w....y.^,1h.A+.V
+00001490: b022 9a46 8cbe 16b8 c213 a3d8 3920 63a7  .".F........9 c.
+000014a0: e683 0eb1 8246 f996 6f70 9239 dfc6 7df5  .....F..op.9..}.
+000014b0: 638b fb9e 368c fce4 b8d0 dff5 8364 b96e  c...6........d.n
+000014c0: 7f5f 9f03 838f f060 d12b be9d 9c01 c316  ._.....`.+......
+000014d0: 980e 06e7 bd80 e0af 97ff 803f 2e82 739f  ...........?..s.
+000014e0: efff 007e 5d04 e73f f9a7 8004 6318 8000  ...~]..?....c...
+000014f0: 584d 5020 9a03 0000 3c78 3a78 6d70 6d65  XMP ....<x:xmpme
+00001500: 7461 2078 6d6c 6e73 3a78 3d22 6164 6f62  ta xmlns:x="adob
+00001510: 653a 6e73 3a6d 6574 612f 2220 783a 786d  e:ns:meta/" x:xm
+00001520: 7074 6b3d 2258 4d50 2043 6f72 6520 362e  ptk="XMP Core 6.
+00001530: 302e 3022 3e0a 2020 203c 7264 663a 5244  0.0">.   <rdf:RD
+00001540: 4620 786d 6c6e 733a 7264 663d 2268 7474  F xmlns:rdf="htt
+00001550: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
+00001560: 3939 392f 3032 2f32 322d 7264 662d 7379  999/02/22-rdf-sy
+00001570: 6e74 6178 2d6e 7323 223e 0a20 2020 2020  ntax-ns#">.     
+00001580: 203c 7264 663a 4465 7363 7269 7074 696f   <rdf:Descriptio
+00001590: 6e20 7264 663a 6162 6f75 743d 2222 0a20  n rdf:about="". 
+000015a0: 2020 2020 2020 2020 2020 2078 6d6c 6e73             xmlns
+000015b0: 3a65 7869 663d 2268 7474 703a 2f2f 6e73  :exif="http://ns
+000015c0: 2e61 646f 6265 2e63 6f6d 2f65 7869 662f  .adobe.com/exif/
+000015d0: 312e 302f 220a 2020 2020 2020 2020 2020  1.0/".          
+000015e0: 2020 786d 6c6e 733a 7469 6666 3d22 6874    xmlns:tiff="ht
+000015f0: 7470 3a2f 2f6e 732e 6164 6f62 652e 636f  tp://ns.adobe.co
+00001600: 6d2f 7469 6666 2f31 2e30 2f22 0a20 2020  m/tiff/1.0/".   
+00001610: 2020 2020 2020 2020 2078 6d6c 6e73 3a78           xmlns:x
+00001620: 6d70 3d22 6874 7470 3a2f 2f6e 732e 6164  mp="http://ns.ad
+00001630: 6f62 652e 636f 6d2f 7861 702f 312e 302f  obe.com/xap/1.0/
+00001640: 223e 0a20 2020 2020 2020 2020 3c65 7869  ">.         <exi
+00001650: 663a 5069 7865 6c59 4469 6d65 6e73 696f  f:PixelYDimensio
+00001660: 6e3e 3439 3c2f 6578 6966 3a50 6978 656c  n>49</exif:Pixel
+00001670: 5944 696d 656e 7369 6f6e 3e0a 2020 2020  YDimension>.    
+00001680: 2020 2020 203c 6578 6966 3a50 6978 656c       <exif:Pixel
+00001690: 5844 696d 656e 7369 6f6e 3e34 383c 2f65  XDimension>48</e
+000016a0: 7869 663a 5069 7865 6c58 4469 6d65 6e73  xif:PixelXDimens
+000016b0: 696f 6e3e 0a20 2020 2020 2020 2020 3c74  ion>.         <t
+000016c0: 6966 663a 5265 736f 6c75 7469 6f6e 556e  iff:ResolutionUn
+000016d0: 6974 3e32 3c2f 7469 6666 3a52 6573 6f6c  it>2</tiff:Resol
+000016e0: 7574 696f 6e55 6e69 743e 0a20 2020 2020  utionUnit>.     
+000016f0: 2020 2020 3c74 6966 663a 5852 6573 6f6c      <tiff:XResol
+00001700: 7574 696f 6e3e 3732 3030 3030 2f31 3030  ution>720000/100
+00001710: 3030 3c2f 7469 6666 3a58 5265 736f 6c75  00</tiff:XResolu
+00001720: 7469 6f6e 3e0a 2020 2020 2020 2020 203c  tion>.         <
+00001730: 7469 6666 3a4f 7269 656e 7461 7469 6f6e  tiff:Orientation
+00001740: 3e31 3c2f 7469 6666 3a4f 7269 656e 7461  >1</tiff:Orienta
+00001750: 7469 6f6e 3e0a 2020 2020 2020 2020 203c  tion>.         <
+00001760: 7469 6666 3a59 5265 736f 6c75 7469 6f6e  tiff:YResolution
+00001770: 3e37 3230 3030 302f 3130 3030 303c 2f74  >720000/10000</t
+00001780: 6966 663a 5952 6573 6f6c 7574 696f 6e3e  iff:YResolution>
+00001790: 0a20 2020 2020 2020 2020 3c78 6d70 3a4d  .         <xmp:M
+000017a0: 6574 6164 6174 6144 6174 653e 3230 3234  etadataDate>2024
+000017b0: 2d30 342d 3038 5431 343a 3433 3a35 322b  -04-08T14:43:52+
+000017c0: 3038 3a30 303c 2f78 6d70 3a4d 6574 6164  08:00</xmp:Metad
+000017d0: 6174 6144 6174 653e 0a20 2020 2020 2020  ataDate>.       
+000017e0: 2020 3c78 6d70 3a43 7265 6174 6f72 546f    <xmp:CreatorTo
+000017f0: 6f6c 3e50 6978 656c 6d61 746f 7220 5072  ol>Pixelmator Pr
+00001800: 6f20 332e 352e 373c 2f78 6d70 3a43 7265  o 3.5.7</xmp:Cre
+00001810: 6174 6f72 546f 6f6c 3e0a 2020 2020 2020  atorTool>.      
+00001820: 2020 203c 786d 703a 4372 6561 7465 4461     <xmp:CreateDa
+00001830: 7465 3e32 3032 342d 3034 2d30 3854 3133  te>2024-04-08T13
+00001840: 3a34 313a 3134 2b30 383a 3030 3c2f 786d  :41:14+08:00</xm
+00001850: 703a 4372 6561 7465 4461 7465 3e0a 2020  p:CreateDate>.  
+00001860: 2020 2020 3c2f 7264 663a 4465 7363 7269      </rdf:Descri
+00001870: 7074 696f 6e3e 0a20 2020 3c2f 7264 663a  ption>.   </rdf:
+00001880: 5244 463e 0a3c 2f78 3a78 6d70 6d65 7461  RDF>.</x:xmpmeta
+00001890: 3e0a                                     >.
```

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_001.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_002.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg1/cambg_003.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg1/cambg_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_001.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_002.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/images/vmove_cambg2/cambg_003.webp` & `SightTraining-0.1.22/spacedefense/assets/images/vmove_cambg2/cambg_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/.DS_Store` & `SightTraining-0.1.22/spacedefense/assets/sounds/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/bgm.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/bgm.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/fire.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/fire_blast.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/fire_blast.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/firehit.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/smyf_join.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/smyf_join.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_angry.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_angry.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_end_loss.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_end_loss.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_end_win.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_end_win.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_mid.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_mid.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_pre.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_pre.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/stage_start.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/stage_start.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/sufo_join.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/sufo_join.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/super_fire.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/super_fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/super_firehit.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/super_firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/ufo_fire.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/ufo_fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/assets/sounds/ufo_firehit.ogg` & `SightTraining-0.1.22/spacedefense/assets/sounds/ufo_firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/common.py` & `SightTraining-0.1.22/spacedefense/common.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/config.py` & `SightTraining-0.1.22/spacedefense/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,61 +47,61 @@
         "sound_volume": 0.4,
     },
     "smyf_join": {
         "sound": "sounds/smyf_join.ogg",
         "sound_volume": 0.4,
     },
     "my_score_step": 5,
-    "ufo_score_step": 3,
+    "ufo_score_step": 2,
     "unit_collision_cooldown": 1000,
     "ufo_master": {
         "image_sequence": "images/ufo_master",
         "images": ["images/ufo_master/ufo_master_001.webp"],
         "first_pos": (720, 100),
-        "life_value": 30000,
-        "shield_value": 1000,
+        "life_value": 50000,
+        "shield_value": 2000,
         "shield_recharge_step": 1,
         "bullet_color": "cyan",
         "bullet_speed": 7,
         "bullet_damage": 20,
         "bullet_radius": 10,
         "trace_fire_delay": 30,
         "fire_interceptor_delay": 20,
         "fire_delay": 30,
         "fire_score": 5,
         "fire_sound": "sounds/ufo_fire.ogg",
         "firehit_sound": "sounds/ufo_firehit.ogg",
         "fire_sound_volume": 0.4,
         "firehit_sound_volume": 0.4,
         "super_bullet": {
-            "score_cast": 200,
+            "score_cast": 50,
             "life_value": 300,
             "speed": 2,
             "acc_distance_1": 350,
             "acc_distance_2": 150,
             "damage": 200,
-            "fire_delay": 300,
+            "fire_delay": 200,
             "image": "images/ufo_super_bullet.webp",
             "fire_sound": "sounds/super_fire.ogg",
             "firehit_sound": "sounds/firehit.ogg",
         },
     },
     "ufo_slave": {
         "image_sequence": "images/ufo_slave",
         "images": ["images/ufo_slave/ufo_slave_001.webp", "images/ufo_slave/ufo_slave_002.webp"],
         "first_pos": (400, -100),
         "score_cast": 50,
         "max_limit": 8,
         "min_limit": 3,
         "shield_value": 100,
         "shield_recharge_step": 5,
-        "life_value": 500,
+        "life_value": 700,
         "bullet_speed": 9,
         "bullet_color": "cyan",
-        "bullet_damage": 10,
+        "bullet_damage": 15,
         "bullet_radius": 8,
         "trace_fire_delay": 40,
         "fire_interceptor_delay": 20,
         "fire_delay": 15,
         "fire_sound": "sounds/ufo_fire.ogg",
         "firehit_sound": "sounds/ufo_firehit.ogg",
         "fire_sound_volume": 0.4,
@@ -118,15 +118,15 @@
         "fire_sound_volume": 0.4,
         "firehit_sound_volume": 0.4,
         "upgrade_cast": 100,
         "level1": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 2,
             "bullet_speed": 15,
-            "bullet_damage": 10,
+            "bullet_damage": 15,
             "bullet_radius": 5,
             "fire_delay": 8,
             "fire_sound": "sounds/fire.ogg",
         },
         "level2": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 1,
@@ -136,15 +136,15 @@
             "fire_delay": 12,
             "fire_sound": "sounds/fire.ogg",
         },
         "level3": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 2,
             "bullet_speed": 7,
-            "bullet_damage": 3,
+            "bullet_damage": 5,
             "bullet_radius": 5,
             "fire_delay": 10,
             "fire_sound": "sounds/fire.ogg",
         },
         "super_bullet": {
             "score_cast": 200,
             "life_value": 300,
@@ -167,15 +167,15 @@
         "max_limit": 7,
         "min_limit": 2,
         "life_value": 500,
         "bullet_speed": 10,
         "bullet_color": "light_yellow",
         "bullet_damage": 20,
         "bullet_radius": 8,
-        "fire_delay": 15,
+        "fire_delay": 12,
         "trace_fire_delay": 30,
         "fire_sound": "sounds/fire.ogg",
         "firehit_sound": "sounds/firehit.ogg",
         "fire_sound_volume": 0.4,
         "firehit_sound_volume": 0.4,
     },
 }
```

### Comparing `SightTraining-0.1.21/spacedefense/flight_unit.py` & `SightTraining-0.1.22/spacedefense/flight_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class FlightUnit(pygame.sprite.Sprite):
     """飞行单位"""
 
     def __init__(self, type: str, config_data, sound_channel=None):
         pygame.sprite.Sprite.__init__(self)
         self.config = config_data
-        self.sound_channel = pygame.mixer.Channel(1)
+        self.sound_channel = pygame.mixer.Channel(2)
         self.type = type
         self.hp = self.config["life_value"]
         self.life_value = self.config["life_value"]
         self.shield_hp = self.config["shield_value"]
         self.shield_value = self.config["shield_value"]
         self.image_sequence = []
         self.image_index = 0
@@ -41,15 +41,15 @@
         self.frame_rate = 300  # 每帧间隔毫秒数
         self.speed_x = random.randint(1, 6)  # 在x方向上设置随机速度
         self.speed_y = random.randint(1, 4)  # 在y方向上设置随机速度
         # 被消灭的时间
         self.kill_time = None
         self.fire_delay = 0
         self.trace_fire_delay = 0
-        self.super_fire_delay = 600
+        self.super_fire_delay = 0
         self.fire_interceptor_delay = 0
         self.is_angry = False
 
         self.recharge_delay = 0  # 护盾充能延迟
         self.shield_recharge_step = self.config["shield_recharge_step"]  # 护盾充能步长
 
     def fire(
```

### Comparing `SightTraining-0.1.21/spacedefense/game.py` & `SightTraining-0.1.22/spacedefense/game.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.21/spacedefense/my_master.py` & `SightTraining-0.1.22/spacedefense/my_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,18 @@
 
     def trace_fire(self, src_group, target_groups, particle_group, level, priority: str = "distance"):
         # self.recharge_delay = 0
         if self.fire_delay == 0:
             _bullet_per_num = self.config[level]["bullet_per_num"]  # 想要发射的子弹总数
             total_bullets = _bullet_per_num  # 想要发射的子弹总数
             bullet_spacing = 25
-            if self.level >= 3:
+            if self.level > 1:
+                total_bullets = self.level
+            
+            if total_bullets > 2:
                 total_bullets = 2
                 
 
             # 计算第一个子弹的偏移量
             offset = bullet_spacing * (total_bullets - 1) / 2
             for i in range(total_bullets):
                 bullet_x = self.rect.centerx - offset + i * bullet_spacing
```

### Comparing `SightTraining-0.1.21/spacedefense/scene_main.py` & `SightTraining-0.1.22/spacedefense/scene_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,19 +357,22 @@
 
                 ufo.fire(
                     group=self.ufo_bullets,
                     direction=random.choice(directions),
                     target_groups=[self.my_flight_units, self.my_bullets],
                     particle_group=self.particles,
                 )
-                ufo.super_fire(
-                    self.ufo_super_bullets,
-                    self.my_master_fighter,
-                    self.particles,
-                )
+                score_cast = configmap["ufo_master"]["super_bullet"]["score_cast"]
+                if self.ufo_score > score_cast * 3 and self.ufo_master.super_fire_delay == 0:
+                    ufo.super_fire(
+                        self.ufo_super_bullets,
+                        self.my_master_fighter,
+                        self.particles,
+                    )
+                    self.update_ufo_socre(-score_cast)
                 ufo.fire_interceptor(
                     group=self.ufo_bullets,
                     target_groups=[self.my_super_bullets],
                     particle_group=self.particles,
                 )
 
         elif event.type == self.MY_FIGHTER_FIRE_TIMEREVENT:
@@ -607,14 +610,15 @@
             self.ufo_super_bullets, self.my_bullets, False, True
         )
 
         for usupb, mybs in usbub_collisions.items():
             for myb in mybs:
                 self.create_hit_particle(usupb, 10)
                 usupb.hit(myb.damage)
+                self.update_my_socre(myb.damage // self.my_score_step)
 
 
         # 检测导弹冲击波与UF方炮弹的碰撞
         pygame.sprite.groupcollide(
             self.shock_particles, self.ufo_bullets, dokilla=True, dokillb=True
         )
```

### Comparing `SightTraining-0.1.21/spacedefense/scenes.py` & `SightTraining-0.1.22/spacedefense/scenes.py`

 * *Files identical despite different names*

