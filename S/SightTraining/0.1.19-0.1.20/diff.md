# Comparing `tmp/SightTraining-0.1.19.tar.gz` & `tmp/SightTraining-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SightTraining-0.1.19.tar", last modified: Mon Apr  8 02:57:12 2024, max compression
+gzip compressed data, was "SightTraining-0.1.20.tar", last modified: Mon Apr  8 03:14:46 2024, max compression
```

## Comparing `SightTraining-0.1.19.tar` & `SightTraining-0.1.20.tar`

### file list

```diff
@@ -1,84 +1,82 @@
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.100620 SightTraining-0.1.19/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.19/LICENSE
--rw-r--r--   0 wangjuntao   (501) staff       (20)       58 2024-04-01 09:37:31.000000 SightTraining-0.1.19/MANIFEST.in
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 02:57:12.100291 SightTraining-0.1.19/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.19/Readme.md
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.099895 SightTraining-0.1.19/SightTraining.egg-info/
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2967 2024-04-08 02:57:12.000000 SightTraining-0.1.19/SightTraining.egg-info/SOURCES.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/dependency_links.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/entry_points.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/requires.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/top_level.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-08 02:57:12.101150 SightTraining-0.1.19/setup.cfg
--rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-01 18:49:57.000000 SightTraining-0.1.19/setup.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.065717 SightTraining-0.1.19/spacedefense/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1261 2024-04-07 13:38:55.000000 SightTraining-0.1.19/spacedefense/__init__.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    17516 2024-04-08 01:33:20.000000 SightTraining-0.1.19/spacedefense/actors.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.065892 SightTraining-0.1.19/spacedefense/assets/
--rw-r--r--   0 wangjuntao   (501) staff       (20)    10244 2024-04-08 02:55:20.000000 SightTraining-0.1.19/spacedefense/assets/.DS_Store
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.072018 SightTraining-0.1.19/spacedefense/assets/images/
--rw-r--r--   0 wangjuntao   (501) staff       (20)    18436 2024-04-08 02:55:20.000000 SightTraining-0.1.19/spacedefense/assets/images/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)    93950 2024-04-08 02:52:13.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   115516 2024-04-08 02:53:25.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover_loss.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   129152 2024-04-08 02:53:06.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover_win.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)    31179 2024-04-01 06:54:20.000000 SightTraining-0.1.19/spacedefense/assets/images/icon.png
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7138 2024-04-07 13:31:54.000000 SightTraining-0.1.19/spacedefense/assets/images/master_fighter.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6772 2024-04-07 13:57:36.000000 SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter1.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6578 2024-04-07 13:59:55.000000 SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter2.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.074867 SightTraining-0.1.19/spacedefense/assets/images/myf_master/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:42:44.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7568 2024-04-07 13:41:47.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7358 2024-04-07 13:41:55.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     7442 2024-04-07 13:42:06.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6916 2024-04-07 13:42:17.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_004.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)    95336 2024-04-07 14:00:31.000000 SightTraining-0.1.19/spacedefense/assets/images/scale_cambg1.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5298 2024-04-08 01:24:57.000000 SightTraining-0.1.19/spacedefense/assets/images/super_bullet.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.076598 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:00.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     8908 2024-04-07 13:49:06.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9406 2024-04-07 13:49:20.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9166 2024-04-07 13:49:28.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9482 2024-04-07 13:49:58.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_004.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.077978 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:40.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5838 2024-04-07 13:52:06.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5676 2024-04-07 13:52:20.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5802 2024-04-07 13:52:28.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5682 2024-04-07 13:52:42.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.081262 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:18:10.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   323000 2024-04-07 13:16:38.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   262066 2024-04-07 13:16:50.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   322282 2024-04-07 13:17:12.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_003.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.083298 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:27:10.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   212520 2024-04-07 13:24:30.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_001.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   210670 2024-04-07 13:24:44.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_002.webp
--rw-r--r--   0 wangjuntao   (501) staff       (20)   221782 2024-04-07 13:25:46.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_003.webp
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.099552 SightTraining-0.1.19/spacedefense/assets/sounds/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-01 07:13:33.000000 SightTraining-0.1.19/spacedefense/assets/sounds/.DS_Store
--rw-r--r--   0 wangjuntao   (501) staff       (20)   781119 2024-03-29 14:19:53.000000 SightTraining-0.1.19/spacedefense/assets/sounds/bgm1.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   613595 2024-04-01 06:38:42.000000 SightTraining-0.1.19/spacedefense/assets/sounds/bgm3.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    19873 2024-03-29 14:26:24.000000 SightTraining-0.1.19/spacedefense/assets/sounds/fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    18471 2024-03-29 14:25:00.000000 SightTraining-0.1.19/spacedefense/assets/sounds/fire_blast.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    26919 2024-03-29 14:24:28.000000 SightTraining-0.1.19/spacedefense/assets/sounds/firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    40320 2024-03-31 18:25:38.000000 SightTraining-0.1.19/spacedefense/assets/sounds/smyf_join.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   265674 2024-03-29 14:22:39.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_angry.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   214184 2024-03-29 14:21:15.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_loss.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   128369 2024-03-29 14:21:54.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_win.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   213937 2024-03-29 14:22:18.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_mid.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   295241 2024-03-29 14:22:58.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_pre.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)   224144 2024-03-29 14:23:21.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_start.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    49560 2024-03-31 18:25:08.000000 SightTraining-0.1.19/spacedefense/assets/sounds/sufo_join.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    24129 2024-03-29 18:13:37.000000 SightTraining-0.1.19/spacedefense/assets/sounds/super_fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    56632 2024-03-29 18:24:26.000000 SightTraining-0.1.19/spacedefense/assets/sounds/super_firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    10368 2024-03-29 14:23:49.000000 SightTraining-0.1.19/spacedefense/assets/sounds/ufo_fire.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)    12270 2024-03-29 14:24:06.000000 SightTraining-0.1.19/spacedefense/assets/sounds/ufo_firehit.ogg
--rw-r--r--   0 wangjuntao   (501) staff       (20)     3705 2024-04-07 13:21:07.000000 SightTraining-0.1.19/spacedefense/common.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     5159 2024-04-08 02:54:18.000000 SightTraining-0.1.19/spacedefense/config.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    11805 2024-04-08 02:18:23.000000 SightTraining-0.1.19/spacedefense/flight_unit.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2064 2024-04-07 14:10:18.000000 SightTraining-0.1.19/spacedefense/game.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     9531 2024-04-08 02:38:49.000000 SightTraining-0.1.19/spacedefense/my_master.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    27346 2024-04-08 02:29:54.000000 SightTraining-0.1.19/spacedefense/scene_main.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     3653 2024-04-01 17:56:03.000000 SightTraining-0.1.19/spacedefense/scenes.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.360439 SightTraining-0.1.20/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.20/LICENSE
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       58 2024-04-01 09:37:31.000000 SightTraining-0.1.20/MANIFEST.in
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 03:14:46.360191 SightTraining-0.1.20/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.20/Readme.md
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.359878 SightTraining-0.1.20/SightTraining.egg-info/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2883 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/entry_points.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/requires.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-08 03:14:46.000000 SightTraining-0.1.20/SightTraining.egg-info/top_level.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-08 03:14:46.360484 SightTraining-0.1.20/setup.cfg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-08 03:14:29.000000 SightTraining-0.1.20/setup.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.329840 SightTraining-0.1.20/spacedefense/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1261 2024-04-07 13:38:55.000000 SightTraining-0.1.20/spacedefense/__init__.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    17516 2024-04-08 01:33:20.000000 SightTraining-0.1.20/spacedefense/actors.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.330088 SightTraining-0.1.20/spacedefense/assets/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10244 2024-04-08 03:01:25.000000 SightTraining-0.1.20/spacedefense/assets/.DS_Store
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.335727 SightTraining-0.1.20/spacedefense/assets/images/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18436 2024-04-08 03:03:21.000000 SightTraining-0.1.20/spacedefense/assets/images/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    93950 2024-04-08 02:52:13.000000 SightTraining-0.1.20/spacedefense/assets/images/game_cover.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   115516 2024-04-08 02:53:25.000000 SightTraining-0.1.20/spacedefense/assets/images/game_cover_loss.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   129152 2024-04-08 02:53:06.000000 SightTraining-0.1.20/spacedefense/assets/images/game_cover_win.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    31179 2024-04-01 06:54:20.000000 SightTraining-0.1.20/spacedefense/assets/images/icon.png
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6772 2024-04-07 13:57:36.000000 SightTraining-0.1.20/spacedefense/assets/images/my_slave_fighter1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6578 2024-04-07 13:59:55.000000 SightTraining-0.1.20/spacedefense/assets/images/my_slave_fighter2.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.337726 SightTraining-0.1.20/spacedefense/assets/images/myf_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:42:44.000000 SightTraining-0.1.20/spacedefense/assets/images/myf_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7568 2024-04-07 13:41:47.000000 SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7358 2024-04-07 13:41:55.000000 SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7442 2024-04-07 13:42:06.000000 SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6916 2024-04-07 13:42:17.000000 SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_004.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    95336 2024-04-07 14:00:31.000000 SightTraining-0.1.20/spacedefense/assets/images/scale_cambg1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5298 2024-04-08 01:24:57.000000 SightTraining-0.1.20/spacedefense/assets/images/super_bullet.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.339149 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:00.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     8908 2024-04-07 13:49:06.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9406 2024-04-07 13:49:20.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9166 2024-04-07 13:49:28.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9482 2024-04-07 13:49:58.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_004.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.340626 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:40.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5838 2024-04-07 13:52:06.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5676 2024-04-07 13:52:20.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5802 2024-04-07 13:52:28.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5682 2024-04-07 13:52:42.000000 SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.343311 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:18:10.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   323000 2024-04-07 13:16:38.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   262066 2024-04-07 13:16:50.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   322282 2024-04-07 13:17:12.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.346207 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:27:10.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   212520 2024-04-07 13:24:30.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   210670 2024-04-07 13:24:44.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   221782 2024-04-07 13:25:46.000000 SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 03:14:46.359518 SightTraining-0.1.20/spacedefense/assets/sounds/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-08 03:00:49.000000 SightTraining-0.1.20/spacedefense/assets/sounds/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   613595 2024-04-01 06:38:42.000000 SightTraining-0.1.20/spacedefense/assets/sounds/bgm.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    19873 2024-03-29 14:26:24.000000 SightTraining-0.1.20/spacedefense/assets/sounds/fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18471 2024-03-29 14:25:00.000000 SightTraining-0.1.20/spacedefense/assets/sounds/fire_blast.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    26919 2024-03-29 14:24:28.000000 SightTraining-0.1.20/spacedefense/assets/sounds/firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    40320 2024-03-31 18:25:38.000000 SightTraining-0.1.20/spacedefense/assets/sounds/smyf_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   265674 2024-03-29 14:22:39.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_angry.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   214184 2024-03-29 14:21:15.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_end_loss.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   128369 2024-03-29 14:21:54.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_end_win.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   213937 2024-03-29 14:22:18.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_mid.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   295241 2024-03-29 14:22:58.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_pre.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   224144 2024-03-29 14:23:21.000000 SightTraining-0.1.20/spacedefense/assets/sounds/stage_start.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    49560 2024-03-31 18:25:08.000000 SightTraining-0.1.20/spacedefense/assets/sounds/sufo_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    24129 2024-03-29 18:13:37.000000 SightTraining-0.1.20/spacedefense/assets/sounds/super_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    56632 2024-03-29 18:24:26.000000 SightTraining-0.1.20/spacedefense/assets/sounds/super_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10368 2024-03-29 14:23:49.000000 SightTraining-0.1.20/spacedefense/assets/sounds/ufo_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    12270 2024-03-29 14:24:06.000000 SightTraining-0.1.20/spacedefense/assets/sounds/ufo_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3705 2024-04-07 13:21:07.000000 SightTraining-0.1.20/spacedefense/common.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5171 2024-04-08 03:02:57.000000 SightTraining-0.1.20/spacedefense/config.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    11805 2024-04-08 02:18:23.000000 SightTraining-0.1.20/spacedefense/flight_unit.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2064 2024-04-07 14:10:18.000000 SightTraining-0.1.20/spacedefense/game.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9531 2024-04-08 02:38:49.000000 SightTraining-0.1.20/spacedefense/my_master.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    27346 2024-04-08 02:29:54.000000 SightTraining-0.1.20/spacedefense/scene_main.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3653 2024-04-01 17:56:03.000000 SightTraining-0.1.20/spacedefense/scenes.py
```

### Comparing `SightTraining-0.1.19/LICENSE` & `SightTraining-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/PKG-INFO` & `SightTraining-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.19
+Version: 0.1.20
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.19/SightTraining.egg-info/PKG-INFO` & `SightTraining-0.1.20/SightTraining.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.19
+Version: 0.1.20
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.19/SightTraining.egg-info/SOURCES.txt` & `SightTraining-0.1.20/SightTraining.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 spacedefense/scenes.py
 spacedefense/assets/.DS_Store
 spacedefense/assets/images/.DS_Store
 spacedefense/assets/images/game_cover.webp
 spacedefense/assets/images/game_cover_loss.webp
 spacedefense/assets/images/game_cover_win.webp
 spacedefense/assets/images/icon.png
-spacedefense/assets/images/master_fighter.webp
 spacedefense/assets/images/my_slave_fighter1.webp
 spacedefense/assets/images/my_slave_fighter2.webp
 spacedefense/assets/images/scale_cambg1.webp
 spacedefense/assets/images/super_bullet.webp
 spacedefense/assets/images/myf_master/.DS_Store
 spacedefense/assets/images/myf_master/myf_master_001.webp
 spacedefense/assets/images/myf_master/myf_master_002.webp
@@ -49,16 +48,15 @@
 spacedefense/assets/images/vmove_cambg1/cambg_002.webp
 spacedefense/assets/images/vmove_cambg1/cambg_003.webp
 spacedefense/assets/images/vmove_cambg2/.DS_Store
 spacedefense/assets/images/vmove_cambg2/cambg_001.webp
 spacedefense/assets/images/vmove_cambg2/cambg_002.webp
 spacedefense/assets/images/vmove_cambg2/cambg_003.webp
 spacedefense/assets/sounds/.DS_Store
-spacedefense/assets/sounds/bgm1.ogg
-spacedefense/assets/sounds/bgm3.ogg
+spacedefense/assets/sounds/bgm.ogg
 spacedefense/assets/sounds/fire.ogg
 spacedefense/assets/sounds/fire_blast.ogg
 spacedefense/assets/sounds/firehit.ogg
 spacedefense/assets/sounds/smyf_join.ogg
 spacedefense/assets/sounds/stage_angry.ogg
 spacedefense/assets/sounds/stage_end_loss.ogg
 spacedefense/assets/sounds/stage_end_win.ogg
```

### Comparing `SightTraining-0.1.19/setup.py` & `SightTraining-0.1.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 readme = """
 SightTraining  is a game for children's amblyopia training
 """
 
 setup(
     name="SightTraining",
-    version="0.1.19",
+    version="0.1.20",
     author="jett.wang",
     author_email="jamiesun.net@gmail.com",
     description="SightTraining  is a game for children's amblyopia training",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `SightTraining-0.1.19/spacedefense/__init__.py` & `SightTraining-0.1.20/spacedefense/__init__.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/actors.py` & `SightTraining-0.1.20/spacedefense/actors.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 000010a0: 2035 347d 2c20 7b31 3436 362c 2038 3932   54}, {1466, 892
 000010b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 000010c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 000010d0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 000010e0: 0000 0006 0069 006d 0061 0067 0065 0073  .....i.m.a.g.e.s
 000010f0: 6473 636c 626f 6f6c 0000 0000 0600 6900  dsclbool......i.
 00001100: 6d00 6100 6700 6500 736c 6731 5363 6f6d  m.a.g.e.slg1Scom
-00001110: 7000 0000 0000 2142 1b00 0000 0600 6900  p.....!B......i.
+00001110: 7000 0000 0000 214a 1b00 0000 0600 6900  p.....!J......i.
 00001120: 6d00 6100 6700 6500 736c 7376 4362 6c6f  m.a.g.e.slsvCblo
 00001130: 6200 0002 f362 706c 6973 7430 30d8 0102  b....bplist00...
 00001140: 0304 0506 0708 090a 0b16 5253 0a55 5f10  ..........RS.U_.
 00001150: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
 00001160: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
 00001170: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
 00001180: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
@@ -380,15 +380,15 @@
 000017b0: 5368 6f77 5369 6465 6261 7209 0908 095f  ShowSidebar...._
 000017c0: 1018 7b7b 3233 392c 2034 3635 7d2c 207b  ..{{239, 465}, {
 000017d0: 3932 302c 2034 3634 7d7d 0908 1523 2f3b  920, 464}}...#/;
 000017e0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000017f0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 008b 0000 0006 0073 006f  .............s.o
 00001810: 0075 006e 0064 0073 6473 636c 626f 6f6c  .u.n.d.sdsclbool
-00001820: 0000 0000 0600 7300 6f00 7500 6e00 6400  ......s.o.u.n.d.
+00001820: 0100 0000 0600 7300 6f00 7500 6e00 6400  ......s.o.u.n.d.
 00001830: 736c 6731 5363 6f6d 7000 0000 0000 2dca  slg1Scomp.....-.
 00001840: 7900 0000 0600 7300 6f00 7500 6e00 6400  y.....s.o.u.n.d.
 00001850: 736d 6f44 4462 6c6f 6200 0000 0803 dcb4  smoDDblob.......
 00001860: b34c ddc5 4100 0000 0600 7300 6f00 7500  .L..A.....s.o.u.
 00001870: 6e00 6400 736d 6f64 4462 6c6f 6200 0000  n.d.smodDblob...
 00001880: 0803 dcb4 b34c ddc5 4100 0000 0600 7300  .....L..A.....s.
 00001890: 6f00 7500 6e00 6400 7370 6831 5363 6f6d  o.u.n.d.sph1Scom
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 4000 0000 0800  ....Bud1..@.....
 00000010: 0000 4000 0000 100c 0000 040a 0000 200c  ..@........... .
 00000020: 0000 300c 0000 0000 0000 0000 0000 0800  ..0.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 003c  ...............<
+00000040: 0000 0000 0000 0003 0000 0001 0000 003b  ...............;
 00000050: 0000 0004 0000 1000 006f 005f 006d 0061  .........o._.m.a
 00000060: 0073 0074 0000 0000 0000 0000 0000 0000  .s.t............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -506,15 +506,15 @@
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0000 0000 0018 0000 000f  ................
+00002000: 0000 0000 0000 0000 0000 0017 0000 000f  ................
 00002010: 0067 0061 006d 0065 005f 0063 006f 0076  .g.a.m.e._.c.o.v
 00002020: 0065 0072 002e 0077 0065 0062 0070 496c  .e.r...w.e.b.pIl
 00002030: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
 00002040: 009e ffff ffff ffff 0000 0000 0014 0067  ...............g
 00002050: 0061 006d 0065 005f 0063 006f 0076 0065  .a.m.e._.c.o.v.e
 00002060: 0072 005f 006c 006f 0073 0073 002e 0077  .r._.l.o.s.s...w
 00002070: 0065 0062 0070 496c 6f63 626c 6f62 0000  .e.b.pIlocblob..
@@ -522,234 +522,234 @@
 00002090: 0000 0000 0013 0067 0061 006d 0065 005f  .......g.a.m.e._
 000020a0: 0063 006f 0076 0065 0072 005f 0077 0069  .c.o.v.e.r._.w.i
 000020b0: 006e 002e 0077 0065 0062 0070 496c 6f63  .n...w.e.b.pIloc
 000020c0: 626c 6f62 0000 0010 0000 01f9 0000 009e  blob............
 000020d0: ffff ffff ffff 0000 0000 0008 0069 0063  .............i.c
 000020e0: 006f 006e 002e 0070 006e 0067 496c 6f63  .o.n...p.n.gIloc
 000020f0: 626c 6f62 0000 0010 0000 041f 0000 002e  blob............
-00002100: ffff ffff ffff 0000 0000 0013 006d 0061  .............m.a
-00002110: 0073 0074 0065 0072 005f 0066 0069 0067  .s.t.e.r._.f.i.g
-00002120: 0068 0074 0065 0072 002e 0077 0065 0062  .h.t.e.r...w.e.b
-00002130: 0070 496c 6f63 626c 6f62 0000 0010 0000  .pIlocblob......
-00002140: 00af 0000 009e ffff ffff ffff 0000 0000  ................
-00002150: 0016 006d 0079 005f 0073 006c 0061 0076  ...m.y._.s.l.a.v
-00002160: 0065 005f 0066 0069 0067 0068 0074 0065  .e._.f.i.g.h.t.e
-00002170: 0072 0031 002e 0077 0065 0062 0070 496c  .r.1...w.e.b.pIl
-00002180: 6f63 626c 6f62 0000 0010 0000 018b 0000  ocblob..........
-00002190: 009e ffff ffff ffff 0000 0000 0016 006d  ...............m
-000021a0: 0079 005f 0073 006c 0061 0076 0065 005f  .y._.s.l.a.v.e._
-000021b0: 0066 0069 0067 0068 0074 0065 0072 0032  .f.i.g.h.t.e.r.2
-000021c0: 002e 0077 0065 0062 0070 496c 6f63 626c  ...w.e.b.pIlocbl
-000021d0: 6f62 0000 0010 0000 0267 0000 009e ffff  ob.......g......
-000021e0: ffff ffff 0000 0000 000a 006d 0079 0066  ...........m.y.f
-000021f0: 005f 006d 0061 0073 0074 0065 0072 496c  ._.m.a.s.t.e.rIl
-00002200: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
-00002210: 002e ffff ffff ffff 0000 0000 000a 006d  ...............m
-00002220: 0079 0066 005f 006d 0061 0073 0074 0065  .y.f._.m.a.s.t.e
-00002230: 0072 6277 7370 626c 6f62 0000 00b8 6270  .rbwspblob....bp
-00002240: 6c69 7374 3030 d601 0203 0405 0607 0709  list00..........
-00002250: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00002260: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00002270: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00002280: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00002290: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-000022a0: 6f77 5369 6465 6261 7209 0908 095f 1018  owSidebar...._..
-000022b0: 7b7b 3235 392c 2035 347d 2c20 7b31 3436  {{259, 54}, {146
-000022c0: 362c 2038 3932 7d7d 0908 1523 2f3b 525f  6, 892}}...#/;R_
-000022d0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
-000022e0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
-000022f0: 0000 0000 008b 0000 000a 006d 0079 0066  ...........m.y.f
-00002300: 005f 006d 0061 0073 0074 0065 0072 6473  ._.m.a.s.t.e.rds
-00002310: 636c 626f 6f6c 0000 0000 0a00 6d00 7900  clbool......m.y.
-00002320: 6600 5f00 6d00 6100 7300 7400 6500 726c  f._.m.a.s.t.e.rl
-00002330: 6731 5363 6f6d 7000 0000 0000 008a 6800  g1Scomp.......h.
-00002340: 0000 0a00 6d00 7900 6600 5f00 6d00 6100  ....m.y.f._.m.a.
-00002350: 7300 7400 6500 726c 7376 4362 6c6f 6200  s.t.e.rlsvCblob.
-00002360: 0003 1162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
-00002370: 0506 0708 090a 0b1b 5556 0a58 5f10 1276  ........UV.X_..v
-00002380: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00002390: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-000023a0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-000023b0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-000023c0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-000023d0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-000023e0: 6544 6174 6573 5869 636f 6e53 697a 6514  eDatesXiconSize.
-000023f0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00002400: 09ae 0c15 1d22 262b 3035 3a3e 4347 4c50  ....."&+05:>CGLP
-00002410: d40d 0e0f 1011 120a 0a5a 6964 656e 7469  .........Zidenti
-00002420: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
-00002430: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
-00002440: 6511 012c 0909 d40d 1617 1819 1a1b 1b55  e..,...........U
-00002450: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00002460: 7669 7369 626c 6558 7562 6971 7569 7479  visibleXubiquity
-00002470: 1023 0808 d40d 0e0f 101e 1f1b 0a5c 6461  .#...........\da
-00002480: 7465 4d6f 6469 6669 6564 10b5 0809 d40d  teModified......
-00002490: 0e0f 1023 1f1b 1b5b 6461 7465 4372 6561  ...#...[dateCrea
-000024a0: 7465 6408 08d4 0d0e 0f10 2728 1b0a 5473  ted.......'(..Ts
-000024b0: 697a 6510 6108 09d4 100e 0f0d 0a2d 1b2f  ize.a........-./
-000024c0: 0910 7308 546b 696e 64d4 0d0e 0f10 3132  ..s.Tkind.....12
-000024d0: 0a1b 556c 6162 656c 1064 0908 d40d 0e0f  ..Ulabel.d......
-000024e0: 1036 370a 1b57 7665 7273 696f 6e10 4b09  .67..Wversion.K.
-000024f0: 08d4 0d0e 0f10 3b12 0a1b 5863 6f6d 6d65  ......;...Xcomme
-00002500: 6e74 7309 08d4 0d0e 0f10 3f40 1b1b 5e64  nts.......?@..^d
-00002510: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
-00002520: 08d4 0d16 1718 441f 1b1b 5964 6174 6541  ......D...YdateA
-00002530: 6464 6564 0808 d418 1617 0d1b 491b 4b08  dded........I.K.
-00002540: 10d2 085a 7368 6172 654f 776e 6572 d418  ...ZshareOwner..
-00002550: 1617 0d1b 491b 4f08 085f 100f 7368 6172  ....I.O.._..shar
-00002560: 654c 6173 7445 6469 746f 72d4 1816 170d  eLastEditor.....
-00002570: 1b49 1b53 0808 5f10 1069 6e76 6974 6174  .I.S.._..invitat
-00002580: 696f 6e53 7461 7475 7308 2340 2a00 0000  ionStatus.#@*...
-00002590: 0000 0054 6b69 6e64 0923 4030 0000 0000  ...Tkind.#@0....
-000025a0: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-000025b0: 0070 0083 008c 009d 009e 00ad 00b6 00c1  .p..............
-000025c0: 00c7 00d1 00d9 00de 00e1 00e2 00e3 00ec  ................
-000025d0: 00f2 00fc 0104 010d 010f 0110 0111 011a  ................
-000025e0: 0127 0129 012a 012b 0134 0140 0141 0142  .'.).*.+.4.@.A.B
-000025f0: 014b 0150 0152 0153 0154 015d 015e 0160  .K.P.R.S.T.].^.`
-00002600: 0161 0166 016f 0175 0177 0178 0179 0182  .a.f.o.u.w.x.y..
-00002610: 018a 018c 018d 018e 0197 01a0 01a1 01a2  ................
-00002620: 01ab 01ba 01bc 01bd 01be 01c7 01d1 01d2  ................
-00002630: 01d3 01dc 01dd 01df 01e0 01eb 01f4 01f5  ................
-00002640: 01f6 0208 0211 0212 0213 0226 0227 0230  ...........&.'.0
-00002650: 0235 0236 0000 0000 0000 0201 0000 0000  .5.6............
-00002660: 0000 0059 0000 0000 0000 0000 0000 0000  ...Y............
-00002670: 0000 023f 0000 000a 006d 0079 0066 005f  ...?.....m.y.f._
-00002680: 006d 0061 0073 0074 0065 0072 6c73 7670  .m.a.s.t.e.rlsvp
-00002690: 626c 6f62 0000 026c 6270 6c69 7374 3030  blob...lbplist00
-000026a0: d801 0203 0405 0607 0809 0a0b 1a45 460a  .............EF.
-000026b0: 485f 1012 7669 6577 4f70 7469 6f6e 7356  H_..viewOptionsV
-000026c0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-000026d0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-000026e0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-000026f0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00002700: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-00002710: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
-00002720: 5369 7a65 1400 0000 0000 0000 0000 0000  Size............
-00002730: 0000 0000 0109 d90c 0d0e 0f10 1112 1314  ................
-00002740: 151e 2328 2d32 363b 3f58 636f 6d6d 656e  ..#(-26;?Xcommen
-00002750: 7473 556c 6162 656c 5776 6572 7369 6f6e  tsUlabelWversion
-00002760: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-00002770: 655c 6461 7465 4d6f 6469 6669 6564 546b  e\dateModifiedTk
-00002780: 696e 6454 6e61 6d65 5e64 6174 654c 6173  indTname^dateLas
-00002790: 744f 7065 6e65 64d4 1617 1819 1a1b 0a1d  tOpened.........
-000027a0: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-000027b0: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-000027c0: 012c 0910 07d4 1617 1819 1a20 0a22 0810  .,......... ."..
-000027d0: 6409 1005 d416 1718 191a 250a 2708 104b  d.........%.'..K
-000027e0: 0910 06d4 1617 1819 1a2a 1a2c 0810 b508  .........*.,....
-000027f0: 1002 d416 1718 190a 2f1a 3109 1061 0810  ......../.1..a..
-00002800: 03d4 1617 1819 0a2a 1a35 0908 1001 d419  .......*.5......
-00002810: 1718 1637 381a 0a10 0410 7308 09d4 1617  ...78.....s.....
-00002820: 1819 0a1b 0a3e 0909 1000 d416 1718 191a  .....>..........
-00002830: 411a 4308 10c8 0810 0808 2340 2a00 0000  A.C.......#@*...
-00002840: 0000 0054 6b69 6e64 0923 4030 0000 0000  ...Tkind.#@0....
-00002850: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00002860: 0070 0083 008c 009d 009e 00b1 00ba 00c0  .p..............
-00002870: 00c8 00d4 00d9 00e6 00eb 00f0 00ff 0108  ................
-00002880: 0110 0116 0120 0126 0127 012a 012b 012d  ..... .&.'.*.+.-
-00002890: 0136 0137 0139 013a 013c 0145 0146 0148  .6.7.9.:.<.E.F.H
-000028a0: 0149 014b 0154 0155 0157 0158 015a 0163  .I.K.T.U.W.X.Z.c
-000028b0: 0164 0166 0167 0169 0172 0173 0174 0176  .d.f.g.i.r.s.t.v
-000028c0: 017f 0181 0183 0184 0185 018e 018f 0190  ................
-000028d0: 0192 019b 019c 019e 019f 01a1 01a2 01ab  ................
-000028e0: 01b0 01b1 0000 0000 0000 0201 0000 0000  ................
-000028f0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-00002900: 0000 01ba 0000 000a 006d 0079 0066 005f  .........m.y.f._
-00002910: 006d 0061 0073 0074 0065 0072 6d6f 4444  .m.a.s.t.e.rmoDD
-00002920: 626c 6f62 0000 0008 1170 5c2a 6de1 c541  blob.....p\*m..A
-00002930: 0000 000a 006d 0079 0066 005f 006d 0061  .....m.y.f._.m.a
-00002940: 0073 0074 0065 0072 6d6f 6444 626c 6f62  .s.t.e.rmodDblob
-00002950: 0000 0008 1170 5c2a 6de1 c541 0000 000a  .....p\*m..A....
-00002960: 006d 0079 0066 005f 006d 0061 0073 0074  .m.y.f._.m.a.s.t
-00002970: 0065 0072 7068 3153 636f 6d70 0000 0000  .e.rph1Scomp....
-00002980: 0000 a000 0000 000a 006d 0079 0066 005f  .........m.y.f._
-00002990: 006d 0061 0073 0074 0065 0072 7653 726e  .m.a.s.t.e.rvSrn
-000029a0: 6c6f 6e67 0000 0001 0000 0011 0073 0063  long.........s.c
-000029b0: 0061 006c 0065 005f 0063 0061 006d 0062  .a.l.e._.c.a.m.b
-000029c0: 0067 0031 002e 0077 0065 0062 0070 496c  .g.1...w.e.b.pIl
-000029d0: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
-000029e0: 002e ffff ffff ffff 0000 0000 0011 0073  ...............s
-000029f0: 0075 0070 0065 0072 005f 0062 0075 006c  .u.p.e.r._.b.u.l
-00002a00: 006c 0065 0074 002e 0077 0065 0062 0070  .l.e.t...w.e.b.p
-00002a10: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
-00002a20: 0000 009e ffff ffff ffff 0000 0000 000a  ................
-00002a30: 0075 0066 006f 005f 006d 0061 0073 0074  .u.f.o._.m.a.s.t
-00002a40: 0065 0072 496c 6f63 626c 6f62 0000 0010  .e.rIlocblob....
-00002a50: 0000 00af 0000 002e ffff ffff ffff 0000  ................
-00002a60: 0000 000a 0075 0066 006f 005f 006d 0061  .....u.f.o._.m.a
-00002a70: 0073 0074 0065 0072 6277 7370 626c 6f62  .s.t.e.rbwspblob
-00002a80: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-00002a90: 0405 0607 0709 070b 075d 5368 6f77 5374  .........]ShowSt
-00002aa0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00002ab0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002ac0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002ad0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002ae0: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
-00002af0: 0908 095f 1018 7b7b 3235 392c 2035 347d  ..._..{{259, 54}
-00002b00: 2c20 7b31 3436 362c 2038 3932 7d7d 0908  , {1466, 892}}..
-00002b10: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00002b20: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00002b30: 0000 0000 0000 0000 0000 008b 0000 000a  ................
-00002b40: 0075 0066 006f 005f 006d 0061 0073 0074  .u.f.o._.m.a.s.t
-00002b50: 0065 0072 6473 636c 626f 6f6c 0000 0000  .e.rdsclbool....
-00002b60: 0a00 7500 6600 6f00 5f00 6d00 6100 7300  ..u.f.o._.m.a.s.
-00002b70: 7400 6500 726c 6731 5363 6f6d 7000 0000  t.e.rlg1Scomp...
-00002b80: 0000 00a8 6600 0000 0a00 7500 6600 6f00  ....f.....u.f.o.
-00002b90: 5f00 6d00 6100 7300 7400 6500 726c 7376  _.m.a.s.t.e.rlsv
-00002ba0: 4362 6c6f 6200 0003 1162 706c 6973 7430  Cblob....bplist0
-00002bb0: 30d8 0102 0304 0506 0708 090a 0b19 5556  0.............UV
-00002bc0: 0a58 5f10 1276 6965 774f 7074 696f 6e73  .X_..viewOptions
-00002bd0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00002be0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00002bf0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00002c00: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00002c10: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00002c20: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
-00002c30: 6e53 697a 6514 0000 0000 0000 0000 0000  nSize...........
-00002c40: 0000 0000 0001 09ae 0c15 1d22 262b 3035  ..........."&+05
-00002c50: 3a3e 4347 4c50 d40d 0e0f 1011 120a 0a5a  :>CGLP.........Z
-00002c60: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-00002c70: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00002c80: 6c65 546e 616d 6511 012c 0909 d416 1718  leTname..,......
-00002c90: 0d19 1a19 1c57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00002ca0: 6474 6859 6173 6365 6e64 696e 6708 1023  dthYascending..#
-00002cb0: 0858 7562 6971 7569 7479 d410 0e0f 0d0a  .Xubiquity......
-00002cc0: 1f19 2109 10b5 085c 6461 7465 4d6f 6469  ..!....\dateModi
-00002cd0: 6669 6564 d410 0e0f 0d19 1f19 2508 085b  fied........%..[
-00002ce0: 6461 7465 4372 6561 7465 64d4 100e 0f0d  dateCreated.....
-00002cf0: 0a28 192a 0910 6108 5473 697a 65d4 0d0e  .(.*..a.Tsize...
-00002d00: 0f10 2c2d 190a 546b 696e 6410 7308 09d4  ..,-..Tkind.s...
-00002d10: 100e 0f0d 1932 0a34 0810 6409 556c 6162  .....2.4..d.Ulab
-00002d20: 656c d410 0e0f 0d19 370a 3908 104b 0957  el......7.9..K.W
-00002d30: 7665 7273 696f 6ed4 100e 0f0d 1912 0a3d  version........=
-00002d40: 0809 5863 6f6d 6d65 6e74 73d4 100e 0f0d  ..Xcomments.....
-00002d50: 1940 1942 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
-00002d60: 744f 7065 6e65 64d4 1617 180d 191f 1946  tOpened........F
-00002d70: 0808 5964 6174 6541 6464 6564 d40d 1718  ..YdateAdded....
-00002d80: 1648 4919 195a 7368 6172 654f 776e 6572  .HI..ZshareOwner
-00002d90: 10d2 0808 d40d 1718 164d 4919 195f 100f  .........MI.._..
-00002da0: 7368 6172 654c 6173 7445 6469 746f 7208  shareLastEditor.
-00002db0: 08d4 0d17 1816 5149 1919 5f10 1069 6e76  ......QI.._..inv
-00002dc0: 6974 6174 696f 6e53 7461 7475 7308 0808  itationStatus...
-00002dd0: 2340 2a00 0000 0000 0054 6b69 6e64 0923  #@*......Tkind.#
-00002de0: 4030 0000 0000 0000 0008 0019 002e 0040  @0.............@
-00002df0: 0048 005c 0065 0070 0083 008c 009d 009e  .H.\.e.p........
-00002e00: 00ad 00b6 00c1 00c7 00d1 00d9 00de 00e1  ................
-00002e10: 00e2 00e3 00ec 00f4 00fa 0104 0105 0107  ................
-00002e20: 0108 0111 011a 011b 011d 011e 012b 0134  .............+.4
-00002e30: 0135 0136 0142 014b 014c 014e 014f 0154  .5.6.B.K.L.N.O.T
-00002e40: 015d 0162 0164 0165 0166 016f 0170 0172  .].b.d.e.f.o.p.r
-00002e50: 0173 0179 0182 0183 0185 0186 018e 0197  .s.y............
-00002e60: 0198 0199 01a2 01ab 01ac 01ae 01af 01be  ................
-00002e70: 01c7 01c8 01c9 01d3 01dc 01e7 01e9 01ea  ................
-00002e80: 01eb 01f4 0206 0207 0208 0211 0224 0225  .............$.%
-00002e90: 0226 0227 0230 0235 0236 0000 0000 0000  .&.'.0.5.6......
-00002ea0: 0201 0000 0000 0000 0059 0000 0000 0000  .........Y......
-00002eb0: 0000 0000 0000 0000 023f 0000 0000 0000  .........?......
+00002100: ffff ffff ffff 0000 0000 0016 006d 0079  .............m.y
+00002110: 005f 0073 006c 0061 0076 0065 005f 0066  ._.s.l.a.v.e._.f
+00002120: 0069 0067 0068 0074 0065 0072 0031 002e  .i.g.h.t.e.r.1..
+00002130: 0077 0065 0062 0070 496c 6f63 626c 6f62  .w.e.b.pIlocblob
+00002140: 0000 0010 0000 018b 0000 009e ffff ffff  ................
+00002150: ffff 0000 0000 0016 006d 0079 005f 0073  .........m.y._.s
+00002160: 006c 0061 0076 0065 005f 0066 0069 0067  .l.a.v.e._.f.i.g
+00002170: 0068 0074 0065 0072 0032 002e 0077 0065  .h.t.e.r.2...w.e
+00002180: 0062 0070 496c 6f63 626c 6f62 0000 0010  .b.pIlocblob....
+00002190: 0000 0267 0000 009e ffff ffff ffff 0000  ...g............
+000021a0: 0000 000a 006d 0079 0066 005f 006d 0061  .....m.y.f._.m.a
+000021b0: 0073 0074 0065 0072 496c 6f63 626c 6f62  .s.t.e.rIlocblob
+000021c0: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
+000021d0: ffff 0000 0000 000a 006d 0079 0066 005f  .........m.y.f._
+000021e0: 006d 0061 0073 0074 0065 0072 6277 7370  .m.a.s.t.e.rbwsp
+000021f0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00002200: d601 0203 0405 0607 0709 070b 075d 5368  .............]Sh
+00002210: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002220: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00002230: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00002240: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00002250: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00002260: 6261 7209 0908 095f 1018 7b7b 3235 392c  bar...._..{{259,
+00002270: 2035 347d 2c20 7b31 3436 362c 2038 3932   54}, {1466, 892
+00002280: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00002290: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000022a0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+000022b0: 0000 000a 006d 0079 0066 005f 006d 0061  .....m.y.f._.m.a
+000022c0: 0073 0074 0065 0072 6473 636c 626f 6f6c  .s.t.e.rdsclbool
+000022d0: 0100 0000 0a00 6d00 7900 6600 5f00 6d00  ......m.y.f._.m.
+000022e0: 6100 7300 7400 6500 726c 6731 5363 6f6d  a.s.t.e.rlg1Scom
+000022f0: 7000 0000 0000 008a 6800 0000 0a00 6d00  p.......h.....m.
+00002300: 7900 6600 5f00 6d00 6100 7300 7400 6500  y.f._.m.a.s.t.e.
+00002310: 726c 7376 4362 6c6f 6200 0003 1162 706c  rlsvCblob....bpl
+00002320: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
+00002330: 0b1b 5556 0a58 5f10 1276 6965 774f 7074  ..UV.X_..viewOpt
+00002340: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
+00002350: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00002360: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00002370: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00002380: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+00002390: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000023a0: 5869 636f 6e53 697a 6514 0000 0000 0000  XiconSize.......
+000023b0: 0000 0000 0000 0000 0001 09ae 0c15 1d22  ..............."
+000023c0: 262b 3035 3a3e 4347 4c50 d40d 0e0f 1011  &+05:>CGLP......
+000023d0: 120a 0a5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
+000023e0: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+000023f0: 6973 6962 6c65 546e 616d 6511 012c 0909  isibleTname..,..
+00002400: d40d 1617 1819 1a1b 1b55 7769 6474 6859  .........UwidthY
+00002410: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+00002420: 6558 7562 6971 7569 7479 1023 0808 d40d  eXubiquity.#....
+00002430: 0e0f 101e 1f1b 0a5c 6461 7465 4d6f 6469  .......\dateModi
+00002440: 6669 6564 10b5 0809 d40d 0e0f 1023 1f1b  fied.........#..
+00002450: 1b5b 6461 7465 4372 6561 7465 6408 08d4  .[dateCreated...
+00002460: 0d0e 0f10 2728 1b0a 5473 697a 6510 6108  ....'(..Tsize.a.
+00002470: 09d4 100e 0f0d 0a2d 1b2f 0910 7308 546b  .......-./..s.Tk
+00002480: 696e 64d4 0d0e 0f10 3132 0a1b 556c 6162  ind.....12..Ulab
+00002490: 656c 1064 0908 d40d 0e0f 1036 370a 1b57  el.d.......67..W
+000024a0: 7665 7273 696f 6e10 4b09 08d4 0d0e 0f10  version.K.......
+000024b0: 3b12 0a1b 5863 6f6d 6d65 6e74 7309 08d4  ;...Xcomments...
+000024c0: 0d0e 0f10 3f40 1b1b 5e64 6174 654c 6173  ....?@..^dateLas
+000024d0: 744f 7065 6e65 6410 c808 08d4 0d16 1718  tOpened.........
+000024e0: 441f 1b1b 5964 6174 6541 6464 6564 0808  D...YdateAdded..
+000024f0: d418 1617 0d1b 491b 4b08 10d2 085a 7368  ......I.K....Zsh
+00002500: 6172 654f 776e 6572 d418 1617 0d1b 491b  areOwner......I.
+00002510: 4f08 085f 100f 7368 6172 654c 6173 7445  O.._..shareLastE
+00002520: 6469 746f 72d4 1816 170d 1b49 1b53 0808  ditor......I.S..
+00002530: 5f10 1069 6e76 6974 6174 696f 6e53 7461  _..invitationSta
+00002540: 7475 7308 2340 2a00 0000 0000 0054 6b69  tus.#@*......Tki
+00002550: 6e64 0923 4030 0000 0000 0000 0008 0019  nd.#@0..........
+00002560: 002e 0040 0048 005c 0065 0070 0083 008c  ...@.H.\.e.p....
+00002570: 009d 009e 00ad 00b6 00c1 00c7 00d1 00d9  ................
+00002580: 00de 00e1 00e2 00e3 00ec 00f2 00fc 0104  ................
+00002590: 010d 010f 0110 0111 011a 0127 0129 012a  ...........'.).*
+000025a0: 012b 0134 0140 0141 0142 014b 0150 0152  .+.4.@.A.B.K.P.R
+000025b0: 0153 0154 015d 015e 0160 0161 0166 016f  .S.T.].^.`.a.f.o
+000025c0: 0175 0177 0178 0179 0182 018a 018c 018d  .u.w.x.y........
+000025d0: 018e 0197 01a0 01a1 01a2 01ab 01ba 01bc  ................
+000025e0: 01bd 01be 01c7 01d1 01d2 01d3 01dc 01dd  ................
+000025f0: 01df 01e0 01eb 01f4 01f5 01f6 0208 0211  ................
+00002600: 0212 0213 0226 0227 0230 0235 0236 0000  .....&.'.0.5.6..
+00002610: 0000 0000 0201 0000 0000 0000 0059 0000  .............Y..
+00002620: 0000 0000 0000 0000 0000 0000 023f 0000  .............?..
+00002630: 000a 006d 0079 0066 005f 006d 0061 0073  ...m.y.f._.m.a.s
+00002640: 0074 0065 0072 6c73 7670 626c 6f62 0000  .t.e.rlsvpblob..
+00002650: 026c 6270 6c69 7374 3030 d801 0203 0405  .lbplist00......
+00002660: 0607 0809 0a0b 1a45 460a 485f 1012 7669  .......EF.H_..vi
+00002670: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00002680: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00002690: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+000026a0: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+000026b0: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+000026c0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000026d0: 4461 7465 7358 6963 6f6e 5369 7a65 1400  DatesXiconSize..
+000026e0: 0000 0000 0000 0000 0000 0000 0000 0109  ................
+000026f0: d90c 0d0e 0f10 1112 1314 151e 2328 2d32  ............#(-2
+00002700: 363b 3f58 636f 6d6d 656e 7473 556c 6162  6;?XcommentsUlab
+00002710: 656c 5776 6572 7369 6f6e 5b64 6174 6543  elWversion[dateC
+00002720: 7265 6174 6564 5473 697a 655c 6461 7465  reatedTsize\date
+00002730: 4d6f 6469 6669 6564 546b 696e 6454 6e61  ModifiedTkindTna
+00002740: 6d65 5e64 6174 654c 6173 744f 7065 6e65  me^dateLastOpene
+00002750: 64d4 1617 1819 1a1b 0a1d 5776 6973 6962  d.........Wvisib
+00002760: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00002770: 6e67 5569 6e64 6578 0811 012c 0910 07d4  ngUindex...,....
+00002780: 1617 1819 1a20 0a22 0810 6409 1005 d416  ..... ."..d.....
+00002790: 1718 191a 250a 2708 104b 0910 06d4 1617  ....%.'..K......
+000027a0: 1819 1a2a 1a2c 0810 b508 1002 d416 1718  ...*.,..........
+000027b0: 190a 2f1a 3109 1061 0810 03d4 1617 1819  ../.1..a........
+000027c0: 0a2a 1a35 0908 1001 d419 1718 1637 381a  .*.5.........78.
+000027d0: 0a10 0410 7308 09d4 1617 1819 0a1b 0a3e  ....s..........>
+000027e0: 0909 1000 d416 1718 191a 411a 4308 10c8  ..........A.C...
+000027f0: 0810 0808 2340 2a00 0000 0000 0054 6b69  ....#@*......Tki
+00002800: 6e64 0923 4030 0000 0000 0000 0008 0019  nd.#@0..........
+00002810: 002e 0040 0048 005c 0065 0070 0083 008c  ...@.H.\.e.p....
+00002820: 009d 009e 00b1 00ba 00c0 00c8 00d4 00d9  ................
+00002830: 00e6 00eb 00f0 00ff 0108 0110 0116 0120  ............... 
+00002840: 0126 0127 012a 012b 012d 0136 0137 0139  .&.'.*.+.-.6.7.9
+00002850: 013a 013c 0145 0146 0148 0149 014b 0154  .:.<.E.F.H.I.K.T
+00002860: 0155 0157 0158 015a 0163 0164 0166 0167  .U.W.X.Z.c.d.f.g
+00002870: 0169 0172 0173 0174 0176 017f 0181 0183  .i.r.s.t.v......
+00002880: 0184 0185 018e 018f 0190 0192 019b 019c  ................
+00002890: 019e 019f 01a1 01a2 01ab 01b0 01b1 0000  ................
+000028a0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
+000028b0: 0000 0000 0000 0000 0000 0000 01ba 0000  ................
+000028c0: 000a 006d 0079 0066 005f 006d 0061 0073  ...m.y.f._.m.a.s
+000028d0: 0074 0065 0072 6d6f 4444 626c 6f62 0000  .t.e.rmoDDblob..
+000028e0: 0008 1170 5c2a 6de1 c541 0000 000a 006d  ...p\*m..A.....m
+000028f0: 0079 0066 005f 006d 0061 0073 0074 0065  .y.f._.m.a.s.t.e
+00002900: 0072 6d6f 6444 626c 6f62 0000 0008 1170  .rmodDblob.....p
+00002910: 5c2a 6de1 c541 0000 000a 006d 0079 0066  \*m..A.....m.y.f
+00002920: 005f 006d 0061 0073 0074 0065 0072 7068  ._.m.a.s.t.e.rph
+00002930: 3153 636f 6d70 0000 0000 0000 a000 0000  1Scomp..........
+00002940: 000a 006d 0079 0066 005f 006d 0061 0073  ...m.y.f._.m.a.s
+00002950: 0074 0065 0072 7653 726e 6c6f 6e67 0000  .t.e.rvSrnlong..
+00002960: 0001 0000 0011 0073 0063 0061 006c 0065  .......s.c.a.l.e
+00002970: 005f 0063 0061 006d 0062 0067 0031 002e  ._.c.a.m.b.g.1..
+00002980: 0077 0065 0062 0070 496c 6f63 626c 6f62  .w.e.b.pIlocblob
+00002990: 0000 0010 0000 011d 0000 002e ffff ffff  ................
+000029a0: ffff 0000 0000 0011 0073 0075 0070 0065  .........s.u.p.e
+000029b0: 0072 005f 0062 0075 006c 006c 0065 0074  .r._.b.u.l.l.e.t
+000029c0: 002e 0077 0065 0062 0070 496c 6f63 626c  ...w.e.b.pIlocbl
+000029d0: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
+000029e0: ffff ffff 0000 0000 000a 0075 0066 006f  ...........u.f.o
+000029f0: 005f 006d 0061 0073 0074 0065 0072 496c  ._.m.a.s.t.e.rIl
+00002a00: 6f63 626c 6f62 0000 0010 0000 00af 0000  ocblob..........
+00002a10: 002e ffff ffff ffff 0000 0000 000a 0075  ...............u
+00002a20: 0066 006f 005f 006d 0061 0073 0074 0065  .f.o._.m.a.s.t.e
+00002a30: 0072 6277 7370 626c 6f62 0000 00b8 6270  .rbwspblob....bp
+00002a40: 6c69 7374 3030 d601 0203 0405 0607 0709  list00..........
+00002a50: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00002a60: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00002a70: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00002a80: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00002a90: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00002aa0: 6f77 5369 6465 6261 7209 0908 095f 1018  owSidebar...._..
+00002ab0: 7b7b 3235 392c 2035 347d 2c20 7b31 3436  {{259, 54}, {146
+00002ac0: 362c 2038 3932 7d7d 0908 1523 2f3b 525f  6, 892}}...#/;R_
+00002ad0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
+00002ae0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00002af0: 0000 0000 008b 0000 000a 0075 0066 006f  ...........u.f.o
+00002b00: 005f 006d 0061 0073 0074 0065 0072 6473  ._.m.a.s.t.e.rds
+00002b10: 636c 626f 6f6c 0100 0000 0a00 7500 6600  clbool......u.f.
+00002b20: 6f00 5f00 6d00 6100 7300 7400 6500 726c  o._.m.a.s.t.e.rl
+00002b30: 6731 5363 6f6d 7000 0000 0000 00a8 6600  g1Scomp.......f.
+00002b40: 0000 0a00 7500 6600 6f00 5f00 6d00 6100  ....u.f.o._.m.a.
+00002b50: 7300 7400 6500 726c 7376 4362 6c6f 6200  s.t.e.rlsvCblob.
+00002b60: 0003 1162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+00002b70: 0506 0708 090a 0b19 5556 0a58 5f10 1276  ........UV.X_..v
+00002b80: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00002b90: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00002ba0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00002bb0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00002bc0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00002bd0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+00002be0: 6544 6174 6573 5869 636f 6e53 697a 6514  eDatesXiconSize.
+00002bf0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00002c00: 09ae 0c15 1d22 262b 3035 3a3e 4347 4c50  ....."&+05:>CGLP
+00002c10: d40d 0e0f 1011 120a 0a5a 6964 656e 7469  .........Zidenti
+00002c20: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
+00002c30: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
+00002c40: 6511 012c 0909 d416 1718 0d19 1a19 1c57  e..,...........W
+00002c50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+00002c60: 6365 6e64 696e 6708 1023 0858 7562 6971  cending..#.Xubiq
+00002c70: 7569 7479 d410 0e0f 0d0a 1f19 2109 10b5  uity........!...
+00002c80: 085c 6461 7465 4d6f 6469 6669 6564 d410  .\dateModified..
+00002c90: 0e0f 0d19 1f19 2508 085b 6461 7465 4372  ......%..[dateCr
+00002ca0: 6561 7465 64d4 100e 0f0d 0a28 192a 0910  eated......(.*..
+00002cb0: 6108 5473 697a 65d4 0d0e 0f10 2c2d 190a  a.Tsize.....,-..
+00002cc0: 546b 696e 6410 7308 09d4 100e 0f0d 1932  Tkind.s........2
+00002cd0: 0a34 0810 6409 556c 6162 656c d410 0e0f  .4..d.Ulabel....
+00002ce0: 0d19 370a 3908 104b 0957 7665 7273 696f  ..7.9..K.Wversio
+00002cf0: 6ed4 100e 0f0d 1912 0a3d 0809 5863 6f6d  n........=..Xcom
+00002d00: 6d65 6e74 73d4 100e 0f0d 1940 1942 0810  ments......@.B..
+00002d10: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00002d20: 64d4 1617 180d 191f 1946 0808 5964 6174  d........F..Ydat
+00002d30: 6541 6464 6564 d40d 1718 1648 4919 195a  eAdded.....HI..Z
+00002d40: 7368 6172 654f 776e 6572 10d2 0808 d40d  shareOwner......
+00002d50: 1718 164d 4919 195f 100f 7368 6172 654c  ...MI.._..shareL
+00002d60: 6173 7445 6469 746f 7208 08d4 0d17 1816  astEditor.......
+00002d70: 5149 1919 5f10 1069 6e76 6974 6174 696f  QI.._..invitatio
+00002d80: 6e53 7461 7475 7308 0808 2340 2a00 0000  nStatus...#@*...
+00002d90: 0000 0054 6b69 6e64 0923 4030 0000 0000  ...Tkind.#@0....
+00002da0: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+00002db0: 0070 0083 008c 009d 009e 00ad 00b6 00c1  .p..............
+00002dc0: 00c7 00d1 00d9 00de 00e1 00e2 00e3 00ec  ................
+00002dd0: 00f4 00fa 0104 0105 0107 0108 0111 011a  ................
+00002de0: 011b 011d 011e 012b 0134 0135 0136 0142  .......+.4.5.6.B
+00002df0: 014b 014c 014e 014f 0154 015d 0162 0164  .K.L.N.O.T.].b.d
+00002e00: 0165 0166 016f 0170 0172 0173 0179 0182  .e.f.o.p.r.s.y..
+00002e10: 0183 0185 0186 018e 0197 0198 0199 01a2  ................
+00002e20: 01ab 01ac 01ae 01af 01be 01c7 01c8 01c9  ................
+00002e30: 01d3 01dc 01e7 01e9 01ea 01eb 01f4 0206  ................
+00002e40: 0207 0208 0211 0224 0225 0226 0227 0230  .......$.%.&.'.0
+00002e50: 0235 0236 0000 0000 0000 0201 0000 0000  .5.6............
+00002e60: 0000 0059 0000 0000 0000 0000 0000 0000  ...Y............
+00002e70: 0000 023f 0000 0000 0a10 0000 0000 0c00  ...?............
+00002e80: 7600 6d00 6f00 7600 6500 5f00 6300 6100  v.m.o.v.e._.c.a.
+00002e90: 6d00 6200 6700 3276 5372 6e6c 6f6e 6700  m.b.g.2vSrnlong.
+00002ea0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -791,15 +791,15 @@
 00003160: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
 00003170: 0908 095f 1018 7b7b 3235 392c 2035 347d  ..._..{{259, 54}
 00003180: 2c20 7b31 3436 362c 2038 3932 7d7d 0908  , {1466, 892}}..
 00003190: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 000031a0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 000031b0: 0000 0000 0000 0000 0000 008b 0000 0009  ................
 000031c0: 0075 0066 006f 005f 0073 006c 0061 0076  .u.f.o._.s.l.a.v
-000031d0: 0065 6473 636c 626f 6f6c 0000 0000 0900  .edsclbool......
+000031d0: 0065 6473 636c 626f 6f6c 0100 0000 0900  .edsclbool......
 000031e0: 7500 6600 6f00 5f00 7300 6c00 6100 7600  u.f.o._.s.l.a.v.
 000031f0: 656c 6731 5363 6f6d 7000 0000 0000 0071  elg1Scomp......q
 00003200: da00 0000 0900 7500 6600 6f00 5f00 7300  ......u.f.o._.s.
 00003210: 6c00 6100 7600 656c 7376 4362 6c6f 6200  l.a.v.elsvCblob.
 00003220: 0003 1162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
 00003230: 0506 0708 090a 0b1b 5556 0a58 5f10 1276  ........UV.X_..v
 00003240: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
@@ -915,97 +915,97 @@
 00003920: 6f77 5369 6465 6261 7209 0908 095f 1018  owSidebar...._..
 00003930: 7b7b 3235 392c 2035 347d 2c20 7b31 3436  {{259, 54}, {146
 00003940: 362c 2038 3932 7d7d 0908 1523 2f3b 525f  6, 892}}...#/;R_
 00003950: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
 00003960: 0000 0000 000d 0000 0000 0000 0000 0000  ................
 00003970: 0000 0000 008b 0000 000c 0076 006d 006f  ...........v.m.o
 00003980: 0076 0065 005f 0063 0061 006d 0062 0067  .v.e._.c.a.m.b.g
-00003990: 0031 6473 636c 626f 6f6c 0072 7653 726e  .1dsclbool.rvSrn
-000039a0: 6c6f 6e67 0000 0001 0000 0011 0073 0063  long.........s.c
-000039b0: 0061 006c 0065 005f 0063 0061 006d 0062  .a.l.e._.c.a.m.b
-000039c0: 0067 0031 002e 0077 0065 0062 0070 496c  .g.1...w.e.b.pIl
-000039d0: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
-000039e0: 002e ffff ffff ffff 0000 0000 0011 0073  ...............s
-000039f0: 0075 0070 0065 0072 005f 0062 0075 006c  .u.p.e.r._.b.u.l
-00003a00: 006c 0065 0074 002e 0077 0065 0062 0070  .l.e.t...w.e.b.p
-00003a10: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
-00003a20: 0000 009e ffff ffff ffff 0000 0000 000a  ................
-00003a30: 0075 0066 006f 005f 006d 0061 0073 0074  .u.f.o._.m.a.s.t
-00003a40: 0065 0072 496c 6f63 626c 6f62 0000 0010  .e.rIlocblob....
-00003a50: 0000 00af 0000 002e ffff ffff ffff 0000  ................
-00003a60: 0000 000a 0075 0066 006f 005f 006d 0061  .....u.f.o._.m.a
-00003a70: 0073 0074 0065 0072 6277 7370 626c 6f62  .s.t.e.rbwspblob
-00003a80: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-00003a90: 0405 0607 0709 070b 075d 5368 6f77 5374  .........]ShowSt
-00003aa0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00003ab0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00003ac0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00003ad0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00003ae0: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
-00003af0: 0908 095f 1018 7b7b 3235 392c 2035 347d  ..._..{{259, 54}
-00003b00: 2c20 7b31 3436 362c 2038 3932 7d7d 0908  , {1466, 892}}..
-00003b10: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00003b20: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00003b30: 0000 0000 0000 0000 0000 008b 0000 000a  ................
-00003b40: 0075 0066 006f 005f 006d 0061 0073 0074  .u.f.o._.m.a.s.t
-00003b50: 0065 0072 6473 636c 626f 6f6c 0000 0000  .e.rdsclbool....
-00003b60: 0a00 7500 6600 6f00 5f00 6d00 6100 7300  ..u.f.o._.m.a.s.
-00003b70: 7400 6500 726c 6731 5363 6f6d 7000 0000  t.e.rlg1Scomp...
-00003b80: 0000 00a8 6600 0000 0a00 7500 6600 6f00  ....f.....u.f.o.
-00003b90: 5f00 6d00 6100 7300 7400 6500 726c 7376  _.m.a.s.t.e.rlsv
-00003ba0: 4362 6c6f 6200 0003 1162 706c 6973 7430  Cblob....bplist0
-00003bb0: 30d8 0102 0304 0506 0708 090a 0b19 5556  0.............UV
-00003bc0: 0a58 5f10 1276 6965 774f 7074 696f 6e73  .X_..viewOptions
-00003bd0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00003be0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00003bf0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00003c00: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00003c10: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00003c20: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
-00003c30: 6e53 697a 6514 0000 0000 0000 0000 0000  nSize...........
-00003c40: 0000 0000 0001 09ae 0c15 1d22 262b 3035  ..........."&+05
-00003c50: 3a3e 4347 4c50 d40d 0e0f 1011 120a 0a5a  :>CGLP.........Z
-00003c60: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-00003c70: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00003c80: 6c65 546e 616d 6511 012c 0909 d416 1718  leTname..,......
-00003c90: 0d19 1a19 1c57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00003ca0: 6474 6859 6173 6365 6e64 696e 6708 1023  dthYascending..#
-00003cb0: 0858 7562 6971 7569 7479 d410 0e0f 0d0a  .Xubiquity......
-00003cc0: 1f19 2109 10b5 085c 6461 7465 4d6f 6469  ..!....\dateModi
-00003cd0: 6669 6564 d410 0e0f 0d19 1f19 2508 085b  fied........%..[
-00003ce0: 6461 7465 4372 6561 7465 64d4 100e 0f0d  dateCreated.....
-00003cf0: 0a28 192a 0910 6108 5473 697a 65d4 0d0e  .(.*..a.Tsize...
-00003d00: 0f10 2c2d 190a 546b 696e 6410 7308 09d4  ..,-..Tkind.s...
-00003d10: 100e 0f0d 1932 0a34 0810 6409 556c 6162  .....2.4..d.Ulab
-00003d20: 656c d410 0e0f 0d19 370a 3908 104b 0957  el......7.9..K.W
-00003d30: 7665 7273 696f 6ed4 100e 0f0d 1912 0a3d  version........=
-00003d40: 0809 5863 6f6d 6d65 6e74 73d4 100e 0f0d  ..Xcomments.....
-00003d50: 1940 1942 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
-00003d60: 744f 7065 6e65 64d4 1617 180d 191f 1946  tOpened........F
-00003d70: 0808 5964 6174 6541 6464 6564 d40d 1718  ..YdateAdded....
-00003d80: 1648 4919 195a 7368 6172 654f 776e 6572  .HI..ZshareOwner
-00003d90: 10d2 0808 d40d 1718 164d 4919 195f 100f  .........MI.._..
-00003da0: 7368 6172 654c 6173 7445 6469 746f 7208  shareLastEditor.
-00003db0: 08d4 0d17 1816 5149 1919 5f10 1069 6e76  ......QI.._..inv
-00003dc0: 6974 6174 696f 6e53 7461 7475 7308 0808  itationStatus...
-00003dd0: 2340 2a00 0000 0000 0054 6b69 6e64 0923  #@*......Tkind.#
-00003de0: 4030 0000 0000 0000 0008 0019 002e 0040  @0.............@
-00003df0: 0048 005c 0065 0070 0083 008c 009d 009e  .H.\.e.p........
-00003e00: 00ad 00b6 00c1 00c7 00d1 00d9 00de 00e1  ................
-00003e10: 00e2 00e3 00ec 00f4 00fa 0104 0105 0107  ................
-00003e20: 0108 0111 011a 011b 011d 011e 012b 0134  .............+.4
-00003e30: 0135 0136 0142 014b 014c 014e 014f 0154  .5.6.B.K.L.N.O.T
-00003e40: 015d 0162 0164 0165 0166 016f 0170 0172  .].b.d.e.f.o.p.r
-00003e50: 0173 0179 0182 0183 0185 0186 018e 0197  .s.y............
-00003e60: 0198 0199 01a2 01ab 01ac 01ae 01af 01be  ................
-00003e70: 01c7 01c8 01c9 01d3 01dc 01e7 01e9 01ea  ................
-00003e80: 01eb 01f4 0206 0207 0208 0211 0224 0225  .............$.%
-00003e90: 0226 0227 0230 0235 0236 0000 0000 0000  .&.'.0.5.6......
-00003ea0: 0201 0000 0000 0000 0059 0000 0000 0000  .........Y......
-00003eb0: 0000 0000 0000 0000 023f 0000 0000 0000  .........?......
+00003990: 0031 6473 636c 626f 6f6c 002e ffff ffff  .1dsclbool......
+000039a0: ffff 0000 0000 0011 0073 0075 0070 0065  .........s.u.p.e
+000039b0: 0072 005f 0062 0075 006c 006c 0065 0074  .r._.b.u.l.l.e.t
+000039c0: 002e 0077 0065 0062 0070 496c 6f63 626c  ...w.e.b.pIlocbl
+000039d0: 6f62 0000 0010 0000 0041 0000 009e ffff  ob.......A......
+000039e0: ffff ffff 0000 0000 000a 0075 0066 006f  ...........u.f.o
+000039f0: 005f 006d 0061 0073 0074 0065 0072 496c  ._.m.a.s.t.e.rIl
+00003a00: 6f63 626c 6f62 0000 0010 0000 00af 0000  ocblob..........
+00003a10: 002e ffff ffff ffff 0000 0000 000a 0075  ...............u
+00003a20: 0066 006f 005f 006d 0061 0073 0074 0065  .f.o._.m.a.s.t.e
+00003a30: 0072 6277 7370 626c 6f62 0000 00b8 6270  .rbwspblob....bp
+00003a40: 6c69 7374 3030 d601 0203 0405 0607 0709  list00..........
+00003a50: 070b 075d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00003a60: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+00003a70: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+00003a80: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+00003a90: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+00003aa0: 6f77 5369 6465 6261 7209 0908 095f 1018  owSidebar...._..
+00003ab0: 7b7b 3235 392c 2035 347d 2c20 7b31 3436  {{259, 54}, {146
+00003ac0: 362c 2038 3932 7d7d 0908 1523 2f3b 525f  6, 892}}...#/;R_
+00003ad0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
+00003ae0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00003af0: 0000 0000 008b 0000 000a 0075 0066 006f  ...........u.f.o
+00003b00: 005f 006d 0061 0073 0074 0065 0072 6473  ._.m.a.s.t.e.rds
+00003b10: 636c 626f 6f6c 0100 0000 0a00 7500 6600  clbool......u.f.
+00003b20: 6f00 5f00 6d00 6100 7300 7400 6500 726c  o._.m.a.s.t.e.rl
+00003b30: 6731 5363 6f6d 7000 0000 0000 00a8 6600  g1Scomp.......f.
+00003b40: 0000 0a00 7500 6600 6f00 5f00 6d00 6100  ....u.f.o._.m.a.
+00003b50: 7300 7400 6500 726c 7376 4362 6c6f 6200  s.t.e.rlsvCblob.
+00003b60: 0003 1162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+00003b70: 0506 0708 090a 0b19 5556 0a58 5f10 1276  ........UV.X_..v
+00003b80: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00003b90: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00003ba0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00003bb0: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00003bc0: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00003bd0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
+00003be0: 6544 6174 6573 5869 636f 6e53 697a 6514  eDatesXiconSize.
+00003bf0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00003c00: 09ae 0c15 1d22 262b 3035 3a3e 4347 4c50  ....."&+05:>CGLP
+00003c10: d40d 0e0f 1011 120a 0a5a 6964 656e 7469  .........Zidenti
+00003c20: 6669 6572 5577 6964 7468 5961 7363 656e  fierUwidthYascen
+00003c30: 6469 6e67 5776 6973 6962 6c65 546e 616d  dingWvisibleTnam
+00003c40: 6511 012c 0909 d416 1718 0d19 1a19 1c57  e..,...........W
+00003c50: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+00003c60: 6365 6e64 696e 6708 1023 0858 7562 6971  cending..#.Xubiq
+00003c70: 7569 7479 d410 0e0f 0d0a 1f19 2109 10b5  uity........!...
+00003c80: 085c 6461 7465 4d6f 6469 6669 6564 d410  .\dateModified..
+00003c90: 0e0f 0d19 1f19 2508 085b 6461 7465 4372  ......%..[dateCr
+00003ca0: 6561 7465 64d4 100e 0f0d 0a28 192a 0910  eated......(.*..
+00003cb0: 6108 5473 697a 65d4 0d0e 0f10 2c2d 190a  a.Tsize.....,-..
+00003cc0: 546b 696e 6410 7308 09d4 100e 0f0d 1932  Tkind.s........2
+00003cd0: 0a34 0810 6409 556c 6162 656c d410 0e0f  .4..d.Ulabel....
+00003ce0: 0d19 370a 3908 104b 0957 7665 7273 696f  ..7.9..K.Wversio
+00003cf0: 6ed4 100e 0f0d 1912 0a3d 0809 5863 6f6d  n........=..Xcom
+00003d00: 6d65 6e74 73d4 100e 0f0d 1940 1942 0810  ments......@.B..
+00003d10: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00003d20: 64d4 1617 180d 191f 1946 0808 5964 6174  d........F..Ydat
+00003d30: 6541 6464 6564 d40d 1718 1648 4919 195a  eAdded.....HI..Z
+00003d40: 7368 6172 654f 776e 6572 10d2 0808 d40d  shareOwner......
+00003d50: 1718 164d 4919 195f 100f 7368 6172 654c  ...MI.._..shareL
+00003d60: 6173 7445 6469 746f 7208 08d4 0d17 1816  astEditor.......
+00003d70: 5149 1919 5f10 1069 6e76 6974 6174 696f  QI.._..invitatio
+00003d80: 6e53 7461 7475 7308 0808 2340 2a00 0000  nStatus...#@*...
+00003d90: 0000 0054 6b69 6e64 0923 4030 0000 0000  ...Tkind.#@0....
+00003da0: 0000 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
+00003db0: 0070 0083 008c 009d 009e 00ad 00b6 00c1  .p..............
+00003dc0: 00c7 00d1 00d9 00de 00e1 00e2 00e3 00ec  ................
+00003dd0: 00f4 00fa 0104 0105 0107 0108 0111 011a  ................
+00003de0: 011b 011d 011e 012b 0134 0135 0136 0142  .......+.4.5.6.B
+00003df0: 014b 014c 014e 014f 0154 015d 0162 0164  .K.L.N.O.T.].b.d
+00003e00: 0165 0166 016f 0170 0172 0173 0179 0182  .e.f.o.p.r.s.y..
+00003e10: 0183 0185 0186 018e 0197 0198 0199 01a2  ................
+00003e20: 01ab 01ac 01ae 01af 01be 01c7 01c8 01c9  ................
+00003e30: 01d3 01dc 01e7 01e9 01ea 01eb 01f4 0206  ................
+00003e40: 0207 0208 0211 0224 0225 0226 0227 0230  .......$.%.&.'.0
+00003e50: 0235 0236 0000 0000 0000 0201 0000 0000  .5.6............
+00003e60: 0000 0059 0000 0000 0000 0000 0000 0000  ...Y............
+00003e70: 0000 023f 0000 0000 0a10 0000 0000 0c00  ...?............
+00003e80: 7600 6d00 6f00 7600 6500 5f00 6300 6100  v.m.o.v.e._.c.a.
+00003e90: 6d00 6200 6700 3276 5372 6e6c 6f6e 6700  m.b.g.2vSrnlong.
+00003ea0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
+00003eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/game_cover.webp` & `SightTraining-0.1.20/spacedefense/assets/images/game_cover.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/game_cover_loss.webp` & `SightTraining-0.1.20/spacedefense/assets/images/game_cover_loss.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/game_cover_win.webp` & `SightTraining-0.1.20/spacedefense/assets/images/game_cover_win.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/icon.png` & `SightTraining-0.1.20/spacedefense/assets/images/icon.png`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/master_fighter.webp` & `SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_004.webp`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-00000000: 5249 4646 da1b 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
-00000010: 0a00 0000 3400 0000 4f00 0045 0000 4943  ....4...O..E..IC
+00000000: 5249 4646 fc1a 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
+00000010: 0a00 0000 3400 0000 5900 004e 0000 4943  ....4...Y..N..IC
 00000020: 4350 480c 0000 0000 0c48 4c69 6e6f 0210  CPH......HLino..
 00000030: 0000 6d6e 7472 5247 4220 5859 5a20 07ce  ..mntrRGB XYZ ..
 00000040: 0002 0009 0006 0031 0000 6163 7370 4d53  .......1..acspMS
 00000050: 4654 0000 0000 4945 4320 7352 4742 0000  FT....IEC sRGB..
 00000060: 0000 0000 0000 0000 0000 0000 f6d6 0001  ................
 00000070: 0000 0000 d32d 4850 2020 0000 0000 0000  .....-HP  ......
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -193,255 +193,241 @@
 00000c00: e253 e2db e363 e3eb e473 e4fc e584 e60d  .S...c...s......
 00000c10: e696 e71f e7a9 e832 e8bc e946 e9d0 ea5b  .......2...F...[
 00000c20: eae5 eb70 ebfb ec86 ed11 ed9c ee28 eeb4  ...p.........(..
 00000c30: ef40 efcc f058 f0e5 f172 f1ff f28c f319  .@...X...r......
 00000c40: f3a7 f434 f4c2 f550 f5de f66d f6fb f78a  ...4...P...m....
 00000c50: f819 f8a8 f938 f9c7 fa57 fae7 fb77 fc07  .....8...W...w..
 00000c60: fc98 fd29 fdba fe4b fedc ff6d ffff 414c  ...)...K...m..AL
-00000c70: 5048 4504 0000 0190 bf6d dbd9 e62b 7ade  PHE......m...+z.
-00000c80: 54b3 6def b36d dbb6 6ddb b66d dbb6 6ddb  T.m..m..m..m..m.
-00000c90: d6bc 7d6b d7e4 7d7e 689a bc49 1311 1300  ..}k..}~h..I....
-00000ca0: 2a35 b6c8 0b9a 4ada fc3b 1ba6 29e1 f7d1  *5....J..;..)...
-00000cb0: 3a41 a725 5dcd 888f c235 c4e5 0022 fe6f  :A.%]....5...".o
-00000cc0: a221 d16f 1091 cee1 b4a3 622a 22e2 6957  .!.o......b*".iW
-00000cd0: ede8 c9db bc0e d50c 6e09 da26 15d5 0ce7  ........n..&....
-00000ce0: 5322 9646 9a11 f45c 840e d38c 027f 4470  S".F...\......Dp
-00000cf0: ad4e 2b1a 99c5 ae7a 6a04 994a c5be e6d6  .N+....zj..J....
-00000d00: 08f7 8b28 6e69 a711 65ff d9c1 bd2e 9ae0  ...(ni..e.......
-00000d10: ba8d da4b 6940 3480 eb9c 8112 6f45 3b1e  ...Ki@4.....oE;.
-00000d20: a9f8 11a5 0a5b bc1c 8dcb 7d0f a59b a738  .....[....}....8
-00000d30: 3b94 3ef7 c42b 5406 a66c 68e4 ee30 8682  ;.>..+T..lh..0..
-00000d40: 733f 08c8 30fd 6863 2f87 d095 59f5 8d22  s?..0.hc/...Y.."
-00000d50: e3cc 73ed 7c1c 20f2 018f 2850 1659 3c62  ..s.|. ...(P.Y<b
-00000d60: c628 a23e 97ca 7d97 1f5d f08d 01bf 60e5  .(.>..}..]....`.
-00000d70: 9e69 6de2 e471 9c62 00c0 996a a731 c033  .im..q.b...j.1.3
-00000d80: fe06 60a9 7796 a1e3 9880 cb6e 6499 d904  ..`.w......nd...
-00000d90: 9812 3f22 cd83 51a5 2426 78d8 9509 04b9  ..?"..Q.$&x.....
-00000da0: 4a32 0601 538f cd94 4d72 358e 896f b4a4  J2..S...Mr5..o..
-00000db0: a060 06c4 b7e9 912c 644b 5f8e 4bd4 3330  .`.....,dK_.K.30
-00000dc0: 95d3 4929 ec21 8b8b ec79 350b d90b 1f16  ..I).!...y5.....
-00000dd0: 9775 9105 65fc 2538 95e7 c438 11a2 cf3d  .u..e.%8...8...=
-00000de0: ee69 0e2a 4bff eeac e921 27a1 8884 88c2  .i.*K....!'.....
-00000df0: 20d9 a7e1 da8f 02aa 30ed 7467 7f22 c9a3   .......0.tg."..
-00000e00: 81ce 5ef9 5029 6e95 77a7 a05a cdd7 ba86  ..^.P)n.w..Z....
-00000e10: 7012 4883 003b 2e4d 8d76 885f b323 2914  p.H..;.M.v._.#).
-00000e20: 556c 7938 3a41 6707 8a56 2522 a691 cd41  Uly8:Ag..V%"...A
-00000e30: 9484 76bb 9285 6ae7 dfcc 2a6a 12f3 5d53  ..v...j...*j..]S
-00000e40: 5424 cf83 c236 fa5c a31e 5bd0 11e9 afad  T$...6.\..[.....
-00000e50: b53c 6db8 154b f500 4006 3f0e 0530 9558  .<m..K..@.?..0.X
-00000e60: fc91 4787 4d3f df39 9800 0c7c 1e05 00fe  ..G.M?.9...|....
-00000e70: b7d7 e8dd aa6d f945 d1a1 2df7 87c7 e98a  .....m.E..-.....
-00000e80: 7eef 4500 1aa7 746a 7030 051d dffa 664e  ~.E...tjp0....fN
-00000e90: b92b 173c c1b8 2df3 503a 6a23 7dff 3abd  .+.<..-.P:j#}.:.
-00000ea0: 3ae4 f9ca bf36 6b84 ed1a c310 fe51 bb24  :....6k......Q.$
-00000eb0: 0d79 1fff 909e 5a2b 6888 a567 f7df 028f  .y....Z+h..g....
-00000ec0: 1aba b363 8964 d4d4 6d45 e3d6 9dff 6bd5  ...c.d..mE....k.
-00000ed0: 0821 edc9 9e9e 4ea0 f72c d27e e995 ef16  .!....N..,.~....
-00000ee0: 07e3 931f 6ee9 572e c448 4094 f3c8 dd74  ....n.W..H@....t
-00000ef0: ce85 afd9 540a 5591 90f2 6843 f712 fe7a  ....T.U...hC...z
-00000f00: 904b dc13 ea4d bef0 3193 8a59 0575 58ff  .K...M..1..Y.uX.
-00000f10: 3cde dca7 5480 1e58 13af d89a e34f bfcf  <...T..X.....O..
-00000f20: 1010 9f5d 1594 483e 9e8d 68f9 f97c 43c7  ...]..H>..h..|C.
-00000f30: c241 0650 9ab8 4656 1ab0 f5c1 88f8 5394  .A.P..FV......S.
-00000f40: ddbf eeb1 17cf cf6a 9a37 c808 aad5 fb79  .......j.7.....y
-00000f50: 9016 d9ec 4e7a 73c1 6e04 54ee dce8 0165  ....Nzs.n.T....e
-00000f60: 97b5 3296 80ca b9dc 6b52 5149 e171 0737  ..2.....kRQI.q.7
-00000f70: 75f9 0d78 2da0 c299 3b8b e8d4 63aa 75de  u..x-...;...c.u.
-00000f80: 82ca d34f c303 5440 0080 8b5f fa0f d569  ...O..T@..._...i
-00000f90: b950 cba4 1800 f8f4 7e2e a0fd 4c9e 09b5  .P......~...L...
-00000fa0: 8398 b42c 9153 ca58 f5a4 1925 0a2b deb2  ...,.S.X...%.+..
-00000fb0: f8f1 5502 0a2f fbfa 2a42 a2e6 ff41 c969  ..U../..*B...A.i
-00000fc0: b58f daa1 3956 3be6 9ecb a520 9a4f 5735  ....9V;.... .OW5
-00000fd0: 2a50 fa0e 8fd2 3fc7 f7b6 8a3d 6f33 d32a  *P....?....=o3.*
-00000fe0: f626 6ab4 34c4 df93 9c99 e956 a0dc 6741  .&j.4......V..gA
-00000ff0: b1af c4f6 1aca a48a f073 0c3d 0519 f82b  .........s.=...+
-00001000: 3f33 bf7b 72e8 3e57 6e92 6043 a791 8897  ?3.{r.>Wn.`C....
-00001010: 225f f241 ad64 39d6 aecc 4aa7 c810 2ee4  "_.A.d9...J.....
-00001020: 0128 fec7 e67d 1130 4cb1 da6c 3381 d3c0  .(...}.0L..l3...
-00001030: 2419 b8dd c0aa bf20 4d38 190b 004e 5392  $...... M8...NS.
-00001040: 284d 9aa4 0788 be9a 8339 378a 0280 b1fb  (M.......97.....
-00001050: 1f19 2f43 5835 c990 c41f 8c02 5ba7 8ac3  ../CX5......[...
-00001060: 8795 7705 0012 de6e 7cc7 7002 0060 68f7  ..w....n|.p..`h.
-00001070: 43da 192f 562e 631f 270b 76ac db43 4049  C../V.c.'.v..C@I
-00001080: 7df3 2ff6 b23f 1e29 01cc f541 a507 ec7c  }./..?.)...A...|
-00001090: 9ac2 23e6 6c0a 0465 750d 3e21 d2ec cfe7  ..#.l..eu.>!....
-000010a0: 6737 8e73 0565 0d41 a5ba 6e3c 37de 0f94  g7.s.e.A..n<7...
-000010b0: e6aa 1e3c 39bd 5eac 2b01 d900 5650 3820  ...<9.^.+...VP8 
-000010c0: 5207 0000 9021 009d 012a 5000 4600 3e91  R....!...*P.F.>.
-000010d0: 3895 4825 a322 2135 b96c 00b0 1209 6c00  8.H%."!5.l....l.
-000010e0: c985 ef59 7e4b 7e03 cd2a 9cfd bff1 a71c  ...Y~K~..*......
-000010f0: 94c1 fccf ec03 dc4f 98bf c5ff 53fe 93fb  .......O....S...
-00001100: 71da 03cc 03f5 4ba4 2f98 0fda 8f46 1fd5  q.....K./....F..
-00001110: cf71 9fb0 9ec0 1fd2 ffc0 7586 7f68 ff71  .q........u..h.q
-00001120: ec35 fb31 e97f fbb5 f063 fd9f fd97 ee57  .5.1.....c.....W
-00001130: c08f ed6f ff5e b00e 100f e3bf 841e 0c7f  ...o.^..........
-00001140: 8efc 55f3 67c3 5fa9 b36d c9dc ee31 94c8  ..U.g._..m...1..
-00001150: 89cb 2e59 f04f 443d faf8 11fc f791 9ba8  ...Y.OD=........
-00001160: 0dad df52 6900 72b9 c9d4 6f76 df13 a070  ...Ri.r...ov...p
-00001170: 6f58 a2e2 9625 c0fe cfb5 3be3 4ec0 802d  oX...%....;.N..-
-00001180: 651e edfc c8f7 445b b54a 695f f47e caee  e.....D[.Ji_.~..
-00001190: b56c fc5c bd42 440f 20e0 ffd7 bf3c 60c8  .l.\.BD. ....<`.
-000011a0: ed8a b0c0 2c42 39e7 560f 3277 6611 e954  ....,B9.V.2wf..T
-000011b0: 12ec f771 ae4a e42e b83f 3d04 2926 683b  ...q.J...?=.)&h;
-000011c0: 8384 1766 0283 ca7c 8e24 80b8 1044 dfe1  ...f...|.$...D..
-000011d0: 6262 28f4 8aec 54d8 0000 fefd b4e8 c7a5  bb(...T.........
-000011e0: 0180 dfbe b27f cc76 8b04 708b 36be 0ef2  .......v..p.6...
-000011f0: 7fb2 60ec b0fe 52a4 84b0 6e21 a9ea ac70  ..`...R...n!...p
-00001200: e877 fc93 21df 691f d763 e722 4faa 1fa2  .w..!.i..c."O...
-00001210: 1736 d20e 2471 6b32 2906 26c7 cbc5 62b2  .6..$qk2).&...b.
-00001220: e93c 7115 dc8f e60c 113d 9214 a060 a69a  .<q......=...`..
-00001230: 3d56 776f 2f24 cfa0 0a93 0c3f 3710 4a9b  =Vwo/$.....?7.J.
-00001240: 19f0 f21f fa87 b67c 6a02 245c 4b89 d07b  .......|j.$\K..{
-00001250: 7195 cf95 a6f8 86de e6ea 4dd5 6864 a69e  q.........M.hd..
-00001260: 1599 6d30 cacc 78af 2806 ae50 0b18 2bbd  ..m0..x.(..P..+.
-00001270: e1cd 0718 e5bf e258 0f23 d5e1 d9e7 ec88  .......X.#......
-00001280: 8c79 8d68 8b44 936e fe5f 85c0 1fd1 42d1  .y.h.D.n._....B.
-00001290: 5e8f dfc3 eb1e 1098 f3e9 7429 4aa9 b14a  ^.........t)J..J
-000012a0: 48de 5ec0 e0d5 7eb3 b48f 7ada 6e1d c4c4  H.^...~...z.n...
-000012b0: 352f 8a4e e788 41a4 b0ae a596 8035 faec  5/.N..A......5..
-000012c0: 4efb 791d 08c6 ffea 491c e9ff df6e 08c3  N.y.....I....n..
-000012d0: 0b6e 814d 41ba ef66 9484 1093 e6ff e1c8  .n.MA..f........
-000012e0: f6c8 90c5 d205 c83c 730b 64f0 f919 1eee  .......<s.d.....
-000012f0: 1e02 1f49 1455 956f a60b 316e b943 f0d9  ...I.U.o..1n.C..
-00001300: d278 98b6 7ce0 7367 fff7 20ae a9e8 2994  .x..|.sg.. ...).
-00001310: 454c 7be1 a43c 218e 583c 46a5 1fa7 38f8  EL{..<!.X<F...8.
-00001320: 2004 fb3c 99b8 cff5 dd27 bfc6 4b13 ab98   ..<.....'..K...
-00001330: bd80 08b4 b075 60a5 1d28 45bf f314 8c9e  .....u`..(E.....
-00001340: be1d b1d6 0a70 6c67 6f26 c74b 851b 0d96  .....plgo&.K....
-00001350: 91e4 f098 bcd6 17b4 6bb9 74dd 74e3 f12f  ........k.t.t../
-00001360: ae44 4920 7c91 10c7 b219 3691 0a01 f0e2  .DI |.....6.....
-00001370: 0b38 4dad fd5a 7cb4 b1e1 aa14 7809 1e2b  .8M..Z|.....x..+
-00001380: c9f0 83f3 5fce 3e11 8df9 3c7b 4f46 6035  ...._.>...<{OF`5
-00001390: 212e 3fb7 c868 6a33 7599 5ee2 2bcb 28e7  !.?..hj3u.^.+.(.
-000013a0: 0fbc 9029 ad61 1fe7 d426 2f44 260b 9524  ...).a...&/D&..$
-000013b0: f46d 3734 e6f9 082d a426 97ac 2992 b7a1  .m74...-.&..)...
-000013c0: b558 b249 7e1e 5d86 64c0 f583 850a 94b4  .X.I~.].d.......
-000013d0: 13d6 5ceb f181 c849 107c d264 b069 2f29  ..\....I.|.d.i/)
-000013e0: 648c 91f6 d4ef 349c 0a76 e8eb 4666 7051  d.....4..v..FfpQ
-000013f0: a5ef f4e7 4825 63dd bae8 eedf 9ac1 7ce9  ....H%c.......|.
-00001400: 0b53 f9b0 1df2 096f a5c1 9664 4521 bf03  .S.....o...dE!..
-00001410: 79a5 0c38 4a09 0245 d095 18ee c354 b4d4  y..8J..E.....T..
-00001420: 4ba8 c5c9 d1c1 3e1b 535e 27ea 71e2 1a43  K.....>.S^'.q..C
-00001430: cd3d bb74 2aed 2240 f90c c8eb 2299 2352  .=.t*."@....".#R
-00001440: f6c0 8ff4 bdaa 8dbf 9315 59ce 764b da39  ..........Y.vK.9
-00001450: 309e 592b 55b5 1191 03f6 5529 faef cb1e  0.Y+U.....U)....
-00001460: 7aeb 8397 dbd5 b37b 1ed6 7eeb 5388 ce72  z......{..~.S..r
-00001470: 5abc f55c 10e0 249a 0556 e1df e59d 6207  Z..\..$..V....b.
-00001480: 207d a297 c6af 2b8d d591 bd95 bf21 a7af   }....+......!..
-00001490: b7d3 71cd ef9f a755 8511 3ced 156a 44e5  ..q....U..<..jD.
-000014a0: 9204 1f4a 90b8 ab1e 88c9 57ea 3f79 be1d  ...J......W.?y..
-000014b0: eaaf 7442 8cb4 6d92 3be2 7b99 f64d 6026  ..tB..m.;.{..M`&
-000014c0: e726 5860 c324 a642 2fd4 4bbc da31 d8ea  .&X`.$.B/.K..1..
-000014d0: 1799 bc2b f67f b69f 8fcd 74d4 f380 b13f  ...+......t....?
-000014e0: 7b14 72bc c4a1 95bc fb96 2c77 e862 0349  {.r.......,w.b.I
-000014f0: 4f62 ed25 2b75 ac43 4ce1 d8d7 4431 cec5  Ob.%+u.CL...D1..
-00001500: b6a2 bef6 c597 5662 4ee6 e91c fab4 bc05  ......VbN.......
-00001510: a3d3 72f3 67b2 8216 dbbc 4d6c b1ad bad7  ..r.g.....Ml....
-00001520: 1b93 7f16 1e32 1203 e274 78b0 4ce4 6279  .....2...tx.L.by
-00001530: 62a0 4c3f 1d3f 6bac 90ee e84e bc99 b7b0  b.L?.?k....N....
-00001540: 951c e4eb 52cc d600 6fea 7332 eff9 030b  ....R...o.s2....
-00001550: 7cc1 82db ec3b fa43 5501 fbf5 4a46 8032  |....;.CU...JF.2
-00001560: 9710 265b c46d 4a4c 09f1 f0ff 5f8b 1d9e  ..&[.mJL...._...
-00001570: 12c7 13d9 1e7e 2eaf 526a 21ff 45aa 04be  .....~..Rj!.E...
-00001580: 478b 6a7d 0196 996a b419 1fa2 9969 5a31  G.j}...j.....iZ1
-00001590: b132 cc01 e032 b21f 603b 8e2c 7b46 97a0  .2...2..`;.,{F..
-000015a0: bdf6 eefd 9e44 0198 898a 96fe 6ded 6fe5  .....D......m.o.
-000015b0: 1a11 06bb d6cc 6717 1645 153a 760d 318e  ......g..E.:v.1.
-000015c0: d4a9 afe0 deb8 d1ae 8823 3d3e 8b1a 509f  .........#=>..P.
-000015d0: f562 770e 220a ef72 1c72 4f1f 9097 fe90  .bw."..r.rO.....
-000015e0: fdd4 ab82 fd0d f941 68f1 c84c 5e0d e7cb  .......Ah..L^...
-000015f0: 7b62 6140 c2b2 8855 ad10 1a05 a464 ce2b  {ba@...U.....d.+
-00001600: a526 bce2 2a8a fc35 afa7 eb7b 2f19 21df  .&..*..5...{/.!.
-00001610: cfc6 d0e1 c3b7 9ca4 8127 bb78 6956 efd4  .........'.xiV..
-00001620: 29dd 874d 38e4 abce 6270 f344 b18f 39d7  )..M8...bp.D..9.
-00001630: 7c71 db04 1c1a ed2e 6159 7c59 3c88 d7a3  |q......aY|Y<...
-00001640: 972c 6ace 5608 bc0f f2aa 67dd 117b 2720  .,j.V.....g..{' 
-00001650: f401 83b4 788d 3eaf a54c bf19 6be7 65be  ....x.>..L..k.e.
-00001660: be97 9091 535d f4d9 9d3c 7818 fe2a 94f4  ....S]...<x..*..
-00001670: c8f4 c73c 8571 6e83 3cad 4841 16c5 1ee0  ...<.qn.<.HA....
-00001680: 77b2 38cd be66 a066 ed2e a066 4e16 e7dc  w.8..f.f...fN...
-00001690: 8e0d ae54 3e78 2b83 96aa a75c 7259 846e  ...T>x+....\rY.n
-000016a0: 9376 fce6 433b fa38 c37e c0f1 a223 a019  .v..C;.8.~...#..
-000016b0: c6e3 2faf 2dd1 c609 9642 dc8d 4eaf 8d55  ../.-....B..N..U
-000016c0: 6b11 3c8f e481 51aa 68b2 2cdb 09bf 2524  k.<...Q.h.,...%$
-000016d0: 4e6b 6cae cfc2 6549 0f25 95c8 5b39 111f  Nkl...eI.%..[9..
-000016e0: de52 2c99 e316 7093 2910 48e9 f9d6 ded0  .R,...p.).H.....
-000016f0: 4f77 446a 2619 d156 7ad3 96a4 560c 0a20  OwDj&..Vz...V.. 
-00001700: 346f c26f 9718 09af 07ca af1f 1de2 fa0f  4o.o............
-00001710: 9bd4 8051 6d81 ccb9 43b3 ee3b 4ec2 512b  ...Qm...C..;N.Q+
-00001720: c88c 8b24 ea98 58c8 de6b ff59 6ea4 17d5  ...$..X..k.Yn...
-00001730: b0f0 b07e 0e44 eef4 18a0 67d2 b3a8 81f5  ...~.D....g.....
-00001740: 3d01 e951 659d aee0 a878 80ee 4cd3 60fc  =..Qe....x..L.`.
-00001750: 6976 66c1 4a56 cfda 4589 84ce 5a73 2824  ivf.JV..E...Zs($
-00001760: 2d04 5213 4ab7 45e5 7374 05f6 bb31 a546  -.R.J.E.st...1.F
-00001770: de0d 94ce cf83 1a2d 5d09 4669 454a e08e  .......-].FiEJ..
-00001780: 6009 d92e 8d13 3787 b668 b69e 6b5c aa09  `.....7..h..k\..
-00001790: d39b ab88 e4c1 8b2b 069e 0622 a119 bbce  .......+..."....
-000017a0: 0e5a fdee b31f 3bd7 03ad ef6e 2ef2 d990  .Z....;....n....
-000017b0: 75da aa92 d27b de26 8b55 ec2a 5963 00cf  u....{.&.U.*Yc..
-000017c0: ff7f dd02 8777 8386 656b fb2a 0a3f ffaa  .....w..ek.*.?..
-000017d0: bb05 6735 b26c 6613 980c 69d2 2e89 f3e8  ..g5.lf...i.....
-000017e0: c5cb 5f2a 74db 9ea2 6cf9 89f9 e21f ffe5  .._*t...l.......
-000017f0: cd7d 21e1 072d c224 6335 4999 2f13 d106  .}!..-.$c5I./...
-00001800: 4d0a 0f7b a502 eb88 89a3 f185 9765 be36  M..{.........e.6
-00001810: 0081 7a00 0000 584d 5020 c403 0000 3c78  ..z...XMP ....<x
-00001820: 3a78 6d70 6d65 7461 2078 6d6c 6e73 3a78  :xmpmeta xmlns:x
-00001830: 3d22 6164 6f62 653a 6e73 3a6d 6574 612f  ="adobe:ns:meta/
-00001840: 2220 783a 786d 7074 6b3d 2258 4d50 2043  " x:xmptk="XMP C
-00001850: 6f72 6520 362e 302e 3022 3e0a 2020 203c  ore 6.0.0">.   <
-00001860: 7264 663a 5244 4620 786d 6c6e 733a 7264  rdf:RDF xmlns:rd
-00001870: 663d 2268 7474 703a 2f2f 7777 772e 7733  f="http://www.w3
-00001880: 2e6f 7267 2f31 3939 392f 3032 2f32 322d  .org/1999/02/22-
-00001890: 7264 662d 7379 6e74 6178 2d6e 7323 223e  rdf-syntax-ns#">
-000018a0: 0a20 2020 2020 203c 7264 663a 4465 7363  .      <rdf:Desc
-000018b0: 7269 7074 696f 6e20 7264 663a 6162 6f75  ription rdf:abou
-000018c0: 743d 2222 0a20 2020 2020 2020 2020 2020  t="".           
-000018d0: 2078 6d6c 6e73 3a65 7869 663d 2268 7474   xmlns:exif="htt
-000018e0: 703a 2f2f 6e73 2e61 646f 6265 2e63 6f6d  p://ns.adobe.com
-000018f0: 2f65 7869 662f 312e 302f 220a 2020 2020  /exif/1.0/".    
-00001900: 2020 2020 2020 2020 786d 6c6e 733a 7469          xmlns:ti
-00001910: 6666 3d22 6874 7470 3a2f 2f6e 732e 6164  ff="http://ns.ad
-00001920: 6f62 652e 636f 6d2f 7469 6666 2f31 2e30  obe.com/tiff/1.0
-00001930: 2f22 0a20 2020 2020 2020 2020 2020 2078  /".            x
-00001940: 6d6c 6e73 3a78 6d70 3d22 6874 7470 3a2f  mlns:xmp="http:/
-00001950: 2f6e 732e 6164 6f62 652e 636f 6d2f 7861  /ns.adobe.com/xa
-00001960: 702f 312e 302f 223e 0a20 2020 2020 2020  p/1.0/">.       
-00001970: 2020 3c65 7869 663a 5069 7865 6c59 4469    <exif:PixelYDi
-00001980: 6d65 6e73 696f 6e3e 3730 3c2f 6578 6966  mension>70</exif
-00001990: 3a50 6978 656c 5944 696d 656e 7369 6f6e  :PixelYDimension
-000019a0: 3e0a 2020 2020 2020 2020 203c 6578 6966  >.         <exif
-000019b0: 3a50 6978 656c 5844 696d 656e 7369 6f6e  :PixelXDimension
-000019c0: 3e38 303c 2f65 7869 663a 5069 7865 6c58  >80</exif:PixelX
-000019d0: 4469 6d65 6e73 696f 6e3e 0a20 2020 2020  Dimension>.     
-000019e0: 2020 2020 3c65 7869 663a 436f 6c6f 7253      <exif:ColorS
-000019f0: 7061 6365 3e31 3c2f 6578 6966 3a43 6f6c  pace>1</exif:Col
-00001a00: 6f72 5370 6163 653e 0a20 2020 2020 2020  orSpace>.       
-00001a10: 2020 3c74 6966 663a 5852 6573 6f6c 7574    <tiff:XResolut
-00001a20: 696f 6e3e 3231 3630 3030 302f 3130 3030  ion>2160000/1000
-00001a30: 303c 2f74 6966 663a 5852 6573 6f6c 7574  0</tiff:XResolut
-00001a40: 696f 6e3e 0a20 2020 2020 2020 2020 3c74  ion>.         <t
-00001a50: 6966 663a 5265 736f 6c75 7469 6f6e 556e  iff:ResolutionUn
-00001a60: 6974 3e32 3c2f 7469 6666 3a52 6573 6f6c  it>2</tiff:Resol
-00001a70: 7574 696f 6e55 6e69 743e 0a20 2020 2020  utionUnit>.     
-00001a80: 2020 2020 3c74 6966 663a 4f72 6965 6e74      <tiff:Orient
-00001a90: 6174 696f 6e3e 313c 2f74 6966 663a 4f72  ation>1</tiff:Or
-00001aa0: 6965 6e74 6174 696f 6e3e 0a20 2020 2020  ientation>.     
-00001ab0: 2020 2020 3c74 6966 663a 5952 6573 6f6c      <tiff:YResol
-00001ac0: 7574 696f 6e3e 3231 3630 3030 302f 3130  ution>2160000/10
-00001ad0: 3030 303c 2f74 6966 663a 5952 6573 6f6c  000</tiff:YResol
-00001ae0: 7574 696f 6e3e 0a20 2020 2020 2020 2020  ution>.         
-00001af0: 3c78 6d70 3a4d 6574 6164 6174 6144 6174  <xmp:MetadataDat
-00001b00: 653e 3230 3234 2d30 342d 3037 5432 313a  e>2024-04-07T21:
-00001b10: 3331 3a35 342b 3038 3a30 303c 2f78 6d70  31:54+08:00</xmp
-00001b20: 3a4d 6574 6164 6174 6144 6174 653e 0a20  :MetadataDate>. 
-00001b30: 2020 2020 2020 2020 3c78 6d70 3a43 7265          <xmp:Cre
-00001b40: 6174 6f72 546f 6f6c 3e50 6978 656c 6d61  atorTool>Pixelma
-00001b50: 746f 7220 5072 6f20 332e 352e 373c 2f78  tor Pro 3.5.7</x
-00001b60: 6d70 3a43 7265 6174 6f72 546f 6f6c 3e0a  mp:CreatorTool>.
-00001b70: 2020 2020 2020 2020 203c 786d 703a 4372           <xmp:Cr
-00001b80: 6561 7465 4461 7465 3e32 3032 342d 3033  eateDate>2024-03
-00001b90: 2d33 3054 3137 3a32 383a 3339 3c2f 786d  -30T17:28:39</xm
-00001ba0: 703a 4372 6561 7465 4461 7465 3e0a 2020  p:CreateDate>.  
-00001bb0: 2020 2020 3c2f 7264 663a 4465 7363 7269      </rdf:Descri
-00001bc0: 7074 696f 6e3e 0a20 2020 3c2f 7264 663a  ption>.   </rdf:
-00001bd0: 5244 463e 0a3c 2f78 3a78 6d70 6d65 7461  RDF>.</x:xmpmeta
-00001be0: 3e0a                                     >.
+00000c70: 5048 0205 0000 01a0 766d db31 b79e d3fd  PH......vm.1....
+00000c80: bcf3 ce64 6227 bb8d b3ca a8b6 6ddb b66d  ...db'......m..m
+00000c90: dbb6 6ddb b6bb 6bbb 4d1a 371a bccf fd21  ..m...k.M.7....!
+00000ca0: afe7 8988 0900 3d73 b179 80d5 e51f 6df5  ......=s.y....m.
+00000cb0: 6394 df49 216b 8c81 4d6d 9290 3e8a 6092  c..I!k..Mm..>.`.
+00000cc0: eb4e 0131 bd13 930a bf47 4461 bb99 458d  .N.1.....GDa..E.
+00000cd0: d310 11ef e465 1099 68cb 155f 8e41 4e07  .....e..h.._.AN.
+00000ce0: 30b7 b533 83fc 1e8a d059 843d 513f 4470  0..3.....Y.=Q?Dp
+00000cf0: 9f89 3d75 32c4 eefa b0a7 bf5d ec53 2473  ..=u2......].S$s
+00000d00: b865 542c ad0a 73dc cea3 b8ad 2f73 0a7c  .eT,..s...../s.|
+00000d10: 96a0 9b78 d6b4 c996 c067 7919 63de 4ea5  ...x.....gy.c.N.
+00000d20: 325a 30a6 5a3c 4ad3 b37e 4c09 3c43 6560  2Z0.Z<J..~L.<Ce`
+00000d30: f628 2343 cc73 2c28 fb67 7dc2 0cbe 570a  .(#C.s,(.g}...W.
+00000d40: 2a7c 5694 11c4 a3ee 3754 2a9c 8934 3180  *|V.....7T*..41.
+00000d50: 0474 3dfb 992a 42eb d335 a54c 0ec6 05f5  .t=..*B..5.L....
+00000d60: b999 85ea 0a3f d696 333b 1089 18f9 2807  .....?..3;....(.
+00000d70: d5a7 bfb7 d470 7618 f703 1654 df66 43a4  .....pv....T.fC.
+00000d80: f11d 1dc6 a9d1 ec43 0f9f ee4c 53e7 d8fc  .......C...LS...
+00000d90: 57d7 b78d 8c52 8310 5d00 1027 bfa0 e6ff  W....R..]..'....
+00000da0: d479 902f d893 0755 09af 1300 703b 48d5  .y./...U....p;H.
+00000db0: c9e9 4740 6d33 51c2 13d5 6a26 a1ca b703  ..G@m3Q...j&....
+00000dc0: 5573 312a e0cc a0b6 f376 aa56 667b d5cc  Us1*.....v.Vf{..
+00000dd0: 9e0a 9c5d d432 37fc 83aa 9f0b 262a 19c2  ...].27.....&*..
+00000de0: 3879 ff39 a9e3 5e73 cb6f aa9e f5ee 9070  8y.9..^s.o.....p
+00000df0: 832a 10e9 218b cfc7 a940 025a 1d4b a2a8  .*..!....@.Z.K..
+00000e00: a9e5 c5cc e266 3502 2265 7987 8224 91e0  .....f5."ey..$..
+00000e10: c2fa ddce 40ed ed3f 3655 7655 662e 6d90  ....@..?6UvUf.m.
+00000e20: 93cf 474a 94b8 579a fcdc 82fa a47f 0fb5  ..GJ..W.........
+00000e30: f057 424a 79cb e04b 1be5 992b ecfc 6d47  .WBJy..K...+..mG
+00000e40: 1d67 5eee e44f 6441 64b4 0cbf e220 d7bd  .g^..OdAd.... ..
+00000e50: d6d6 9f02 ea3c f3c6 8070 831c b75a 0609  .....<...p...Z..
+00000e60: a75a 6152 c4af cd89 648a 0e68 f97f 4a94  .ZaR....d..h..J.
+00000e70: 518a b428 4144 48db 8d2e 625c 489f 6b19  Q..(ADH...b\H.k.
+00000e80: e8a8 f68f 2b2a ba8a 4185 9311 222e fb17  ....+*..A..."...
+00000e90: 935c c6a8 094f 72d0 9185 8403 2dfc 49ae  .\...Or.....-.I.
+00000ea0: 9067 dd44 4a7d ee0d 00e6 32cb 3eda d0d1  .g.DJ}....2.>...
+00000eb0: 69c6 8d7e a11c 80fb f9a3 6e00 c02f f812  i..~......n../..
+00000ec0: 0d6e 35b7 fd16 9089 9667 13a3 8c64 dc9f  .n5......g...d..
+00000ed0: 8a00 10f1 ea44 50b3 23c9 1499 69fb b4a2  .....DP.#...i...
+00000ee0: 5cb5 84a5 3c40 f79c 6d7b d229 3255 f8b3  \...<@..m{.)2U..
+00000ef0: f6f3 db7c e076 0293 3290 b956 bb75 0029  ...|.v..2..V.u.)
+00000f00: 9760 dfb8 833d 8878 d16b bef0 a9cc 2926  .`...=.x.k....)&
+00000f10: a5d4 bc99 f5f7 502a 9312 c6c7 3e46 360b  ......P*....>F6.
+00000f20: 53ab e4fb c828 ba21 6fe0 8223 5f72 2863  S....(.!o..#_r(c
+00000f30: a82d e9e6 ce0e 46e0 9da3 5acd 3fff 2943  .-....F...Z.?.)C
+00000f40: 6004 b5c6 dfdb d8bb 9cbf 9180 28e7 96af  `...........(...
+00000f50: e1d4 93ef 3304 7994 ea8e 5ae3 efac ee52  ....3.y...Z....R
+00000f60: dc97 07a5 c425 a2fe c4c3 affe 0952 42ba  .....%.......RB.
+00000f70: 5d4f d41a 7f7f 638f 923e 0650 9b98 831b  ]O....c..>.P....
+00000f80: 8fdc f33c c59e 0bd3 bf09 5ad9 5368 2e6a  ...<......Z.Sh.j
+00000f90: fb71 6d69 b732 7e3c 686e ca53 75e4 f607  .qmi.2~<hn.Su...
+00000fa0: 7f2c f45c dbf7 1a59 f774 4c14 323e 9c5d  .,.\...Y.tL.2>.]
+00000fb0: 3428 ce93 03dd f2be 716d 17b6 33d4 f9a6  4(......qm..3...
+00000fc0: 897d 47a0 d79c 09b5 c25d 08e8 9e33 40d8  .}G......]...3@.
+00000fd0: 434d aca3 cdc0 1370 4c63 e5d3 564d 3069  CM.....pLc..VM0i
+00000fe0: 5e28 0187 2421 337e 50d4 d87a a7b9 8b23  ^(..$!3~P..z...#
+00000ff0: b8b7 b96b 451d 26af 8be2 f4c6 97da 9586  ...kE.&.........
+00001000: fa14 5ef5 f1d6 1509 9af8 4540 dd66 1ead  ..^.......E@.f..
+00001010: 6cd4 8f6b b31b 16d4 33fd 3933 8ce8 c350  l..k....3.93...P
+00001020: 6c4b 0aca b5dc b2a8 9449 a510 adf7 dbb9  lK.......I......
+00001030: eb21 70cc 4701 657f 6ffe 559d af1b b2e4  .!p.G.e.o.U.....
+00001040: 20a6 ef29 c36b 65aa 7bd5 820a 2f87 5c94   ..).ke.{.../.\.
+00001050: b2a6 a451 09db b8e2 f1f2 907e 9f16 4434  ...Q.......~..D4
+00001060: 318d 8ba7 a874 8769 984d e24a a5f6 4912  1....t.i.M.J..I.
+00001070: 7f4a 467e 5280 68bd 5e42 93f0 b7a8 982e  .JF~R.h.^B......
+00001080: 2251 1fc4 e832 2ee8 a518 dde1 9ae7 7f45  "Q...2.........E
+00001090: 28cc e7b4 6898 a12c a73f f073 0411 5b7f  (...h..,.?.s..[.
+000010a0: 703d 2996 5415 3ccf 5145 78c3 5b03 6e3e  p=).T.<.QEx.[.n>
+000010b0: 5564 d91a 0050 eeaf c88b 5820 7d32 45ce  Ud...P....X }2E.
+000010c0: 7b02 a9f6 822a 4a28 a581 f775 549a bdda  {....*J(...uT...
+000010d0: 1f00 dc77 d810 3167 3407 e073 4140 c484  ...w..1g4..sA@..
+000010e0: 8e04 8054 7e4a 95d8 8769 10f4 4249 d632  ...T~J...i..BI.2
+000010f0: 1fc8 1d3c f7c9 c73b 6303 0180 94dc fcf2  ...<...;c.......
+00001100: c3d9 e626 0000 52e6 3e55 20cc 27ea 19a7  ...&..R.>U .'...
+00001110: 65ca cb98 eb09 e27c 60a4 2f07 a24e c111  e......|`./..N..
+00001120: 1e04 4449 b19b 822c fabe 1c68 e8d5 67ef  ..DI...,...h..g.
+00001130: 8b34 bb44 da64 37d0 9ac4 5c16 c4a8 e5d7  .4.D.d7...\.....
+00001140: d5c5 950d 5a00 9882 aa8d 3cf0 22d9 8698  ....Z.....<."...
+00001150: 32c6 0574 58f0 9c1d 69f6 f7ab cbdb c779  2..tX...i......y
+00001160: 72a0 43a7 a0f2 7d77 1c68 6f06 5d46 2e38  r.C...}w.ho.]F.8
+00001170: beac 5594 2707 6a02 5650 3820 b805 0000  ..U.'.j.VP8 ....
+00001180: 901b 009d 012a 5a00 4f00 3e9d 4099 4925  .....*Z.O.>.@.I%
+00001190: a3a2 212e f80b 00b0 1389 6900 15e0 1fca  ..!.......i.....
+000011a0: 3f0b fbf1 feef e11f 88ef 6e67 0589 bad2  ?.........ng....
+000011b0: 7e10 fdf7 093f 0f75 0276 bda0 566b 6a59  ~....?.u.v..VkjY
+000011c0: 2746 52be 33d0 bb9f cfaf 3d81 ff5d facc  'FR.3.....=..]..
+000011d0: f933 36b0 d77a a0d9 df23 a83c 60b0 f2be  .36..z...#.<`...
+000011e0: 5822 99fc fe6e b688 382d fce4 d67e b9b8  X"...n..8-...~..
+000011f0: 2dd9 12a1 e746 03ef e60a c98e db63 165f  -....F.......c._
+00001200: cdf0 8eeb 60a2 cf61 bdff 7edf 7f17 4a20  ....`..a..~...J 
+00001210: fbde 70cf 9c99 2ced cf40 df3f 65b8 f332  ..p...,..@.?e..2
+00001220: 3d71 87ba 8bf4 88b3 ebe0 37f7 ca06 d8a8  =q........7.....
+00001230: b95b 6399 d08c 1139 6b8c f1c4 f861 04f7  .[c....9k....a..
+00001240: 0dfe 0b02 aa74 811f 8e9f 5d46 b088 7e95  .....t....]F..~.
+00001250: 301d 654c 5587 0c8a 970c 015e 2f7d d777  0.eLU......^/}.w
+00001260: 7b22 e7fb 8000 fefd 3694 5149 0a41 f02d  {"......6.QI.A.-
+00001270: c980 832b c033 02db 4197 f478 9332 c9fa  ...+.3..A..x.2..
+00001280: a229 a47c d272 fb48 cb26 5f2e 0c06 55e8  .).|.r.H.&_...U.
+00001290: cb89 2027 3fba 1d80 07ea ae27 d546 135d  .. '?......'.F.]
+000012a0: a07f 913e fa54 102a a413 1793 b421 6c2b  ...>.T.*.....!l+
+000012b0: 85b8 1be8 8e35 0d0a 018f b280 7fa8 3219  .....5........2.
+000012c0: e8ca f3c2 64ce 3980 032c 7ede 2df0 bfe3  ....d.9..,~.-...
+000012d0: 3fc1 6687 2a75 f02c cba4 ebd1 5977 c029  ?.f.*u.,....Yw.)
+000012e0: bd50 a142 1729 f4d5 1e3d 8fc9 52f1 749c  .P.B.)...=..R.t.
+000012f0: a255 bbea f4d6 74e0 05ab 1a71 1a0f 36d7  .U....t....q..6.
+00001300: fd85 1ff8 cc3e 5c03 e6ac 6786 c17a ec7d  .....>\...g..z.}
+00001310: 2a0b 8e77 6797 a895 6731 5864 ec45 8fc0  *..wg...g1Xd.E..
+00001320: 74fc 7627 2035 4949 dcde e3f2 6c94 e87e  t.v' 5II....l..~
+00001330: c65d 18d6 c35b d9e8 fb2c ca05 ec3b 9fe0  .]...[...,...;..
+00001340: 7431 0598 300c aa87 d735 00c6 2bb1 ee6b  t1..0....5..+..k
+00001350: 397b 295c 9f9e aabf 8b26 e13b 3ad3 4ea3  9{)\.....&.;:.N.
+00001360: 285e 7edf e2a5 32e9 a6c7 db6a de04 ec40  (^~...2....j...@
+00001370: d3f5 d7df eb42 e5c1 3504 3b52 2256 ec74  .....B..5.;R"V.t
+00001380: c4e6 c8b4 80aa d8b2 7308 eb66 8ba1 8c9a  ........s..f....
+00001390: 0745 8679 f64c 023e 5a55 71c3 2dd4 7939  .E.y.L.>ZUq.-.y9
+000013a0: c9f9 1329 ef1a 78b8 f3c0 5df3 9def 618e  ...)..x...]...a.
+000013b0: 3cdc 27a9 912c 6748 05ab 3f93 7a72 d688  <.'..,gH..?.zr..
+000013c0: 210c 70f7 e66d 4164 d9ed e294 3007 7424  !.p..mAd....0.t$
+000013d0: e45e 8196 99a1 34e7 a97b d1c7 5316 5e27  .^....4..{..S.^'
+000013e0: 5b44 edec 2f5d f1bc 02a5 0e28 fb24 8384  [D../].....(.$..
+000013f0: 25a8 60f1 b04e 7af9 fc1a fe17 e1f6 0028  %.`..Nz........(
+00001400: 6c30 b6a3 6aed edcd a706 2f2c 1fce e80f  l0..j...../,....
+00001410: 8ba4 741f dfb7 9806 5279 a740 f235 5f8b  ..t.....Ry.@.5_.
+00001420: 007f 48ad cfca d80c 3d39 8ba1 a6d2 199c  ..H.....=9......
+00001430: 7d53 d0a8 d9db bbde 5f19 9766 f639 da10  }S......_..f.9..
+00001440: 0b65 e51f 707b 4508 b13f 128a a6b0 f149  .e..p{E..?.....I
+00001450: 179c 0268 5fc8 bd9a b9bb 44cf 7942 fd60  ...h_.....D.yB.`
+00001460: 8776 2109 f6df 4c65 3976 abee 7637 c96b  .v!...Le9v..v7.k
+00001470: 7e4d 0abb acc5 4b75 4420 6b12 c2cb 6c8b  ~M....KuD k...l.
+00001480: 29d4 471b f037 7460 748b b55d 6894 6892  ).G..7t`t..]h.h.
+00001490: 762f 9d84 106d bd8b 249b 9a2e c36b a0e8  v/...m..$....k..
+000014a0: 6e30 f68b d617 c36b e1bc 2af7 87d7 5e1c  n0.....k..*...^.
+000014b0: bbd2 50fb 75bd 73c5 73bc 043b 7acd 2044  ..P.u.s.s..;z. D
+000014c0: 7b10 466c 931b 5d90 bd64 1895 1704 548b  {.Fl..]..d....T.
+000014d0: dead d154 1942 990c b1ce 8bbe f7b2 c4ab  ...T.B..........
+000014e0: 9239 4194 00b6 bbe0 6dfe cf5c 41df d323  .9A.....m..\A..#
+000014f0: b40c d42c dfe1 38e9 cded 0ee1 a50b 6733  ...,..8.......g3
+00001500: 456a 7d64 887b 7296 5182 3d92 ad18 58b1  Ej}d.{r.Q.=...X.
+00001510: 54ac ca7f e083 4d05 fecc 6f9c 681a 25be  T.....M...o.h.%.
+00001520: 788a 190a 02da 3314 889a d413 4e2f fb4b  x.....3.....N/.K
+00001530: d609 acfc d98a 7103 2a41 e95d e304 2ac1  ......q.*A.]..*.
+00001540: 6f87 823e 8bf9 5c04 3742 f51b 2794 0715  o..>..\.7B..'...
+00001550: b511 7670 7326 c42b 37a5 bcaa 284d 89f8  ..vps&.+7...(M..
+00001560: ede3 68fc 097f 40a4 35a1 55ca c0a4 d843  ..h...@.5.U....C
+00001570: d2c3 acf7 0bfd 35aa 4ef6 4210 5547 8d7c  ......5.N.B.UG.|
+00001580: b2df c866 30a4 609e 704a 9349 7911 2cae  ...f0.`.pJ.Iy.,.
+00001590: f2f6 4150 4459 a12d f235 4b6f 425d c1ff  ..APDY.-.5KoB]..
+000015a0: 72b7 fd00 6482 c064 1207 d665 8793 751b  r...d..d...e..u.
+000015b0: eae2 fbe4 a9fb c0f3 3147 ccb5 3976 d027  ........1G..9v.'
+000015c0: 843a de4c 061a fcc1 dc6b 48e4 7548 81ad  .:.L.....kH.uH..
+000015d0: 8afc 6dd4 8ca8 a29b cb0b 8178 9113 45b1  ..m........x..E.
+000015e0: 4a60 715b b35a fe96 8845 1696 75a8 4ece  J`q[.Z...E..u.N.
+000015f0: 5115 3fdf 6404 5203 3577 22ac 3e5a 8543  Q.?.d.R.5w".>Z.C
+00001600: bb16 ecbe 5875 3b0d 7aa6 2815 53fb 4de7  ....Xu;.z.(.S.M.
+00001610: 433d de81 58f5 530e 832c 8ae7 9496 0c9d  C=..X.S..,......
+00001620: 920e 3d91 7b10 8d88 a4c7 fc6b 9708 c79f  ..=.{......k....
+00001630: 10c9 8dfc 3475 29f6 54e4 aa73 256d 34a2  ....4u).T..s%m4.
+00001640: 69eb 36ad 28f8 dd7b 9dcf 252f 2606 122c  i.6.(..{..%/&..,
+00001650: 1ee2 6ec4 b12f b98b 8491 49e7 0782 5a56  ..n../....I...ZV
+00001660: 8afd 0c62 226c 82c2 2e62 85b8 c044 5ce2  ...b"l...b...D\.
+00001670: 1440 799a ec50 3d4a 134a 1d10 b520 460c  .@y..P=J.J... F.
+00001680: d98a c8f7 fc51 da4b 8d2e dbb2 a7cf 2ccd  .....Q.K......,.
+00001690: 18d6 83ed 9cac 4d95 c3c6 cc4b c1d0 03ba  ......M....K....
+000016a0: fcef 1b89 580b ff2a d126 658f 1199 c4cc  ....X..*.&e.....
+000016b0: 67be e3ac bfdd c1ba f5c3 9795 0e89 a151  g..............Q
+000016c0: d4eb 75e1 49af b46b fb33 5536 c38b f41a  ..u.I..k.3U6....
+000016d0: 5e4b b797 b348 c4f7 aee3 f090 7446 693b  ^K...H......tFi;
+000016e0: fafb 6089 59b8 1d88 513f 34e6 68db 19cb  ..`.Y...Q?4.h...
+000016f0: d99f 9988 4d19 d02f 4cfb d213 b84f 9f11  ....M../L....O..
+00001700: 7ebc 9cb7 5a59 bfe2 7841 b958 2f63 bfbe  ~...ZY..xA.X/c..
+00001710: 69a4 d5e2 4dc7 f16d 1658 7be4 ed14 8cb3  i...M..m.X{.....
+00001720: 4fd7 782a 5060 5237 31dc 830e 71d7 9ef4  O.x*P`R71...q...
+00001730: 8547 ac3c ae00 0000 584d 5020 c403 0000  .G.<....XMP ....
+00001740: 3c78 3a78 6d70 6d65 7461 2078 6d6c 6e73  <x:xmpmeta xmlns
+00001750: 3a78 3d22 6164 6f62 653a 6e73 3a6d 6574  :x="adobe:ns:met
+00001760: 612f 2220 783a 786d 7074 6b3d 2258 4d50  a/" x:xmptk="XMP
+00001770: 2043 6f72 6520 362e 302e 3022 3e0a 2020   Core 6.0.0">.  
+00001780: 203c 7264 663a 5244 4620 786d 6c6e 733a   <rdf:RDF xmlns:
+00001790: 7264 663d 2268 7474 703a 2f2f 7777 772e  rdf="http://www.
+000017a0: 7733 2e6f 7267 2f31 3939 392f 3032 2f32  w3.org/1999/02/2
+000017b0: 322d 7264 662d 7379 6e74 6178 2d6e 7323  2-rdf-syntax-ns#
+000017c0: 223e 0a20 2020 2020 203c 7264 663a 4465  ">.      <rdf:De
+000017d0: 7363 7269 7074 696f 6e20 7264 663a 6162  scription rdf:ab
+000017e0: 6f75 743d 2222 0a20 2020 2020 2020 2020  out="".         
+000017f0: 2020 2078 6d6c 6e73 3a65 7869 663d 2268     xmlns:exif="h
+00001800: 7474 703a 2f2f 6e73 2e61 646f 6265 2e63  ttp://ns.adobe.c
+00001810: 6f6d 2f65 7869 662f 312e 302f 220a 2020  om/exif/1.0/".  
+00001820: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
+00001830: 7469 6666 3d22 6874 7470 3a2f 2f6e 732e  tiff="http://ns.
+00001840: 6164 6f62 652e 636f 6d2f 7469 6666 2f31  adobe.com/tiff/1
+00001850: 2e30 2f22 0a20 2020 2020 2020 2020 2020  .0/".           
+00001860: 2078 6d6c 6e73 3a78 6d70 3d22 6874 7470   xmlns:xmp="http
+00001870: 3a2f 2f6e 732e 6164 6f62 652e 636f 6d2f  ://ns.adobe.com/
+00001880: 7861 702f 312e 302f 223e 0a20 2020 2020  xap/1.0/">.     
+00001890: 2020 2020 3c65 7869 663a 5069 7865 6c59      <exif:PixelY
+000018a0: 4469 6d65 6e73 696f 6e3e 3739 3c2f 6578  Dimension>79</ex
+000018b0: 6966 3a50 6978 656c 5944 696d 656e 7369  if:PixelYDimensi
+000018c0: 6f6e 3e0a 2020 2020 2020 2020 203c 6578  on>.         <ex
+000018d0: 6966 3a50 6978 656c 5844 696d 656e 7369  if:PixelXDimensi
+000018e0: 6f6e 3e39 303c 2f65 7869 663a 5069 7865  on>90</exif:Pixe
+000018f0: 6c58 4469 6d65 6e73 696f 6e3e 0a20 2020  lXDimension>.   
+00001900: 2020 2020 2020 3c65 7869 663a 436f 6c6f        <exif:Colo
+00001910: 7253 7061 6365 3e31 3c2f 6578 6966 3a43  rSpace>1</exif:C
+00001920: 6f6c 6f72 5370 6163 653e 0a20 2020 2020  olorSpace>.     
+00001930: 2020 2020 3c74 6966 663a 5852 6573 6f6c      <tiff:XResol
+00001940: 7574 696f 6e3e 3231 3630 3030 302f 3130  ution>2160000/10
+00001950: 3030 303c 2f74 6966 663a 5852 6573 6f6c  000</tiff:XResol
+00001960: 7574 696f 6e3e 0a20 2020 2020 2020 2020  ution>.         
+00001970: 3c74 6966 663a 5265 736f 6c75 7469 6f6e  <tiff:Resolution
+00001980: 556e 6974 3e32 3c2f 7469 6666 3a52 6573  Unit>2</tiff:Res
+00001990: 6f6c 7574 696f 6e55 6e69 743e 0a20 2020  olutionUnit>.   
+000019a0: 2020 2020 2020 3c74 6966 663a 4f72 6965        <tiff:Orie
+000019b0: 6e74 6174 696f 6e3e 313c 2f74 6966 663a  ntation>1</tiff:
+000019c0: 4f72 6965 6e74 6174 696f 6e3e 0a20 2020  Orientation>.   
+000019d0: 2020 2020 2020 3c74 6966 663a 5952 6573        <tiff:YRes
+000019e0: 6f6c 7574 696f 6e3e 3231 3630 3030 302f  olution>2160000/
+000019f0: 3130 3030 303c 2f74 6966 663a 5952 6573  10000</tiff:YRes
+00001a00: 6f6c 7574 696f 6e3e 0a20 2020 2020 2020  olution>.       
+00001a10: 2020 3c78 6d70 3a4d 6574 6164 6174 6144    <xmp:MetadataD
+00001a20: 6174 653e 3230 3234 2d30 342d 3037 5432  ate>2024-04-07T2
+00001a30: 313a 3432 3a31 372b 3038 3a30 303c 2f78  1:42:17+08:00</x
+00001a40: 6d70 3a4d 6574 6164 6174 6144 6174 653e  mp:MetadataDate>
+00001a50: 0a20 2020 2020 2020 2020 3c78 6d70 3a43  .         <xmp:C
+00001a60: 7265 6174 6f72 546f 6f6c 3e50 6978 656c  reatorTool>Pixel
+00001a70: 6d61 746f 7220 5072 6f20 332e 352e 373c  mator Pro 3.5.7<
+00001a80: 2f78 6d70 3a43 7265 6174 6f72 546f 6f6c  /xmp:CreatorTool
+00001a90: 3e0a 2020 2020 2020 2020 203c 786d 703a  >.         <xmp:
+00001aa0: 4372 6561 7465 4461 7465 3e32 3032 342d  CreateDate>2024-
+00001ab0: 3033 2d33 3054 3137 3a32 383a 3339 3c2f  03-30T17:28:39</
+00001ac0: 786d 703a 4372 6561 7465 4461 7465 3e0a  xmp:CreateDate>.
+00001ad0: 2020 2020 2020 3c2f 7264 663a 4465 7363        </rdf:Desc
+00001ae0: 7269 7074 696f 6e3e 0a20 2020 3c2f 7264  ription>.   </rd
+00001af0: 663a 5244 463e 0a3c 2f78 3a78 6d70 6d65  f:RDF>.</x:xmpme
+00001b00: 7461 3e0a                                ta>.
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter1.webp` & `SightTraining-0.1.20/spacedefense/assets/images/my_slave_fighter1.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter2.webp` & `SightTraining-0.1.20/spacedefense/assets/images/my_slave_fighter2.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/myf_master/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/myf_master/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_001.webp` & `SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_002.webp` & `SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_003.webp` & `SightTraining-0.1.20/spacedefense/assets/images/myf_master/myf_master_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_004.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-00000000: 5249 4646 fc1a 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
-00000010: 0a00 0000 3400 0000 5900 004e 0000 4943  ....4...Y..N..IC
+00000000: 5249 4646 2416 0000 5745 4250 5650 3858  RIFF$...WEBPVP8X
+00000010: 0a00 0000 3400 0000 4f00 002c 0000 4943  ....4...O..,..IC
 00000020: 4350 480c 0000 0000 0c48 4c69 6e6f 0210  CPH......HLino..
 00000030: 0000 6d6e 7472 5247 4220 5859 5a20 07ce  ..mntrRGB XYZ ..
 00000040: 0002 0009 0006 0031 0000 6163 7370 4d53  .......1..acspMS
 00000050: 4654 0000 0000 4945 4320 7352 4742 0000  FT....IEC sRGB..
 00000060: 0000 0000 0000 0000 0000 0000 f6d6 0001  ................
 00000070: 0000 0000 d32d 4850 2020 0000 0000 0000  .....-HP  ......
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -193,241 +193,163 @@
 00000c00: e253 e2db e363 e3eb e473 e4fc e584 e60d  .S...c...s......
 00000c10: e696 e71f e7a9 e832 e8bc e946 e9d0 ea5b  .......2...F...[
 00000c20: eae5 eb70 ebfb ec86 ed11 ed9c ee28 eeb4  ...p.........(..
 00000c30: ef40 efcc f058 f0e5 f172 f1ff f28c f319  .@...X...r......
 00000c40: f3a7 f434 f4c2 f550 f5de f66d f6fb f78a  ...4...P...m....
 00000c50: f819 f8a8 f938 f9c7 fa57 fae7 fb77 fc07  .....8...W...w..
 00000c60: fc98 fd29 fdba fe4b fedc ff6d ffff 414c  ...)...K...m..AL
-00000c70: 5048 0205 0000 01a0 766d db31 b79e d3fd  PH......vm.1....
-00000c80: bcf3 ce64 6227 bb8d b3ca a8b6 6ddb b66d  ...db'......m..m
-00000c90: dbb6 6ddb b6bb 6bbb 4d1a 371a bccf fd21  ..m...k.M.7....!
-00000ca0: afe7 8988 0900 3d73 b179 80d5 e51f 6df5  ......=s.y....m.
-00000cb0: 6394 df49 216b 8c81 4d6d 9290 3e8a 6092  c..I!k..Mm..>.`.
-00000cc0: eb4e 0131 bd13 930a bf47 4461 bb99 458d  .N.1.....GDa..E.
-00000cd0: d310 11ef e465 1099 68cb 155f 8e41 4e07  .....e..h.._.AN.
-00000ce0: 30b7 b533 83fc 1e8a d059 843d 513f 4470  0..3.....Y.=Q?Dp
-00000cf0: 9f89 3d75 32c4 eefa b0a7 bf5d ec53 2473  ..=u2......].S$s
-00000d00: b865 542c ad0a 73dc cea3 b8ad 2f73 0a7c  .eT,..s...../s.|
-00000d10: 96a0 9b78 d6b4 c996 c067 7919 63de 4ea5  ...x.....gy.c.N.
-00000d20: 325a 30a6 5a3c 4ad3 b37e 4c09 3c43 6560  2Z0.Z<J..~L.<Ce`
-00000d30: f628 2343 cc73 2c28 fb67 7dc2 0cbe 570a  .(#C.s,(.g}...W.
-00000d40: 2a7c 5694 11c4 a3ee 3754 2a9c 8934 3180  *|V.....7T*..41.
-00000d50: 0474 3dfb 992a 42eb d335 a54c 0ec6 05f5  .t=..*B..5.L....
-00000d60: b999 85ea 0a3f d696 333b 1089 18f9 2807  .....?..3;....(.
-00000d70: d5a7 bfb7 d470 7618 f703 1654 df66 43a4  .....pv....T.fC.
-00000d80: f11d 1dc6 a9d1 ec43 0f9f ee4c 53e7 d8fc  .......C...LS...
-00000d90: 57d7 b78d 8c52 8310 5d00 1027 bfa0 e6ff  W....R..]..'....
-00000da0: d479 902f d893 0755 09af 1300 703b 48d5  .y./...U....p;H.
-00000db0: c9e9 4740 6d33 51c2 13d5 6a26 a1ca b703  ..G@m3Q...j&....
-00000dc0: 5573 312a e0cc a0b6 f376 aa56 667b d5cc  Us1*.....v.Vf{..
-00000dd0: 9e0a 9c5d d432 37fc 83aa 9f0b 262a 19c2  ...].27.....&*..
-00000de0: 3879 ff39 a9e3 5e73 cb6f aa9e f5ee 9070  8y.9..^s.o.....p
-00000df0: 832a 10e9 218b cfc7 a940 025a 1d4b a2a8  .*..!....@.Z.K..
-00000e00: a9e5 c5cc e266 3502 2265 7987 8224 91e0  .....f5."ey..$..
-00000e10: c2fa ddce 40ed ed3f 3655 7655 662e 6d90  ....@..?6UvUf.m.
-00000e20: 93cf 474a 94b8 579a fcdc 82fa a47f 0fb5  ..GJ..W.........
-00000e30: f057 424a 79cb e04b 1be5 992b ecfc 6d47  .WBJy..K...+..mG
-00000e40: 1d67 5eee e44f 6441 64b4 0cbf e220 d7bd  .g^..OdAd.... ..
-00000e50: d6d6 9f02 ea3c f3c6 8070 831c b75a 0609  .....<...p...Z..
-00000e60: a75a 6152 c4af cd89 648a 0e68 f97f 4a94  .ZaR....d..h..J.
-00000e70: 518a b428 4144 48db 8d2e 625c 489f 6b19  Q..(ADH...b\H.k.
-00000e80: e8a8 f68f 2b2a ba8a 4185 9311 222e fb17  ....+*..A..."...
-00000e90: 935c c6a8 094f 72d0 9185 8403 2dfc 49ae  .\...Or.....-.I.
-00000ea0: 9067 dd44 4a7d ee0d 00e6 32cb 3eda d0d1  .g.DJ}....2.>...
-00000eb0: 69c6 8d7e a11c 80fb f9a3 6e00 c02f f812  i..~......n../..
-00000ec0: 0d6e 35b7 fd16 9089 9667 13a3 8c64 dc9f  .n5......g...d..
-00000ed0: 8a00 10f1 ea44 50b3 23c9 1499 69fb b4a2  .....DP.#...i...
-00000ee0: 5cb5 84a5 3c40 f79c 6d7b d229 3255 f8b3  \...<@..m{.)2U..
-00000ef0: f6f3 db7c e076 0293 3290 b956 bb75 0029  ...|.v..2..V.u.)
-00000f00: 9760 dfb8 833d 8878 d16b bef0 a9cc 2926  .`...=.x.k....)&
-00000f10: a5d4 bc99 f5f7 502a 9312 c6c7 3e46 360b  ......P*....>F6.
-00000f20: 53ab e4fb c828 ba21 6fe0 8223 5f72 2863  S....(.!o..#_r(c
-00000f30: a82d e9e6 ce0e 46e0 9da3 5acd 3fff 2943  .-....F...Z.?.)C
-00000f40: 6004 b5c6 dfdb d8bb 9cbf 9180 28e7 96af  `...........(...
-00000f50: e1d4 93ef 3304 7994 ea8e 5ae3 efac ee52  ....3.y...Z....R
-00000f60: dc97 07a5 c425 a2fe c4c3 affe 0952 42ba  .....%.......RB.
-00000f70: 5d4f d41a 7f7f 638f 923e 0650 9b98 831b  ]O....c..>.P....
-00000f80: 8fdc f33c c59e 0bd3 bf09 5ad9 5368 2e6a  ...<......Z.Sh.j
-00000f90: fb71 6d69 b732 7e3c 686e ca53 75e4 f607  .qmi.2~<hn.Su...
-00000fa0: 7f2c f45c dbf7 1a59 f774 4c14 323e 9c5d  .,.\...Y.tL.2>.]
-00000fb0: 3428 ce93 03dd f2be 716d 17b6 33d4 f9a6  4(......qm..3...
-00000fc0: 897d 47a0 d79c 09b5 c25d 08e8 9e33 40d8  .}G......]...3@.
-00000fd0: 434d aca3 cdc0 1370 4c63 e5d3 564d 3069  CM.....pLc..VM0i
-00000fe0: 5e28 0187 2421 337e 50d4 d87a a7b9 8b23  ^(..$!3~P..z...#
-00000ff0: b8b7 b96b 451d 26af 8be2 f4c6 97da 9586  ...kE.&.........
-00001000: fa14 5ef5 f1d6 1509 9af8 4540 dd66 1ead  ..^.......E@.f..
-00001010: 6cd4 8f6b b31b 16d4 33fd 3933 8ce8 c350  l..k....3.93...P
-00001020: 6c4b 0aca b5dc b2a8 9449 a510 adf7 dbb9  lK.......I......
-00001030: eb21 70cc 4701 657f 6ffe 559d af1b b2e4  .!p.G.e.o.U.....
-00001040: 20a6 ef29 c36b 65aa 7bd5 820a 2f87 5c94   ..).ke.{.../.\.
-00001050: b2a6 a451 09db b8e2 f1f2 907e 9f16 4434  ...Q.......~..D4
-00001060: 318d 8ba7 a874 8769 984d e24a a5f6 4912  1....t.i.M.J..I.
-00001070: 7f4a 467e 5280 68bd 5e42 93f0 b7a8 982e  .JF~R.h.^B......
-00001080: 2251 1fc4 e832 2ee8 a518 dde1 9ae7 7f45  "Q...2.........E
-00001090: 28cc e7b4 6898 a12c a73f f073 0411 5b7f  (...h..,.?.s..[.
-000010a0: 703d 2996 5415 3ccf 5145 78c3 5b03 6e3e  p=).T.<.QEx.[.n>
-000010b0: 5564 d91a 0050 eeaf c88b 5820 7d32 45ce  Ud...P....X }2E.
-000010c0: 7b02 a9f6 822a 4a28 a581 f775 549a bdda  {....*J(...uT...
-000010d0: 1f00 dc77 d810 3167 3407 e073 4140 c484  ...w..1g4..sA@..
-000010e0: 8e04 8054 7e4a 95d8 8769 10f4 4249 d632  ...T~J...i..BI.2
-000010f0: 1fc8 1d3c f7c9 c73b 6303 0180 94dc fcf2  ...<...;c.......
-00001100: c3d9 e626 0000 52e6 3e55 20cc 27ea 19a7  ...&..R.>U .'...
-00001110: 65ca cb98 eb09 e27c 60a4 2f07 a24e c111  e......|`./..N..
-00001120: 1e04 4449 b19b 822c fabe 1c68 e8d5 67ef  ..DI...,...h..g.
-00001130: 8b34 bb44 da64 37d0 9ac4 5c16 c4a8 e5d7  .4.D.d7...\.....
-00001140: d5c5 950d 5a00 9882 aa8d 3cf0 22d9 8698  ....Z.....<."...
-00001150: 32c6 0574 58f0 9c1d 69f6 f7ab cbdb c779  2..tX...i......y
-00001160: 72a0 43a7 a0f2 7d77 1c68 6f06 5d46 2e38  r.C...}w.ho.]F.8
-00001170: beac 5594 2707 6a02 5650 3820 b805 0000  ..U.'.j.VP8 ....
-00001180: 901b 009d 012a 5a00 4f00 3e9d 4099 4925  .....*Z.O.>.@.I%
-00001190: a3a2 212e f80b 00b0 1389 6900 15e0 1fca  ..!.......i.....
-000011a0: 3f0b fbf1 feef e11f 88ef 6e67 0589 bad2  ?.........ng....
-000011b0: 7e10 fdf7 093f 0f75 0276 bda0 566b 6a59  ~....?.u.v..VkjY
-000011c0: 2746 52be 33d0 bb9f cfaf 3d81 ff5d facc  'FR.3.....=..]..
-000011d0: f933 36b0 d77a a0d9 df23 a83c 60b0 f2be  .36..z...#.<`...
-000011e0: 5822 99fc fe6e b688 382d fce4 d67e b9b8  X"...n..8-...~..
-000011f0: 2dd9 12a1 e746 03ef e60a c98e db63 165f  -....F.......c._
-00001200: cdf0 8eeb 60a2 cf61 bdff 7edf 7f17 4a20  ....`..a..~...J 
-00001210: fbde 70cf 9c99 2ced cf40 df3f 65b8 f332  ..p...,..@.?e..2
-00001220: 3d71 87ba 8bf4 88b3 ebe0 37f7 ca06 d8a8  =q........7.....
-00001230: b95b 6399 d08c 1139 6b8c f1c4 f861 04f7  .[c....9k....a..
-00001240: 0dfe 0b02 aa74 811f 8e9f 5d46 b088 7e95  .....t....]F..~.
-00001250: 301d 654c 5587 0c8a 970c 015e 2f7d d777  0.eLU......^/}.w
-00001260: 7b22 e7fb 8000 fefd 3694 5149 0a41 f02d  {"......6.QI.A.-
-00001270: c980 832b c033 02db 4197 f478 9332 c9fa  ...+.3..A..x.2..
-00001280: a229 a47c d272 fb48 cb26 5f2e 0c06 55e8  .).|.r.H.&_...U.
-00001290: cb89 2027 3fba 1d80 07ea ae27 d546 135d  .. '?......'.F.]
-000012a0: a07f 913e fa54 102a a413 1793 b421 6c2b  ...>.T.*.....!l+
-000012b0: 85b8 1be8 8e35 0d0a 018f b280 7fa8 3219  .....5........2.
-000012c0: e8ca f3c2 64ce 3980 032c 7ede 2df0 bfe3  ....d.9..,~.-...
-000012d0: 3fc1 6687 2a75 f02c cba4 ebd1 5977 c029  ?.f.*u.,....Yw.)
-000012e0: bd50 a142 1729 f4d5 1e3d 8fc9 52f1 749c  .P.B.)...=..R.t.
-000012f0: a255 bbea f4d6 74e0 05ab 1a71 1a0f 36d7  .U....t....q..6.
-00001300: fd85 1ff8 cc3e 5c03 e6ac 6786 c17a ec7d  .....>\...g..z.}
-00001310: 2a0b 8e77 6797 a895 6731 5864 ec45 8fc0  *..wg...g1Xd.E..
-00001320: 74fc 7627 2035 4949 dcde e3f2 6c94 e87e  t.v' 5II....l..~
-00001330: c65d 18d6 c35b d9e8 fb2c ca05 ec3b 9fe0  .]...[...,...;..
-00001340: 7431 0598 300c aa87 d735 00c6 2bb1 ee6b  t1..0....5..+..k
-00001350: 397b 295c 9f9e aabf 8b26 e13b 3ad3 4ea3  9{)\.....&.;:.N.
-00001360: 285e 7edf e2a5 32e9 a6c7 db6a de04 ec40  (^~...2....j...@
-00001370: d3f5 d7df eb42 e5c1 3504 3b52 2256 ec74  .....B..5.;R"V.t
-00001380: c4e6 c8b4 80aa d8b2 7308 eb66 8ba1 8c9a  ........s..f....
-00001390: 0745 8679 f64c 023e 5a55 71c3 2dd4 7939  .E.y.L.>ZUq.-.y9
-000013a0: c9f9 1329 ef1a 78b8 f3c0 5df3 9def 618e  ...)..x...]...a.
-000013b0: 3cdc 27a9 912c 6748 05ab 3f93 7a72 d688  <.'..,gH..?.zr..
-000013c0: 210c 70f7 e66d 4164 d9ed e294 3007 7424  !.p..mAd....0.t$
-000013d0: e45e 8196 99a1 34e7 a97b d1c7 5316 5e27  .^....4..{..S.^'
-000013e0: 5b44 edec 2f5d f1bc 02a5 0e28 fb24 8384  [D../].....(.$..
-000013f0: 25a8 60f1 b04e 7af9 fc1a fe17 e1f6 0028  %.`..Nz........(
-00001400: 6c30 b6a3 6aed edcd a706 2f2c 1fce e80f  l0..j...../,....
-00001410: 8ba4 741f dfb7 9806 5279 a740 f235 5f8b  ..t.....Ry.@.5_.
-00001420: 007f 48ad cfca d80c 3d39 8ba1 a6d2 199c  ..H.....=9......
-00001430: 7d53 d0a8 d9db bbde 5f19 9766 f639 da10  }S......_..f.9..
-00001440: 0b65 e51f 707b 4508 b13f 128a a6b0 f149  .e..p{E..?.....I
-00001450: 179c 0268 5fc8 bd9a b9bb 44cf 7942 fd60  ...h_.....D.yB.`
-00001460: 8776 2109 f6df 4c65 3976 abee 7637 c96b  .v!...Le9v..v7.k
-00001470: 7e4d 0abb acc5 4b75 4420 6b12 c2cb 6c8b  ~M....KuD k...l.
-00001480: 29d4 471b f037 7460 748b b55d 6894 6892  ).G..7t`t..]h.h.
-00001490: 762f 9d84 106d bd8b 249b 9a2e c36b a0e8  v/...m..$....k..
-000014a0: 6e30 f68b d617 c36b e1bc 2af7 87d7 5e1c  n0.....k..*...^.
-000014b0: bbd2 50fb 75bd 73c5 73bc 043b 7acd 2044  ..P.u.s.s..;z. D
-000014c0: 7b10 466c 931b 5d90 bd64 1895 1704 548b  {.Fl..]..d....T.
-000014d0: dead d154 1942 990c b1ce 8bbe f7b2 c4ab  ...T.B..........
-000014e0: 9239 4194 00b6 bbe0 6dfe cf5c 41df d323  .9A.....m..\A..#
-000014f0: b40c d42c dfe1 38e9 cded 0ee1 a50b 6733  ...,..8.......g3
-00001500: 456a 7d64 887b 7296 5182 3d92 ad18 58b1  Ej}d.{r.Q.=...X.
-00001510: 54ac ca7f e083 4d05 fecc 6f9c 681a 25be  T.....M...o.h.%.
-00001520: 788a 190a 02da 3314 889a d413 4e2f fb4b  x.....3.....N/.K
-00001530: d609 acfc d98a 7103 2a41 e95d e304 2ac1  ......q.*A.]..*.
-00001540: 6f87 823e 8bf9 5c04 3742 f51b 2794 0715  o..>..\.7B..'...
-00001550: b511 7670 7326 c42b 37a5 bcaa 284d 89f8  ..vps&.+7...(M..
-00001560: ede3 68fc 097f 40a4 35a1 55ca c0a4 d843  ..h...@.5.U....C
-00001570: d2c3 acf7 0bfd 35aa 4ef6 4210 5547 8d7c  ......5.N.B.UG.|
-00001580: b2df c866 30a4 609e 704a 9349 7911 2cae  ...f0.`.pJ.Iy.,.
-00001590: f2f6 4150 4459 a12d f235 4b6f 425d c1ff  ..APDY.-.5KoB]..
-000015a0: 72b7 fd00 6482 c064 1207 d665 8793 751b  r...d..d...e..u.
-000015b0: eae2 fbe4 a9fb c0f3 3147 ccb5 3976 d027  ........1G..9v.'
-000015c0: 843a de4c 061a fcc1 dc6b 48e4 7548 81ad  .:.L.....kH.uH..
-000015d0: 8afc 6dd4 8ca8 a29b cb0b 8178 9113 45b1  ..m........x..E.
-000015e0: 4a60 715b b35a fe96 8845 1696 75a8 4ece  J`q[.Z...E..u.N.
-000015f0: 5115 3fdf 6404 5203 3577 22ac 3e5a 8543  Q.?.d.R.5w".>Z.C
-00001600: bb16 ecbe 5875 3b0d 7aa6 2815 53fb 4de7  ....Xu;.z.(.S.M.
-00001610: 433d de81 58f5 530e 832c 8ae7 9496 0c9d  C=..X.S..,......
-00001620: 920e 3d91 7b10 8d88 a4c7 fc6b 9708 c79f  ..=.{......k....
-00001630: 10c9 8dfc 3475 29f6 54e4 aa73 256d 34a2  ....4u).T..s%m4.
-00001640: 69eb 36ad 28f8 dd7b 9dcf 252f 2606 122c  i.6.(..{..%/&..,
-00001650: 1ee2 6ec4 b12f b98b 8491 49e7 0782 5a56  ..n../....I...ZV
-00001660: 8afd 0c62 226c 82c2 2e62 85b8 c044 5ce2  ...b"l...b...D\.
-00001670: 1440 799a ec50 3d4a 134a 1d10 b520 460c  .@y..P=J.J... F.
-00001680: d98a c8f7 fc51 da4b 8d2e dbb2 a7cf 2ccd  .....Q.K......,.
-00001690: 18d6 83ed 9cac 4d95 c3c6 cc4b c1d0 03ba  ......M....K....
-000016a0: fcef 1b89 580b ff2a d126 658f 1199 c4cc  ....X..*.&e.....
-000016b0: 67be e3ac bfdd c1ba f5c3 9795 0e89 a151  g..............Q
-000016c0: d4eb 75e1 49af b46b fb33 5536 c38b f41a  ..u.I..k.3U6....
-000016d0: 5e4b b797 b348 c4f7 aee3 f090 7446 693b  ^K...H......tFi;
-000016e0: fafb 6089 59b8 1d88 513f 34e6 68db 19cb  ..`.Y...Q?4.h...
-000016f0: d99f 9988 4d19 d02f 4cfb d213 b84f 9f11  ....M../L....O..
-00001700: 7ebc 9cb7 5a59 bfe2 7841 b958 2f63 bfbe  ~...ZY..xA.X/c..
-00001710: 69a4 d5e2 4dc7 f16d 1658 7be4 ed14 8cb3  i...M..m.X{.....
-00001720: 4fd7 782a 5060 5237 31dc 830e 71d7 9ef4  O.x*P`R71...q...
-00001730: 8547 ac3c ae00 0000 584d 5020 c403 0000  .G.<....XMP ....
-00001740: 3c78 3a78 6d70 6d65 7461 2078 6d6c 6e73  <x:xmpmeta xmlns
-00001750: 3a78 3d22 6164 6f62 653a 6e73 3a6d 6574  :x="adobe:ns:met
-00001760: 612f 2220 783a 786d 7074 6b3d 2258 4d50  a/" x:xmptk="XMP
-00001770: 2043 6f72 6520 362e 302e 3022 3e0a 2020   Core 6.0.0">.  
-00001780: 203c 7264 663a 5244 4620 786d 6c6e 733a   <rdf:RDF xmlns:
-00001790: 7264 663d 2268 7474 703a 2f2f 7777 772e  rdf="http://www.
-000017a0: 7733 2e6f 7267 2f31 3939 392f 3032 2f32  w3.org/1999/02/2
-000017b0: 322d 7264 662d 7379 6e74 6178 2d6e 7323  2-rdf-syntax-ns#
-000017c0: 223e 0a20 2020 2020 203c 7264 663a 4465  ">.      <rdf:De
-000017d0: 7363 7269 7074 696f 6e20 7264 663a 6162  scription rdf:ab
-000017e0: 6f75 743d 2222 0a20 2020 2020 2020 2020  out="".         
-000017f0: 2020 2078 6d6c 6e73 3a65 7869 663d 2268     xmlns:exif="h
-00001800: 7474 703a 2f2f 6e73 2e61 646f 6265 2e63  ttp://ns.adobe.c
-00001810: 6f6d 2f65 7869 662f 312e 302f 220a 2020  om/exif/1.0/".  
-00001820: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
-00001830: 7469 6666 3d22 6874 7470 3a2f 2f6e 732e  tiff="http://ns.
-00001840: 6164 6f62 652e 636f 6d2f 7469 6666 2f31  adobe.com/tiff/1
-00001850: 2e30 2f22 0a20 2020 2020 2020 2020 2020  .0/".           
-00001860: 2078 6d6c 6e73 3a78 6d70 3d22 6874 7470   xmlns:xmp="http
-00001870: 3a2f 2f6e 732e 6164 6f62 652e 636f 6d2f  ://ns.adobe.com/
-00001880: 7861 702f 312e 302f 223e 0a20 2020 2020  xap/1.0/">.     
-00001890: 2020 2020 3c65 7869 663a 5069 7865 6c59      <exif:PixelY
-000018a0: 4469 6d65 6e73 696f 6e3e 3739 3c2f 6578  Dimension>79</ex
-000018b0: 6966 3a50 6978 656c 5944 696d 656e 7369  if:PixelYDimensi
-000018c0: 6f6e 3e0a 2020 2020 2020 2020 203c 6578  on>.         <ex
-000018d0: 6966 3a50 6978 656c 5844 696d 656e 7369  if:PixelXDimensi
-000018e0: 6f6e 3e39 303c 2f65 7869 663a 5069 7865  on>90</exif:Pixe
-000018f0: 6c58 4469 6d65 6e73 696f 6e3e 0a20 2020  lXDimension>.   
-00001900: 2020 2020 2020 3c65 7869 663a 436f 6c6f        <exif:Colo
-00001910: 7253 7061 6365 3e31 3c2f 6578 6966 3a43  rSpace>1</exif:C
-00001920: 6f6c 6f72 5370 6163 653e 0a20 2020 2020  olorSpace>.     
-00001930: 2020 2020 3c74 6966 663a 5852 6573 6f6c      <tiff:XResol
-00001940: 7574 696f 6e3e 3231 3630 3030 302f 3130  ution>2160000/10
-00001950: 3030 303c 2f74 6966 663a 5852 6573 6f6c  000</tiff:XResol
-00001960: 7574 696f 6e3e 0a20 2020 2020 2020 2020  ution>.         
-00001970: 3c74 6966 663a 5265 736f 6c75 7469 6f6e  <tiff:Resolution
-00001980: 556e 6974 3e32 3c2f 7469 6666 3a52 6573  Unit>2</tiff:Res
-00001990: 6f6c 7574 696f 6e55 6e69 743e 0a20 2020  olutionUnit>.   
-000019a0: 2020 2020 2020 3c74 6966 663a 4f72 6965        <tiff:Orie
-000019b0: 6e74 6174 696f 6e3e 313c 2f74 6966 663a  ntation>1</tiff:
-000019c0: 4f72 6965 6e74 6174 696f 6e3e 0a20 2020  Orientation>.   
-000019d0: 2020 2020 2020 3c74 6966 663a 5952 6573        <tiff:YRes
-000019e0: 6f6c 7574 696f 6e3e 3231 3630 3030 302f  olution>2160000/
-000019f0: 3130 3030 303c 2f74 6966 663a 5952 6573  10000</tiff:YRes
-00001a00: 6f6c 7574 696f 6e3e 0a20 2020 2020 2020  olution>.       
-00001a10: 2020 3c78 6d70 3a4d 6574 6164 6174 6144    <xmp:MetadataD
-00001a20: 6174 653e 3230 3234 2d30 342d 3037 5432  ate>2024-04-07T2
-00001a30: 313a 3432 3a31 372b 3038 3a30 303c 2f78  1:42:17+08:00</x
-00001a40: 6d70 3a4d 6574 6164 6174 6144 6174 653e  mp:MetadataDate>
-00001a50: 0a20 2020 2020 2020 2020 3c78 6d70 3a43  .         <xmp:C
-00001a60: 7265 6174 6f72 546f 6f6c 3e50 6978 656c  reatorTool>Pixel
-00001a70: 6d61 746f 7220 5072 6f20 332e 352e 373c  mator Pro 3.5.7<
-00001a80: 2f78 6d70 3a43 7265 6174 6f72 546f 6f6c  /xmp:CreatorTool
-00001a90: 3e0a 2020 2020 2020 2020 203c 786d 703a  >.         <xmp:
-00001aa0: 4372 6561 7465 4461 7465 3e32 3032 342d  CreateDate>2024-
-00001ab0: 3033 2d33 3054 3137 3a32 383a 3339 3c2f  03-30T17:28:39</
-00001ac0: 786d 703a 4372 6561 7465 4461 7465 3e0a  xmp:CreateDate>.
-00001ad0: 2020 2020 2020 3c2f 7264 663a 4465 7363        </rdf:Desc
-00001ae0: 7269 7074 696f 6e3e 0a20 2020 3c2f 7264  ription>.   </rd
-00001af0: 663a 5244 463e 0a3c 2f78 3a78 6d70 6d65  f:RDF>.</x:xmpme
-00001b00: 7461 3e0a                                ta>.
+00000c70: 5048 2002 0000 0190 0400 6019 4949 bd67  PH .......`.II.g
+00000c80: dbb6 6dfb 5eb6 6ddb b66d dbb6 6ddb c6d8  ..m.^.m..m..m...
+00000c90: b345 4e45 92d5 3322 2600 c406 a194 3455  .ENE..3"&.....4U
+00000ca0: 964c a993 4a4c 94c0 a6ac 38fc f09d 07ef  .L..JL....8.....
+00000cb0: df3d bd7b 7c55 f712 c919 cae2 579c 71db  .=.{|U......W.q.
+00000cc0: a922 7dc5 7e63 505a 4891 5875 e32f 1599  ."}.~cPZH.Xu./..
+00000cd0: 0d5f 6997 9c16 9875 ae4d 4356 068f 56e6  ._i....u.MCV..V.
+00000ce0: a860 2add 5491 d55f 3a4b 1470 4dde 208c  .`*.T.._:K.pM. .
+00000cf0: ae69 4988 e35b 7f43 5843 e379 d21a fe40  .iI..[.CXC.y...@
+00000d00: 98ed 9d58 b232 5d43 d83f 5526 0926 5ba6  ...X.2]C.?U&.&[.
+00000d10: e243 17b3 11c3 64ee 7b3e 8808 544e b7c9  .C....d.{>..TN..
+00000d20: c8f2 99d2 f058 60ce 2e43 4b8f 7e22 2342  .....X`..CK.~"#B
+00000d30: c38f 572c 7bf5 685e 260c b0c2 3d45 fea5  ..W,{.h^&...=E..
+00000d40: 20c2 9513 f9a0 454c d63e 4f11 95da cd6a   .....EL.>O....j
+00000d50: 8225 c907 3f55 10ad dfa7 6682 a6d8 3207  .%..?U....f...2.
+00000d60: c288 62f9 6a3d de84 d8f1 03a2 fc6b 4fc1  ..b.j=.......kO.
+00000d70: 103f c086 a8ff d592 3152 fd07 8a02 5f95  .?......1R...._.
+00000d80: 3220 6c41 51a1 b63d 422f ebcb 2801 7dc9  2 lAQ..=B/..(.}.
+00000d90: af57 2f10 3544 b6d4 ebae 460d 6884 5e1b  .W/.5D....F.h.^.
+00000da0: 852e e56e f83f 6a1f bda2 1fe9 d27e c8ff  ...n.?j......~..
+00000db0: f956 5a4f 5c2c 53a5 abad 90f4 40a5 af51  .VZO\,S.....@..Q
+00000dc0: 81ad 1230 187f 9d4a 5fe4 2cd1 08c8 f1c0  ...0...J_.,.....
+00000dd0: 9cfa ca47 5678 734a 6018 36fe 6e4a bee6  ...GVxsJ`.6.nJ..
+00000de0: 26ca 3b2b 2530 c937 7ead 9930 fded a586  &.;+%0.7~..0....
+00000df0: e57b 8f08 609a 29b6 c583 e5c2 5c05 837a  .{..`.).....\..z
+00000e00: bb2e 07ac 4cd0 e888 4db3 4e09 21cb e567  ....L...M.N.!..g
+00000e10: 53b2 4360 71fc d2f3 3f68 5659 aeb9 cff7  S.C`q...?hVY....
+00000e20: cccc 008c 5ce1 c937 5c1a 39be dbd3 aa24  ....\..7\.9....$
+00000e30: 8500 339f aaca 987d 4f5d 2a3e d5f3 6873  ..3....}O]*>..hs
+00000e40: d3d4 0c20 128a e9ca f559 79f1 a35f b34a  ... .....Yy.._.J
+00000e50: 0efc 7cb8 a75f a5b4 3c20 9a49 98a3 f6e0  ..|.._..< .I....
+00000e60: 257b 2e3e fbf6 d366 b7bb 7c7e bfdf 6bff  %{.>...f..|~..k.
+00000e70: fcec cae1 7593 5a56 2f98 5200 7442 3e41  ....u.ZV/.R.tB>A
+00000e80: da3c 050b 172b 5aaa 52d5 ead5 2b16 cd99  .<...+Z.R...+...
+00000e90: 3691 c880 3846 5650 3820 ec03 0000 9014  6...8FVP8 ......
+00000ea0: 009d 012a 5000 2d00 3e99 3c99 4825 a322  ...*P.-.>.<.H%."
+00000eb0: a131 180c 90b0 1309 6c00 b953 c2c6 148e  .1......l..S....
+00000ec0: eadf db37 e44a 8583 3d4f fe59 f42b e987  ...7.J..=O.Y.+..
+00000ed0: e683 ee03 de77 d2d7 faef 4ece a3bd e59c  .....w....N.....
+00000ee0: 02bf e35d 8df7 b7e4 a01f c64b 72e8 37f7  ...].......Kr.7.
+00000ef0: 5afa a68b 6b2e cb40 76a4 7d8d 9a1f 53f2  Z...k..@v.}...S.
+00000f00: 7ed8 bc19 bbc0 bd11 947f cabc 8f5a a159  ~............Z.Y
+00000f10: a5f7 f9d5 6575 a4e9 2ee7 292e bea6 b925  ....eu....)....%
+00000f20: 6b2c 14bb 2215 effe 0385 08ed e243 9e4e  k,.."........C.N
+00000f30: 7c4c 3efc 89c5 45ee 780d e3c7 cd99 889e  |L>...E.x.......
+00000f40: 14cf 3544 719f 7ffe 7a49 0000 fee4 423f  ..5Dq...zI....B?
+00000f50: ff4a 176e d30f cd1c d2e7 087c 4e10 5b00  .J.n.......|N.[.
+00000f60: 5e67 ad9d 88da 2c84 ac2f fbdb ddf4 5b67  ^g....,../....[g
+00000f70: 804b bbec 12d8 447c 4a29 9dd6 d3b9 cfdd  .K....D|J)......
+00000f80: 04df 0f52 2e4d 3410 c76d 1abb f19f 0e05  ...R.M4..m......
+00000f90: fcdd 6471 0f63 c15c 33f2 9370 a711 ecc5  ..dq.c.\3..p....
+00000fa0: 28b3 1137 811f d1a2 6c96 16b3 3607 06bd  (..7....l...6...
+00000fb0: fd73 0d56 3969 20d5 8f46 962d b132 1c83  .s.V9i ..F.-.2..
+00000fc0: f022 fe97 9037 3e18 4587 e612 e6a6 1b12  ."...7>.E.......
+00000fd0: c137 e0ab cad4 b278 d6f4 ba65 8d9e ae21  .7.....x...e...!
+00000fe0: b0cd 203f f3da 3013 930d b64f 4184 39ff  .. ?..0....OA.9.
+00000ff0: 0090 8cbd a5b7 a027 5b65 9697 3d0b a401  .......'[e..=...
+00001000: 9063 0054 26f5 0b25 e3d1 c066 7514 8211  .c.T&..%...fu...
+00001010: c829 771d 7fd4 80a1 fb84 0b4b 4788 c7ef  .)w........KG...
+00001020: 9545 636f 4b2f 44e9 d000 4d8e fc12 fa39  .EcoK/D...M....9
+00001030: 3725 b92e 6db7 82e8 edc8 e375 1305 5230  7%..m......u..R0
+00001040: a4b4 2fb3 afb6 419e 6eb2 e50d 7f8d 1042  ../...A.n......B
+00001050: b53f 9db8 84eb 28dd 6354 0fc9 c198 0ae9  .?....(.cT......
+00001060: a37b 94b8 57c1 66e1 bc28 f780 8dab 00ca  .{..W.f..(......
+00001070: 341b 5955 1fb1 6e39 cccf d42f de25 6125  4.YU..n9.../.%a%
+00001080: 13ee dec3 70ac d680 f616 48b0 912a 327f  ....p.....H..*2.
+00001090: fe78 31d7 124f 3e52 ed65 0a03 7b28 6cb8  .x1..O>R.e..{(l.
+000010a0: b01f 2bde b598 431a 5bfe 2fb7 8f28 08c0  ..+...C.[./..(..
+000010b0: 64db e978 1a13 b729 7418 97ad dd03 92dd  d..x...)t.......
+000010c0: df04 4f21 6ce1 42fb 496a f4a7 a25f ae6d  ..O!l.B.Ij..._.m
+000010d0: 94d2 e037 05ec 406e 417c 650e 4caf 6b1b  ...7..@nA|e.L.k.
+000010e0: 9ce6 59a7 80dc d9fc 2721 2e07 6a1e ce49  ..Y.....'!..j..I
+000010f0: bea0 9582 85a3 49ff 8ba7 b0ba 1cd7 6f1b  ......I.......o.
+00001100: 9bfa 9a6c ad17 cdbb 7b20 a3f6 06ac ae9b  ...l....{ ......
+00001110: 833e 4518 6ec5 49f6 7fea 473f d357 65ae  .>E.n.I...G?.We.
+00001120: b714 adc8 3267 524e 8995 62a9 5ef4 444f  ....2gRN..b.^.DO
+00001130: 1321 3251 f378 ed69 6496 900c 54f6 58bc  .!2Q.x.id...T.X.
+00001140: 9d35 ea95 f8d9 38cf 955e 7dc9 011f 73ce  .5....8..^}...s.
+00001150: f681 8814 75c7 54ec 3d61 69d5 066e f52a  ....u.T.=ai..n.*
+00001160: 49ce 9639 1393 c28b a734 5233 d82c f187  I..9.....4R3.,..
+00001170: bf76 1154 6249 b2cc ef0f fb95 dd9e 12ce  .v.TbI..........
+00001180: d42d 9c10 a4a8 6f33 8dab 6ba2 ecfd f993  .-....o3..k.....
+00001190: e2ab ad0f 1fbf 447d 6bcd 9312 69e5 c030  ......D}k...i..0
+000011a0: cd62 b3a6 c759 8be3 c575 1eb8 b8e0 aa63  .b...Y...u.....c
+000011b0: ffbc c912 ae9b 7b96 9d24 3017 1b78 8c73  ......{..$0..x.s
+000011c0: 7e01 9bf3 b8c4 aea3 5e97 36d0 60ea a5cb  ~.......^.6.`...
+000011d0: 2afd d897 d219 9516 2da8 e168 8764 631f  *.......-..h.dc.
+000011e0: 01ca 9549 bc8a 49c9 c6f2 5652 7b4d e8f7  ...I..I...VR{M..
+000011f0: dc9d 37a0 b569 95f4 9593 e15b 2439 86b5  ..7..i.....[$9..
+00001200: b765 8fc8 d6d9 7304 f5e1 dec3 b5bb 6d7c  .e....s.......m|
+00001210: 4897 c984 8666 62c1 847e 984b 14bc ea94  H....fb..~.K....
+00001220: 449b cb8f 8449 a321 4787 581f 6c00 066b  D....I.!G.X.l..k
+00001230: 6fc3 f948 0c38 7712 a4c7 1250 5bb9 a954  o..H.8w....P[..T
+00001240: b379 7c96 943b 4653 9f13 4265 f126 5f77  .y|..;FS..Be.&_w
+00001250: 4b01 b676 db07 6b9f 99e0 73ff 5ae5 df4e  K..v..k...s.Z..N
+00001260: 3ccd 728c 23ad dce7 e9cf 2024 23e2 ea87  <.r.#..... $#...
+00001270: 38d1 5e57 047b ed66 3185 ea00 272b bb08  8.^W.{.f1...'+..
+00001280: 6963 8488 31f5 9000 0000 584d 5020 9a03  ic..1.....XMP ..
+00001290: 0000 3c78 3a78 6d70 6d65 7461 2078 6d6c  ..<x:xmpmeta xml
+000012a0: 6e73 3a78 3d22 6164 6f62 653a 6e73 3a6d  ns:x="adobe:ns:m
+000012b0: 6574 612f 2220 783a 786d 7074 6b3d 2258  eta/" x:xmptk="X
+000012c0: 4d50 2043 6f72 6520 362e 302e 3022 3e0a  MP Core 6.0.0">.
+000012d0: 2020 203c 7264 663a 5244 4620 786d 6c6e     <rdf:RDF xmln
+000012e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
+000012f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
+00001300: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
+00001310: 7323 223e 0a20 2020 2020 203c 7264 663a  s#">.      <rdf:
+00001320: 4465 7363 7269 7074 696f 6e20 7264 663a  Description rdf:
+00001330: 6162 6f75 743d 2222 0a20 2020 2020 2020  about="".       
+00001340: 2020 2020 2078 6d6c 6e73 3a65 7869 663d       xmlns:exif=
+00001350: 2268 7474 703a 2f2f 6e73 2e61 646f 6265  "http://ns.adobe
+00001360: 2e63 6f6d 2f65 7869 662f 312e 302f 220a  .com/exif/1.0/".
+00001370: 2020 2020 2020 2020 2020 2020 786d 6c6e              xmln
+00001380: 733a 7469 6666 3d22 6874 7470 3a2f 2f6e  s:tiff="http://n
+00001390: 732e 6164 6f62 652e 636f 6d2f 7469 6666  s.adobe.com/tiff
+000013a0: 2f31 2e30 2f22 0a20 2020 2020 2020 2020  /1.0/".         
+000013b0: 2020 2078 6d6c 6e73 3a78 6d70 3d22 6874     xmlns:xmp="ht
+000013c0: 7470 3a2f 2f6e 732e 6164 6f62 652e 636f  tp://ns.adobe.co
+000013d0: 6d2f 7861 702f 312e 302f 223e 0a20 2020  m/xap/1.0/">.   
+000013e0: 2020 2020 2020 3c65 7869 663a 5069 7865        <exif:Pixe
+000013f0: 6c59 4469 6d65 6e73 696f 6e3e 3435 3c2f  lYDimension>45</
+00001400: 6578 6966 3a50 6978 656c 5944 696d 656e  exif:PixelYDimen
+00001410: 7369 6f6e 3e0a 2020 2020 2020 2020 203c  sion>.         <
+00001420: 6578 6966 3a50 6978 656c 5844 696d 656e  exif:PixelXDimen
+00001430: 7369 6f6e 3e38 303c 2f65 7869 663a 5069  sion>80</exif:Pi
+00001440: 7865 6c58 4469 6d65 6e73 696f 6e3e 0a20  xelXDimension>. 
+00001450: 2020 2020 2020 2020 3c74 6966 663a 5265          <tiff:Re
+00001460: 736f 6c75 7469 6f6e 556e 6974 3e32 3c2f  solutionUnit>2</
+00001470: 7469 6666 3a52 6573 6f6c 7574 696f 6e55  tiff:ResolutionU
+00001480: 6e69 743e 0a20 2020 2020 2020 2020 3c74  nit>.         <t
+00001490: 6966 663a 5852 6573 6f6c 7574 696f 6e3e  iff:XResolution>
+000014a0: 3732 3030 3030 2f31 3030 3030 3c2f 7469  720000/10000</ti
+000014b0: 6666 3a58 5265 736f 6c75 7469 6f6e 3e0a  ff:XResolution>.
+000014c0: 2020 2020 2020 2020 203c 7469 6666 3a4f           <tiff:O
+000014d0: 7269 656e 7461 7469 6f6e 3e31 3c2f 7469  rientation>1</ti
+000014e0: 6666 3a4f 7269 656e 7461 7469 6f6e 3e0a  ff:Orientation>.
+000014f0: 2020 2020 2020 2020 203c 7469 6666 3a59           <tiff:Y
+00001500: 5265 736f 6c75 7469 6f6e 3e37 3230 3030  Resolution>72000
+00001510: 302f 3130 3030 303c 2f74 6966 663a 5952  0/10000</tiff:YR
+00001520: 6573 6f6c 7574 696f 6e3e 0a20 2020 2020  esolution>.     
+00001530: 2020 2020 3c78 6d70 3a4d 6574 6164 6174      <xmp:Metadat
+00001540: 6144 6174 653e 3230 3234 2d30 342d 3037  aDate>2024-04-07
+00001550: 5432 313a 3532 3a32 302b 3038 3a30 303c  T21:52:20+08:00<
+00001560: 2f78 6d70 3a4d 6574 6164 6174 6144 6174  /xmp:MetadataDat
+00001570: 653e 0a20 2020 2020 2020 2020 3c78 6d70  e>.         <xmp
+00001580: 3a43 7265 6174 6f72 546f 6f6c 3e50 6978  :CreatorTool>Pix
+00001590: 656c 6d61 746f 7220 5072 6f20 332e 352e  elmator Pro 3.5.
+000015a0: 373c 2f78 6d70 3a43 7265 6174 6f72 546f  7</xmp:CreatorTo
+000015b0: 6f6c 3e0a 2020 2020 2020 2020 203c 786d  ol>.         <xm
+000015c0: 703a 4372 6561 7465 4461 7465 3e32 3032  p:CreateDate>202
+000015d0: 342d 3034 2d30 3154 3133 3a33 323a 3339  4-04-01T13:32:39
+000015e0: 2b30 383a 3030 3c2f 786d 703a 4372 6561  +08:00</xmp:Crea
+000015f0: 7465 4461 7465 3e0a 2020 2020 2020 3c2f  teDate>.      </
+00001600: 7264 663a 4465 7363 7269 7074 696f 6e3e  rdf:Description>
+00001610: 0a20 2020 3c2f 7264 663a 5244 463e 0a3c  .   </rdf:RDF>.<
+00001620: 2f78 3a78 6d70 6d65 7461 3e0a            /x:xmpmeta>.
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/scale_cambg1.webp` & `SightTraining-0.1.20/spacedefense/assets/images/scale_cambg1.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/super_bullet.webp` & `SightTraining-0.1.20/spacedefense/assets/images/super_bullet.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_master/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_master/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_001.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_002.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_003.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_004.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_master/ufo_master_004.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 5249 4646 2416 0000 5745 4250 5650 3858  RIFF$...WEBPVP8X
+00000000: 5249 4646 a216 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
 00000010: 0a00 0000 3400 0000 4f00 002c 0000 4943  ....4...O..,..IC
 00000020: 4350 480c 0000 0000 0c48 4c69 6e6f 0210  CPH......HLino..
 00000030: 0000 6d6e 7472 5247 4220 5859 5a20 07ce  ..mntrRGB XYZ ..
 00000040: 0002 0009 0006 0031 0000 6163 7370 4d53  .......1..acspMS
 00000050: 4654 0000 0000 4945 4320 7352 4742 0000  FT....IEC sRGB..
 00000060: 0000 0000 0000 0000 0000 0000 f6d6 0001  ................
 00000070: 0000 0000 d32d 4850 2020 0000 0000 0000  .....-HP  ......
@@ -193,163 +193,171 @@
 00000c00: e253 e2db e363 e3eb e473 e4fc e584 e60d  .S...c...s......
 00000c10: e696 e71f e7a9 e832 e8bc e946 e9d0 ea5b  .......2...F...[
 00000c20: eae5 eb70 ebfb ec86 ed11 ed9c ee28 eeb4  ...p.........(..
 00000c30: ef40 efcc f058 f0e5 f172 f1ff f28c f319  .@...X...r......
 00000c40: f3a7 f434 f4c2 f550 f5de f66d f6fb f78a  ...4...P...m....
 00000c50: f819 f8a8 f938 f9c7 fa57 fae7 fb77 fc07  .....8...W...w..
 00000c60: fc98 fd29 fdba fe4b fedc ff6d ffff 414c  ...)...K...m..AL
-00000c70: 5048 2002 0000 0190 0400 6019 4949 bd67  PH .......`.II.g
-00000c80: dbb6 6dfb 5eb6 6ddb b66d dbb6 6ddb c6d8  ..m.^.m..m..m...
-00000c90: b345 4e45 92d5 3322 2600 c406 a194 3455  .ENE..3"&.....4U
-00000ca0: 964c a993 4a4c 94c0 a6ac 38fc f09d 07ef  .L..JL....8.....
-00000cb0: df3d bd7b 7c55 f712 c919 cae2 579c 71db  .=.{|U......W.q.
-00000cc0: a922 7dc5 7e63 505a 4891 5875 e32f 1599  ."}.~cPZH.Xu./..
-00000cd0: 0d5f 6997 9c16 9875 ae4d 4356 068f 56e6  ._i....u.MCV..V.
-00000ce0: a860 2add 5491 d55f 3a4b 1470 4dde 208c  .`*.T.._:K.pM. .
-00000cf0: ae69 4988 e35b 7f43 5843 e379 d21a fe40  .iI..[.CXC.y...@
-00000d00: 98ed 9d58 b232 5d43 d83f 5526 0926 5ba6  ...X.2]C.?U&.&[.
-00000d10: e243 17b3 11c3 64ee 7b3e 8808 544e b7c9  .C....d.{>..TN..
-00000d20: c8f2 99d2 f058 60ce 2e43 4b8f 7e22 2342  .....X`..CK.~"#B
-00000d30: c38f 572c 7bf5 685e 260c b0c2 3d45 fea5  ..W,{.h^&...=E..
-00000d40: 20c2 9513 f9a0 454c d63e 4f11 95da cd6a   .....EL.>O....j
-00000d50: 8225 c907 3f55 10ad dfa7 6682 a6d8 3207  .%..?U....f...2.
-00000d60: c288 62f9 6a3d de84 d8f1 03a2 fc6b 4fc1  ..b.j=.......kO.
-00000d70: 103f c086 a8ff d592 3152 fd07 8a02 5f95  .?......1R...._.
-00000d80: 3220 6c41 51a1 b63d 422f ebcb 2801 7dc9  2 lAQ..=B/..(.}.
-00000d90: af57 2f10 3544 b6d4 ebae 460d 6884 5e1b  .W/.5D....F.h.^.
-00000da0: 852e e56e f83f 6a1f bda2 1fe9 d27e c8ff  ...n.?j......~..
-00000db0: f956 5a4f 5c2c 53a5 abad 90f4 40a5 af51  .VZO\,S.....@..Q
-00000dc0: 81ad 1230 187f 9d4a 5fe4 2cd1 08c8 f1c0  ...0...J_.,.....
-00000dd0: 9cfa ca47 5678 734a 6018 36fe 6e4a bee6  ...GVxsJ`.6.nJ..
-00000de0: 26ca 3b2b 2530 c937 7ead 9930 fded a586  &.;+%0.7~..0....
-00000df0: e57b 8f08 609a 29b6 c583 e5c2 5c05 837a  .{..`.).....\..z
-00000e00: bb2e 07ac 4cd0 e888 4db3 4e09 21cb e567  ....L...M.N.!..g
-00000e10: 53b2 4360 71fc d2f3 3f68 5659 aeb9 cff7  S.C`q...?hVY....
-00000e20: cccc 008c 5ce1 c937 5c1a 39be dbd3 aa24  ....\..7\.9....$
-00000e30: 8500 339f aaca 987d 4f5d 2a3e d5f3 6873  ..3....}O]*>..hs
-00000e40: d3d4 0c20 128a e9ca f559 79f1 a35f b34a  ... .....Yy.._.J
-00000e50: 0efc 7cb8 a75f a5b4 3c20 9a49 98a3 f6e0  ..|.._..< .I....
-00000e60: 257b 2e3e fbf6 d366 b7bb 7c7e bfdf 6bff  %{.>...f..|~..k.
-00000e70: fcec cae1 7593 5a56 2f98 5200 7442 3e41  ....u.ZV/.R.tB>A
-00000e80: da3c 050b 172b 5aaa 52d5 ead5 2b16 cd99  .<...+Z.R...+...
-00000e90: 3691 c880 3846 5650 3820 ec03 0000 9014  6...8FVP8 ......
-00000ea0: 009d 012a 5000 2d00 3e99 3c99 4825 a322  ...*P.-.>.<.H%."
-00000eb0: a131 180c 90b0 1309 6c00 b953 c2c6 148e  .1......l..S....
-00000ec0: eadf db37 e44a 8583 3d4f fe59 f42b e987  ...7.J..=O.Y.+..
-00000ed0: e683 ee03 de77 d2d7 faef 4ece a3bd e59c  .....w....N.....
-00000ee0: 02bf e35d 8df7 b7e4 a01f c64b 72e8 37f7  ...].......Kr.7.
-00000ef0: 5afa a68b 6b2e cb40 76a4 7d8d 9a1f 53f2  Z...k..@v.}...S.
-00000f00: 7ed8 bc19 bbc0 bd11 947f cabc 8f5a a159  ~............Z.Y
-00000f10: a5f7 f9d5 6575 a4e9 2ee7 292e bea6 b925  ....eu....)....%
-00000f20: 6b2c 14bb 2215 effe 0385 08ed e243 9e4e  k,.."........C.N
-00000f30: 7c4c 3efc 89c5 45ee 780d e3c7 cd99 889e  |L>...E.x.......
-00000f40: 14cf 3544 719f 7ffe 7a49 0000 fee4 423f  ..5Dq...zI....B?
-00000f50: ff4a 176e d30f cd1c d2e7 087c 4e10 5b00  .J.n.......|N.[.
-00000f60: 5e67 ad9d 88da 2c84 ac2f fbdb ddf4 5b67  ^g....,../....[g
-00000f70: 804b bbec 12d8 447c 4a29 9dd6 d3b9 cfdd  .K....D|J)......
-00000f80: 04df 0f52 2e4d 3410 c76d 1abb f19f 0e05  ...R.M4..m......
-00000f90: fcdd 6471 0f63 c15c 33f2 9370 a711 ecc5  ..dq.c.\3..p....
-00000fa0: 28b3 1137 811f d1a2 6c96 16b3 3607 06bd  (..7....l...6...
-00000fb0: fd73 0d56 3969 20d5 8f46 962d b132 1c83  .s.V9i ..F.-.2..
-00000fc0: f022 fe97 9037 3e18 4587 e612 e6a6 1b12  ."...7>.E.......
-00000fd0: c137 e0ab cad4 b278 d6f4 ba65 8d9e ae21  .7.....x...e...!
-00000fe0: b0cd 203f f3da 3013 930d b64f 4184 39ff  .. ?..0....OA.9.
-00000ff0: 0090 8cbd a5b7 a027 5b65 9697 3d0b a401  .......'[e..=...
-00001000: 9063 0054 26f5 0b25 e3d1 c066 7514 8211  .c.T&..%...fu...
-00001010: c829 771d 7fd4 80a1 fb84 0b4b 4788 c7ef  .)w........KG...
-00001020: 9545 636f 4b2f 44e9 d000 4d8e fc12 fa39  .EcoK/D...M....9
-00001030: 3725 b92e 6db7 82e8 edc8 e375 1305 5230  7%..m......u..R0
-00001040: a4b4 2fb3 afb6 419e 6eb2 e50d 7f8d 1042  ../...A.n......B
-00001050: b53f 9db8 84eb 28dd 6354 0fc9 c198 0ae9  .?....(.cT......
-00001060: a37b 94b8 57c1 66e1 bc28 f780 8dab 00ca  .{..W.f..(......
-00001070: 341b 5955 1fb1 6e39 cccf d42f de25 6125  4.YU..n9.../.%a%
-00001080: 13ee dec3 70ac d680 f616 48b0 912a 327f  ....p.....H..*2.
-00001090: fe78 31d7 124f 3e52 ed65 0a03 7b28 6cb8  .x1..O>R.e..{(l.
-000010a0: b01f 2bde b598 431a 5bfe 2fb7 8f28 08c0  ..+...C.[./..(..
-000010b0: 64db e978 1a13 b729 7418 97ad dd03 92dd  d..x...)t.......
-000010c0: df04 4f21 6ce1 42fb 496a f4a7 a25f ae6d  ..O!l.B.Ij..._.m
-000010d0: 94d2 e037 05ec 406e 417c 650e 4caf 6b1b  ...7..@nA|e.L.k.
-000010e0: 9ce6 59a7 80dc d9fc 2721 2e07 6a1e ce49  ..Y.....'!..j..I
-000010f0: bea0 9582 85a3 49ff 8ba7 b0ba 1cd7 6f1b  ......I.......o.
-00001100: 9bfa 9a6c ad17 cdbb 7b20 a3f6 06ac ae9b  ...l....{ ......
-00001110: 833e 4518 6ec5 49f6 7fea 473f d357 65ae  .>E.n.I...G?.We.
-00001120: b714 adc8 3267 524e 8995 62a9 5ef4 444f  ....2gRN..b.^.DO
-00001130: 1321 3251 f378 ed69 6496 900c 54f6 58bc  .!2Q.x.id...T.X.
-00001140: 9d35 ea95 f8d9 38cf 955e 7dc9 011f 73ce  .5....8..^}...s.
-00001150: f681 8814 75c7 54ec 3d61 69d5 066e f52a  ....u.T.=ai..n.*
-00001160: 49ce 9639 1393 c28b a734 5233 d82c f187  I..9.....4R3.,..
-00001170: bf76 1154 6249 b2cc ef0f fb95 dd9e 12ce  .v.TbI..........
-00001180: d42d 9c10 a4a8 6f33 8dab 6ba2 ecfd f993  .-....o3..k.....
-00001190: e2ab ad0f 1fbf 447d 6bcd 9312 69e5 c030  ......D}k...i..0
-000011a0: cd62 b3a6 c759 8be3 c575 1eb8 b8e0 aa63  .b...Y...u.....c
-000011b0: ffbc c912 ae9b 7b96 9d24 3017 1b78 8c73  ......{..$0..x.s
-000011c0: 7e01 9bf3 b8c4 aea3 5e97 36d0 60ea a5cb  ~.......^.6.`...
-000011d0: 2afd d897 d219 9516 2da8 e168 8764 631f  *.......-..h.dc.
-000011e0: 01ca 9549 bc8a 49c9 c6f2 5652 7b4d e8f7  ...I..I...VR{M..
-000011f0: dc9d 37a0 b569 95f4 9593 e15b 2439 86b5  ..7..i.....[$9..
-00001200: b765 8fc8 d6d9 7304 f5e1 dec3 b5bb 6d7c  .e....s.......m|
-00001210: 4897 c984 8666 62c1 847e 984b 14bc ea94  H....fb..~.K....
-00001220: 449b cb8f 8449 a321 4787 581f 6c00 066b  D....I.!G.X.l..k
-00001230: 6fc3 f948 0c38 7712 a4c7 1250 5bb9 a954  o..H.8w....P[..T
-00001240: b379 7c96 943b 4653 9f13 4265 f126 5f77  .y|..;FS..Be.&_w
-00001250: 4b01 b676 db07 6b9f 99e0 73ff 5ae5 df4e  K..v..k...s.Z..N
-00001260: 3ccd 728c 23ad dce7 e9cf 2024 23e2 ea87  <.r.#..... $#...
-00001270: 38d1 5e57 047b ed66 3185 ea00 272b bb08  8.^W.{.f1...'+..
-00001280: 6963 8488 31f5 9000 0000 584d 5020 9a03  ic..1.....XMP ..
-00001290: 0000 3c78 3a78 6d70 6d65 7461 2078 6d6c  ..<x:xmpmeta xml
-000012a0: 6e73 3a78 3d22 6164 6f62 653a 6e73 3a6d  ns:x="adobe:ns:m
-000012b0: 6574 612f 2220 783a 786d 7074 6b3d 2258  eta/" x:xmptk="X
-000012c0: 4d50 2043 6f72 6520 362e 302e 3022 3e0a  MP Core 6.0.0">.
-000012d0: 2020 203c 7264 663a 5244 4620 786d 6c6e     <rdf:RDF xmln
-000012e0: 733a 7264 663d 2268 7474 703a 2f2f 7777  s:rdf="http://ww
-000012f0: 772e 7733 2e6f 7267 2f31 3939 392f 3032  w.w3.org/1999/02
-00001300: 2f32 322d 7264 662d 7379 6e74 6178 2d6e  /22-rdf-syntax-n
-00001310: 7323 223e 0a20 2020 2020 203c 7264 663a  s#">.      <rdf:
-00001320: 4465 7363 7269 7074 696f 6e20 7264 663a  Description rdf:
-00001330: 6162 6f75 743d 2222 0a20 2020 2020 2020  about="".       
-00001340: 2020 2020 2078 6d6c 6e73 3a65 7869 663d       xmlns:exif=
-00001350: 2268 7474 703a 2f2f 6e73 2e61 646f 6265  "http://ns.adobe
-00001360: 2e63 6f6d 2f65 7869 662f 312e 302f 220a  .com/exif/1.0/".
-00001370: 2020 2020 2020 2020 2020 2020 786d 6c6e              xmln
-00001380: 733a 7469 6666 3d22 6874 7470 3a2f 2f6e  s:tiff="http://n
-00001390: 732e 6164 6f62 652e 636f 6d2f 7469 6666  s.adobe.com/tiff
-000013a0: 2f31 2e30 2f22 0a20 2020 2020 2020 2020  /1.0/".         
-000013b0: 2020 2078 6d6c 6e73 3a78 6d70 3d22 6874     xmlns:xmp="ht
-000013c0: 7470 3a2f 2f6e 732e 6164 6f62 652e 636f  tp://ns.adobe.co
-000013d0: 6d2f 7861 702f 312e 302f 223e 0a20 2020  m/xap/1.0/">.   
-000013e0: 2020 2020 2020 3c65 7869 663a 5069 7865        <exif:Pixe
-000013f0: 6c59 4469 6d65 6e73 696f 6e3e 3435 3c2f  lYDimension>45</
-00001400: 6578 6966 3a50 6978 656c 5944 696d 656e  exif:PixelYDimen
-00001410: 7369 6f6e 3e0a 2020 2020 2020 2020 203c  sion>.         <
-00001420: 6578 6966 3a50 6978 656c 5844 696d 656e  exif:PixelXDimen
-00001430: 7369 6f6e 3e38 303c 2f65 7869 663a 5069  sion>80</exif:Pi
-00001440: 7865 6c58 4469 6d65 6e73 696f 6e3e 0a20  xelXDimension>. 
-00001450: 2020 2020 2020 2020 3c74 6966 663a 5265          <tiff:Re
-00001460: 736f 6c75 7469 6f6e 556e 6974 3e32 3c2f  solutionUnit>2</
-00001470: 7469 6666 3a52 6573 6f6c 7574 696f 6e55  tiff:ResolutionU
-00001480: 6e69 743e 0a20 2020 2020 2020 2020 3c74  nit>.         <t
-00001490: 6966 663a 5852 6573 6f6c 7574 696f 6e3e  iff:XResolution>
-000014a0: 3732 3030 3030 2f31 3030 3030 3c2f 7469  720000/10000</ti
-000014b0: 6666 3a58 5265 736f 6c75 7469 6f6e 3e0a  ff:XResolution>.
-000014c0: 2020 2020 2020 2020 203c 7469 6666 3a4f           <tiff:O
-000014d0: 7269 656e 7461 7469 6f6e 3e31 3c2f 7469  rientation>1</ti
-000014e0: 6666 3a4f 7269 656e 7461 7469 6f6e 3e0a  ff:Orientation>.
-000014f0: 2020 2020 2020 2020 203c 7469 6666 3a59           <tiff:Y
-00001500: 5265 736f 6c75 7469 6f6e 3e37 3230 3030  Resolution>72000
-00001510: 302f 3130 3030 303c 2f74 6966 663a 5952  0/10000</tiff:YR
-00001520: 6573 6f6c 7574 696f 6e3e 0a20 2020 2020  esolution>.     
-00001530: 2020 2020 3c78 6d70 3a4d 6574 6164 6174      <xmp:Metadat
-00001540: 6144 6174 653e 3230 3234 2d30 342d 3037  aDate>2024-04-07
-00001550: 5432 313a 3532 3a32 302b 3038 3a30 303c  T21:52:20+08:00<
-00001560: 2f78 6d70 3a4d 6574 6164 6174 6144 6174  /xmp:MetadataDat
-00001570: 653e 0a20 2020 2020 2020 2020 3c78 6d70  e>.         <xmp
-00001580: 3a43 7265 6174 6f72 546f 6f6c 3e50 6978  :CreatorTool>Pix
-00001590: 656c 6d61 746f 7220 5072 6f20 332e 352e  elmator Pro 3.5.
-000015a0: 373c 2f78 6d70 3a43 7265 6174 6f72 546f  7</xmp:CreatorTo
-000015b0: 6f6c 3e0a 2020 2020 2020 2020 203c 786d  ol>.         <xm
-000015c0: 703a 4372 6561 7465 4461 7465 3e32 3032  p:CreateDate>202
-000015d0: 342d 3034 2d30 3154 3133 3a33 323a 3339  4-04-01T13:32:39
-000015e0: 2b30 383a 3030 3c2f 786d 703a 4372 6561  +08:00</xmp:Crea
-000015f0: 7465 4461 7465 3e0a 2020 2020 2020 3c2f  teDate>.      </
-00001600: 7264 663a 4465 7363 7269 7074 696f 6e3e  rdf:Description>
-00001610: 0a20 2020 3c2f 7264 663a 5244 463e 0a3c  .   </rdf:RDF>.<
-00001620: 2f78 3a78 6d70 6d65 7461 3e0a            /x:xmpmeta>.
+00000c70: 5048 2c02 0000 0190 0400 6019 4949 673a  PH,.......`.IIg:
+00000c80: 33bb 67db b66d f367 dbb6 6ddb f6bd d6b6  3.g..m.g..m.....
+00000c90: 6ddb b639 6d72 2ad3 c333 2226 00fc 0b42  m..9mr*..3"&...B
+00000ca0: 5db3 565d 3bb7 69a6 a314 41d5 6ae2 318b  ].V];.i...A.j.1.
+00000cb0: c0b0 94e4 e820 9b97 db47 b6a0 086b 30f1  ..... ...G...k0.
+00000cc0: ba7f 318b b999 22df 836d 2141 daa9 1ff2  ..1..."..m!A....
+00000cd0: 592c b4ce 736d 7352 60d7 3b05 088b 5963  Y,..smsR`.;...Yc
+00000ce0: 3559 4d04 35d9 9fc5 6267 6ed2 11a0 5e92  5YM.5...bgn...^.
+00000cf0: 8425 2cb9 da54 76f4 ea6c 2c69 ed39 5a6e  .%,..Tv..l,i.9Zn
+00000d00: 0bf3 b0c4 851b 55f2 eaec 8325 4f9f 2c27  ......U....%O.,'
+00000d10: d8fc 1923 1d76 ef26 1baa cb1e d76a 2c43  ...#.v.&.....j,C
+00000d20: c661 4d27 15dd b9ad 5a12 d86b f391 31a7  .aM'....Z..k..1.
+00000d30: a2f4 58a6 7511 cf9f c647 dced 2c01 9c18  ..X.u....G..,...
+00000d40: ccd4 e733 58e6 8c6d 7f28 12d5 6d77 3426  ...3X..m.(..mw4&
+00000d50: 12f9 4da3 4569 7e38 8ac1 84a2 eccb 9da1  ..M.Ei~8........
+00000d60: 20d5 58b3 3a4c 70bd c75c 5a80 7643 2ac2   .X.:Lp..\Z.vC*.
+00000d70: 44a3 cced 1a5e f4fe 024c 7cde 728a cff4  D....^...L|.r...
+00000d80: 3cac 8071 a378 68be 6025 44df 0cb8 bac6  <..q.xh.`%D.....
+00000d90: 2902 ceea cf35 bf5a 19ea 5770 6d63 9501  )....5.Z..Wpmc..
+00000da0: 9fe0 5ac3 90c5 04d5 fe86 ddcd 3534 8d2c  ..Z.........54.,
+00000db0: 94a7 ff4d ce68 2ecd 433d 519c e8b9 960b  ...M.h..C=Q.....
+00000dc0: 4ccc 5482 c2c9 8067 83b7 2c71 a8ee a696  L.T....g..,q....
+00000dd0: 0fe8 192a 8c8d af94 1342 759f 5a01 de70  ...*.....Bu.Z..p
+00000de0: 712e 12a2 f72a 9304 0940 a8e2 662b 2090  q....*...@..f+ .
+00000df0: 5e9c 8004 08ce 8943 fc04 229c bbdd 0008  ^......C..".....
+00000e00: a686 7d29 97c4 e50e 2301 1b30 4f0d c46c  ..})....#..0O..l
+00000e10: b8c8 b200 89c7 d462 d1f5 3157 7a40 2072  .......b..1Wz@ r
+00000e20: 8331 f752 9158 a2a3 32d7 9d5d 2820 a17a  .1.R.X..2..]( .z
+00000e30: c865 bf52 249f cac0 6b53 9b41 2031 dd6a  .e.R$...kS.A 1.j
+00000e40: ca69 e3e8 5256 32c4 9647 7c5e da9a 02b2  .i..RV2..G|^....
+00000e50: 84da f6e3 f7bc 704f af42 62e9 abf3 c38d  ......pO.Bb.....
+00000e60: f64d 6e47 0359 538d 7ace 39fc d8c8 2d26  .MnG.YS.z.9...-&
+00000e70: 27bf b0a8 a8a4 b2aa aaaa a230 23c6 cbe2  '..........0#...
+00000e80: dda5 9533 06b5 d200 3221 ddb0 5ddf 8143  ...3....2!..]..C
+00000e90: 860f 1b3d 79da 8c19 9386 f56c d758 4b81  ...=y......l.XK.
+00000ea0: ff8c 5650 3820 5e04 0000 1015 009d 012a  ..VP8 ^........*
+00000eb0: 5000 2d00 3e99 3c99 4825 a322 a12e f92c  P.-.>.<.H%."...,
+00000ec0: f8b0 1309 6c00 b953 9346 1492 ab3f e2b7  ....l..S.F...?..
+00000ed0: 68ca b426 3f2c ef35 f32d e725 e963 fd97  h..&?,.5.-.%.c..
+00000ee0: a2e7 51d7 3eb7 b2ae 00ef f20e ccbb e3f0  ..Q.>...........
+00000ef0: ba08 6b5d debc b02c 9bc5 1695 0674 f408  ..k]...,.....t..
+00000f00: e94b e880 dbfa cdb8 8914 73c4 986b ddb2  .K........s..k..
+00000f10: d1f5 e98f e101 6753 7b5a 6fd7 d6d2 ad82  ......gS{Zo.....
+00000f20: bf80 30b7 d308 ef32 acdd 7dfd 66ff b12d  ..0....2..}.f..-
+00000f30: 18a7 e2ca a75c fff1 75ed 05f9 791f 97f8  .....\..u...y...
+00000f40: 4dea 30f9 c75d c390 0bb4 f66d 0d55 8fed  M.0..].....m.U..
+00000f50: 6a5a 4612 531a 42b6 eaf4 1000 fee4 423f  jZF.S.B.......B?
+00000f60: ff25 09af f92f 2dec 1fc4 4cd8 33c0 98e2  .%.../-...L.3...
+00000f70: ef84 c173 c695 a825 79fb 2a7a 5917 0e1f  ...s...%y.*zY...
+00000f80: 9be0 48fc c4fe 7cf4 7784 f3f6 c5fb abca  ..H...|.w.......
+00000f90: ffd0 1dd9 7bf1 c02e a419 0e73 a938 f144  ....{......s.8.D
+00000fa0: 6977 24fb ecaa 5b67 9635 ffa2 4cb7 be75  iw$...[g.5..L..u
+00000fb0: 448b f729 2b3a 411e 6d47 2371 33d6 37b5  D..)+:A.mG#q3.7.
+00000fc0: c77a 01c3 4303 5a6f 3e5b 7571 df8e f213  .z..C.Zo>[uq....
+00000fd0: fae0 1f10 9485 829b cdb1 d07d e7a8 f64b  ...........}...K
+00000fe0: f322 0a71 df81 48f4 2f7a 0b05 6b91 f95d  .".q..H./z..k..]
+00000ff0: 870c 1a8a dcce 4564 9f64 b8c4 5f26 a23e  ......Ed.d.._&.>
+00001000: 3912 4f8a a13d 0ad7 e436 fd10 bb4f b13b  9.O..=...6...O.;
+00001010: 5477 f4b5 eef6 689f 80d7 3147 8dfe 0c8f  Tw....h...1G....
+00001020: fc5d 94bd b96b bd46 4b46 8c2c 03f4 0cb8  .]...k.FKF.,....
+00001030: c0e0 2474 fda1 b1f7 df56 d5d7 6df6 e310  ..$t.....V..m...
+00001040: 2ef3 91db 4432 a719 9c49 353f 8aef 6a13  ....D2...I5?..j.
+00001050: 3d99 0bb9 a9c7 48a3 53ca 961c 53fd c9f4  =.....H.S...S...
+00001060: 28c2 49d3 89bb 0374 ab99 6aae 016a 8966  (.I....t..j..j.f
+00001070: 4465 0d55 d380 3145 e411 4124 a304 136a  De.U..1E..A$...j
+00001080: 26c1 617a 597f b248 ada7 b1ff 4052 d630  &.azY..H....@R.0
+00001090: 2bba 67ea 6459 b29c 2c6f afbe 8d5b dd81  +.g.dY..,o...[..
+000010a0: 8b52 3ab2 e8e1 c93a 03c4 d0f9 2255 68cb  .R:....:...."Uh.
+000010b0: 5568 f946 693a 48a9 ef1c 702d 38e1 1314  Uh.Fi:H...p-8...
+000010c0: c1f1 a26d 7967 6bac 242f 7804 6702 8f95  ...mygk.$/x.g...
+000010d0: f22a ff0f 9974 3df2 c980 57ae b57c 79a4  .*...t=...W..|y.
+000010e0: 70df 9bbe 474c 8cf3 bd54 3bb0 55d5 7613  p...GL...T;.U.v.
+000010f0: 72ce 278f ba5b 59fe ee8d efd9 34b5 aed6  r.'..[Y.....4...
+00001100: 509b 4ab6 6c3e 295b 89ca 92a8 d38a 60d9  P.J.l>)[......`.
+00001110: 9cf2 38df b7a3 33db 61b9 29c9 8d36 ffe1  ..8...3.a.)..6..
+00001120: 3462 69cd c336 5cc5 2e15 2f44 9c0f 2df2  4bi..6\.../D..-.
+00001130: 1931 d7f5 2251 5783 5941 e4ec 85e6 e690  .1.."QW.YA......
+00001140: 5db3 9335 5b76 dbfd c37b 284e a7ff fe32  ]..5[v...{(N...2
+00001150: caad dd76 b91a 2af9 6bae 289d a9dc 4ee0  ...v..*.k.(...N.
+00001160: c885 654d 4b8e 40ef ce8b dd39 0141 e08b  ..eMK.@....9.A..
+00001170: cc35 457d 6af1 3d60 19da 4fd7 4ee0 94ad  .5E}j.=`..O.N...
+00001180: 5b98 0aab a61e 6e01 85a4 bee6 ee0b 103e  [.....n........>
+00001190: 59fd 8673 f347 6a48 c6ef 6a94 a8ba 5f86  Y..s.GjH..j..._.
+000011a0: 8b65 9e47 c8b5 cdd5 6d65 ff27 fc7d 6cf2  .e.G....me.'.}l.
+000011b0: e1c4 13f2 874e 4218 ffe8 a1db 2e7f b72f  .....NB......../
+000011c0: c048 a422 756a 7310 e02f 1e2c 0f71 f76e  .H."ujs../.,.q.n
+000011d0: b69f a895 68bc 005c 7a72 4be9 0b98 a5a4  ....h..\zrK.....
+000011e0: f754 e2f9 c625 488e 9d9b 6bfe 656a ac28  .T...%H...k.ej.(
+000011f0: 5d63 d471 7fbd 6389 834c 9bd0 5c76 0fb9  ]c.q..c..L..\v..
+00001200: 53e2 8764 8fa6 ea94 91bd e3b8 09ab 4d51  S..d..........MQ
+00001210: fc4b a3c9 2db5 61ba 2fcc 8d5a dff1 fc9f  .K..-.a./..Z....
+00001220: 8b0a 3ed2 ebbb 7b14 308e a745 428e 69fc  ..>...{.0..EB.i.
+00001230: 7139 2da8 aca9 4266 c9b8 eb5f 2dcc db40  q9-...Bf..._-..@
+00001240: 7fd9 7d41 2822 84d2 518f 64f8 ccc1 d71f  ..}A("..Q.d.....
+00001250: 671a 2b68 75ea d04d a257 1e59 4dfa feeb  g.+hu..M.W.YM...
+00001260: 1360 f370 15fc c669 dbb1 a926 b65c b395  .`.p...i...&.\..
+00001270: bf38 127c 484b 43c5 cebb 4995 f783 78c2  .8.|HKC...I...x.
+00001280: cdd9 9c95 0776 98ac f3d0 8520 b64e 3238  .....v..... .N28
+00001290: 8a76 e307 f185 b9c7 4f52 6c92 bfac 8d5f  .v......ORl...._
+000012a0: 1836 5b80 ef61 030e 603c cef4 2e6e e7c9  .6[..a..`<...n..
+000012b0: 3abf f3a6 3083 fa20 e529 f122 80a6 f834  :...0.. .)."...4
+000012c0: 34a8 cbe0 2ced 40a4 6594 0191 c722 1d02  4...,.@.e...."..
+000012d0: 3cf8 9eb1 9b2f a41e 3051 2697 55de 59e9  <..../..0Q&.U.Y.
+000012e0: ac01 7a61 7cb2 830e d6dc 45d0 4064 a230  ..za|.....E.@d.0
+000012f0: 88c9 b9b0 0a73 f3b0 828e f1eb c6cf 41a5  .....s........A.
+00001300: f1e7 b1f4 f7c0 0000 584d 5020 9a03 0000  ........XMP ....
+00001310: 3c78 3a78 6d70 6d65 7461 2078 6d6c 6e73  <x:xmpmeta xmlns
+00001320: 3a78 3d22 6164 6f62 653a 6e73 3a6d 6574  :x="adobe:ns:met
+00001330: 612f 2220 783a 786d 7074 6b3d 2258 4d50  a/" x:xmptk="XMP
+00001340: 2043 6f72 6520 362e 302e 3022 3e0a 2020   Core 6.0.0">.  
+00001350: 203c 7264 663a 5244 4620 786d 6c6e 733a   <rdf:RDF xmlns:
+00001360: 7264 663d 2268 7474 703a 2f2f 7777 772e  rdf="http://www.
+00001370: 7733 2e6f 7267 2f31 3939 392f 3032 2f32  w3.org/1999/02/2
+00001380: 322d 7264 662d 7379 6e74 6178 2d6e 7323  2-rdf-syntax-ns#
+00001390: 223e 0a20 2020 2020 203c 7264 663a 4465  ">.      <rdf:De
+000013a0: 7363 7269 7074 696f 6e20 7264 663a 6162  scription rdf:ab
+000013b0: 6f75 743d 2222 0a20 2020 2020 2020 2020  out="".         
+000013c0: 2020 2078 6d6c 6e73 3a65 7869 663d 2268     xmlns:exif="h
+000013d0: 7474 703a 2f2f 6e73 2e61 646f 6265 2e63  ttp://ns.adobe.c
+000013e0: 6f6d 2f65 7869 662f 312e 302f 220a 2020  om/exif/1.0/".  
+000013f0: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
+00001400: 7469 6666 3d22 6874 7470 3a2f 2f6e 732e  tiff="http://ns.
+00001410: 6164 6f62 652e 636f 6d2f 7469 6666 2f31  adobe.com/tiff/1
+00001420: 2e30 2f22 0a20 2020 2020 2020 2020 2020  .0/".           
+00001430: 2078 6d6c 6e73 3a78 6d70 3d22 6874 7470   xmlns:xmp="http
+00001440: 3a2f 2f6e 732e 6164 6f62 652e 636f 6d2f  ://ns.adobe.com/
+00001450: 7861 702f 312e 302f 223e 0a20 2020 2020  xap/1.0/">.     
+00001460: 2020 2020 3c65 7869 663a 5069 7865 6c59      <exif:PixelY
+00001470: 4469 6d65 6e73 696f 6e3e 3435 3c2f 6578  Dimension>45</ex
+00001480: 6966 3a50 6978 656c 5944 696d 656e 7369  if:PixelYDimensi
+00001490: 6f6e 3e0a 2020 2020 2020 2020 203c 6578  on>.         <ex
+000014a0: 6966 3a50 6978 656c 5844 696d 656e 7369  if:PixelXDimensi
+000014b0: 6f6e 3e38 303c 2f65 7869 663a 5069 7865  on>80</exif:Pixe
+000014c0: 6c58 4469 6d65 6e73 696f 6e3e 0a20 2020  lXDimension>.   
+000014d0: 2020 2020 2020 3c74 6966 663a 5265 736f        <tiff:Reso
+000014e0: 6c75 7469 6f6e 556e 6974 3e32 3c2f 7469  lutionUnit>2</ti
+000014f0: 6666 3a52 6573 6f6c 7574 696f 6e55 6e69  ff:ResolutionUni
+00001500: 743e 0a20 2020 2020 2020 2020 3c74 6966  t>.         <tif
+00001510: 663a 5852 6573 6f6c 7574 696f 6e3e 3732  f:XResolution>72
+00001520: 3030 3030 2f31 3030 3030 3c2f 7469 6666  0000/10000</tiff
+00001530: 3a58 5265 736f 6c75 7469 6f6e 3e0a 2020  :XResolution>.  
+00001540: 2020 2020 2020 203c 7469 6666 3a4f 7269         <tiff:Ori
+00001550: 656e 7461 7469 6f6e 3e31 3c2f 7469 6666  entation>1</tiff
+00001560: 3a4f 7269 656e 7461 7469 6f6e 3e0a 2020  :Orientation>.  
+00001570: 2020 2020 2020 203c 7469 6666 3a59 5265         <tiff:YRe
+00001580: 736f 6c75 7469 6f6e 3e37 3230 3030 302f  solution>720000/
+00001590: 3130 3030 303c 2f74 6966 663a 5952 6573  10000</tiff:YRes
+000015a0: 6f6c 7574 696f 6e3e 0a20 2020 2020 2020  olution>.       
+000015b0: 2020 3c78 6d70 3a4d 6574 6164 6174 6144    <xmp:MetadataD
+000015c0: 6174 653e 3230 3234 2d30 342d 3037 5432  ate>2024-04-07T2
+000015d0: 313a 3532 3a32 382b 3038 3a30 303c 2f78  1:52:28+08:00</x
+000015e0: 6d70 3a4d 6574 6164 6174 6144 6174 653e  mp:MetadataDate>
+000015f0: 0a20 2020 2020 2020 2020 3c78 6d70 3a43  .         <xmp:C
+00001600: 7265 6174 6f72 546f 6f6c 3e50 6978 656c  reatorTool>Pixel
+00001610: 6d61 746f 7220 5072 6f20 332e 352e 373c  mator Pro 3.5.7<
+00001620: 2f78 6d70 3a43 7265 6174 6f72 546f 6f6c  /xmp:CreatorTool
+00001630: 3e0a 2020 2020 2020 2020 203c 786d 703a  >.         <xmp:
+00001640: 4372 6561 7465 4461 7465 3e32 3032 342d  CreateDate>2024-
+00001650: 3034 2d30 3154 3133 3a33 323a 3339 2b30  04-01T13:32:39+0
+00001660: 383a 3030 3c2f 786d 703a 4372 6561 7465  8:00</xmp:Create
+00001670: 4461 7465 3e0a 2020 2020 2020 3c2f 7264  Date>.      </rd
+00001680: 663a 4465 7363 7269 7074 696f 6e3e 0a20  f:Description>. 
+00001690: 2020 3c2f 7264 663a 5244 463e 0a3c 2f78    </rdf:RDF>.</x
+000016a0: 3a78 6d70 6d65 7461 3e0a                 :xmpmeta>.
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp` & `SightTraining-0.1.20/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 5249 4646 a216 0000 5745 4250 5650 3858  RIFF....WEBPVP8X
+00000000: 5249 4646 2a16 0000 5745 4250 5650 3858  RIFF*...WEBPVP8X
 00000010: 0a00 0000 3400 0000 4f00 002c 0000 4943  ....4...O..,..IC
 00000020: 4350 480c 0000 0000 0c48 4c69 6e6f 0210  CPH......HLino..
 00000030: 0000 6d6e 7472 5247 4220 5859 5a20 07ce  ..mntrRGB XYZ ..
 00000040: 0002 0009 0006 0031 0000 6163 7370 4d53  .......1..acspMS
 00000050: 4654 0000 0000 4945 4320 7352 4742 0000  FT....IEC sRGB..
 00000060: 0000 0000 0000 0000 0000 0000 f6d6 0001  ................
 00000070: 0000 0000 d32d 4850 2020 0000 0000 0000  .....-HP  ......
@@ -193,171 +193,164 @@
 00000c00: e253 e2db e363 e3eb e473 e4fc e584 e60d  .S...c...s......
 00000c10: e696 e71f e7a9 e832 e8bc e946 e9d0 ea5b  .......2...F...[
 00000c20: eae5 eb70 ebfb ec86 ed11 ed9c ee28 eeb4  ...p.........(..
 00000c30: ef40 efcc f058 f0e5 f172 f1ff f28c f319  .@...X...r......
 00000c40: f3a7 f434 f4c2 f550 f5de f66d f6fb f78a  ...4...P...m....
 00000c50: f819 f8a8 f938 f9c7 fa57 fae7 fb77 fc07  .....8...W...w..
 00000c60: fc98 fd29 fdba fe4b fedc ff6d ffff 414c  ...)...K...m..AL
-00000c70: 5048 2c02 0000 0190 0400 6019 4949 673a  PH,.......`.IIg:
-00000c80: 33bb 67db b66d f367 dbb6 6ddb f6bd d6b6  3.g..m.g..m.....
-00000c90: 6ddb b639 6d72 2ad3 c333 2226 00fc 0b42  m..9mr*..3"&...B
-00000ca0: 5db3 565d 3bb7 69a6 a314 41d5 6ae2 318b  ].V];.i...A.j.1.
-00000cb0: c0b0 94e4 e820 9b97 db47 b6a0 086b 30f1  ..... ...G...k0.
-00000cc0: ba7f 318b b999 22df 836d 2141 daa9 1ff2  ..1..."..m!A....
-00000cd0: 592c b4ce 736d 7352 60d7 3b05 088b 5963  Y,..smsR`.;...Yc
-00000ce0: 3559 4d04 35d9 9fc5 6267 6ed2 11a0 5e92  5YM.5...bgn...^.
-00000cf0: 8425 2cb9 da54 76f4 ea6c 2c69 ed39 5a6e  .%,..Tv..l,i.9Zn
-00000d00: 0bf3 b0c4 851b 55f2 eaec 8325 4f9f 2c27  ......U....%O.,'
-00000d10: d8fc 1923 1d76 ef26 1baa cb1e d76a 2c43  ...#.v.&.....j,C
-00000d20: c661 4d27 15dd b9ad 5a12 d86b f391 31a7  .aM'....Z..k..1.
-00000d30: a2f4 58a6 7511 cf9f c647 dced 2c01 9c18  ..X.u....G..,...
-00000d40: ccd4 e733 58e6 8c6d 7f28 12d5 6d77 3426  ...3X..m.(..mw4&
-00000d50: 12f9 4da3 4569 7e38 8ac1 84a2 eccb 9da1  ..M.Ei~8........
-00000d60: 20d5 58b3 3a4c 70bd c75c 5a80 7643 2ac2   .X.:Lp..\Z.vC*.
-00000d70: 44a3 cced 1a5e f4fe 024c 7cde 728a cff4  D....^...L|.r...
-00000d80: 3cac 8071 a378 68be 6025 44df 0cb8 bac6  <..q.xh.`%D.....
-00000d90: 2902 ceea cf35 bf5a 19ea 5770 6d63 9501  )....5.Z..Wpmc..
-00000da0: 9fe0 5ac3 90c5 04d5 fe86 ddcd 3534 8d2c  ..Z.........54.,
-00000db0: 94a7 ff4d ce68 2ecd 433d 519c e8b9 960b  ...M.h..C=Q.....
-00000dc0: 4ccc 5482 c2c9 8067 83b7 2c71 a8ee a696  L.T....g..,q....
-00000dd0: 0fe8 192a 8c8d af94 1342 759f 5a01 de70  ...*.....Bu.Z..p
-00000de0: 712e 12a2 f72a 9304 0940 a8e2 662b 2090  q....*...@..f+ .
-00000df0: 5e9c 8004 08ce 8943 fc04 229c bbdd 0008  ^......C..".....
-00000e00: a686 7d29 97c4 e50e 2301 1b30 4f0d c46c  ..})....#..0O..l
-00000e10: b8c8 b200 89c7 d462 d1f5 3157 7a40 2072  .......b..1Wz@ r
-00000e20: 8331 f752 9158 a2a3 32d7 9d5d 2820 a17a  .1.R.X..2..]( .z
-00000e30: c865 bf52 249f cac0 6b53 9b41 2031 dd6a  .e.R$...kS.A 1.j
-00000e40: ca69 e3e8 5256 32c4 9647 7c5e da9a 02b2  .i..RV2..G|^....
-00000e50: 84da f6e3 f7bc 704f af42 62e9 abf3 c38d  ......pO.Bb.....
-00000e60: f64d 6e47 0359 538d 7ace 39fc d8c8 2d26  .MnG.YS.z.9...-&
-00000e70: 27bf b0a8 a8a4 b2aa aaaa a230 23c6 cbe2  '..........0#...
-00000e80: dda5 9533 06b5 d200 3221 ddb0 5ddf 8143  ...3....2!..]..C
-00000e90: 860f 1b3d 79da 8c19 9386 f56c d758 4b81  ...=y......l.XK.
-00000ea0: ff8c 5650 3820 5e04 0000 1015 009d 012a  ..VP8 ^........*
-00000eb0: 5000 2d00 3e99 3c99 4825 a322 a12e f92c  P.-.>.<.H%."...,
-00000ec0: f8b0 1309 6c00 b953 9346 1492 ab3f e2b7  ....l..S.F...?..
-00000ed0: 68ca b426 3f2c ef35 f32d e725 e963 fd97  h..&?,.5.-.%.c..
-00000ee0: a2e7 51d7 3eb7 b2ae 00ef f20e ccbb e3f0  ..Q.>...........
-00000ef0: ba08 6b5d debc b02c 9bc5 1695 0674 f408  ..k]...,.....t..
-00000f00: e94b e880 dbfa cdb8 8914 73c4 986b ddb2  .K........s..k..
-00000f10: d1f5 e98f e101 6753 7b5a 6fd7 d6d2 ad82  ......gS{Zo.....
-00000f20: bf80 30b7 d308 ef32 acdd 7dfd 66ff b12d  ..0....2..}.f..-
-00000f30: 18a7 e2ca a75c fff1 75ed 05f9 791f 97f8  .....\..u...y...
-00000f40: 4dea 30f9 c75d c390 0bb4 f66d 0d55 8fed  M.0..].....m.U..
-00000f50: 6a5a 4612 531a 42b6 eaf4 1000 fee4 423f  jZF.S.B.......B?
-00000f60: ff25 09af f92f 2dec 1fc4 4cd8 33c0 98e2  .%.../-...L.3...
-00000f70: ef84 c173 c695 a825 79fb 2a7a 5917 0e1f  ...s...%y.*zY...
-00000f80: 9be0 48fc c4fe 7cf4 7784 f3f6 c5fb abca  ..H...|.w.......
-00000f90: ffd0 1dd9 7bf1 c02e a419 0e73 a938 f144  ....{......s.8.D
-00000fa0: 6977 24fb ecaa 5b67 9635 ffa2 4cb7 be75  iw$...[g.5..L..u
-00000fb0: 448b f729 2b3a 411e 6d47 2371 33d6 37b5  D..)+:A.mG#q3.7.
-00000fc0: c77a 01c3 4303 5a6f 3e5b 7571 df8e f213  .z..C.Zo>[uq....
-00000fd0: fae0 1f10 9485 829b cdb1 d07d e7a8 f64b  ...........}...K
-00000fe0: f322 0a71 df81 48f4 2f7a 0b05 6b91 f95d  .".q..H./z..k..]
-00000ff0: 870c 1a8a dcce 4564 9f64 b8c4 5f26 a23e  ......Ed.d.._&.>
-00001000: 3912 4f8a a13d 0ad7 e436 fd10 bb4f b13b  9.O..=...6...O.;
-00001010: 5477 f4b5 eef6 689f 80d7 3147 8dfe 0c8f  Tw....h...1G....
-00001020: fc5d 94bd b96b bd46 4b46 8c2c 03f4 0cb8  .]...k.FKF.,....
-00001030: c0e0 2474 fda1 b1f7 df56 d5d7 6df6 e310  ..$t.....V..m...
-00001040: 2ef3 91db 4432 a719 9c49 353f 8aef 6a13  ....D2...I5?..j.
-00001050: 3d99 0bb9 a9c7 48a3 53ca 961c 53fd c9f4  =.....H.S...S...
-00001060: 28c2 49d3 89bb 0374 ab99 6aae 016a 8966  (.I....t..j..j.f
-00001070: 4465 0d55 d380 3145 e411 4124 a304 136a  De.U..1E..A$...j
-00001080: 26c1 617a 597f b248 ada7 b1ff 4052 d630  &.azY..H....@R.0
-00001090: 2bba 67ea 6459 b29c 2c6f afbe 8d5b dd81  +.g.dY..,o...[..
-000010a0: 8b52 3ab2 e8e1 c93a 03c4 d0f9 2255 68cb  .R:....:...."Uh.
-000010b0: 5568 f946 693a 48a9 ef1c 702d 38e1 1314  Uh.Fi:H...p-8...
-000010c0: c1f1 a26d 7967 6bac 242f 7804 6702 8f95  ...mygk.$/x.g...
-000010d0: f22a ff0f 9974 3df2 c980 57ae b57c 79a4  .*...t=...W..|y.
-000010e0: 70df 9bbe 474c 8cf3 bd54 3bb0 55d5 7613  p...GL...T;.U.v.
-000010f0: 72ce 278f ba5b 59fe ee8d efd9 34b5 aed6  r.'..[Y.....4...
-00001100: 509b 4ab6 6c3e 295b 89ca 92a8 d38a 60d9  P.J.l>)[......`.
-00001110: 9cf2 38df b7a3 33db 61b9 29c9 8d36 ffe1  ..8...3.a.)..6..
-00001120: 3462 69cd c336 5cc5 2e15 2f44 9c0f 2df2  4bi..6\.../D..-.
-00001130: 1931 d7f5 2251 5783 5941 e4ec 85e6 e690  .1.."QW.YA......
-00001140: 5db3 9335 5b76 dbfd c37b 284e a7ff fe32  ]..5[v...{(N...2
-00001150: caad dd76 b91a 2af9 6bae 289d a9dc 4ee0  ...v..*.k.(...N.
-00001160: c885 654d 4b8e 40ef ce8b dd39 0141 e08b  ..eMK.@....9.A..
-00001170: cc35 457d 6af1 3d60 19da 4fd7 4ee0 94ad  .5E}j.=`..O.N...
-00001180: 5b98 0aab a61e 6e01 85a4 bee6 ee0b 103e  [.....n........>
-00001190: 59fd 8673 f347 6a48 c6ef 6a94 a8ba 5f86  Y..s.GjH..j..._.
-000011a0: 8b65 9e47 c8b5 cdd5 6d65 ff27 fc7d 6cf2  .e.G....me.'.}l.
-000011b0: e1c4 13f2 874e 4218 ffe8 a1db 2e7f b72f  .....NB......../
-000011c0: c048 a422 756a 7310 e02f 1e2c 0f71 f76e  .H."ujs../.,.q.n
-000011d0: b69f a895 68bc 005c 7a72 4be9 0b98 a5a4  ....h..\zrK.....
-000011e0: f754 e2f9 c625 488e 9d9b 6bfe 656a ac28  .T...%H...k.ej.(
-000011f0: 5d63 d471 7fbd 6389 834c 9bd0 5c76 0fb9  ]c.q..c..L..\v..
-00001200: 53e2 8764 8fa6 ea94 91bd e3b8 09ab 4d51  S..d..........MQ
-00001210: fc4b a3c9 2db5 61ba 2fcc 8d5a dff1 fc9f  .K..-.a./..Z....
-00001220: 8b0a 3ed2 ebbb 7b14 308e a745 428e 69fc  ..>...{.0..EB.i.
-00001230: 7139 2da8 aca9 4266 c9b8 eb5f 2dcc db40  q9-...Bf..._-..@
-00001240: 7fd9 7d41 2822 84d2 518f 64f8 ccc1 d71f  ..}A("..Q.d.....
-00001250: 671a 2b68 75ea d04d a257 1e59 4dfa feeb  g.+hu..M.W.YM...
-00001260: 1360 f370 15fc c669 dbb1 a926 b65c b395  .`.p...i...&.\..
-00001270: bf38 127c 484b 43c5 cebb 4995 f783 78c2  .8.|HKC...I...x.
-00001280: cdd9 9c95 0776 98ac f3d0 8520 b64e 3238  .....v..... .N28
-00001290: 8a76 e307 f185 b9c7 4f52 6c92 bfac 8d5f  .v......ORl...._
-000012a0: 1836 5b80 ef61 030e 603c cef4 2e6e e7c9  .6[..a..`<...n..
-000012b0: 3abf f3a6 3083 fa20 e529 f122 80a6 f834  :...0.. .)."...4
-000012c0: 34a8 cbe0 2ced 40a4 6594 0191 c722 1d02  4...,.@.e...."..
-000012d0: 3cf8 9eb1 9b2f a41e 3051 2697 55de 59e9  <..../..0Q&.U.Y.
-000012e0: ac01 7a61 7cb2 830e d6dc 45d0 4064 a230  ..za|.....E.@d.0
-000012f0: 88c9 b9b0 0a73 f3b0 828e f1eb c6cf 41a5  .....s........A.
-00001300: f1e7 b1f4 f7c0 0000 584d 5020 9a03 0000  ........XMP ....
-00001310: 3c78 3a78 6d70 6d65 7461 2078 6d6c 6e73  <x:xmpmeta xmlns
-00001320: 3a78 3d22 6164 6f62 653a 6e73 3a6d 6574  :x="adobe:ns:met
-00001330: 612f 2220 783a 786d 7074 6b3d 2258 4d50  a/" x:xmptk="XMP
-00001340: 2043 6f72 6520 362e 302e 3022 3e0a 2020   Core 6.0.0">.  
-00001350: 203c 7264 663a 5244 4620 786d 6c6e 733a   <rdf:RDF xmlns:
-00001360: 7264 663d 2268 7474 703a 2f2f 7777 772e  rdf="http://www.
-00001370: 7733 2e6f 7267 2f31 3939 392f 3032 2f32  w3.org/1999/02/2
-00001380: 322d 7264 662d 7379 6e74 6178 2d6e 7323  2-rdf-syntax-ns#
-00001390: 223e 0a20 2020 2020 203c 7264 663a 4465  ">.      <rdf:De
-000013a0: 7363 7269 7074 696f 6e20 7264 663a 6162  scription rdf:ab
-000013b0: 6f75 743d 2222 0a20 2020 2020 2020 2020  out="".         
-000013c0: 2020 2078 6d6c 6e73 3a65 7869 663d 2268     xmlns:exif="h
-000013d0: 7474 703a 2f2f 6e73 2e61 646f 6265 2e63  ttp://ns.adobe.c
-000013e0: 6f6d 2f65 7869 662f 312e 302f 220a 2020  om/exif/1.0/".  
-000013f0: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
-00001400: 7469 6666 3d22 6874 7470 3a2f 2f6e 732e  tiff="http://ns.
-00001410: 6164 6f62 652e 636f 6d2f 7469 6666 2f31  adobe.com/tiff/1
-00001420: 2e30 2f22 0a20 2020 2020 2020 2020 2020  .0/".           
-00001430: 2078 6d6c 6e73 3a78 6d70 3d22 6874 7470   xmlns:xmp="http
-00001440: 3a2f 2f6e 732e 6164 6f62 652e 636f 6d2f  ://ns.adobe.com/
-00001450: 7861 702f 312e 302f 223e 0a20 2020 2020  xap/1.0/">.     
-00001460: 2020 2020 3c65 7869 663a 5069 7865 6c59      <exif:PixelY
-00001470: 4469 6d65 6e73 696f 6e3e 3435 3c2f 6578  Dimension>45</ex
-00001480: 6966 3a50 6978 656c 5944 696d 656e 7369  if:PixelYDimensi
-00001490: 6f6e 3e0a 2020 2020 2020 2020 203c 6578  on>.         <ex
-000014a0: 6966 3a50 6978 656c 5844 696d 656e 7369  if:PixelXDimensi
-000014b0: 6f6e 3e38 303c 2f65 7869 663a 5069 7865  on>80</exif:Pixe
-000014c0: 6c58 4469 6d65 6e73 696f 6e3e 0a20 2020  lXDimension>.   
-000014d0: 2020 2020 2020 3c74 6966 663a 5265 736f        <tiff:Reso
-000014e0: 6c75 7469 6f6e 556e 6974 3e32 3c2f 7469  lutionUnit>2</ti
-000014f0: 6666 3a52 6573 6f6c 7574 696f 6e55 6e69  ff:ResolutionUni
-00001500: 743e 0a20 2020 2020 2020 2020 3c74 6966  t>.         <tif
-00001510: 663a 5852 6573 6f6c 7574 696f 6e3e 3732  f:XResolution>72
-00001520: 3030 3030 2f31 3030 3030 3c2f 7469 6666  0000/10000</tiff
-00001530: 3a58 5265 736f 6c75 7469 6f6e 3e0a 2020  :XResolution>.  
-00001540: 2020 2020 2020 203c 7469 6666 3a4f 7269         <tiff:Ori
-00001550: 656e 7461 7469 6f6e 3e31 3c2f 7469 6666  entation>1</tiff
-00001560: 3a4f 7269 656e 7461 7469 6f6e 3e0a 2020  :Orientation>.  
-00001570: 2020 2020 2020 203c 7469 6666 3a59 5265         <tiff:YRe
-00001580: 736f 6c75 7469 6f6e 3e37 3230 3030 302f  solution>720000/
-00001590: 3130 3030 303c 2f74 6966 663a 5952 6573  10000</tiff:YRes
-000015a0: 6f6c 7574 696f 6e3e 0a20 2020 2020 2020  olution>.       
-000015b0: 2020 3c78 6d70 3a4d 6574 6164 6174 6144    <xmp:MetadataD
-000015c0: 6174 653e 3230 3234 2d30 342d 3037 5432  ate>2024-04-07T2
-000015d0: 313a 3532 3a32 382b 3038 3a30 303c 2f78  1:52:28+08:00</x
-000015e0: 6d70 3a4d 6574 6164 6174 6144 6174 653e  mp:MetadataDate>
-000015f0: 0a20 2020 2020 2020 2020 3c78 6d70 3a43  .         <xmp:C
-00001600: 7265 6174 6f72 546f 6f6c 3e50 6978 656c  reatorTool>Pixel
-00001610: 6d61 746f 7220 5072 6f20 332e 352e 373c  mator Pro 3.5.7<
-00001620: 2f78 6d70 3a43 7265 6174 6f72 546f 6f6c  /xmp:CreatorTool
-00001630: 3e0a 2020 2020 2020 2020 203c 786d 703a  >.         <xmp:
-00001640: 4372 6561 7465 4461 7465 3e32 3032 342d  CreateDate>2024-
-00001650: 3034 2d30 3154 3133 3a33 323a 3339 2b30  04-01T13:32:39+0
-00001660: 383a 3030 3c2f 786d 703a 4372 6561 7465  8:00</xmp:Create
-00001670: 4461 7465 3e0a 2020 2020 2020 3c2f 7264  Date>.      </rd
-00001680: 663a 4465 7363 7269 7074 696f 6e3e 0a20  f:Description>. 
-00001690: 2020 3c2f 7264 663a 5244 463e 0a3c 2f78    </rdf:RDF>.</x
-000016a0: 3a78 6d70 6d65 7461 3e0a                 :xmpmeta>.
+00000c70: 5048 6902 0000 0190 866d db11 4dd5 f4d9  PHi......m..M...
+00000c80: 36d6 b66d dbb6 6ddb b66d dbb6 6ddb f60e  6..m..m..m..m...
+00000c90: eaed 7d9e 459a 9ac5 cf88 9800 e69f d0dd  ..}.E...........
+00000ca0: d73f 3626 34c0 9d75 09ac 7fc6 c6cb 0e1d  .?6&4..u........
+00000cb0: bc73 efea e94d 931b 670a 604d e69e beeb  .s...M..g.`M....
+00000cc0: be17 02a0 2279 73b8 55a8 99dc b28c b92f  ...."ys.U....../
+00000cd0: a256 fbbe ea01 a689 1df2 98a0 9edf d7e7  .V..............
+00000ce0: b098 82cb 735c 429d e161 6d77 1358 2ade  ....s\B..amw.X*.
+00000cf0: 01d4 ff5d 5f3f c3f1 359e a253 addd 78a3  ...]_?..5..S..x.
+00000d00: 957a 894e 7e5d 8b33 56cc 5174 fafd 9c46  .z.N~].3V.Qt...F
+00000d10: 6203 a648 ce83 3db1 86e1 625b efb3 a201  b..H..=...b[....
+00000d20: c996 6a91 1c1f 196c 710a 9bb4 51fb 2c3d  ..j....lq...Q.,=
+00000d30: ae88 6850 fb85 09a3 af9e 1914 e104 36d7  ..hP..........6.
+00000d40: 5922 bc22 6864 4014 d624 d18b 8d6f 7105  Y"."hd@..$...oq.
+00000d50: 4d29 edcb c1eb 12d4 f1aa 8026 a5d7 db86  M).........&....
+00000d60: 69e3 b2ad 73a0 79e1 d38a 1c16 0dee 75ee  i...s.y.......u.
+00000d70: 5054 0d06 4314 4f97 b3a8 e25b 3da0 6872  PT..C.O....[=.hr
+00000d80: b856 9055 93ef 399a 9f1e 4da1 829f 0b2e  .V.U..9...M.....
+00000d90: 00c9 6c0f a5c8 0b08 2e00 9fa4 542a f009  ..l.........T*..
+00000da0: 5da2 505d a981 c335 6017 a56a 3673 8987  ].P]...5`..j6s..
+00000db0: 6c32 a491 528a 2bd4 2494 fe06 cf04 99c7  l2..R.+.$.......
+00000dc0: e995 2c5d be83 3900 55c3 2437 2526 c929  ..,]..9.U.$7%&.)
+00000dd0: c91c eae9 9b3c 8c4a 8f89 0218 05d4 8144  .....<.J.......D
+00000de0: a91c b57f 1ee1 ae86 4972 4ea4 5ac8 d52f  ........IrN.Z../
+00000df0: ba00 ca03 fc86 4041 86d8 3e2d 0861 54b3  ......@A..>-.aT.
+00000e00: 159f d825 0dc2 de0f ba28 4b54 469e d884  ...%.....(KTF...
+00000e10: cfc3 8319 8d7c c51b 4492 5469 7e7a 1dd4  .....|..D.Ti~z..
+00000e20: a906 d141 5f36 f364 3473 1916 7f06 00fd  ...A_6.d4s......
+00000e30: 760e 15f5 0200 e954 719e d1d3 bbe2 e637  v......Tq......7
+00000e40: 543f 6243 ddc5 6b83 93b0 8cce ded9 c63e  T?bC..k........>
+00000e50: a07a e90e 9ff6 b788 e518 275a d2f6 3bf6  .z........'Z..;.
+00000e60: 811a 0200 11bf 9d1a 9a3f 8071 3617 94b7  .........?.q6...
+00000e70: e7da 6b1f e96f 00a0 0200 400d 91c4 cf97  ..k..o....@.....
+00000e80: 1655 09e5 1863 ba47 e66a 3de3 e0e3 ef80  .U...c.G.j=.....
+00000e90: 6a89 4808 5019 d1fa eae2 eab6 79c3 79c6  j.H.P.......y.y.
+00000ea0: d0ac 4f92 629d 27ad 3e70 fdd9 9b77 efde  ..O.b.'.>p...w..
+00000eb0: 7df8 fadd 6afd f2f6 f1b5 a39b e70e ac51  }...j..........Q
+00000ec0: 386d 881b 634e 96f7 0e4f 9e36 43c6 8c99  8m..cN...O.6C...
+00000ed0: f315 2a5c 384f 8624 e1be ee1c f39f 1100  ..*\8O.$........
+00000ee0: 5650 3820 a803 0000 7013 009d 012a 5000  VP8 ....p....*P.
+00000ef0: 2d00 3e9d 3e9a 4825 a322 a12c d80d 50b0  -.>.>.H%.".,..P.
+00000f00: 1389 6c00 bb30 1050 bf4c 5f1f b790 58a1  ..l..0.P.L_...X.
+00000f10: 31fa 0379 f799 cc78 8de5 af26 6cd1 afe0  1..y...x...&l...
+00000f20: 1d9d f7bf e44c 1ad6 c7bd f958 b093 4d3b  .....L.....X..M;
+00000f30: 406f 0c68 7d66 dbfc 0972 8518 b0d7 202e  @o.h}f...r.... .
+00000f40: 64dd ddbd 9d9e ce1f bba2 aa65 d7d6 dc62  d..........e...b
+00000f50: 0b1b d3a7 1667 69a9 49c0 a5fa 4e42 10e6  .....gi.I...NB..
+00000f60: 6b15 84fd b661 8336 c4f7 f266 d9d5 db9f  k....a.6...f....
+00000f70: f74b e13e a542 1fe5 6d82 bf2e 6a29 97bb  .K.>.B..m...j)..
+00000f80: 4c19 6ef8 c1fc 213b 4c85 8c00 00fe df06  L.n...!;L.......
+00000f90: a3fe 69d1 f7dd 939f aa8e 5adf 6043 30db  ..i.......Z.`C0.
+00000fa0: a320 0be2 1d40 ce56 d015 0bea 95c3 7808  . ...@.V......x.
+00000fb0: 07b6 6e2c 06af b4b7 7555 b9d9 0fe7 ee04  ..n,....uU......
+00000fc0: a387 21c2 a7f1 44e6 ea45 9c17 4e90 23c2  ..!...D..E..N.#.
+00000fd0: 6348 c3f8 79c9 8273 f562 dde4 f862 193a  cH..y..s.b...b.:
+00000fe0: b37e 6b14 0465 3cf2 2fcd 944a d91e d50f  .~k..e<./..J....
+00000ff0: bc97 538e 5bd2 25f9 dbbb 47ac 7562 6816  ..S.[.%...G.ubh.
+00001000: b49c f073 1a2e a7f6 73c2 b491 dbe7 d9e8  ...s....s.......
+00001010: 05e7 5da6 b60c 7921 ea89 055f 2666 c5bb  ..]...y!..._&f..
+00001020: 0fd0 083f 2332 dc68 b460 5d82 136f fa67  ...?#2.h.`]..o.g
+00001030: cb24 8c4b ec50 16cc c9c4 9226 6256 cbf9  .$.K.P.....&bV..
+00001040: c349 a914 57eb 7c9a e18b 2c01 0927 46da  .I..W.|...,..'F.
+00001050: 6698 5fda 3023 7d68 582f 91b9 5bee fd20  f._.0#}hX/..[.. 
+00001060: c7ea 7e12 c344 5327 ea6b 5c01 c96f 3e81  ..~..DS'.k\..o>.
+00001070: 4743 58f6 62ac 954b f142 afbc 21be b4b8  GCX.b..K.B..!...
+00001080: f968 a656 8f4e 4b8a 25dd 217f 16b1 0cee  .h.V.NK.%.!.....
+00001090: be07 1245 ca53 f0ad 6388 e11d 8aa1 a9e9  ...E.S..c.......
+000010a0: 2ea4 1f25 3d51 3a4b ecac a077 e854 ef29  ...%=Q:K...w.T.)
+000010b0: 9120 520b b4d1 f77c 839a 120f 94fd daa4  . R....|........
+000010c0: a812 4a21 1370 05db 330a 6fa8 9fd2 d417  ..J!.p..3.o.....
+000010d0: eeda b445 c587 7f99 630f 47da 35a5 bb75  ...E....c.G.5..u
+000010e0: c557 56de 35a4 46a9 0339 3ea7 677a b155  .WV.5.F..9>.gz.U
+000010f0: 8ec2 f848 23ec 5eda 20e1 fe86 da7b 47ab  ...H#.^. ....{G.
+00001100: 699f c4e8 5906 29b8 cfa2 f59b ffb2 ca15  i...Y.).........
+00001110: c53f 95dc 0006 351e b9ec 6f4a 8b2b ea75  .?....5...oJ.+.u
+00001120: 5b9f 6452 00dc 678a b80b db97 93c5 cf14  [.dR..g.........
+00001130: 08d5 8335 66fc 02f8 aa30 3859 be56 cb9d  ...5f....08Y.V..
+00001140: bccd bfde f027 5ae0 9133 bf76 eeb1 99ca  .....'Z..3.v....
+00001150: fe38 ba3c 8a84 f290 9f63 d66e f4b8 4e7a  .8.<.....c.n..Nz
+00001160: 9fae 777d daa7 e86d b08b c305 5fa4 26be  ..w}...m...._.&.
+00001170: 2b43 b236 8421 990d 5623 973c 2c35 2844  +C.6.!..V#.<,5(D
+00001180: ced7 38d9 9c3d 5bfe d572 76fa 069c 3a8f  ..8..=[..rv...:.
+00001190: cae6 acf0 1627 6881 f57c 6238 af88 2d69  .....'h..|b8..-i
+000011a0: 07e7 4ede ae2e e0a4 f3e0 fb1e 1187 7098  ..N...........p.
+000011b0: eb1a cf3a a2e1 4b3f dcb2 29d6 537f 14ce  ...:..K?..).S...
+000011c0: 9238 5cb6 6054 c047 d231 1e6f 83a2 bfd3  .8\.`T.G.1.o....
+000011d0: 7fb1 fc56 db3f 665b 18ba 13b4 135a aa57  ...V.?f[.....Z.W
+000011e0: c0e7 d35b a336 bbc0 0e18 b3e8 2ee5 5584  ...[.6........U.
+000011f0: 6eb5 6f40 f6b2 fabb b362 40ea b98a 50a5  n.o@.....b@...P.
+00001200: 3009 56a1 3037 387e e088 3119 8039 9d29  0.V.078~..1..9.)
+00001210: 2866 d5a9 bf71 be70 3107 8ccc 818b cc4e  (f...q.p1......N
+00001220: b7e4 2ea8 62b1 2409 52dd db0b 5a9f b8c1  ....b.$.R...Z...
+00001230: 6e84 cefb e520 f8dc 4780 8920 1816 adf0  n.... ..G.. ....
+00001240: 168f d49b 4a2f bf1e 3e97 d13d 74f4 cd70  ....J/..>..=t..p
+00001250: 9f3f b972 c821 4a98 7c64 c7f5 53f7 3ce7  .?.r.!J.|d..S.<.
+00001260: f2b2 2119 a307 6cd7 215a ce62 4e69 ca32  ..!...l.!Z.bNi.2
+00001270: b665 b8a7 022a 3bfb e82d 64e9 8eda cfc4  .e...*;..-d.....
+00001280: 4e02 fc88 dc44 66c0 d408 c61b 1b60 0000  N....Df......`..
+00001290: 584d 5020 9a03 0000 3c78 3a78 6d70 6d65  XMP ....<x:xmpme
+000012a0: 7461 2078 6d6c 6e73 3a78 3d22 6164 6f62  ta xmlns:x="adob
+000012b0: 653a 6e73 3a6d 6574 612f 2220 783a 786d  e:ns:meta/" x:xm
+000012c0: 7074 6b3d 2258 4d50 2043 6f72 6520 362e  ptk="XMP Core 6.
+000012d0: 302e 3022 3e0a 2020 203c 7264 663a 5244  0.0">.   <rdf:RD
+000012e0: 4620 786d 6c6e 733a 7264 663d 2268 7474  F xmlns:rdf="htt
+000012f0: 703a 2f2f 7777 772e 7733 2e6f 7267 2f31  p://www.w3.org/1
+00001300: 3939 392f 3032 2f32 322d 7264 662d 7379  999/02/22-rdf-sy
+00001310: 6e74 6178 2d6e 7323 223e 0a20 2020 2020  ntax-ns#">.     
+00001320: 203c 7264 663a 4465 7363 7269 7074 696f   <rdf:Descriptio
+00001330: 6e20 7264 663a 6162 6f75 743d 2222 0a20  n rdf:about="". 
+00001340: 2020 2020 2020 2020 2020 2078 6d6c 6e73             xmlns
+00001350: 3a65 7869 663d 2268 7474 703a 2f2f 6e73  :exif="http://ns
+00001360: 2e61 646f 6265 2e63 6f6d 2f65 7869 662f  .adobe.com/exif/
+00001370: 312e 302f 220a 2020 2020 2020 2020 2020  1.0/".          
+00001380: 2020 786d 6c6e 733a 7469 6666 3d22 6874    xmlns:tiff="ht
+00001390: 7470 3a2f 2f6e 732e 6164 6f62 652e 636f  tp://ns.adobe.co
+000013a0: 6d2f 7469 6666 2f31 2e30 2f22 0a20 2020  m/tiff/1.0/".   
+000013b0: 2020 2020 2020 2020 2078 6d6c 6e73 3a78           xmlns:x
+000013c0: 6d70 3d22 6874 7470 3a2f 2f6e 732e 6164  mp="http://ns.ad
+000013d0: 6f62 652e 636f 6d2f 7861 702f 312e 302f  obe.com/xap/1.0/
+000013e0: 223e 0a20 2020 2020 2020 2020 3c65 7869  ">.         <exi
+000013f0: 663a 5069 7865 6c59 4469 6d65 6e73 696f  f:PixelYDimensio
+00001400: 6e3e 3435 3c2f 6578 6966 3a50 6978 656c  n>45</exif:Pixel
+00001410: 5944 696d 656e 7369 6f6e 3e0a 2020 2020  YDimension>.    
+00001420: 2020 2020 203c 6578 6966 3a50 6978 656c       <exif:Pixel
+00001430: 5844 696d 656e 7369 6f6e 3e38 303c 2f65  XDimension>80</e
+00001440: 7869 663a 5069 7865 6c58 4469 6d65 6e73  xif:PixelXDimens
+00001450: 696f 6e3e 0a20 2020 2020 2020 2020 3c74  ion>.         <t
+00001460: 6966 663a 5265 736f 6c75 7469 6f6e 556e  iff:ResolutionUn
+00001470: 6974 3e32 3c2f 7469 6666 3a52 6573 6f6c  it>2</tiff:Resol
+00001480: 7574 696f 6e55 6e69 743e 0a20 2020 2020  utionUnit>.     
+00001490: 2020 2020 3c74 6966 663a 5852 6573 6f6c      <tiff:XResol
+000014a0: 7574 696f 6e3e 3732 3030 3030 2f31 3030  ution>720000/100
+000014b0: 3030 3c2f 7469 6666 3a58 5265 736f 6c75  00</tiff:XResolu
+000014c0: 7469 6f6e 3e0a 2020 2020 2020 2020 203c  tion>.         <
+000014d0: 7469 6666 3a4f 7269 656e 7461 7469 6f6e  tiff:Orientation
+000014e0: 3e31 3c2f 7469 6666 3a4f 7269 656e 7461  >1</tiff:Orienta
+000014f0: 7469 6f6e 3e0a 2020 2020 2020 2020 203c  tion>.         <
+00001500: 7469 6666 3a59 5265 736f 6c75 7469 6f6e  tiff:YResolution
+00001510: 3e37 3230 3030 302f 3130 3030 303c 2f74  >720000/10000</t
+00001520: 6966 663a 5952 6573 6f6c 7574 696f 6e3e  iff:YResolution>
+00001530: 0a20 2020 2020 2020 2020 3c78 6d70 3a4d  .         <xmp:M
+00001540: 6574 6164 6174 6144 6174 653e 3230 3234  etadataDate>2024
+00001550: 2d30 342d 3037 5432 313a 3532 3a34 322b  -04-07T21:52:42+
+00001560: 3038 3a30 303c 2f78 6d70 3a4d 6574 6164  08:00</xmp:Metad
+00001570: 6174 6144 6174 653e 0a20 2020 2020 2020  ataDate>.       
+00001580: 2020 3c78 6d70 3a43 7265 6174 6f72 546f    <xmp:CreatorTo
+00001590: 6f6c 3e50 6978 656c 6d61 746f 7220 5072  ol>Pixelmator Pr
+000015a0: 6f20 332e 352e 373c 2f78 6d70 3a43 7265  o 3.5.7</xmp:Cre
+000015b0: 6174 6f72 546f 6f6c 3e0a 2020 2020 2020  atorTool>.      
+000015c0: 2020 203c 786d 703a 4372 6561 7465 4461     <xmp:CreateDa
+000015d0: 7465 3e32 3032 342d 3034 2d30 3154 3133  te>2024-04-01T13
+000015e0: 3a33 323a 3339 2b30 383a 3030 3c2f 786d  :32:39+08:00</xm
+000015f0: 703a 4372 6561 7465 4461 7465 3e0a 2020  p:CreateDate>.  
+00001600: 2020 2020 3c2f 7264 663a 4465 7363 7269      </rdf:Descri
+00001610: 7074 696f 6e3e 0a20 2020 3c2f 7264 663a  ption>.   </rdf:
+00001620: 5244 463e 0a3c 2f78 3a78 6d70 6d65 7461  RDF>.</x:xmpmeta
+00001630: 3e0a                                     >.
```

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_001.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_002.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_003.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg1/cambg_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_001.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_001.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_002.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_002.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_003.webp` & `SightTraining-0.1.20/spacedefense/assets/images/vmove_cambg2/cambg_003.webp`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/.DS_Store` & `SightTraining-0.1.20/spacedefense/assets/sounds/.DS_Store`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/bgm3.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/bgm.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/fire.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/fire_blast.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/fire_blast.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/firehit.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/smyf_join.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/smyf_join.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_angry.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_angry.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_loss.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_end_loss.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_win.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_end_win.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_mid.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_mid.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_pre.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_pre.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/stage_start.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/stage_start.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/sufo_join.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/sufo_join.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/super_fire.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/super_fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/super_firehit.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/super_firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/ufo_fire.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/ufo_fire.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/assets/sounds/ufo_firehit.ogg` & `SightTraining-0.1.20/spacedefense/assets/sounds/ufo_firehit.ogg`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/common.py` & `SightTraining-0.1.20/spacedefense/common.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/config.py` & `SightTraining-0.1.20/spacedefense/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 configmap = {
     "display_width": 1280,
     "display_height": 720,
     "fullscreen": False,
     "game_time": 600,
     "bgm": {
-        "sound": "sounds/bgm3.ogg",
+        "sound": "sounds/bgm.ogg",
         "sound_volume": 1.0,
     },
     "game_cover": {
         "cover_image": "images/game_cover.webp",
         "cover_win": "images/game_cover_win.webp",
         "cover_loss": "images/game_cover_loss.webp",
     },
@@ -23,15 +23,14 @@
         "type": "vmove",
     },
     "stage_angry": {
         "sound": "sounds/stage_angry.ogg",
         "sound_volume": 0.4,
     },
     "stage_pre": {
-        "images": "images/stage_pre.png",
         "sound": "sounds/stage_pre.ogg",
         "sound_volume": 0.4,
     },
     "stage_start": {
         "sound": "sounds/stage_start.ogg",
         "sound_volume": 0.4,
     },
@@ -52,15 +51,15 @@
         "sound_volume": 0.4,
     },
     "my_score_step": 5,
     "ufo_score_step": 3,
     "unit_collision_cooldown": 1000,
     "ufo_master": {
         "image_sequence": "images/ufo_master",
-        "images": ["images/ufo_master.png"],
+        "images": ["images/ufo_master/ufo_master_001.webp"],
         "first_pos": (720, 100),
         "life_value": 30000,
         "shield_value": 1000,
         "shield_recharge_step": 1,
         "bullet_color": "cyan",
         "bullet_speed": 7,
         "bullet_damage": 20,
@@ -72,15 +71,15 @@
         "fire_sound": "sounds/ufo_fire.ogg",
         "firehit_sound": "sounds/ufo_firehit.ogg",
         "fire_sound_volume": 0.4,
         "firehit_sound_volume": 0.4,
     },
     "ufo_slave": {
         "image_sequence": "images/ufo_slave",
-        "images": ["images/ufo_slave1.png", "images/ufo_slave2.png"],
+        "images": ["images/ufo_slave/ufo_slave_001.webp", "images/ufo_slave/ufo_slave_002.webp"],
         "first_pos": (400, -100),
         "score_cast": 50,
         "max_limit": 8,
         "min_limit": 3,
         "shield_value": 100,
         "shield_recharge_step": 5,
         "life_value": 500,
@@ -98,15 +97,15 @@
     },
     "myf_master": {
         "life_value": 700,
         "shield_value": 300,
         "shield_recharge_step": 3,
         "speed_x": 8,
         "image_sequence": "images/myf_master",
-        "image": "images/master_fighter.webp",
+        "image": "images/myf_master/myf_master_001.webp",
         "firehit_sound": "sounds/firehit.ogg",
         "fire_sound_volume": 0.4,
         "firehit_sound_volume": 0.4,
         "upgrade_cast": 100,
         "level1": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 2,
```

### Comparing `SightTraining-0.1.19/spacedefense/flight_unit.py` & `SightTraining-0.1.20/spacedefense/flight_unit.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/game.py` & `SightTraining-0.1.20/spacedefense/game.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/my_master.py` & `SightTraining-0.1.20/spacedefense/my_master.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/scene_main.py` & `SightTraining-0.1.20/spacedefense/scene_main.py`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.19/spacedefense/scenes.py` & `SightTraining-0.1.20/spacedefense/scenes.py`

 * *Files identical despite different names*

