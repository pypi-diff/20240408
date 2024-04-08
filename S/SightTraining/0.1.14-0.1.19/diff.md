# Comparing `tmp/SightTraining-0.1.14.tar.gz` & `tmp/SightTraining-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SightTraining-0.1.14.tar", last modified: Mon Apr  1 09:36:22 2024, max compression
+gzip compressed data, was "SightTraining-0.1.19.tar", last modified: Mon Apr  8 02:57:12 2024, max compression
```

## Comparing `SightTraining-0.1.14.tar` & `SightTraining-0.1.19.tar`

### file list

```diff
@@ -1,20 +1,84 @@
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:36:22.156798 SightTraining-0.1.14/
--rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.14/LICENSE
--rw-r--r--   0 wangjuntao   (501) staff       (20)       45 2024-04-01 09:34:56.000000 SightTraining-0.1.14/MANIFEST.in
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:36:22.156469 SightTraining-0.1.14/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.14/Readme.md
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:36:22.155754 SightTraining-0.1.14/SightTraining.egg-info/
--rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/PKG-INFO
--rw-r--r--   0 wangjuntao   (501) staff       (20)      387 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/SOURCES.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/dependency_links.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/entry_points.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/requires.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-01 09:36:22.000000 SightTraining-0.1.14/SightTraining.egg-info/top_level.txt
--rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-01 09:36:22.156851 SightTraining-0.1.14/setup.cfg
--rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-01 09:36:19.000000 SightTraining-0.1.14/setup.py
-drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-01 09:36:22.155319 SightTraining-0.1.14/spacedefense/
--rw-r--r--   0 wangjuntao   (501) staff       (20)       64 2024-04-01 09:31:18.000000 SightTraining-0.1.14/spacedefense/__init__.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    31552 2024-04-01 09:20:04.000000 SightTraining-0.1.14/spacedefense/actors.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     2239 2024-04-01 09:01:37.000000 SightTraining-0.1.14/spacedefense/common.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)     4980 2024-04-01 08:48:15.000000 SightTraining-0.1.14/spacedefense/config.py
--rw-r--r--   0 wangjuntao   (501) staff       (20)    24303 2024-04-01 09:19:50.000000 SightTraining-0.1.14/spacedefense/main.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.100620 SightTraining-0.1.19/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1067 2024-03-26 11:06:37.000000 SightTraining-0.1.19/LICENSE
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       58 2024-04-01 09:37:31.000000 SightTraining-0.1.19/MANIFEST.in
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 02:57:12.100291 SightTraining-0.1.19/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      211 2024-03-27 13:26:23.000000 SightTraining-0.1.19/Readme.md
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.099895 SightTraining-0.1.19/SightTraining.egg-info/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      539 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/PKG-INFO
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2967 2024-04-08 02:57:12.000000 SightTraining-0.1.19/SightTraining.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)        1 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       49 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/entry_points.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       35 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/requires.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       13 2024-04-08 02:57:11.000000 SightTraining-0.1.19/SightTraining.egg-info/top_level.txt
+-rw-r--r--   0 wangjuntao   (501) staff       (20)       38 2024-04-08 02:57:12.101150 SightTraining-0.1.19/setup.cfg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)      882 2024-04-01 18:49:57.000000 SightTraining-0.1.19/setup.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.065717 SightTraining-0.1.19/spacedefense/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     1261 2024-04-07 13:38:55.000000 SightTraining-0.1.19/spacedefense/__init__.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    17516 2024-04-08 01:33:20.000000 SightTraining-0.1.19/spacedefense/actors.py
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.065892 SightTraining-0.1.19/spacedefense/assets/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10244 2024-04-08 02:55:20.000000 SightTraining-0.1.19/spacedefense/assets/.DS_Store
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.072018 SightTraining-0.1.19/spacedefense/assets/images/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18436 2024-04-08 02:55:20.000000 SightTraining-0.1.19/spacedefense/assets/images/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    93950 2024-04-08 02:52:13.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   115516 2024-04-08 02:53:25.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover_loss.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   129152 2024-04-08 02:53:06.000000 SightTraining-0.1.19/spacedefense/assets/images/game_cover_win.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    31179 2024-04-01 06:54:20.000000 SightTraining-0.1.19/spacedefense/assets/images/icon.png
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7138 2024-04-07 13:31:54.000000 SightTraining-0.1.19/spacedefense/assets/images/master_fighter.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6772 2024-04-07 13:57:36.000000 SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6578 2024-04-07 13:59:55.000000 SightTraining-0.1.19/spacedefense/assets/images/my_slave_fighter2.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.074867 SightTraining-0.1.19/spacedefense/assets/images/myf_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:42:44.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7568 2024-04-07 13:41:47.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7358 2024-04-07 13:41:55.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     7442 2024-04-07 13:42:06.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6916 2024-04-07 13:42:17.000000 SightTraining-0.1.19/spacedefense/assets/images/myf_master/myf_master_004.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    95336 2024-04-07 14:00:31.000000 SightTraining-0.1.19/spacedefense/assets/images/scale_cambg1.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5298 2024-04-08 01:24:57.000000 SightTraining-0.1.19/spacedefense/assets/images/super_bullet.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.076598 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:00.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     8908 2024-04-07 13:49:06.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9406 2024-04-07 13:49:20.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9166 2024-04-07 13:49:28.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9482 2024-04-07 13:49:58.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_master/ufo_master_004.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.077978 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:53:40.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5838 2024-04-07 13:52:06.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5676 2024-04-07 13:52:20.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5802 2024-04-07 13:52:28.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_003.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5682 2024-04-07 13:52:42.000000 SightTraining-0.1.19/spacedefense/assets/images/ufo_slave/ufo_slave_004.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.081262 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:18:10.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   323000 2024-04-07 13:16:38.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   262066 2024-04-07 13:16:50.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   322282 2024-04-07 13:17:12.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg1/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.083298 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-07 13:27:10.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   212520 2024-04-07 13:24:30.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_001.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   210670 2024-04-07 13:24:44.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_002.webp
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   221782 2024-04-07 13:25:46.000000 SightTraining-0.1.19/spacedefense/assets/images/vmove_cambg2/cambg_003.webp
+drwxr-xr-x   0 wangjuntao   (501) staff       (20)        0 2024-04-08 02:57:12.099552 SightTraining-0.1.19/spacedefense/assets/sounds/
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     6148 2024-04-01 07:13:33.000000 SightTraining-0.1.19/spacedefense/assets/sounds/.DS_Store
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   781119 2024-03-29 14:19:53.000000 SightTraining-0.1.19/spacedefense/assets/sounds/bgm1.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   613595 2024-04-01 06:38:42.000000 SightTraining-0.1.19/spacedefense/assets/sounds/bgm3.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    19873 2024-03-29 14:26:24.000000 SightTraining-0.1.19/spacedefense/assets/sounds/fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    18471 2024-03-29 14:25:00.000000 SightTraining-0.1.19/spacedefense/assets/sounds/fire_blast.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    26919 2024-03-29 14:24:28.000000 SightTraining-0.1.19/spacedefense/assets/sounds/firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    40320 2024-03-31 18:25:38.000000 SightTraining-0.1.19/spacedefense/assets/sounds/smyf_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   265674 2024-03-29 14:22:39.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_angry.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   214184 2024-03-29 14:21:15.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_loss.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   128369 2024-03-29 14:21:54.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_end_win.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   213937 2024-03-29 14:22:18.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_mid.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   295241 2024-03-29 14:22:58.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_pre.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)   224144 2024-03-29 14:23:21.000000 SightTraining-0.1.19/spacedefense/assets/sounds/stage_start.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    49560 2024-03-31 18:25:08.000000 SightTraining-0.1.19/spacedefense/assets/sounds/sufo_join.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    24129 2024-03-29 18:13:37.000000 SightTraining-0.1.19/spacedefense/assets/sounds/super_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    56632 2024-03-29 18:24:26.000000 SightTraining-0.1.19/spacedefense/assets/sounds/super_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    10368 2024-03-29 14:23:49.000000 SightTraining-0.1.19/spacedefense/assets/sounds/ufo_fire.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    12270 2024-03-29 14:24:06.000000 SightTraining-0.1.19/spacedefense/assets/sounds/ufo_firehit.ogg
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3705 2024-04-07 13:21:07.000000 SightTraining-0.1.19/spacedefense/common.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     5159 2024-04-08 02:54:18.000000 SightTraining-0.1.19/spacedefense/config.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    11805 2024-04-08 02:18:23.000000 SightTraining-0.1.19/spacedefense/flight_unit.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     2064 2024-04-07 14:10:18.000000 SightTraining-0.1.19/spacedefense/game.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     9531 2024-04-08 02:38:49.000000 SightTraining-0.1.19/spacedefense/my_master.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)    27346 2024-04-08 02:29:54.000000 SightTraining-0.1.19/spacedefense/scene_main.py
+-rw-r--r--   0 wangjuntao   (501) staff       (20)     3653 2024-04-01 17:56:03.000000 SightTraining-0.1.19/spacedefense/scenes.py
```

### Comparing `SightTraining-0.1.14/LICENSE` & `SightTraining-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `SightTraining-0.1.14/PKG-INFO` & `SightTraining-0.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.14
+Version: 0.1.19
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.14/SightTraining.egg-info/PKG-INFO` & `SightTraining-0.1.19/SightTraining.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SightTraining
-Version: 0.1.14
+Version: 0.1.19
 Summary: SightTraining  is a game for children's amblyopia training
 Author: jett.wang
 Author-email: jamiesun.net@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SightTraining-0.1.14/setup.py` & `SightTraining-0.1.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 readme = """
 SightTraining  is a game for children's amblyopia training
 """
 
 setup(
     name="SightTraining",
-    version="0.1.14",
+    version="0.1.19",
     author="jett.wang",
     author_email="jamiesun.net@gmail.com",
     description="SightTraining  is a game for children's amblyopia training",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `SightTraining-0.1.14/spacedefense/config.py` & `SightTraining-0.1.19/spacedefense/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,163 +4,167 @@
     "fullscreen": False,
     "game_time": 600,
     "bgm": {
         "sound": "sounds/bgm3.ogg",
         "sound_volume": 1.0,
     },
     "game_cover": {
-        "cover_image": "images/game_cover.png",
-        "cover_win": "images/game_cover_win.png",
-        "cover_loss": "images/game_cover_loss.png",
+        "cover_image": "images/game_cover.webp",
+        "cover_win": "images/game_cover_win.webp",
+        "cover_loss": "images/game_cover_loss.webp",
     },
     "background": {
         "vmove": {
-            "image_sequence": "images/vmove_cambg1",
-            "images": ["images/vmove_cambg1/cambg_003.png"],
+            "image_sequence_group": ["images/vmove_cambg2", "images/vmove_cambg1"],
+            "images": ["images/vmove_cambg1/cambg_003.webp"],
         },
         "scale": {
-            "image": "images/scale_cambg1.png",
+            "image": "images/scale_cambg1.webp",
         },
         "type": "vmove",
     },
     "stage_angry": {
         "sound": "sounds/stage_angry.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "stage_pre": {
         "images": "images/stage_pre.png",
         "sound": "sounds/stage_pre.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "stage_start": {
         "sound": "sounds/stage_start.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "stage_end_win": {
         "sound": "sounds/stage_end_win.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "stage_end_loss": {
         "sound": "sounds/stage_end_loss.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "sufo_join": {
         "sound": "sounds/sufo_join.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "smyf_join": {
         "sound": "sounds/smyf_join.ogg",
-        "sound_volume": 0.2,
+        "sound_volume": 0.4,
     },
     "my_score_step": 5,
     "ufo_score_step": 3,
+    "unit_collision_cooldown": 1000,
     "ufo_master": {
         "image_sequence": "images/ufo_master",
         "images": ["images/ufo_master.png"],
         "first_pos": (720, 100),
-        "life_value": 20000,
-        "shield_value": 500,
-        "shield_recharge_step": 5,
+        "life_value": 30000,
+        "shield_value": 1000,
+        "shield_recharge_step": 1,
         "bullet_color": "cyan",
         "bullet_speed": 7,
         "bullet_damage": 20,
-        "bullet_radius": 12,
+        "bullet_radius": 10,
         "trace_fire_delay": 30,
+        "fire_interceptor_delay": 20,
         "fire_delay": 30,
         "fire_score": 5,
         "fire_sound": "sounds/ufo_fire.ogg",
         "firehit_sound": "sounds/ufo_firehit.ogg",
-        "fire_sound_volume": 0.2,
-        "firehit_sound_volume": 0.2,
+        "fire_sound_volume": 0.4,
+        "firehit_sound_volume": 0.4,
     },
     "ufo_slave": {
-        "image_sequence": "images/ufo_slave2",
+        "image_sequence": "images/ufo_slave",
         "images": ["images/ufo_slave1.png", "images/ufo_slave2.png"],
         "first_pos": (400, -100),
         "score_cast": 50,
         "max_limit": 8,
         "min_limit": 3,
-        "shield_value": 50,
-        "shield_recharge_step": 10,
+        "shield_value": 100,
+        "shield_recharge_step": 5,
         "life_value": 500,
         "bullet_speed": 9,
         "bullet_color": "cyan",
         "bullet_damage": 10,
-        "bullet_radius": 10,
+        "bullet_radius": 8,
         "trace_fire_delay": 40,
+        "fire_interceptor_delay": 20,
         "fire_delay": 15,
         "fire_sound": "sounds/ufo_fire.ogg",
         "firehit_sound": "sounds/ufo_firehit.ogg",
-        "fire_sound_volume": 0.2,
-        "firehit_sound_volume": 0.2,
+        "fire_sound_volume": 0.4,
+        "firehit_sound_volume": 0.4,
     },
     "myf_master": {
         "life_value": 700,
         "shield_value": 300,
         "shield_recharge_step": 3,
         "speed_x": 8,
         "image_sequence": "images/myf_master",
-        "image": "images/master_fighter.png",
+        "image": "images/master_fighter.webp",
         "firehit_sound": "sounds/firehit.ogg",
-        "fire_sound_volume": 0.2,
-        "firehit_sound_volume": 0.2,
+        "fire_sound_volume": 0.4,
+        "firehit_sound_volume": 0.4,
+        "upgrade_cast": 100,
         "level1": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 2,
             "bullet_speed": 15,
-            "bullet_damage": 15,
-            "bullet_radius": 6,
+            "bullet_damage": 10,
+            "bullet_radius": 5,
             "fire_delay": 8,
             "fire_sound": "sounds/fire.ogg",
         },
         "level2": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 1,
             "bullet_speed": 10,
-            "bullet_damage": 30,
-            "bullet_radius": 10,
+            "bullet_damage": 40,
+            "bullet_radius": 8,
             "fire_delay": 12,
             "fire_sound": "sounds/fire.ogg",
         },
         "level3": {
             "bullet_color": "light_yellow",
             "bullet_per_num": 2,
-            "bullet_speed": 10,
+            "bullet_speed": 7,
             "bullet_damage": 3,
             "bullet_radius": 5,
             "fire_delay": 10,
             "fire_sound": "sounds/fire.ogg",
         },
         "super_bullet": {
             "score_cast": 200,
             "life_value": 300,
             "speed": 3,
             "acc_distance_1": 400,
             "acc_distance_2": 300,
-            "damage": 300,
-            "fire_delay": 300,
-            "image": "images/super_bullet.png",
+            "damage": 200,
+            "fire_delay": 200,
+            "image": "images/super_bullet.webp",
             "fire_sound": "sounds/super_fire.ogg",
             "firehit_sound": "sounds/firehit.ogg",
         },
     },
     "myf_slave": {
-        "images": ["images/my_slave_fighter1.png", "images/my_slave_fighter2.png"],
-        "first_pos": (-100, 600),
-        "shield_value": 50,
-        "shield_recharge_step": 7,
+        "images": ["images/my_slave_fighter1.webp", "images/my_slave_fighter2.webp"],
+        "first_pos": (-10, 300),
+        "shield_value": 100,
+        "shield_recharge_step": 5,
         "score_cast": 100,
         "max_limit": 7,
         "min_limit": 2,
         "life_value": 500,
         "bullet_speed": 10,
         "bullet_color": "light_yellow",
         "bullet_damage": 20,
-        "bullet_radius": 9,
+        "bullet_radius": 8,
         "fire_delay": 15,
         "trace_fire_delay": 30,
         "fire_sound": "sounds/fire.ogg",
         "firehit_sound": "sounds/firehit.ogg",
-        "fire_sound_volume": 0.2,
-        "firehit_sound_volume": 0.2,
+        "fire_sound_volume": 0.4,
+        "firehit_sound_volume": 0.4,
     },
 }
```

