# Comparing `tmp/mapdata-3.4.1.tar.gz` & `tmp/mapdata-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-3.4.1.tar", last modified: Fri Mar 22 19:33:13 2024, max compression
+gzip compressed data, was "mapdata-3.5.0.tar", last modified: Sun Apr  7 23:48:42 2024, max compression
```

## Comparing `mapdata-3.4.1.tar` & `mapdata-3.5.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.548630 mapdata-3.4.1/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.4.1/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.4.1/MANIFEST.in
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7582 2024-03-22 19:33:13.548630 mapdata-3.4.1/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     6158 2024-03-21 15:17:08.000000 mapdata-3.4.1/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.492629 mapdata-3.4.1/mapdata/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.496629 mapdata-3.4.1/mapdata/configfile/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.4.1/mapdata/configfile/mapdata.conf
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   607689 2024-03-22 19:29:11.000000 mapdata-3.4.1/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.492629 mapdata-3.4.1/mapdata/symbols/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.544630 mapdata-3.4.1/mapdata/symbols/16x16/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/0.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.4.1/mapdata/symbols/16x16/1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.4.1/mapdata/symbols/16x16/2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.4.1/mapdata/symbols/16x16/4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.4.1/mapdata/symbols/16x16/5.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.4.1/mapdata/symbols/16x16/6.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.4.1/mapdata/symbols/16x16/7.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.4.1/mapdata/symbols/16x16/9.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.4.1/mapdata/symbols/16x16/A.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.4.1/mapdata/symbols/16x16/B.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.4.1/mapdata/symbols/16x16/C.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.4.1/mapdata/symbols/16x16/D.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.4.1/mapdata/symbols/16x16/E.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.4.1/mapdata/symbols/16x16/F.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.4.1/mapdata/symbols/16x16/G.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.4.1/mapdata/symbols/16x16/H.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.4.1/mapdata/symbols/16x16/I.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.4.1/mapdata/symbols/16x16/J.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.4.1/mapdata/symbols/16x16/K.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.4.1/mapdata/symbols/16x16/L.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.4.1/mapdata/symbols/16x16/M.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.4.1/mapdata/symbols/16x16/N.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.4.1/mapdata/symbols/16x16/O.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.4.1/mapdata/symbols/16x16/P.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.4.1/mapdata/symbols/16x16/Q.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.4.1/mapdata/symbols/16x16/R.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.4.1/mapdata/symbols/16x16/S.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.4.1/mapdata/symbols/16x16/T.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.4.1/mapdata/symbols/16x16/U.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.4.1/mapdata/symbols/16x16/V.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.4.1/mapdata/symbols/16x16/W.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.4.1/mapdata/symbols/16x16/X.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.4.1/mapdata/symbols/16x16/Y.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.4.1/mapdata/symbols/16x16/Z.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.4.1/mapdata/symbols/16x16/airplane.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.4.1/mapdata/symbols/16x16/anchor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.4.1/mapdata/symbols/16x16/ball.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.4.1/mapdata/symbols/16x16/ball_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.4.1/mapdata/symbols/16x16/bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.4.1/mapdata/symbols/16x16/bars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.4.1/mapdata/symbols/16x16/binoculars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.4.1/mapdata/symbols/16x16/bird.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.4.1/mapdata/symbols/16x16/block.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.4.1/mapdata/symbols/16x16/block_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.4.1/mapdata/symbols/16x16/bookmark.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.4.1/mapdata/symbols/16x16/box_stack.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.4.1/mapdata/symbols/16x16/camera.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.4.1/mapdata/symbols/16x16/cancel.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.4.1/mapdata/symbols/16x16/car.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.4.1/mapdata/symbols/16x16/car2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.4.1/mapdata/symbols/16x16/center8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.4.1/mapdata/symbols/16x16/check.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.4.1/mapdata/symbols/16x16/check_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.4.1/mapdata/symbols/16x16/checkbox.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.4.1/mapdata/symbols/16x16/checkerboard.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.4.1/mapdata/symbols/16x16/chevrons.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.4.1/mapdata/symbols/16x16/circle_x.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.4.1/mapdata/symbols/16x16/clock.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.4.1/mapdata/symbols/16x16/columns.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.4.1/mapdata/symbols/16x16/contract.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.4.1/mapdata/symbols/16x16/cross.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/darkeye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.4.1/mapdata/symbols/16x16/decrease.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.4.1/mapdata/symbols/16x16/deposition.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.4.1/mapdata/symbols/16x16/diag_ll.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.4.1/mapdata/symbols/16x16/diag_lr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.4.1/mapdata/symbols/16x16/diag_ul.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.4.1/mapdata/symbols/16x16/diag_ur.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.4.1/mapdata/symbols/16x16/dialog.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.4.1/mapdata/symbols/16x16/diamond.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.4.1/mapdata/symbols/16x16/donkey.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.4.1/mapdata/symbols/16x16/dot.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.4.1/mapdata/symbols/16x16/down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.4.1/mapdata/symbols/16x16/drop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.4.1/mapdata/symbols/16x16/elephant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/expand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.4.1/mapdata/symbols/16x16/eye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.4.1/mapdata/symbols/16x16/fire.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.4.1/mapdata/symbols/16x16/fish.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.4.1/mapdata/symbols/16x16/flag.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.4.1/mapdata/symbols/16x16/flag2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.4.1/mapdata/symbols/16x16/four_arrows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.4.1/mapdata/symbols/16x16/graph.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.4.1/mapdata/symbols/16x16/hand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.4.1/mapdata/symbols/16x16/hash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.4.1/mapdata/symbols/16x16/heart.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.4.1/mapdata/symbols/16x16/hidden.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.4.1/mapdata/symbols/16x16/hourglass.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.4.1/mapdata/symbols/16x16/house.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.4.1/mapdata/symbols/16x16/increase.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/info.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.4.1/mapdata/symbols/16x16/leaf.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.4.1/mapdata/symbols/16x16/lightbulb.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.4.1/mapdata/symbols/16x16/lightning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.4.1/mapdata/symbols/16x16/lightning2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.4.1/mapdata/symbols/16x16/location_ptr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.4.1/mapdata/symbols/16x16/mine.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/nested_boxes.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.4.1/mapdata/symbols/16x16/pennant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.4.1/mapdata/symbols/16x16/pennant2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.4.1/mapdata/symbols/16x16/people.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.4.1/mapdata/symbols/16x16/person.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/person2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.4.1/mapdata/symbols/16x16/person3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.4.1/mapdata/symbols/16x16/phone.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/photo.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.4.1/mapdata/symbols/16x16/picnic.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.4.1/mapdata/symbols/16x16/plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.4.1/mapdata/symbols/16x16/point_down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.4.1/mapdata/symbols/16x16/point_left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.4.1/mapdata/symbols/16x16/point_right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/point_up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.4.1/mapdata/symbols/16x16/pointer_ne.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.4.1/mapdata/symbols/16x16/pointer_nw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.4.1/mapdata/symbols/16x16/pointer_se.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.4.1/mapdata/symbols/16x16/pointer_sw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.4.1/mapdata/symbols/16x16/puzzle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/q1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.4.1/mapdata/symbols/16x16/q1_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.4.1/mapdata/symbols/16x16/q2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.4.1/mapdata/symbols/16x16/q2_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.4.1/mapdata/symbols/16x16/q3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.4.1/mapdata/symbols/16x16/q3_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.4.1/mapdata/symbols/16x16/q4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.4.1/mapdata/symbols/16x16/q4_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.4.1/mapdata/symbols/16x16/qmark_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.4.1/mapdata/symbols/16x16/qmark_circle2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/raincloud.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.4.1/mapdata/symbols/16x16/right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.4.1/mapdata/symbols/16x16/rocket.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.4.1/mapdata/symbols/16x16/rocket2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.4.1/mapdata/symbols/16x16/rose.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/rows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.4.1/mapdata/symbols/16x16/scales.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/search.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.4.1/mapdata/symbols/16x16/search2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.4.1/mapdata/symbols/16x16/skull.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.4.1/mapdata/symbols/16x16/square.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.4.1/mapdata/symbols/16x16/star.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.4.1/mapdata/symbols/16x16/stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.4.1/mapdata/symbols/16x16/stop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.4.1/mapdata/symbols/16x16/surprise_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.4.1/mapdata/symbols/16x16/swamp.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.4.1/mapdata/symbols/16x16/target.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.4.1/mapdata/symbols/16x16/target2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.4.1/mapdata/symbols/16x16/ten.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.4.1/mapdata/symbols/16x16/trash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.4.1/mapdata/symbols/16x16/tree.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.4.1/mapdata/symbols/16x16/tree2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.4.1/mapdata/symbols/16x16/tree3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.4.1/mapdata/symbols/16x16/triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.4.1/mapdata/symbols/16x16/triangle_open.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.4.1/mapdata/symbols/16x16/triangle_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.4.1/mapdata/symbols/16x16/up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.4.1/mapdata/symbols/16x16/vapor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.4.1/mapdata/symbols/16x16/warning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.4.1/mapdata/symbols/16x16/wave.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.4.1/mapdata/symbols/16x16/wave2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.4.1/mapdata/symbols/16x16/wave3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.4.1/mapdata/symbols/16x16/weather.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.4.1/mapdata/symbols/16x16/wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.4.1/mapdata/symbols/16x16/wedge_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.4.1/mapdata/symbols/16x16/wedges_3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.4.1/mapdata/symbols/16x16/well.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.4.1/mapdata/symbols/16x16/whale.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.4.1/mapdata/symbols/16x16/whale2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.4.1/mapdata/symbols/16x16/wheelchair.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.4.1/mapdata/symbols/16x16/zigzags.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.4.1/mapdata/symbols/16x16/zigzags2.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.544630 mapdata-3.4.1/mapdata/symbols/20x20/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.4.1/mapdata/symbols/20x20/ball20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.4.1/mapdata/symbols/20x20/block20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.4.1/mapdata/symbols/20x20/circle20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.4.1/mapdata/symbols/20x20/q1_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.4.1/mapdata/symbols/20x20/q2_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.4.1/mapdata/symbols/20x20/q3_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.4.1/mapdata/symbols/20x20/q4_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.4.1/mapdata/symbols/20x20/square20.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.548630 mapdata-3.4.1/mapdata/symbols/24x24/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.4.1/mapdata/symbols/24x24/ball24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.4.1/mapdata/symbols/24x24/block24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.4.1/mapdata/symbols/24x24/circle24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.4.1/mapdata/symbols/24x24/square24.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.548630 mapdata-3.4.1/mapdata/symbols/28x28/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.4.1/mapdata/symbols/28x28/ball28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.4.1/mapdata/symbols/28x28/block28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.4.1/mapdata/symbols/28x28/circle28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.4.1/mapdata/symbols/28x28/square28.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-03-22 19:33:13.548630 mapdata-3.4.1/mapdata.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7582 2024-03-22 19:33:13.000000 mapdata-3.4.1/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-03-22 19:33:13.000000 mapdata-3.4.1/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-03-22 19:33:13.000000 mapdata-3.4.1/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      120 2024-03-22 19:33:13.000000 mapdata-3.4.1/mapdata.egg-info/requires.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-03-22 19:33:13.000000 mapdata-3.4.1/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-03-22 19:33:13.548630 mapdata-3.4.1/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1784 2024-03-22 19:29:34.000000 mapdata-3.4.1/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.455303 mapdata-3.5.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.5.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.5.0/MANIFEST.in
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-07 23:48:42.451303 mapdata-3.5.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     6306 2024-04-04 16:58:57.000000 mapdata-3.5.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/configfile/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.5.0/mapdata/configfile/mapdata.conf
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   657069 2024-04-07 23:40:24.000000 mapdata-3.5.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/symbols/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/16x16/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/0.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.5.0/mapdata/symbols/16x16/2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/5.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.5.0/mapdata/symbols/16x16/6.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/7.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.5.0/mapdata/symbols/16x16/9.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/A.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.5.0/mapdata/symbols/16x16/B.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/C.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/D.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/E.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/F.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/G.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/H.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.5.0/mapdata/symbols/16x16/I.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/J.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/K.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/L.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.5.0/mapdata/symbols/16x16/M.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/N.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/O.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/P.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.5.0/mapdata/symbols/16x16/Q.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/R.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.5.0/mapdata/symbols/16x16/S.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/T.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/U.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/V.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/W.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/X.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/Y.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/Z.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/airplane.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/anchor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/ball.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/ball_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.5.0/mapdata/symbols/16x16/bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/bars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/binoculars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/bird.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/block.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.5.0/mapdata/symbols/16x16/block_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/bookmark.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.5.0/mapdata/symbols/16x16/box_stack.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/camera.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/cancel.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/car.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/car2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/center8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/check.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/check_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/checkbox.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/checkerboard.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/chevrons.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_x.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/clock.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/columns.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/contract.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.5.0/mapdata/symbols/16x16/cross.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/darkeye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.5.0/mapdata/symbols/16x16/decrease.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/deposition.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ll.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_lr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ul.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ur.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/dialog.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/diamond.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/donkey.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/dot.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.5.0/mapdata/symbols/16x16/down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/drop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/elephant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/expand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.5.0/mapdata/symbols/16x16/eye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/fire.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/fish.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/flag.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.5.0/mapdata/symbols/16x16/flag2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/four_arrows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/graph.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/hand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/hash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/heart.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/hidden.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/hourglass.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/house.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/increase.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/info.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/leaf.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightbulb.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightning2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/location_ptr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/mine.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/nested_boxes.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.5.0/mapdata/symbols/16x16/pennant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/pennant2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/people.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/person.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/person2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/person3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/phone.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/photo.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/picnic.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_ne.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_nw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_se.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_sw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.5.0/mapdata/symbols/16x16/puzzle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/q1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.5.0/mapdata/symbols/16x16/q1_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/q2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/q2_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/q3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.5.0/mapdata/symbols/16x16/q3_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/q4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/q4_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/qmark_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/qmark_circle2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/raincloud.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/rocket.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/rocket2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/rose.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/rows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/scales.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/search.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.5.0/mapdata/symbols/16x16/search2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/skull.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/square.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/star.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/stop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/surprise_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/swamp.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/target.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/target2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/ten.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.5.0/mapdata/symbols/16x16/trash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle_open.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.5.0/mapdata/symbols/16x16/up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/vapor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/warning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/weather.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedge_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedges_3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.5.0/mapdata/symbols/16x16/well.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/whale.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/whale2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/wheelchair.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/zigzags.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/zigzags2.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/20x20/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.5.0/mapdata/symbols/20x20/ball20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.5.0/mapdata/symbols/20x20/block20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.5.0/mapdata/symbols/20x20/circle20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.5.0/mapdata/symbols/20x20/q1_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.5.0/mapdata/symbols/20x20/q2_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.5.0/mapdata/symbols/20x20/q3_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.5.0/mapdata/symbols/20x20/q4_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.5.0/mapdata/symbols/20x20/square20.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/24x24/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.5.0/mapdata/symbols/24x24/ball24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.5.0/mapdata/symbols/24x24/block24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.5.0/mapdata/symbols/24x24/circle24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.5.0/mapdata/symbols/24x24/square24.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/28x28/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.5.0/mapdata/symbols/28x28/ball28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.5.0/mapdata/symbols/28x28/block28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.5.0/mapdata/symbols/28x28/circle28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.5.0/mapdata/symbols/28x28/square28.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/requires.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-04-07 23:48:42.455303 mapdata-3.5.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-04-04 00:31:55.000000 mapdata-3.5.0/setup.py
```

### Comparing `mapdata-3.4.1/LICENSE.txt` & `mapdata-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/PKG-INFO` & `mapdata-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.4.1
+Version: 3.5.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,16 @@
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: loess
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pymannkendall
+Requires-Dist: umap-learn
+Requires-Dist: pynndescent
 
 
 *mapdata.py* is a data explorer for data sets containing geographic coordinates.  Data can be read from a CSV file, spreadsheet, or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also be selected and highlighted by writing a query expression to select rows of the data table.
 
 ![example map](https://mapdata.readthedocs.io/en/latest/_images/UI_CSOs_1.png)
 
@@ -93,15 +95,17 @@
 
   * A contingency table, using either categorical or numeric variables, with flexible
     specification of groups.  Tests of independence, risk ratio, odds ratio and related
     statistics, and conditional probabilities are all shown.
 
   * A Receiver Operating Characteristics (ROC) curve and measures such as sensitivity and specificity for a selected value of the predictor variable.
  
-  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis.
+  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis of multiple variables.
+ 
+  * A scatter plot of the results of a Uniform Manifold Approximation and Projection (UMAP) analysis of multiple variables.
 
 ![Correlation matrix](https://mapdata.readthedocs.io/en/latest/_images/UI_corr_matrix_example.png)
 
 SQL commands can be used when importing data from a database.  The SQL
 commands can be augmented with [execsql](https://pypi.org/project/execsql/)
 metacommands and substitution variables.
```

### Comparing `mapdata-3.4.1/README.md` & `mapdata-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 
   * A contingency table, using either categorical or numeric variables, with flexible
     specification of groups.  Tests of independence, risk ratio, odds ratio and related
     statistics, and conditional probabilities are all shown.
 
   * A Receiver Operating Characteristics (ROC) curve and measures such as sensitivity and specificity for a selected value of the predictor variable.
  
-  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis.
+  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis of multiple variables.
+ 
+  * A scatter plot of the results of a Uniform Manifold Approximation and Projection (UMAP) analysis of multiple variables.
 
 ![Correlation matrix](https://mapdata.readthedocs.io/en/latest/_images/UI_corr_matrix_example.png)
 
 SQL commands can be used when importing data from a database.  The SQL
 commands can be augmented with [execsql](https://pypi.org/project/execsql/)
 metacommands and substitution variables.
```

### Comparing `mapdata-3.4.1/mapdata/configfile/mapdata.conf` & `mapdata-3.5.0/mapdata/configfile/mapdata.conf`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/mapdata.py` & `mapdata-3.5.0/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "3.4.1"
-vdate = "2024-03-22"
+version = "3.5.0"
+vdate = "2024-04-07"
 
 copyright = "2023-2024"
 
 
 import sys
 import os.path
 import io
@@ -79,14 +79,15 @@
 import matplotlib.path as mpl_path
 matplotlib.use('TkAgg')
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
 import seaborn as sns
 from loess.loess_1d import loess_1d
 import scipy.stats as spstats
+import scipy.sparse as sparse
 import statsmodels.api as sm
 from statsmodels.sandbox.stats.runs import runstest_1samp
 from statsmodels.stats.diagnostic import normal_ad, kstest_normal
 try:
 	import pymannkendall as mk
 	mk_available = True
 except:
@@ -1190,28 +1191,88 @@
 	collen = len(quant_colors)
 	if lbllen > collen:
 		ext_colors = quant_colors * math.ceil(lbllen/collen)
 		return dict(zip(lbl_list, ext_colors[:len(lbl_list)]))
 	else:
 		return dict(zip(lbl_list, quant_colors[:len(lbl_list)]))
 
-
 def adjust_tile_color(tile_image):
 	if map_settings.basemap_color_adj is None:
 		return tile_image
 	else:
 		sat, con, bri = map_settings.basemap_color_adj
 		if sat != 0:
 			tile_image = ImageEnhance.Color(tile_image).enhance(sat)
 		if con != 0:
 			tile_image = ImageEnhance.Contrast(tile_image).enhance(con)
 		if bri != 0:
 			tile_image = ImageEnhance.Brightness(tile_image).enhance(bri)
 		return tile_image
 
+def doane_bins(d):
+	# The Doane algorithm for histogram bins.
+	dset = set(d)
+	if len(dset) == 1:
+		return 1
+	else:
+		g1 = spstats.skew(d)
+		if math.isnan(g1):
+			return 1
+		else:
+			nd = len(d)
+			g1_sd = math.sqrt((6*(nd-2))/((nd+1)*(nd+3)))
+			if g1_sd == 0.0:
+				return 1
+			else:
+				return math.ceil(1 + math.log(nd,2) + math.log(1+abs(g1)/g1_sd,2))
+
+#def scott_bins(d):
+	# The Scott algorithm for histogram bins.
+#	dset = set(d)
+#	if len(dset) == 1:
+#		return 1
+#	else:
+#		d_sd = statistics.stdev(d)
+#		if d_sd == 0.0:
+#			return 1
+#		else:
+#			nd = len(d)
+#			return math.ceil((3.49 * d_sd)/(nd**(1.0/3)))
+
+
+class VScrollFrame(ttk.Frame):
+	# A custom frame with a vertical scrollbar.
+	# Widgets should be added to the embedded 'content_frame'.
+	def __init__(self, parent, height=150, *args, **kwargs):
+		ttk.Frame.__init__(self, parent, *args, **kwargs)
+		self.canvas = tk.Canvas(self, bd=0, highlightthickness=0, height=height)
+		self.canvas.grid(row=0, column=0, sticky=tk.NSEW)
+		self.canvas.bind('<Configure>', self.upd_canvas)
+		self.rowconfigure(0, weight=1)
+		self.columnconfigure(0, weight=1)
+		vsb = ttk.Scrollbar(self, orient='vertical')
+		vsb.grid(row=0, column=1, sticky=tk.NS)
+		vsb.configure(command=self.canvas.yview)
+		self.canvas.configure(yscrollcommand=vsb.set)
+		self.content_frame = ttk.Frame(self.canvas)
+		self.content_frame.bind('<Configure>', self.upd_content_frame)
+		self.content_win = self.canvas.create_window(0, 0, window=self.content_frame, anchor=tk.NW)
+	def upd_content_frame(self, event):
+		reqwid = self.content_frame.winfo_reqwidth()
+		self.canvas.config(scrollregion=(0, 0, reqwid, self.content_frame.winfo_reqheight()))
+		if self.content_frame.winfo_reqwidth() != self.canvas.winfo_width():
+			self.canvas.config(width = reqwid)
+	def upd_canvas(self, event):
+		if self.content_frame.winfo_reqwidth() != self.canvas.winfo_width():
+			self.canvas.itemconfigure(self.content_win, width=self.canvas.winfo_width())
+	def scrolltop(self):
+		self.canvas.xview_moveto(0)
+		self.canvas.yview_moveto(0)
+    	
+
 class CsvFile(object):
 	def __init__(self, csvfname, junk_header_lines=0, dialect=None):
 		self.csvfname = csvfname
 		self.junk_header_lines = junk_header_lines
 		self.lineformat_set = False		# Indicates whether delimiter, quotechar, and escapechar have been set
 		self.delimiter = None
 		self.quotechar = None
@@ -1257,19 +1318,19 @@
 		try:
 			return list(sorted(columns[0]))
 		except:
 			return list(sorted([str(v) for v in columns[0]]))
 	nrows = len(columns[0])
 	rowdata = [[columns[c][r] for c in range(ncols)] for r in range(nrows)]
 	try:
-		rowdata.sort(key = lambda c: c[sortby])
+		rowdata.sort(key = lambda c: (c[sortby] is None, c[sortby]))
 	except:
 		for r in range(nrows):
 			rowdata[r][sortby] = str(rowdata[r][sortby])
-		rowdata.sort(key = lambda c: c[sortby])
+		rowdata.sort(key = lambda c: (c[sortby] == 'None', c[sortby]))
 	return [[rowdata[r][c] for r in range(nrows)] for c in range(ncols)]
 
 def treeview_sort_column(tv, col, reverse):
     colvals = [(tv.set(k, col), k) for k in tv.get_children()]
     try:
     	colvals.sort(key=lambda v: float(v[0]), reverse=reverse)
     except ValueError:
@@ -1835,16 +1896,20 @@
 		self.candcol_list = []
 		# List of PlotDialog objects, so they can be told to update themselves, or be deleted.
 		self.plot_list = []
 		# List of UnivarStatsDialog objects, so they can be updated.
 		self.univar_list = []
 		# List of BivarStatsDialog objects, so they can be updated.
 		self.bivar_list = []
+		# List of FitDistDialog objects, so they can be updated.
+		self.fitdist_list = []
 		# List of TSNEDialog objects, so they can be updated.
 		self.tsne_list = []
+		# List of UMAPDialog objects, so they can be updated.
+		self.umap_list = []
 		# List of CorrMatrixDialog objects, so they can be updated.
 		self.corrmat_list = []
 		# List of CategCorrespDialog objects, so they can be updated.
 		self.catcorresp_list = []
 		# List of ContTableDialog objects, so they can be updated.
 		self.conttable_list = []
 		# List of ROCCurveDialog objects, so they can be updated.
@@ -2654,17 +2719,23 @@
 				plot.q_redraw()
 		for dlg in self.univar_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
 		for dlg in self.bivar_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
+		for dlg in self.fitdist_list:
+			if unconditional or dlg.sel_only_var.get() == "1":
+				dlg.q_recalc()
 		for dlg in self.tsne_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
+		for dlg in self.umap_list:
+			if unconditional or dlg.sel_only_var.get() == "1":
+				dlg.q_recalc()
 		for dlg in self.corrmat_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_redraw()
 		for dlg in self.catcorresp_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
 		for dlg in self.conttable_list:
@@ -2786,24 +2857,34 @@
 		except:
 			pass
 	def remove_bivar(self, bivar_dlg):
 		try:
 			self.bivar_list.remove(bivar_dlg)
 		except:
 			pass
+	def remove_fitdist(self, fitdist_dlg):
+		try:
+			self.fitdist_list.remove(bivar_dlg)
+		except:
+			pass
 	def remove_corrmat(self, corrmat_dlg):
 		try:
 			self.corrmat_list.remove(corrmat_dlg)
 		except:
 			pass
 	def remove_tsne(self, tsne_dlg):
 		try:
 			self.tsne_list.remove(tsne_dlg)
 		except:
 			pass
+	def remove_umap(self, umap_dlg):
+		try:
+			self.umap_list.remove(umap_dlg)
+		except:
+			pass
 	def remove_categcorresp(self, categcorresp_dlg):
 		try:
 			self.catcorresp_list.remove(categcorresp_dlg)
 		except:
 			pass
 	def remove_conttable(self, conttable_dlg):
 		try:
@@ -2994,14 +3075,25 @@
 	def show_data_types(self):
 		self.wait_for_data_types()
 		show_table(self.win, "Data Types", \
 				"Data types, data completeness, and number of unique non-missing values for columns of the data table:", \
 				self.data_types, ["Column", "Type", "Missing", "Unique"], "Data Types", \
 				dlg_args={"can_resize": True}, tv_args={"select_mode": "browse"})
 
+	def hide_columns(self):
+		allcols = self.tbl["columns"]
+		dispcols = self.tbl["displaycolumns"]
+		if len(dispcols)==1 and dispcols[0]=='#all':
+			dispcols = allcols
+		dlg = TableHideColsDialog(self.win, allcols, dispcols)
+		result = dlg.show()
+		if result is not None:
+			self.tbl["displaycolumns"] = result
+
+
 	def find_candkeys(self, args=None):
 		dlg = FindCandKeysDialog(self, self.table_row_count, self.data_types)
 		self.candcol_list.append(dlg)
 		dlg.show()
 
 	def recode_data(self, args=None):
 		bad_cols = [self.lat_col, self.lon_col]
@@ -3124,14 +3216,18 @@
 			sqlcmd = "SELECT treeviewid FROM mapdata WHERE %s" % whereclause
 			self.select_by_sqlcmd(sqlcmd, action, "Invalid data selection: %s" % whereclause)
 	def new_plot(self, args=None):
 		self.wait_for_data_types()
 		dlg = PlotDialog(self, self.data_types)
 		self.plot_list.append(dlg)
 		dlg.show()
+	def pairplot(self, args=None):
+		dlg = PairPlotDialog(self, self.data_types)
+		self.plot_list.append(dlg)
+		dlg.show()
 	def select_colocated(self, args=None):
 		dlg = ColocatedDialog()
 		matchstr, num, merge = dlg.show()
 		if matchstr is not None:
 			if matchstr == "more than":
 				comp = ">"
 			elif matchstr == "less than":
@@ -3175,15 +3271,15 @@
 		stats_menu = tk.Menu(mnu, tearoff=0)
 		help_menu = tk.Menu(mnu, tearoff=0)
 		mnu.add_cascade(label="File", menu=file_menu, underline=0)
 		mnu.add_cascade(label="Table", menu=tbl_menu, underline=0)
 		mnu.add_cascade(label="Map", menu=map_menu, underline=0)
 		mnu.add_cascade(label="Selections", menu=sel_menu, underline=0)
 		mnu.add_cascade(label="Plot", menu=plot_menu, underline=0)
-		mnu.add_cascade(label="Stats", menu=stats_menu, underline=2)
+		mnu.add_cascade(label="Statistics", menu=stats_menu, underline=2)
 		mnu.add_cascade(label="Help", menu=help_menu, underline=0)
 		def save_table():
 			if table_object.selection():
 				rowset = []
 				for sel_row in table_object.selection():
 					rowset.append(table_object.item(sel_row)["values"])
 				export_data_table(column_headers, rowset, sheetname="Selected map items")
@@ -3319,26 +3415,47 @@
 
 		def bivar_stats():
 			self.wait_for_data_types()
 			dlg = BivarStatsDialog(self, self.data_types)
 			self.bivar_list.append(dlg)
 			dlg.show()
 
+		def fitdist_stats():
+			self.wait_for_data_types()
+			dlg = FitDistDialog(self, self.data_types)
+			self.fitdist_list.append(dlg)
+			dlg.show()
+
 		def corr_matrix():
 			self.wait_for_data_types()
 			dlg = CorrMatrixDialog(self, self.data_types)
 			self.corrmat_list.append(dlg)
 			dlg.show()
 
 		def tsne_anal():
 			self.wait_for_data_types()
 			dlg = TSNEDialog(self, self.data_types)
 			self.tsne_list.append(dlg)
 			dlg.show()
 
+		def umap_anal():
+			self.loading_dlg.display("Initializing UMAP")
+			try:
+				import umap
+				from sklearn.preprocessing import StandardScaler
+			except:
+				self.loading_dlg.hide()
+				warning("Libraries required for UMAP analysis are missing.", {'parent': self.win})
+			else:
+				self.loading_dlg.hide()
+				self.wait_for_data_types()
+				dlg = UMAPDialog(self, self.data_types)
+				self.umap_list.append(dlg)
+				dlg.show()
+
 		def categ_corresp():
 			self.wait_for_data_types()
 			dlg = CategCorrespDialog(self, self.data_types)
 			self.catcorresp_list.append(dlg)
 			dlg.show()
 
 		def cont_table():
@@ -3387,14 +3504,15 @@
 		file_menu.add_command(label="Set editor", command = set_editor, underline=4)
 		file_menu.add_command(label="Read config", command = read_config_file, underline=0)
 		file_menu.add_command(label="Save config", command = save_config, underline=0)
 		file_menu.add_command(label="Quit", command = self.cancel, underline=0)
 		tbl_menu.add_command(label="Un-select all", command = self.unselect_map, underline=0)
 		tbl_menu.add_command(label="Export selected", command = save_table, underline=1)
 		tbl_menu.add_command(label="Data types", command = self.show_data_types, underline=5)
+		tbl_menu.add_command(label="Hide/show columns", command = self.hide_columns, underline=0)
 		tbl_menu.add_command(label="Counts by location", command=self.counts_by_loc, underline=0)
 		tbl_menu.add_command(label="Find candidate keys", command=self.find_candkeys, underline=0)
 		tbl_menu.add_command(label="Recode data", command=self.recode_data, underline=0)
 		tbl_menu.add_command(label="Add unique row ID", command=self.add_rowid, underline=6)
 		map_menu.add_command(label="Zoom selected", command = self.zoom_selected, underline=5)
 		map_menu.add_command(label="Zoom full", command = self.zoom_full, underline=5)
 		map_menu.add_command(label="Center on selection", command = self.focus_map, underline=0)
@@ -3404,22 +3522,25 @@
 		map_menu.add_command(label="Settings", command = change_map_settings, underline=0)
 		sel_menu.add_command(label="Invert", command = invert_selections, underline=0)
 		sel_menu.add_command(label="Un-select all", command = self.unselect_map, underline=0)
 		sel_menu.add_command(label="Data query", command = self.run_query, underline=5)
 		sel_menu.add_command(label="Co-located data", command = self.select_colocated, underline=0)
 		sel_menu.add_command(label="Random", command = self.select_random, underline=0)
 		plot_menu.add_command(label="New", command = self.new_plot, underline=0)
+		plot_menu.add_command(label="Pair plot", command = self.pairplot, underline=0)
 		plot_menu.add_command(label="Close all", command = self.close_all_plots, underline=0)
 		plot_menu.add_command(label="Settings", command = self.get_plot_config, underline=0)
-		stats_menu.add_command(label="Univariate", command = univar_stats, underline=0)
-		stats_menu.add_command(label="Bivariate", command = bivar_stats, underline=0)
+		stats_menu.add_command(label="Univariate statistics", command = univar_stats, underline=0)
+		stats_menu.add_command(label="Fit univariate distribution", command = fitdist_stats, underline=0)
+		stats_menu.add_command(label="Bivariate statistics", command = bivar_stats, underline=0)
 		stats_menu.add_command(label="Correlation matrix", command = corr_matrix, underline=0)
 		stats_menu.add_command(label="Contingency table", command = cont_table, underline=2)
 		stats_menu.add_command(label="ROC curve", command = roc_curve, underline=0)
 		stats_menu.add_command(label="t-SNE analysis", command = tsne_anal, underline=0)
+		stats_menu.add_command(label="UMAP analysis", command = umap_anal, underline=0)
 		stats_menu.add_command(label="Categorical corresp.", command = categ_corresp, underline=1)
 		help_menu.add_command(label="Online help", command = online_help, underline=7)
 		help_menu.add_command(label="Config files", command = show_config_files, underline=0)
 		help_menu.add_command(label="Hotkeys", command = show_hotkeys, underline=0)
 		help_menu.add_command(label="About", command = show_about, underline=0)
 
 
@@ -3472,14 +3593,111 @@
 	def hide_all(self):
 		self.var_lbl.set("")
 		self.messages = []
 		self.dlg.config(cursor="arrow")
 		self.dlg.withdraw()
 
 
+class TableHideColsDialog(object):
+	def __init__(self, parent, column_list, displayed_columns):
+		self.parent = parent
+		self.column_list = column_list
+		self.displayed_columns = displayed_columns
+		self.dlg = tk.Toplevel(parent)
+		self.dlg.rowconfigure(1, weight=1)
+		self.dlg.columnconfigure(0, weight=1)
+		self.dlg.title("Hide/Show Columns")
+		self.check_vars = [tk.StringVar(self.dlg, "1" if col in self.displayed_columns else "0") for col in self.column_list]
+
+		# Message
+		prompt_frame = tk.Frame(self.dlg)
+		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, width=40, text="Choose the columns to show.\nAt least one column must be selected.")
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+
+		# Controls
+		ctrl_frame = tk.Frame(self.dlg)
+		ctrl_frame.grid(row=1, column=0, sticky=tk.NSEW)
+		ctlbtn_frame = tk.Frame(ctrl_frame)
+		ctlbtn_frame.grid(row=0, column=0, sticky=tk.NW)
+		ttk.Button(ctlbtn_frame, text="Hide", command=self.do_hide, underline=0).grid(row=0, column=0, sticky=tk.W, padx=(3,3), pady=(3,3))
+		ttk.Button(ctlbtn_frame, text="Show", command=self.do_show, underline=0).grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		ck_frame = tk.Frame(ctrl_frame, borderwidth=3, relief=tk.RIDGE)
+		ck_frame.grid(row=1, column=0, sticky=tk.NSEW)
+		ck_frame.rowconfigure(0, weight=1)
+		ck_frame.columnconfigure(0, weight=1)
+		ctrl_frame.rowconfigure(1, weight=1)
+		ctrl_frame.columnconfigure(0, weight=1)
+		self.vs_frame = VScrollFrame(ck_frame, height=300)
+		self.vs_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		self.content_frame = self.vs_frame.content_frame
+
+		# Add checkboxes
+		for i, colname in enumerate(self.column_list):
+			ttk.Checkbutton(self.content_frame, text=colname, variable=self.check_vars[i], command=self.check_sel,
+				onvalue="1", offvalue="0").grid(row=i, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		# Bottom buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=2, column=0, sticky=tk.EW, pady=(3,3))
+		self.canceled = False
+		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
+		ok_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,3))
+		self.dlg.bind('<Alt-o>', self.do_select)
+		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel)
+		cancel_btn.grid(row=0, column=2, sticky=tk.E, padx=(3,6))
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_cancel)
+
+	def do_hide(self):
+		# Hide all but the first
+		for col in self.check_vars[1:]:
+			col.set("0")
+	def do_show(self):
+		for col in self.check_vars:
+			col.set("1")
+	def check_sel(self):
+		# Ensure that at least one column is selected.
+		shown = [cv.get() == "1" for cv in self.check_vars]
+		if not any(shown):
+			self.check_vars[0].set("1")
+			self.vs_frame.scrolltop()
+			warning("At least one column must be shown.", {"parent": self.dlg})
+
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#show-hide-dialog", new=2, autoraise=True)
+	def do_cancel(self, *args):
+		self.canceled = True
+		self.dlg.destroy()
+	def do_select(self, *args):
+		self.canceled = False
+		self.dlg.destroy()
+	def show(self):
+		self.dlg.grab_set()
+		center_window(self.dlg)
+		self.dlg.resizable(True, True)
+		self.vs_frame.scrolltop()
+		self.dlg.wait_window(self.dlg)
+		try:
+			self.dlg.destroy()
+		except:
+			pass
+		if self.canceled:
+			return None
+		else:
+			return [self.column_list[i] for i in range(len(self.column_list)) if self.check_vars[i].get() == "1"]
+
 
 class MapConfigDialog(object):
 	def __init__(self, parent, column_list):
 		self.parent = parent
 		self.column_list = column_list
 		self.old_set = copy.copy(map_settings)
 		fonts = list(set(list(tkfont.families())))
@@ -5094,16 +5312,16 @@
 		self.plot_title = None
 		self.xlabel = None
 		self.ylabel = None
 		# For transparency on some plots; also initial value set by plot type in 'set_xy()'
 		self.alpha = 0.45
 		# For rotation of some plot types
 		self.rotated = False
-		# For histogram
-		self.bins = 10
+		# For histogram; will be initially overridden based on data set
+		self.bins = None
 		# For display of groups at Jenks breaks on Q-Q plots
 		self.qq_groups = False
 		# For display of lines at X and Y Jenks breaks on scatter plots
 		self.scatter_breaks = False
 		self.scatter_x_breaks = None
 		self.scatter_y_breaks = None
 		self.lineplot_breaks = False
@@ -5276,27 +5494,29 @@
 			self.xlog_ck["state"] = tk.DISABLED
 		else:
 			self.xlog_ck["state"] = "readonly"
 		xval = self.x_var.get()
 		yval = self.y_var.get()
 		if xval != '' and yval == xval:
 			self.y_var.set('')
+		self.bins = None
 		self.q_redraw(args)
 
 	def y_changed(self, *args):
 		self.ylabel = None
 		plot_type = self.type_var.get()
 		if plot_type in ("Count by category", "Histogram", "Empirical CDF", "Min-max by category"):
 			self.ylog_ck["state"] = tk.DISABLED
 		else:
 			self.ylog_ck["state"] = "readonly"
 		xval = self.x_var.get()
 		yval = self.y_var.get()
 		if yval != '' and yval == xval:
 			self.x_var.set('')
+		self.bins = None
 		self.q_redraw(args)
 
 	def z_changed(self, *args):
 		self.q_redraw(args)
 
 	def z_width_changed(self, *args):
 		try:
@@ -5319,14 +5539,15 @@
 		self.dlg.bind("<Alt-a>")
 		self.dlg.bind("<Alt-b>")
 		self.dlg.bind("<Alt-f>")
 		self.dlg.bind("<Alt-g>")
 		self.dlg.bind("<Alt-l>")
 		self.dlg.bind("<Alt-r>")
 		self.dlg.bind("<Alt-s>")
+		self.bins = None
 		self.flip_y = False
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.draw()
 		self.dataset = None
 		self.data_labels = None
 		self.plot_data = None
 		self.plot_data_labels = None
@@ -5441,14 +5662,17 @@
 		if self.y_var.get() != '':
 			column_list.append(self.y_var.get())
 		if self.z_var.get() != '':
 			column_list.append(self.z_var.get())
 		grpbyvar = self.groupby_var.get()
 		if grpbyvar != '' and grpbyvar not in ('* Breaks in X', '* Breaks in Y'):
 			column_list.append(self.groupby_var.get())
+			grpby_col_index = len(column_list) - 1
+		else:
+			grpby_col_index = None
 		# Record the number of data columns without labels.
 		self.n_dataset_columns = len(column_list)
 		if map_settings.label_col is not None:
 			column_list.append(map_settings.label_col)
 		# Get either only the selected data or all data.
 		if self.sel_only_var.get() == "1":
 			dataset = self.parent.get_sel_data(column_list)
@@ -5470,14 +5694,17 @@
 				for col in column_indexes:
 					if dataset[col][i] is None or dataset[col][i] == '':
 						ok = False
 				if ok:
 					for col in column_indexes:
 						clean_data[col].append(dataset[col][i])
 			dataset = None
+			# Ensure all values of any grouping variable are strings
+			if grpby_col_index is not None:
+				clean_data[grpby_col_index] = [str(grp) for grp in clean_data[grpby_col_index]]
 			# Convert quantitative data types
 			if plot_type != "Count by category":
 				x_data_type = [cs[1] for cs in self.column_specs if cs[0] == self.x_var.get()][0]
 				cast_fn = data_type_cast_fn(x_data_type)
 				for i in range(len(clean_data[0])):
 					clean_data[0][i] = cast_fn(clean_data[0][i])
 			if self.y_sel["state"] != tk.DISABLED and self.y_var.get() != "" and len(clean_data) > 1:
@@ -5530,14 +5757,16 @@
 				x_vals.sort()
 				x_counts = [counter[k] for k in x_vals]
 				self.plot_data = [x_vals, x_counts]
 				self.plot_data_labels = [self.data_labels[0], "Count"]
 			elif plot_type in ("Box plot", "Histogram", "Kernel density (KD) plot", "Stripchart", "Violin plot"):
 				# The groupby variable may or may not be set
 				if self.groupby_var.get() != '':
+					# Ensure that all values of the labeling variable are strings
+					self.dataset[1] = [str(lbl) for lbl in self.dataset[1]]
 					grp_vals = list(set(self.dataset[1]))
 					grp_vals.sort()
 					ds = list(zip(self.dataset[1], self.dataset[0]))
 					plot_data = []
 					for g in grp_vals:
 						plot_data.append([d[1] for d in ds if d[0] == g])
 					self.plot_data = plot_data
@@ -5570,14 +5799,16 @@
 			elif plot_type == "Empirical CDF":
 				# Y is the fraction of data points below each X value
 				x_counts = np.unique(self.dataset[0], return_counts=True)
 				y_vals = list(np.cumsum(x_counts[1]/np.sum(x_counts[1])))
 				self.plot_data = [list(x_counts[0]), y_vals]
 				self.plot_data_labels = [self.data_labels[0], "Cumulative frequency"]
 			elif plot_type == "Min-max by bin":
+				if self.bins is None:
+					self.bins = doane_bins(self.dataset[1])
 				if len(self.dataset[0]) > 1:
 					min_vals, min_edges, min_no = spstats.binned_statistic(self.dataset[1], self.dataset[0], statistic='min', bins=self.bins)
 					max_vals, max_edges, max_no = spstats.binned_statistic(self.dataset[1], self.dataset[0], statistic='max', bins=self.bins)
 					bin_width = min_edges[1] - min_edges[0]
 					bin_centers = min_edges[1:] - bin_width/2
 					self.plot_data = [bin_centers, min_vals, max_vals]
 				else:
@@ -5734,14 +5965,16 @@
 				else:
 					self.plot_axes.barh(grp_lbls, self.plot_data[1])
 					self.plot_axes.set_xlabel(self.ylabel or self.plot_data_labels[1])
 					self.plot_axes.set_ylabel(self.xlabel or self.plot_data_labels[0])
 					if self.flip_y:
 						self.plot_axes.invert_yaxis()
 			elif plot_type == "Histogram":
+				if self.bins is None:
+					self.bins = doane_bins(self.plot_data[0])
 				if self.groupby_var.get() == '':
 					self.plot_axes.hist(self.plot_data[0], bins=self.bins)
 				else:
 					self.plot_axes.hist(self.plot_data, bins=self.bins, stacked=True, label=self.plot_data_labels)
 					self.plot_axes.legend()
 				self.plot_axes.set_xlabel(self.xlabel or self.x_var.get())
 				self.plot_axes.set_ylabel("Counts")
@@ -6084,20 +6317,21 @@
 				else:
 					self.plot_axes.set_ylabel(self.ylabel or self.y_var.get())
 				if self.flip_y:
 					self.plot_axes.invert_yaxis()
 			elif plot_type == "Box plot":
 				self.dlg.bind("<Alt-r>", self.set_rotated)
 				orient = not self.rotated
-				grplbls = copy.copy(self.plot_data_labels[0:self.n_dataset_columns])
+				breakpoint()
+				grplbls = copy.copy(self.plot_data_labels)
 				if wrap_at_underscores:
 					grplbls = [lbl.replace("_", " ") for lbl in grplbls]
 				grplbls = [textwrap.wrap(lbl, width=wrapwidth) for lbl in grplbls]
 				grplbls = ["\n".join(lbl) for lbl in grplbls]
-				self.plot_axes.boxplot(self.plot_data[0:self.n_dataset_columns], labels=grplbls, vert=orient)
+				self.plot_axes.boxplot(self.plot_data, labels=grplbls, vert=orient)
 				if not self.rotated:
 					self.plot_axes.set_xlabel(self.xlabel or self.groupby_var.get())
 					self.plot_axes.set_ylabel(self.ylabel or self.data_labels[0])
 				else:
 					self.plot_axes.set_ylabel(self.xlabel or self.groupby_var.get())
 					self.plot_axes.set_xlabel(self.ylabel or self.data_labels[0])
 			elif plot_type == "Stripchart":
@@ -6319,14 +6553,284 @@
 	q25, q75 = np.percentile(d, 25), np.percentile(d, 75)
 	bound = 1.5 * (q75 - q25)
 	lbound, ubound = q25 - bound, q75 + bound
 	return len([v for v in x if v < lbound or v > ubound])
 
 
 
+class PairPlotDialog(object):
+	def __init__(self, parent, column_specs):
+		self.parent = parent
+		self.column_specs = column_specs
+		self.dlg = tk.Toplevel()
+		self.dlg.title("Pair Plot")
+		self.alpha = 0.45
+		self.dlg.rowconfigure(0, weight=0)
+		self.dlg.rowconfigure(1, weight=0)
+		self.dlg.rowconfigure(2, weight=1)
+		self.dlg.rowconfigure(3, weight=0)
+		self.dlg.columnconfigure(0, weight=1)
+		# Data
+		self.dataset = None
+		self.data_labels = None
+		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
+		self.numeric_columns.sort()
+		self.categ_columns = [c[0] for c in self.column_specs if c[1] in ("string")]
+		self.categ_columns.sort()
+		self.dlg.bind("<Control-s>")
+		# Message
+		prompt_frame = tk.Frame(self.dlg, borderwidth=5)
+		prompt_frame.grid(row=0, column=0, sticky=tk.N+tk.EW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, width=100, text="Select two or more variables from the left to see the pair plot.  Use Ctrl-click or Shift-click to select multiple rows.")
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+
+		# Controls
+		# Top controls are only the 'Selected only' checkbox.  The 'Group by' dropdown is below the variable list.
+		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
+		ctrl_frame.rowconfigure(0, weight=0)
+		ctrl_frame.columnconfigure(0, weight=1)
+		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
+		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
+		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_redraw, variable=self.sel_only_var,
+				onvalue="1", offvalue="0")
+		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.log10_var = tk.StringVar(ctrl_frame, "0")
+		self.log10_ck = ttk.Checkbutton(ctrl_frame, text="Log10 transform data", command=self.q_redraw, variable=self.log10_var,
+				onvalue="1", offvalue="0")
+		self.log10_ck.grid(row=1, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		# The data_frame encompasses the two panes of the variable frame and the content frame
+		data_frame = tk.Frame(self.dlg, borderwidth=5)
+		data_frame.rowconfigure(0, weight=1)
+		data_frame.columnconfigure(0, weight=1)
+		data_frame.grid(row=2, column=0, sticky=tk.NSEW)
+		frame_panes = ttk.PanedWindow(data_frame, orient=tk.HORIZONTAL)
+		frame_panes.grid(row=0, column=0, sticky=tk.NSEW)
+
+		# Variable frame for list of quantitative columns/variables and the 'Group by' dropdown.
+		var_frame = tk.Frame(frame_panes, borderwidth=2, relief=tk.RIDGE)
+		var_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		var_frame.rowconfigure(0, weight=1)
+		var_frame.columnconfigure(0, weight=1)
+		frame_panes.add(var_frame, weight=1)
+		# Add multi-select list of variables to the leftmost pane
+		self.column_frame, self.column_table = treeview_table(var_frame, rowset=[[v] for v in self.numeric_columns], \
+				column_headers=['Variable'], select_mode=tk.EXTENDED, nrows=min(10, len(self.numeric_columns)))
+		self.column_frame.grid(row=0, column=0, columnspan=2, sticky=tk.NSEW)
+		self.column_table.bind('<ButtonRelease-1>', self.q_redraw)
+		# Add 'Group by' dropdown.
+		self.groupby_var = tk.StringVar(var_frame, "")
+		ttk.Label(var_frame, text="Group by:").grid(row=1, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		groupby_sel = ttk.Combobox(var_frame, state="readonly", textvariable=self.groupby_var, width=24)
+		groupby_sel["values"] = [''] + self.categ_columns
+		groupby_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		groupby_sel.bind('<<ComboboxSelected>>', self.q_redraw)
+
+		# Content frame for pair plot figure
+		self.content_frame = tk.Frame(frame_panes, borderwidth=3, relief=tk.RIDGE)
+		self.content_frame.grid(row=0, column=1, sticky=tk.NSEW)
+		self.content_frame.rowconfigure(0, weight=1)
+		self.content_frame.columnconfigure(0, weight=1)
+		frame_panes.add(self.content_frame, weight=12)
+		self.plotfig = Figure(dpi=100)
+		self.plotfig.set_figheight(4)
+		self.plotfig.set_figwidth(4)
+		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, self.content_frame)
+		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, self.content_frame)
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plot_nav.update()
+		# initialize content frame with an empty plot
+		self.clear_output()
+
+		# Buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=0)
+		btn_frame.columnconfigure(1, weight=1)
+		self.canceled = False
+		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.data_btn = ttk.Button(btn_frame, text="Source Data", state=tk.DISABLED, command=self.show_data, underline=0)
+		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
+		close_btn.grid(row=0, column=2, sticky=tk.E, padx=(6,6))
+		self.dlg.bind("<Alt-c>", self.do_close)
+		self.dlg.bind("<Escape>", self.do_close)
+		center_window(self.dlg)
+		raise_window(self.dlg)
+
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#pair-plot-dialog", new=2, autoraise=True)
+
+	def show_data(self, *args):
+		if self.dataset is not None:
+			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels[0:len(self.dataset)], \
+					"Data for pair plot")
+
+	def clear_output(self):
+		self.plotfig.clear()
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.draw()
+
+	def q_redraw(self, get_data=True, *args):
+		if self.dataset is None or get_data:
+			self.clear_output()
+			self.get_data()
+		if self.dataset is not None and len(self.dataset) > 1 and len(self.dataset[0]) > 1:
+			self.redraw()
+		else:
+			self.clear_output()
+			self.data_btn["state"] = tk.DISABLED
+
+	def get_data(self):
+		# Get the selected data into 'dataset'
+		self.dataset = None
+		column_list = []
+		for sel_row in self.column_table.selection():
+			datarow = self.column_table.item(sel_row)["values"]
+			column_list.append(datarow[0])
+		self.n_data_columns = len(column_list)
+		groupby = self.groupby_var.get()
+		if groupby != '':
+			column_list.append(groupby)
+		if len(column_list) > 0:
+			# Get either only the selected data or all data.
+			if self.sel_only_var.get() == "1":
+				dataset = self.parent.get_sel_data(column_list)
+			else:
+				dataset = self.parent.get_all_data(column_list)
+			if dataset is None or len(dataset[0]) == 0:
+				self.dataset = None
+				self.data_labels = None
+			else:
+				self.dataset = dataset
+				self.data_labels = column_list
+			# Remove missing data
+			column_indexes = range(len(dataset))
+			clean_data = [[] for _ in dataset]
+			clean_labels = copy.copy(self.data_labels)
+			for i in range(len(dataset[0])):
+				ok = True
+				for col in column_indexes:
+					if dataset[col][i] is None or dataset[col][i] == '':
+						ok = False
+				if ok:
+					for col in column_indexes:
+						clean_data[col].append(dataset[col][i])
+			dataset = None
+			# If the last columns is a label, ensure all values are strings.
+			if self.groupby_var.get() != '':
+				clean_data[self.n_data_columns] = [str(lbl) for lbl in clean_data[self.n_data_columns]]
+			# Convert to floats
+			for i in range(self.n_data_columns):
+				clean_data[i] = [conv_float(v) for v in clean_data[i]]
+			# Log-transform data if specified.
+			if self.log10_var.get() == '1':
+				log_data = [[] for _ in clean_data]
+				log_error = False
+				nrows = len(clean_data[0])
+				for v in range(len(clean_data)):
+					for i in range(nrows):
+						try:
+							log_data[v].append(math.log10(clean_data[v][i]))
+						except:
+							log_error = True
+							break
+					if log_error:
+						break
+				if log_error:
+					warning("Data can not all be log-transformed.", {})
+					self.log10_var.set("0")
+				else:
+					clean_data = log_data
+					clean_labels = ["Log10 of " + v for v in clean_labels]
+			#
+			self.dataset = clean_data
+			self.data_labels = clean_labels
+			self.data_btn["state"] = tk.NORMAL
+
+	def redraw(self):
+		# (Re)draw the pair plot.  The Seaborn pairplot function produces a figure that
+		# can't be used with FigureCanvasTkAgg, so this is a custom pairplot routine.
+		self.dlg.bind("<Alt-a>", self.set_alpha)
+		if self.data_labels is not None and self.n_data_columns > 1:
+			groupby = self.groupby_var.get()
+			if groupby != '':
+				grplbls = [lbl for lbl in self.dataset[self.n_data_columns]]
+				if wrap_at_underscores:
+					grplbls = [lbl.replace("_", " ") for lbl in grplbls]
+				grplbls = [textwrap.wrap(lbl, width=wrapwidth) for lbl in grplbls]
+				grplbls = ["\n".join(lbl) for lbl in grplbls]
+				groups = sorted(list(set(self.dataset[self.n_data_columns])))
+				cmap = map_colors(groups)
+				colors = [cmap[g] for g in self.dataset[self.n_data_columns]]
+			self.plotfig.clear()
+			dim = self.n_data_columns
+			orig_xsize = matplotlib.rcParams['xtick.labelsize']
+			orig_ysize = matplotlib.rcParams['ytick.labelsize']
+			matplotlib.rcParams['xtick.labelsize'] = 6
+			matplotlib.rcParams['ytick.labelsize'] = 6
+			for rowindex in range(dim):
+				for colindex in range(dim):
+					subplot_no = (rowindex * dim) + (colindex+1)
+					ax = self.plotfig.add_subplot(dim, dim, subplot_no)
+					if colindex == rowindex:
+						if groupby == '':
+							kdp = sns.kdeplot({self.data_labels[rowindex]: self.dataset[rowindex]}, fill=True, ax=ax)
+						else:
+							kdp = sns.kdeplot({self.data_labels[rowindex]: self.dataset[rowindex], 'colors': colors},
+									x=self.data_labels[rowindex], hue=colors, multiple="layer", alpha=self.alpha, fill=True, ax=ax,
+									warn_singular=False)
+						kdp.set(xlabel=None)
+						kdp.set(ylabel=None)
+					else:
+						if groupby == '':
+							ax.scatter(self.dataset[colindex], self.dataset[rowindex], alpha=self.alpha)
+						else:
+							ax.scatter(self.dataset[colindex], self.dataset[rowindex], c=colors, alpha=self.alpha)
+					ax.legend([]).set_visible(False)
+					if colindex == 0:
+						ax.set_ylabel(self.data_labels[rowindex])
+					if rowindex == dim-1:
+						ax.set_xlabel(self.data_labels[colindex])
+			if groupby != '':
+				handle_list = []
+				lbls = list(cmap.keys())
+				colkey = list(cmap.values())
+				symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
+				self.plotfig.legend(handles=symbs, labels=lbls)
+			self.plotfig_canvas.draw()
+			matplotlib.rcParams['xtick.labelsize'] = orig_xsize
+			matplotlib.rcParams['ytick.labelsize'] = orig_ysize
+
+	def set_alpha(self, *args):
+		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the opacity (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
+		new_alpha = dlg.show()
+		if new_alpha is not None:
+			self.alpha = new_alpha
+			self.q_redraw()
+	def show(self):
+		self.dlg.wait_window(self.dlg)
+	def do_close(self, *args):
+		self.parent.remove_plot(self)
+		try:
+			self.dlg.destroy()
+		except:
+			pass
+
+
+
+
 class UnivarStatsDialog(object):
 	def __init__(self, parent, column_specs):
 		self.parent = parent
 		self.column_specs = column_specs
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Univariate Statistics")
 		self.dlg.rowconfigure(0, weight=0)
@@ -7560,17 +8064,17 @@
 		#self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
 		# Single or grouped scatter plot
 		if self.groupby_col is None:
 			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
 			handle_list = []
 			label_list = []
 		else:
-			groups = sorted(list(set(self.dataset[self.groupby_col-1])))
+			groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
 			cmap = map_colors(groups)
-			colors = [cmap[g] for g in self.dataset[self.groupby_col-1]]
+			colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
 			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], c=colors, alpha=self.alpha)
 			# Custom legend handle for grouped scatter plot
 			lbls = list(cmap.keys())
 			if wrap_at_underscores:
 				lbls = [l.replace("_", " ") for l in lbls]
 			lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
 			colkey = list(cmap.values())
@@ -7645,14 +8149,725 @@
 		self.parent.remove_tsne(self)
 		try:
 			self.dlg.destroy()
 		except:
 			pass
 
 
+
+class UMAPDialog(object):
+	def __init__(self, parent, column_specs):
+		self.parent = parent
+		self.column_specs = column_specs
+		self.alpha = 0.45
+		self.plot_title = None
+		self.dlg = tk.Toplevel()
+		self.dlg.title("UMAP Analysis")
+		self.loading_dlg = LoadingDialog(self.dlg)
+		self.alpha = 0.45
+		self.tsne_coords = None
+		self.tsne_labels = None
+		# Data
+		self.dataset = None
+		self.data_labels = None
+		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
+		self.numeric_columns.sort()
+		self.categ_columns = [c[0] for c in self.column_specs if c[1] == "string"]
+		self.categ_columns.sort()
+		# Message
+		prompt_frame = tk.Frame(self.dlg, borderwidth=5)
+		prompt_frame.grid(row=0, column=0, sticky=tk.N+tk.EW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, width=80, text="Select three or more variables from the list below, and then use the 'Calculate' button.")
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+
+		# Controls
+		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
+		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
+
+		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
+		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_recalc, variable=self.sel_only_var,
+				onvalue="1", offvalue="0")
+		self.sel_only_ck.grid(row=0, column=0, columnspan=2, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		# Frame for input selection and output plot
+		self.content_frame = tk.Frame(self.dlg)
+		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
+		self.dlg.rowconfigure(2, weight=1)
+		self.dlg.columnconfigure(0, weight=1)
+		self.content_frame.rowconfigure(0, weight=1)
+		self.content_frame.columnconfigure(0, weight=1)
+
+		# PanedWindow within content_frame: left is input listbox and 'Calculate' button, right is plot and 'Data Table' button
+		io_panes = ttk.PanedWindow(self.content_frame, orient=tk.HORIZONTAL)
+		io_panes.grid(row=0, column=0, sticky=tk.NSEW)
+
+		self.inp_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
+		self.inp_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		self.inp_frame.rowconfigure(0, weight=1)
+		self.inp_frame.columnconfigure(0, weight=1)
+		io_panes.add(self.inp_frame, weight=1)
+
+		self.output_frame = tk.Frame(io_panes, borderwidth=3, relief=tk.RIDGE)
+		self.output_frame.grid(row=0, column=1, sticky=tk.NSEW)
+		self.output_frame.rowconfigure(0, weight=1)
+		self.output_frame.columnconfigure(0, weight=1)
+		io_panes.add(self.output_frame, weight=1)
+
+		# Variable selection
+		# Add multi-select list of variables to the leftmost pane
+		var_frame = tk.Frame(self.inp_frame)
+		var_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		var_frame.rowconfigure(0, weight=1)
+		var_frame.columnconfigure(0, weight=1)
+		self.column_frame, self.column_table = treeview_table(self.inp_frame, rowset=[[v] for v in self.numeric_columns], \
+				column_headers=['Variable'], select_mode=tk.EXTENDED, nrows=min(10, len(self.numeric_columns)))
+		self.column_frame.grid(row=0, column=0, sticky=tk.NSEW)
+		self.column_table.bind('<ButtonRelease-1>', self.q_recalc)
+
+		# UMAP parameter selection
+		inpopt_frame = tk.Frame(self.inp_frame)
+		inpopt_frame.grid(row=1, column=0, sticky=tk.NSEW)
+		inpopt_frame.columnconfigure(1, weight=1)
+		self.neighbors_var = tk.IntVar(inpopt_frame, min(15, math.floor(self.parent.table_row_count/4)))
+		ttk.Label(inpopt_frame, text="Neighbors:").grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		neighbor_sel = ttk.Spinbox(inpopt_frame, textvariable=self.neighbors_var, from_=2, to=math.floor(self.parent.table_row_count/4), width=5)
+		neighbor_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		ttk.Label(inpopt_frame, text="Minimum distance:").grid(row=1, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.mindist_var = tk.DoubleVar(inpopt_frame, 0.1)
+		mindist_sel = ttk.Spinbox(inpopt_frame, textvariable=self.mindist_var, from_=0.0, to=0.99, increment=0.01, width=4)
+		mindist_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		# n_components is fixed at 2, with no user input allowed.
+		ttk.Label(inpopt_frame, text="Distance metric:").grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.metric_var = tk.StringVar(inpopt_frame, 'euclidean')
+		metric_sel = ttk.Combobox(inpopt_frame, state="readonly", textvariable=self.metric_var, width=15,
+				values=['braycurtis', 'canberra', 'chebyshev', 'cosine', 'correlation', 'euclidean', 'manhattan', 'minkowski'])
+		metric_sel.grid(row=2, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		metric_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+
+		# Optional grouping
+		self.groupby_var = tk.StringVar(self.inp_frame, "")
+		ttk.Label(inpopt_frame, text="Group by:").grid(row=3, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		groupby_sel = ttk.Combobox(inpopt_frame, state="readonly", textvariable=self.groupby_var, width=24)
+		groupby_sel["values"] = [''] + self.categ_columns
+		groupby_sel.grid(row=3, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		groupby_sel.bind('<<ComboboxSelected>>', self.q_recalc)
+
+		# 'Calculate' button
+		self.calc_btn = ttk.Button(inpopt_frame, text="Calculate", command=self.recalculate, state=tk.DISABLED, underline=8)
+		self.calc_btn.grid(row=4, column=1, sticky=tk.E, padx=(3,6), pady=(3,3))
+
+		# UMAP output plot
+		plot_frame = tk.Frame(self.output_frame)
+		plot_frame.rowconfigure(0, weight=1)
+		plot_frame.columnconfigure(0, weight=1)
+		plot_frame.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plotfig = Figure(dpi=100)
+		self.plotfig.set_figheight(3.5)
+		self.plotfig.set_figwidth(3.5)
+		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, plot_frame)
+		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, plot_frame)
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plot_nav.update()
+
+		# t-SNE Data Table button
+		dtbtn_frame = tk.Frame(self.output_frame)
+		dtbtn_frame.pack(side=tk.BOTTOM, fill=tk.X, expand=0)
+		self.dtable_btn = ttk.Button(dtbtn_frame, text="Data Table", command=self.umap_table, state=tk.DISABLED, underline=8)
+		self.dtable_btn.pack(side=tk.LEFT, fill='none', expand=0, padx=(6,3), pady=(3,3))
+
+		# Buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=0)
+		btn_frame.columnconfigure(1, weight=0)
+		btn_frame.columnconfigure(2, weight=1)
+		self.canceled = False
+		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		self.data_btn = ttk.Button(btn_frame, text="Source Data", state=tk.DISABLED, command=self.show_data, underline=0)
+		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
+		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
+		close_btn.grid(row=0, column=2, sticky=tk.E, padx=(6,6))
+		self.dlg.bind("<Alt-c>", self.do_close)
+		self.dlg.bind("<Escape>", self.do_close)
+
+		# Initialize output frames
+		self.clear_output()
+
+		center_window(self.dlg)
+		raise_window(self.dlg)
+
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#umap-dialog", new=2, autoraise=True)
+
+	def q_recalc(self, *args):
+		# At least three variables must be selected
+		self.clear_output()
+		curr_selections = self.column_table.selection()
+		if len(curr_selections) > 2:
+			self.calc_btn["state"] = tk.NORMAL
+		else:
+			self.calc_btn["state"] = tk.NORMAL
+
+	def get_data(self):
+		self.data_btn["state"] = tk.DISABLED
+		self.dataset = None
+		column_list = []
+		for sel_row in self.column_table.selection():
+			datarow = self.column_table.item(sel_row)["values"]
+			column_list.append(datarow[0])
+		# Record the number of data columns without labels.
+		self.n_dataset_columns = len(column_list)
+		# Get additional columns if specified
+		if map_settings.label_col is not None:
+			column_list.append(map_settings.label_col)
+			self.label_col = len(column_list)
+		else:
+			self.label_col = None
+		grpbyvar = self.groupby_var.get()
+		if grpbyvar != '':
+			column_list.append(grpbyvar)
+			self.groupby_col = len(column_list)
+		else:
+			self.groupby_col = None
+		# Get either only the selected data or all data.
+		if self.sel_only_var.get() == "1":
+			dataset = self.parent.get_sel_data(column_list)
+		else:
+			dataset = self.parent.get_all_data(column_list)
+		if dataset is None or len(dataset[0]) < 6:
+			self.dataset = None
+			self.data_labels = None
+			self.data_btn["state"] = tk.DISABLED
+			self.calc_btn["state"] = tk.DISABLED
+		else:
+			# UMAP can operate on sparse arrays, so there's no need to remove missing data
+			clean_data = dataset
+			# Convert to floats for numeric data only
+			for i in range(len(clean_data)):
+				if column_list[i] in self.numeric_columns:
+					clean_data[i] = [conv_float(v) for v in clean_data[i]]
+			#
+			self.dataset = sort_columns(clean_data)
+			self.data_labels = column_list
+			self.data_btn["state"] = tk.NORMAL
+			self.calc_btn["state"] = tk.NORMAL
+			self.dtable_btn["state"] = tk.DISABLED
+
+	def clear_output(self):
+		self.dlg.bind("<Alt-a>")
+		self.dlg.bind("<Alt-s>")
+		self.dlg.bind("<Control-s>")
+		self.data_btn["state"] = tk.DISABLED
+		self.dtable_btn["state"] = tk.DISABLED
+		self.plotfig.clear()
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.draw()
+
+	def recalculate(self):
+		self.loading_dlg.display("Calculating UMAP")
+		import umap
+		from sklearn.preprocessing import StandardScaler
+		self.clear_output()
+		self.get_data()
+		# Check to see if this is a sparse matrix
+		is_sparse = False
+		for col in range(self.n_dataset_columns):
+			if any([x is None or x == 0.0 for x in self.dataset[col]]):
+				is_sparse = True
+				break
+		ds = copy.copy(self.dataset[0:self.n_dataset_columns])
+		if is_sparse:
+			# Replace all None with 0
+			for col in range(len(ds)):
+				ds[col] = [0.0 if x is None else x for x in ds[col]]
+		dsa = np.array(columns_to_rows(ds), dtype=float)
+		if is_sparse:
+			# Convert to a LIL array
+			dsm = sparse.lil_matrix(dsa)
+			# Normalize the variables
+			inp_data = StandardScaler(with_mean=False).fit_transform(dsm)
+		else:
+			# Normalize the variables
+			inp_data = StandardScaler().fit_transform(dsa)
+		reducer = umap.UMAP(n_neighbors=self.neighbors_var.get(), min_dist=self.mindist_var.get(), n_components=2,
+				metric=self.metric_var.get())
+		umap_result = reducer.fit_transform(inp_data)
+		self.umap_coords = [umap_result[:,0], umap_result[:,1]]
+		self.umap_labels = ["Dimension 1", "Dimension 2"]
+		self.dtable_btn["state"] = tk.NORMAL
+		# Single or grouped scatter plot
+		if self.groupby_col is None:
+			splot = self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], alpha=self.alpha)
+			handle_list = []
+			label_list = []
+		else:
+			groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
+			cmap = map_colors(groups)
+			colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
+			splot = self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], c=colors, alpha=self.alpha)
+			# Custom legend handle for grouped scatter plot
+			lbls = list(cmap.keys())
+			if wrap_at_underscores:
+				lbls = [l.replace("_", " ") for l in lbls]
+			lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
+			colkey = list(cmap.values())
+			symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
+			handle_list = symbs
+			label_list = lbls
+		# Hover annotation
+		def update_annot(ind):
+			pos = splot.get_offsets()[ind["ind"][0]]
+			self.annot.xy = pos
+			text = ", ".join([str(self.dataset[self.label_col-1][n]) for n in ind["ind"]])
+			self.annot.set_text(text)
+			self.annot.get_bbox_patch().set_facecolor("wheat")
+			self.annot.get_bbox_patch().set_alpha(0.8)
+		def hover(event):
+			vis = self.annot.get_visible()
+			if event.inaxes == self.plot_axes:
+				cont, ind = splot.contains(event)
+				if cont:
+					update_annot(ind)
+					self.annot.set_visible(True)
+				else:
+					if vis:
+						self.annot.set_visible(False)
+				self.plotfig_canvas.draw_idle()
+		if self.label_col is not None:
+			self.annot = self.plot_axes.annotate("", xy=(0,0), xytext=(8,12), textcoords="offset points", \
+					bbox={"boxstyle": "round", "fc": "w"}, arrowprops={"arrowstyle": "->"})
+			self.annot.set_visible(False)
+			self.canvas_conn_id = self.plotfig_canvas.mpl_connect("motion_notify_event", hover)
+		else:
+			if self.canvas_conn_id is not None:
+				self.plotfig_canvas.mpl_disconnect(self.canvas_conn_id)
+		# Legend
+		if len(handle_list) > 0:
+			self.plot_axes.legend(handles=handle_list, labels=label_list)
+
+		self.plot_axes.set_xlabel(self.umap_labels[0])
+		self.plot_axes.set_ylabel(self.umap_labels[1])
+		self.plotfig_canvas.draw()
+		self.plot_nav.update()
+		self.dlg.bind("<Alt-a>", self.set_alpha)
+		self.loading_dlg.hide()
+
+	def show_data(self, *args):
+		if self.dataset is not None:
+			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels, "Data for UMAP Analysis")
+
+	def umap_table(self, *args):
+		if self.umap_coords is not None:
+			dt = copy.copy(self.umap_coords)
+			dl = copy.copy(self.umap_labels)
+			if self.label_col is not None:
+				dt.append(self.dataset[self.label_col-1])
+				dl.append(self.data_labels[self.label_col-1])
+			if self.groupby_col is not None:
+				dt.append(self.dataset[self.groupby_col-1])
+				dl.append(self.data_labels[self.groupby_col-1])
+			show_columnar_table(self.dlg, "UMAP Results", "Coordinates for the two UMAP dimensions:", dt, dl, "UMAP coordinates")
+
+	def set_alpha(self, *args):
+		dlg = OneFloatDialog(self.dlg, "Transparency", "Enter the transparency (alpha) value", min_value=0.0, max_value=1.0, initial=self.alpha)
+		new_alpha = dlg.show()
+		if new_alpha is not None:
+			self.alpha = new_alpha
+			self.q_recalc()
+
+	def show(self):
+		self.dlg.wait_window(self.dlg)
+	def do_close(self, *args):
+		self.parent.remove_tsne(self)
+		try:
+			self.dlg.destroy()
+		except:
+			pass
+
+
+
+
+class FitDistDialog(object):
+	def __init__(self, parent, column_specs):
+		self.parent = parent
+		self.column_specs = column_specs
+		self.plot_title = None
+		self.dlg = tk.Toplevel()
+		self.dlg.title("Distribution Fitting")
+		self.bins = None
+		self.dlg.bind("<Alt-b>")
+		self.dlg.bind("<Alt-t>")
+		self.dlg.bind("<Alt-x>")
+		self.dlg.bind("<Alt-y>")
+		# scipy.stats distributions, by support and type.
+		# The dictionary itemss are a tuple consisting of:
+		#	* the scipy distribution object
+		#	* a dictionary of arguments to be passed to the 'fit()' function.
+		#	* the user names of the return values of the 'fit()' function.
+		#	* the 'goodness_of_fit()' argument names of the return values of the 'fit()' function.
+		#-- Continguous, -inf to inf:
+		self.dist_cont = {
+				'Laplace': (spstats.laplace, {}, ('Location', 'Scale'), ('loc', 'scale')),
+				'Logistic': (spstats.logistic, {}, ('Location', 'Scale'), ('loc', 'scale')),
+				'Normal': (spstats.norm, {}, ('Mean', 'Std. deviation'), ('loc', 'scale')),
+				# Shifted log-logistic fitting triggers an error in scipy.
+				#'Shifted log-logistic': (spstats.fisk, {}, ('Shape', 'Location', 'Scale'), ('shape', 'loc', 'scale')),
+				'von Mises': (spstats.vonmises, {}, ('Kappa', 'Location', 'Scale'), ('kappa', 'loc', 'scale'))}
+		#-- Continuous, 0 to inf:
+		self.dist_cont_pos = {
+				'Exponential': (spstats.expon, {}, ('Location', 'Scale'), ('loc', 'scale')),
+				'Gamma': (spstats.gamma, {'floc':0}, ('Shape', None, 'Scale'), ('a', 'loc', 'scale')),
+				'Gompertz': (spstats.gompertz, {'floc':0}, ('Shape', None, 'Scale'), ('c', 'loc', 'scale')),
+				# Log-logistic fitting triggers an error in scipy.
+				#'Log-logistic': (spstats.fisk, {'floc':0}, ('Shape', None, 'Scale'), ('shape', 'loc', 'scale')),
+				'Lognormal': (spstats.lognorm, {'floc':0}, ('Log std. dev.', None, 'Log mean'), ('s', 'loc', 'scale')),
+				'Pareto': (spstats.pareto, {'floc':0}, ('Shape', None, 'Scale'), ('b', 'loc', 'scale')),
+				'Rayleigh': (spstats.rayleigh, {}, ('Location', 'Scale'), ('loc', 'scale'))}
+		#-- Continuous, 0 to 1:
+		self.dist_cont_01 = {
+				'Beta': (spstats.beta, {}, ('Shape 1', 'Shape 2', 'Location', 'Scale'), ('a', 'b', 'loc', 'scale')),
+				'Uniform': (spstats.uniform, {}, ('Location', 'Scale'), ('loc', 'scale'))}
+		self.all_dist = {**self.dist_cont, **self.dist_cont_pos, **self.dist_cont_01}
+		#
+		self.xlabel = None
+		self.ylabel = None
+		# Data
+		self.dataset = None
+		self.data_labels = None
+		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
+		self.numeric_columns.sort()
+		self.output_columns = ["Statistic", "Value"]
+		self.statdata = []
+		# Message
+		prompt_frame = tk.Frame(self.dlg, borderwidth=5)
+		prompt_frame.grid(row=0, column=0, sticky=tk.N+tk.EW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, width=70, text="Select a variable and a distribution type to fit.")
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+
+		# Controls
+		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
+		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
+
+		self.x_var = tk.StringVar(ctrl_frame, "")
+		x_lbl = ttk.Label(ctrl_frame, text="X column:")
+		x_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.x_sel = ttk.Combobox(ctrl_frame, state=tk.NORMAL, textvariable=self.x_var, values=self.numeric_columns, width=24)
+		self.x_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(3,3))
+		self.x_sel.bind("<<ComboboxSelected>>", self.set_dist)
+
+		self.xlog_var = tk.StringVar(ctrl_frame, "0")
+		self.xlog_ck = ttk.Checkbutton(ctrl_frame, text="Log X", state=tk.NORMAL, command=self.set_dist, variable=self.xlog_var,
+				onvalue="1", offvalue="0")
+		self.xlog_ck.grid(row=0, column=2, sticky=tk.W, padx=(6,6), pady=(3,3))
+
+		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
+		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.set_dist, variable=self.sel_only_var,
+				onvalue="1", offvalue="0")
+		self.sel_only_ck.grid(row=0, column=3, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.dist_var = tk.StringVar(ctrl_frame, "")
+		dist_lbl = ttk.Label(ctrl_frame, text="Distribution:")
+		dist_lbl.grid(row=1, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		self.dist_sel = ttk.Combobox(ctrl_frame, state=tk.DISABLED, textvariable=self.dist_var, values=[], width=22)
+		self.dist_sel.grid(row=1, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
+		self.dist_sel.bind("<<ComboboxSelected>>", self.refit)
+
+		# Frame for output summary table and plot
+		self.content_frame = tk.Frame(self.dlg)
+		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
+		self.dlg.rowconfigure(2, weight=1)
+		self.dlg.columnconfigure(0, weight=1)
+		self.content_frame.rowconfigure(0, weight=1)
+		self.content_frame.columnconfigure(0, weight=1)
+
+		# PanedWindow within content_frame: left is plot, right is table
+		output_panes = ttk.PanedWindow(self.content_frame, orient=tk.HORIZONTAL)
+		output_panes.grid(row=0, column=0, sticky=tk.NSEW)
+
+		self.out_plt_frm = tk.Frame(output_panes, borderwidth=3, relief=tk.RIDGE)
+		self.out_plt_frm.grid(row=0, column=0, sticky=tk.NSEW)
+		self.out_plt_frm.rowconfigure(0, weight=1)
+		self.out_plt_frm.columnconfigure(0, weight=1)
+		output_panes.add(self.out_plt_frm, weight=1)
+
+		self.out_tbl_frm = tk.Frame(output_panes, borderwidth=3, relief=tk.RIDGE)
+		self.out_tbl_frm.grid(row=0, column=1, sticky=tk.NSEW)
+		self.out_tbl_frm.rowconfigure(0, weight=1)
+		self.out_tbl_frm.columnconfigure(0, weight=1, minsize=400)
+		output_panes.add(self.out_tbl_frm, weight=1)
+
+		# Data plot
+		plot_frame = tk.Frame(self.out_plt_frm)
+		plot_frame.rowconfigure(0, weight=1)
+		plot_frame.columnconfigure(0, weight=1)
+		plot_frame.pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plotfig = Figure(dpi=100)
+		self.plotfig.set_figheight(3.0)
+		self.plotfig.set_figwidth(3.0)
+		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, plot_frame)
+		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, self.out_plt_frm)
+		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
+		self.plot_nav.update()
+
+		# Initialize output frames
+		self.clear_output()
+
+		# Buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=0)
+		btn_frame.columnconfigure(1, weight=0)
+		btn_frame.columnconfigure(2, weight=1)
+		self.canceled = False
+		self.help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
+		self.help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
+		self.dlg.bind("<Alt-h>", self.do_help)
+		self.data_btn = ttk.Button(btn_frame, text="Source Data", state=tk.DISABLED, command=self.show_data, underline=0)
+		self.data_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,3))
+		close_btn = ttk.Button(btn_frame, text="Close", command=self.do_close, underline=0)
+		close_btn.grid(row=0, column=2, sticky=tk.E, padx=(6,6))
+		self.dlg.bind("<Alt-c>", self.do_close)
+		self.dlg.bind("<Escape>", self.do_close)
+		center_window(self.dlg)
+		raise_window(self.dlg)
+
+	def do_help(self, *args):
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#distribution-fitting-dialog", new=2, autoraise=True)
+
+	def q_recalc(self):
+		self.get_data()
+		if self.dataset is not None:
+			self.set_dist()
+
+	def get_data(self):
+		self.dataset = None
+		self.data_labels = None
+		self.dist_sel["state"] = tk.DISABLED
+		self.data_btn["state"] = tk.DISABLED
+		self.dist_var.set('')
+		self.statdata = []
+		if self.x_var.get() != '':
+			column_list = [self.x_var.get()]
+			# Get either only the selected data or all data.
+			if self.sel_only_var.get() == "1":
+				dataset = self.parent.get_sel_data(column_list)
+			else:
+				dataset = self.parent.get_all_data(column_list)
+			if dataset is None or len(dataset[0]) == 0:
+				self.dataset = None
+				self.data_labels = None
+				self.dist_sel["state"] = tk.DISABLED
+				self.data_btn["state"] = tk.DISABLED
+			else:
+				# Remove missing data
+				column_indexes = range(len(dataset))
+				clean_data = [[] for _ in dataset]
+				for i in range(len(dataset[0])):
+					ok = True
+					for col in column_indexes:
+						if dataset[col][i] is None or dataset[col][i] == '':
+							ok = False
+					if ok:
+						for col in column_indexes:
+							clean_data[col].append(dataset[col][i])
+				dataset = None
+				# Convert to floats for numeric data only
+				for i in range(len(clean_data)):
+					if column_list[i] in self.numeric_columns:
+						clean_data[i] = [conv_float(v) for v in clean_data[i]]
+				self.data_labels = [column_list[0]]
+				# Log-transform data if specified.
+				log_data = [[] for _ in clean_data]
+				log_error = False
+				if self.xlog_ck["state"] != tk.DISABLED and self.xlog_var.get() == "1" and self.x_var.get() in self.numeric_columns:
+					for i in range(len(clean_data[0])):
+						try:
+							log_data[0].append(math.log10(clean_data[0][i]))
+						except:
+							log_error = True
+							self.xlog_var.set("0")
+							self.xlog_ck["state"] = tk.DISABLED
+							break
+					if not log_error:
+						clean_data[0] = log_data[0]
+						self.data_labels = ["Log10 of %s" % column_list[0]]
+				log_data = None
+				#
+				self.dataset = [sort_columns(clean_data)]
+				self.dist_sel["state"] = "readonly"
+				self.data_btn["state"] = tk.NORMAL
+				#
+				xpfx = "" if self.xlog_var.get() == '0' else "Log10 of "
+				self.statdata.append(["X variable", self.data_labels[0]])
+				self.statdata.append(["N", len(self.dataset[0])])
+
+	def clear_output(self):
+		self.dlg.bind("<Alt-b>")
+		self.dlg.bind("<Control-s>")
+		for ctl in self.out_tbl_frm.winfo_children():
+			ctl.destroy()
+		tframe, tdata = treeview_table(self.out_tbl_frm, [], ["Statistic", "Value"])
+		tframe.grid(row=0, column=0, sticky=tk.NSEW)
+		self.plotfig.clear()
+		self.plot_axes = self.plotfig.add_subplot(111)
+		self.plotfig_canvas.draw()
+
+	def show_data(self, *args):
+		if self.dataset is not None:
+			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels[0:len(self.dataset)], \
+					"Data for distribution fitting")
+
+	def set_dist(self, *args):
+		# Set the allowable values for the distribution type based on the data range.
+		self.clear_output()
+		if self.x_var.get() != '':
+			self.get_data()
+
+			# Plot the histogram
+			if self.bins is None:
+				self.bins = doane_bins(self.dataset[0])
+			self.hist_val, hist_bins, patches = self.plot_axes.hist(self.dataset[0], bins=self.bins, density=True)
+			hist_ofs = (self.dataset[0][-1] - self.dataset[0][0])/self.bins/2
+			self.hist_centers = [hist_bins[i] + hist_ofs for i in range(len(hist_bins)-1)]
+			self.plot_axes.set_xlabel(self.xlabel or self.data_labels[0])
+			self.plot_axes.set_ylabel("Probability Density")
+			self.dlg.bind("<Alt-b>", self.set_bins)
+			self.plotfig_canvas.draw()
+			self.plot_nav.update()
+
+			# Set the allowable distributions
+			if len(self.dataset[0]) < 5:
+				self.dist_var.set("")
+				self.dist_sel["state"] = tk.DISABLED
+			else:
+				self.dist_sel["state"] = "readonly"
+				if self.dataset is not None:
+					xmin = self.dataset[0][0]
+					xmax = self.dataset[0][-1]
+					if xmin < 0:
+						dist = self.dist_cont
+					elif xmax <= 1.0:
+						dist = self.dist_cont_01
+					else:
+						dist = {**self.dist_cont_pos, **self.dist_cont}
+				if self.dist_var.get() not in dist:
+					self.dist_var.set("")
+				self.dist_sel["values"] = list(dist.keys())
+
+				# Maybe fit the distribution also
+				if self.dist_var.get() != '':
+					self.refit()
+		else:
+			self.clear_output()
+
+
+	def refit(self, *args):
+		running_dlg = LoadingDialog(self.dlg)
+		running_dlg.display("Fitting data")
+		fitter, fitterargs, usernames, argnames = self.all_dist[self.dist_sel.get()]
+		try:
+			fitres = fitter.fit(self.dataset[0], **fitterargs)
+		except:
+			running_dlg.hide()
+			warning("Data fitting unsuccessful", {"parent": self.dlg})
+		else:
+			N = len(self.dataset[0])
+			self.statdata.append(["\u2015"*15, ""])
+			self.statdata.append(["Distribution", self.dist_var.get()])
+			for i, name in enumerate(usernames):
+				if name is not None:
+					self.statdata.append([name, fp_display(fitres[i])])
+			# Add goodness-of-fit statistics to output table
+			fit_pdf = fitter.pdf(self.dataset[0], *fitres) * N
+			sse = sum([(fit_pdf[i] - self.dataset[0][i])**2 for i in range(N)])
+			self.statdata.append(["SSE", fp_display(sse, figs=5)])
+			gf_args = dict(zip(argnames, fitres))
+			gf_succeeded = False
+			gf_statname = None
+			for stat in (("ad", "Anderson-Darling"), ("ks", "Kolmogorov-Smirnov"), ("cvm", "Cramer-von Mises")):
+				try:
+					gf_res = spstats.goodness_of_fit(fitter, self.dataset[0], fit_params=gf_args, statistic=stat[0], n_mc_samples=1000)
+				except:
+					pass
+				else:
+					if not math.isnan(gf_res.statistic):
+						gf_succeeded = True
+						gf_statname = stat[1]
+						break
+			if gf_succeeded:
+				self.statdata.append([gf_statname + " statistic", fp_display(gf_res.statistic)])
+				self.statdata.append([gf_statname + " p value", fp_display(gf_res.pvalue)])
+				loglik = fitter.logpdf(self.dataset[0], *fitres).sum()
+				aic = 2*len(fitres) - 2*loglik
+				self.statdata.append(["AIC", fp_display(aic)])
+			# Display table of statistics
+			tframe, tdata = treeview_table(self.out_tbl_frm, self.statdata, self.output_columns)
+			tframe.grid(row=0, column=0, stick=tk.NSEW)
+			self.dlg.bind("<Control-s>", self.save_table)
+
+			# Display PDF of fitted distribution on the plot
+			fit_x = np.linspace(self.dataset[0][0], self.dataset[0][-1], 100)
+			fit_pdf = fitter.pdf(fit_x, *fitres)
+			self.plot_axes.plot(fit_x, fit_pdf, lw=2, label=self.dist_var.get())
+			self.plot_axes.legend()
+			self.plotfig_canvas.draw()
+
+			running_dlg.hide()
+
+	def set_title(self, *args):
+		dlg = OneEntryDialog(self.dlg, "Plot Title", "Enter a title for the plot:")
+		title = dlg.show()
+		if title is not None:
+			self.plot_title = title
+			self.plot_axes.set_title(title)
+			self.plotfig_canvas.draw()
+	def set_xlabel(self, *args):
+		dlg = OneEntryDialog(self.dlg, "X-Axis Label", "Enter the X-axis label:")
+		xlabel = dlg.show()
+		if xlabel is not None:
+			self.plot_axes.set_xlabel(xlabel)
+			self.plotfig_canvas.draw()
+	def set_ylabel(self, *args):
+		dlg = OneEntryDialog(self.dlg, "Y-Axis Label", "Enter the Y-axis label:")
+		ylabel = dlg.show()
+		if ylabel is not None:
+			self.plot_axes.set_ylabel(ylabel)
+			self.plotfig_canvas.draw()
+	def set_bins(self, *args):
+		dlg = OneIntDialog(self.dlg, "Data Bins", "Enter the number of bins to be used for the histogram", min_value=2, max_value=100, initial=self.bins)
+		num_bins = dlg.show()
+		if num_bins is not None:
+			self.bins = num_bins
+			self.q_recalc()
+	def save_table(self, *args):
+		export_data_table(self.output_columns, self.statdata, sheetname="Bivariate statistsics")
+	def show(self):
+		self.dlg.wait_window(self.dlg)
+	def do_close(self, *args):
+		self.parent.remove_fitdist(self)
+		try:
+			self.dlg.destroy()
+		except:
+			pass
+
+
+
 class ContTableDialog(object):
 	def __init__(self, parent, column_specs):
 		self.parent = parent
 		self.column_specs = column_specs
 		self.plot_title = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Contingency Table")
```

### Comparing `mapdata-3.4.1/mapdata/symbols/24x24/ball24.xbm` & `mapdata-3.5.0/mapdata/symbols/24x24/ball24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/24x24/block24.xbm` & `mapdata-3.5.0/mapdata/symbols/24x24/block24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/24x24/circle24.xbm` & `mapdata-3.5.0/mapdata/symbols/24x24/circle24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/24x24/square24.xbm` & `mapdata-3.5.0/mapdata/symbols/24x24/square24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/28x28/ball28.xbm` & `mapdata-3.5.0/mapdata/symbols/28x28/ball28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/28x28/block28.xbm` & `mapdata-3.5.0/mapdata/symbols/28x28/block28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/28x28/circle28.xbm` & `mapdata-3.5.0/mapdata/symbols/28x28/circle28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata/symbols/28x28/square28.xbm` & `mapdata-3.5.0/mapdata/symbols/28x28/square28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/mapdata.egg-info/PKG-INFO` & `mapdata-3.5.0/mapdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.4.1
+Version: 3.5.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,16 @@
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: loess
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: pymannkendall
+Requires-Dist: umap-learn
+Requires-Dist: pynndescent
 
 
 *mapdata.py* is a data explorer for data sets containing geographic coordinates.  Data can be read from a CSV file, spreadsheet, or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also be selected and highlighted by writing a query expression to select rows of the data table.
 
 ![example map](https://mapdata.readthedocs.io/en/latest/_images/UI_CSOs_1.png)
 
@@ -93,15 +95,17 @@
 
   * A contingency table, using either categorical or numeric variables, with flexible
     specification of groups.  Tests of independence, risk ratio, odds ratio and related
     statistics, and conditional probabilities are all shown.
 
   * A Receiver Operating Characteristics (ROC) curve and measures such as sensitivity and specificity for a selected value of the predictor variable.
  
-  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis.
+  * A scatter plot of the results of a *t*-Distributed Stochastic Neighbor Embedding (t-SNE) analysis of multiple variables.
+ 
+  * A scatter plot of the results of a Uniform Manifold Approximation and Projection (UMAP) analysis of multiple variables.
 
 ![Correlation matrix](https://mapdata.readthedocs.io/en/latest/_images/UI_corr_matrix_example.png)
 
 SQL commands can be used when importing data from a database.  The SQL
 commands can be augmented with [execsql](https://pypi.org/project/execsql/)
 metacommands and substitution variables.
```

### Comparing `mapdata-3.4.1/mapdata.egg-info/SOURCES.txt` & `mapdata-3.5.0/mapdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.4.1/setup.py` & `mapdata-3.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 symbol_files = glob.glob("mapdata/symbols/16x16/*.xbm") + glob.glob("mapdata/symbols/20x20/*.xbm") + \
 			glob.glob("mapdata/symbols/24x24/*.xbm") + glob.glob("mapdata/symbols/28x28/*.xbm")
 
 setuptools.setup(name='mapdata',
-	version='3.4.1',
+	version='3.5.0',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='cortice@tutanota.com',
     url='https://osdn.net/project/mapdata/',
     packages=['mapdata'],
 	scripts=['mapdata/mapdata.py'],
 	data_files=[('symbols', symbol_files), ('config', ['mapdata/configfile/mapdata.conf'])],
     license='GPL',
-	install_requires=['tkintermapview', 'pyproj', 'jenkspy', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib', 'seaborn', 'loess', 'statsmodels', 'scipy', 'scikit-learn', 'pymannkendall'],
+	install_requires=['tkintermapview', 'pyproj', 'jenkspy', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib', 'seaborn', 'loess', 'statsmodels', 'scipy', 'scikit-learn', 'pymannkendall', 'umap-learn', 'pynndescent'],
 	python_requires = '>=3.8',
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: Console',
 		'Environment :: X11 Applications',
 		'Environment :: Win32 (MS Windows)',
 		'Intended Audience :: End Users/Desktop',
```

