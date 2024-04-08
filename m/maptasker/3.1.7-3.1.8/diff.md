# Comparing `tmp/maptasker-3.1.7.tar.gz` & `tmp/maptasker-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptasker-3.1.7.tar", max compression
+gzip compressed data, was "maptasker-3.1.8.tar", max compression
```

## Comparing `maptasker-3.1.7.tar` & `maptasker-3.1.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1079 2024-02-16 16:36:22.405000 maptasker-3.1.7/LICENSE.txt
--rw-r--r--   0        0        0      536 2024-03-04 15:40:38.700000 maptasker-3.1.7/README_PyPl.md
--rw-r--r--   0        0        0        0 2024-03-10 15:08:20.218081 maptasker-3.1.7/maptasker/__init__.py
--rw-r--r--   0        0        0        3 2024-01-26 19:55:41.510000 maptasker-3.1.7/maptasker/assets/.MapTasker_RunCount.txt
--rw-r--r--   0        0        0     9216 2024-02-22 20:13:00.839000 maptasker-3.1.7/maptasker/assets/Thumbs.db
--rw-r--r--   0        0        0      390 2024-03-25 17:21:31.285000 maptasker-3.1.7/maptasker/assets/icons/arrow.png
--rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-3.1.7/maptasker/assets/maptasker_logo_dark.png
--rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-3.1.7/maptasker/assets/maptasker_logo_light.png
--rw-r--r--   0        0        0     1782 2024-01-08 16:34:50.197000 maptasker-3.1.7/maptasker/main.py
--rw-r--r--   0        0        0       17 2024-02-02 20:14:04.969000 maptasker-3.1.7/maptasker/src/__init__.py
--rw-r--r--   0        0        0    13154 2024-03-01 18:04:39.824000 maptasker-3.1.7/maptasker/src/actargs.py
--rw-r--r--   0        0        0    21610 2024-02-22 20:13:11.590000 maptasker-3.1.7/maptasker/src/action.py
--rw-r--r--   0        0        0   116412 2024-03-08 20:16:24.476767 maptasker-3.1.7/maptasker/src/actionc.py
--rw-r--r--   0        0        0     8377 2024-02-22 20:13:10.380000 maptasker-3.1.7/maptasker/src/actiond.py
--rw-r--r--   0        0        0     9449 2024-02-22 20:13:08.920000 maptasker-3.1.7/maptasker/src/actione.py
--rw-r--r--   0        0        0     9324 2024-02-22 20:13:11.464000 maptasker-3.1.7/maptasker/src/actionr.py
--rw-r--r--   0        0        0    15551 2024-02-22 20:13:12.365000 maptasker-3.1.7/maptasker/src/actiont.py
--rw-r--r--   0        0        0     3376 2024-02-22 20:13:12.356000 maptasker-3.1.7/maptasker/src/addcss.py
--rw-r--r--   0        0        0     3783 2024-02-16 16:36:20.478000 maptasker-3.1.7/maptasker/src/caveats.py
--rw-r--r--   0        0        0    11813 2024-02-22 20:13:11.472000 maptasker-3.1.7/maptasker/src/clip.py
--rw-r--r--   0        0        0     8660 2023-12-04 16:08:02.839000 maptasker-3.1.7/maptasker/src/colors.py
--rw-r--r--   0        0        0     3186 2024-03-08 20:16:24.477154 maptasker-3.1.7/maptasker/src/colrmode.py
--rw-r--r--   0        0        0    11539 2024-02-02 20:14:09.416000 maptasker-3.1.7/maptasker/src/condition.py
--rw-r--r--   0        0        0     2739 2024-03-10 19:26:48.459929 maptasker-3.1.7/maptasker/src/config.py
--rw-r--r--   0        0        0     6541 2024-02-02 20:14:15.316000 maptasker-3.1.7/maptasker/src/debug.py
--rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-3.1.7/maptasker/src/deprecate.py
--rw-r--r--   0        0        0    30601 2024-03-25 17:21:29.641646 maptasker-3.1.7/maptasker/src/diagram.py
--rw-r--r--   0        0        0    27007 2024-02-16 16:36:21.774000 maptasker-3.1.7/maptasker/src/diagutil.py
--rw-r--r--   0        0        0    19996 2024-02-09 18:52:35.434000 maptasker-3.1.7/maptasker/src/dirout.py
--rw-r--r--   0        0        0     2567 2024-03-25 17:21:29.642197 maptasker-3.1.7/maptasker/src/error.py
--rw-r--r--   0        0        0     2399 2024-02-02 20:14:19.267000 maptasker-3.1.7/maptasker/src/fonts.py
--rw-r--r--   0        0        0     4455 2024-02-22 20:13:11.559000 maptasker-3.1.7/maptasker/src/format.py
--rw-r--r--   0        0        0     5871 2024-03-01 19:48:51.688000 maptasker-3.1.7/maptasker/src/frontmtr.py
--rw-r--r--   0        0        0     5354 2024-03-25 17:21:29.642583 maptasker-3.1.7/maptasker/src/getbakup.py
--rw-r--r--   0        0        0     2311 2024-03-26 15:58:24.004284 maptasker-3.1.7/maptasker/src/getids.py
--rw-r--r--   0        0        0     9112 2024-03-25 17:21:29.643340 maptasker-3.1.7/maptasker/src/getputer.py
--rw-r--r--   0        0        0     9754 2024-02-22 20:13:15.666000 maptasker-3.1.7/maptasker/src/globalvr.py
--rw-r--r--   0        0        0    57045 2024-03-28 13:25:01.499225 maptasker-3.1.7/maptasker/src/guiutils.py
--rw-r--r--   0        0        0     3645 2024-02-02 20:14:14.232000 maptasker-3.1.7/maptasker/src/initparg.py
--rw-r--r--   0        0        0     2368 2023-11-15 16:38:53.257000 maptasker-3.1.7/maptasker/src/kidapp.py
--rw-r--r--   0        0        0    25269 2024-03-26 15:44:14.513791 maptasker-3.1.7/maptasker/src/lineout.py
--rw-r--r--   0        0        0    30560 2024-03-27 18:52:38.353702 maptasker-3.1.7/maptasker/src/mapit.py
--rw-r--r--   0        0        0    11434 2024-03-25 17:21:29.644163 maptasker-3.1.7/maptasker/src/maputils.py
--rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-3.1.7/maptasker/src/nameattr.py
--rw-r--r--   0        0        0    20711 2024-02-16 16:36:22.869000 maptasker-3.1.7/maptasker/src/outline.py
--rw-r--r--   0        0        0    18958 2024-03-27 18:52:18.353217 maptasker-3.1.7/maptasker/src/parsearg.py
--rw-r--r--   0        0        0     8606 2024-02-02 20:14:19.240000 maptasker-3.1.7/maptasker/src/prefers.py
--rw-r--r--   0        0        0     6536 2024-03-17 15:16:47.058723 maptasker-3.1.7/maptasker/src/primitem.py
--rw-r--r--   0        0        0    11265 2024-02-22 20:13:15.666000 maptasker-3.1.7/maptasker/src/proclist.py
--rw-r--r--   0        0        0    14060 2024-02-22 20:13:18.209000 maptasker-3.1.7/maptasker/src/profiles.py
--rw-r--r--   0        0        0     2280 2024-02-02 20:14:19.331000 maptasker-3.1.7/maptasker/src/progargs.py
--rw-r--r--   0        0        0    14749 2024-03-26 15:23:17.423023 maptasker-3.1.7/maptasker/src/proginit.py
--rw-r--r--   0        0        0    29347 2024-03-19 17:30:17.739585 maptasker-3.1.7/maptasker/src/projects.py
--rw-r--r--   0        0        0     5099 2024-02-09 18:52:43.236000 maptasker-3.1.7/maptasker/src/property.py
--rw-r--r--   0        0        0    20178 2024-03-27 18:52:09.422282 maptasker-3.1.7/maptasker/src/runcli.py
--rw-r--r--   0        0        0     5658 2024-03-25 17:21:29.644789 maptasker-3.1.7/maptasker/src/rungui.py
--rw-r--r--   0        0        0     9758 2024-03-25 17:21:29.645096 maptasker-3.1.7/maptasker/src/scenes.py
--rw-r--r--   0        0        0    16315 2024-02-02 20:14:14.236000 maptasker-3.1.7/maptasker/src/servicec.py
--rw-r--r--   0        0        0     6193 2024-02-22 20:13:15.794000 maptasker-3.1.7/maptasker/src/share.py
--rw-r--r--   0        0        0     3658 2024-02-16 16:36:21.861000 maptasker-3.1.7/maptasker/src/shelsort.py
--rw-r--r--   0        0        0     7450 2024-03-26 13:55:17.295276 maptasker-3.1.7/maptasker/src/sysconst.py
--rw-r--r--   0        0        0     6151 2024-02-22 20:13:15.795000 maptasker-3.1.7/maptasker/src/taskactn.py
--rw-r--r--   0        0        0     6835 2024-03-25 17:21:29.645740 maptasker-3.1.7/maptasker/src/taskerd.py
--rw-r--r--   0        0        0     2695 2023-11-08 17:54:50.622000 maptasker-3.1.7/maptasker/src/taskflag.py
--rw-r--r--   0        0        0    20135 2024-03-08 20:16:24.478872 maptasker-3.1.7/maptasker/src/tasks.py
--rw-r--r--   0        0        0     9946 2024-03-01 19:48:54.083000 maptasker-3.1.7/maptasker/src/taskuniq.py
--rw-r--r--   0        0        0     2100 2024-02-20 15:01:50.903000 maptasker-3.1.7/maptasker/src/twisty.py
--rw-r--r--   0        0        0   103353 2024-03-27 18:34:45.424222 maptasker-3.1.7/maptasker/src/userintr.py
--rw-r--r--   0        0        0    10324 2024-02-22 20:13:25.250000 maptasker-3.1.7/maptasker/src/xmldata.py
--rw-r--r--   0        0        0     4998 2024-03-26 13:55:28.028547 maptasker-3.1.7/pyproject.toml
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 maptasker-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-02-16 16:36:22.405000 maptasker-3.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      536 2024-03-04 15:40:38.700000 maptasker-3.1.8/README_PyPl.md
+-rw-r--r--   0        0        0        0 2024-03-10 15:08:20.218081 maptasker-3.1.8/maptasker/__init__.py
+-rw-r--r--   0        0        0     6148 2024-04-01 19:20:50.516566 maptasker-3.1.8/maptasker/assets/.DS_Store
+-rw-r--r--   0        0        0     9216 2024-02-22 20:13:00.839000 maptasker-3.1.8/maptasker/assets/Thumbs.db
+-rw-r--r--   0        0        0      390 2024-03-25 17:21:31.285000 maptasker-3.1.8/maptasker/assets/icons/arrow.png
+-rw-r--r--   0        0        0   104984 2023-11-21 17:46:03.716000 maptasker-3.1.8/maptasker/assets/maptasker_logo_dark.png
+-rw-r--r--   0        0        0   104904 2023-11-21 17:46:03.717000 maptasker-3.1.8/maptasker/assets/maptasker_logo_light.png
+-rw-r--r--   0        0        0     1782 2024-01-08 16:34:50.197000 maptasker-3.1.8/maptasker/main.py
+-rw-r--r--   0        0        0       17 2024-02-02 20:14:04.969000 maptasker-3.1.8/maptasker/src/__init__.py
+-rw-r--r--   0        0        0    13154 2024-03-01 18:04:39.824000 maptasker-3.1.8/maptasker/src/actargs.py
+-rw-r--r--   0        0        0    21610 2024-02-22 20:13:11.590000 maptasker-3.1.8/maptasker/src/action.py
+-rw-r--r--   0        0        0   116412 2024-03-08 20:16:24.476767 maptasker-3.1.8/maptasker/src/actionc.py
+-rw-r--r--   0        0        0     8377 2024-02-22 20:13:10.380000 maptasker-3.1.8/maptasker/src/actiond.py
+-rw-r--r--   0        0        0     9488 2024-04-08 18:07:30.469224 maptasker-3.1.8/maptasker/src/actione.py
+-rw-r--r--   0        0        0     9324 2024-02-22 20:13:11.464000 maptasker-3.1.8/maptasker/src/actionr.py
+-rw-r--r--   0        0        0    15551 2024-02-22 20:13:12.365000 maptasker-3.1.8/maptasker/src/actiont.py
+-rw-r--r--   0        0        0     3376 2024-02-22 20:13:12.356000 maptasker-3.1.8/maptasker/src/addcss.py
+-rw-r--r--   0        0        0     3783 2024-04-03 14:57:05.818846 maptasker-3.1.8/maptasker/src/caveats.py
+-rw-r--r--   0        0        0    11837 2024-04-03 14:54:27.598863 maptasker-3.1.8/maptasker/src/clip.py
+-rw-r--r--   0        0        0     8660 2023-12-04 16:08:02.839000 maptasker-3.1.8/maptasker/src/colors.py
+-rw-r--r--   0        0        0     3186 2024-03-08 20:16:24.477154 maptasker-3.1.8/maptasker/src/colrmode.py
+-rw-r--r--   0        0        0    11539 2024-02-02 20:14:09.416000 maptasker-3.1.8/maptasker/src/condition.py
+-rw-r--r--   0        0        0     2739 2024-03-10 19:26:48.459929 maptasker-3.1.8/maptasker/src/config.py
+-rw-r--r--   0        0        0     6541 2024-02-02 20:14:15.316000 maptasker-3.1.8/maptasker/src/debug.py
+-rw-r--r--   0        0        0      417 2023-12-04 16:07:45.842000 maptasker-3.1.8/maptasker/src/deprecate.py
+-rw-r--r--   0        0        0    30601 2024-03-25 17:21:29.641646 maptasker-3.1.8/maptasker/src/diagram.py
+-rw-r--r--   0        0        0    27007 2024-02-16 16:36:21.774000 maptasker-3.1.8/maptasker/src/diagutil.py
+-rw-r--r--   0        0        0    19996 2024-02-09 18:52:35.434000 maptasker-3.1.8/maptasker/src/dirout.py
+-rw-r--r--   0        0        0     2567 2024-03-25 17:21:29.642197 maptasker-3.1.8/maptasker/src/error.py
+-rw-r--r--   0        0        0     2399 2024-02-02 20:14:19.267000 maptasker-3.1.8/maptasker/src/fonts.py
+-rw-r--r--   0        0        0     4455 2024-02-22 20:13:11.559000 maptasker-3.1.8/maptasker/src/format.py
+-rw-r--r--   0        0        0     5871 2024-03-01 19:48:51.688000 maptasker-3.1.8/maptasker/src/frontmtr.py
+-rw-r--r--   0        0        0     5354 2024-03-25 17:21:29.642583 maptasker-3.1.8/maptasker/src/getbakup.py
+-rw-r--r--   0        0        0     2311 2024-03-28 13:52:59.398409 maptasker-3.1.8/maptasker/src/getids.py
+-rw-r--r--   0        0        0     9112 2024-03-25 17:21:29.643340 maptasker-3.1.8/maptasker/src/getputer.py
+-rw-r--r--   0        0        0     9754 2024-02-22 20:13:15.666000 maptasker-3.1.8/maptasker/src/globalvr.py
+-rw-r--r--   0        0        0    57097 2024-04-08 18:29:51.608214 maptasker-3.1.8/maptasker/src/guiutils.py
+-rw-r--r--   0        0        0     3542 2024-04-03 14:44:10.486216 maptasker-3.1.8/maptasker/src/initparg.py
+-rw-r--r--   0        0        0     2368 2023-11-15 16:38:53.257000 maptasker-3.1.8/maptasker/src/kidapp.py
+-rw-r--r--   0        0        0    25189 2024-04-04 17:15:09.357136 maptasker-3.1.8/maptasker/src/lineout.py
+-rw-r--r--   0        0        0    30560 2024-03-28 13:52:59.400006 maptasker-3.1.8/maptasker/src/mapit.py
+-rw-r--r--   0        0        0    11434 2024-03-25 17:21:29.644163 maptasker-3.1.8/maptasker/src/maputils.py
+-rw-r--r--   0        0        0     2788 2023-12-28 18:49:26.174000 maptasker-3.1.8/maptasker/src/nameattr.py
+-rw-r--r--   0        0        0    20711 2024-02-16 16:36:22.869000 maptasker-3.1.8/maptasker/src/outline.py
+-rw-r--r--   0        0        0    18958 2024-03-28 13:52:59.400466 maptasker-3.1.8/maptasker/src/parsearg.py
+-rw-r--r--   0        0        0     8606 2024-02-02 20:14:19.240000 maptasker-3.1.8/maptasker/src/prefers.py
+-rw-r--r--   0        0        0     6536 2024-03-17 15:16:47.058723 maptasker-3.1.8/maptasker/src/primitem.py
+-rw-r--r--   0        0        0    11265 2024-02-22 20:13:15.666000 maptasker-3.1.8/maptasker/src/proclist.py
+-rw-r--r--   0        0        0    14060 2024-02-22 20:13:18.209000 maptasker-3.1.8/maptasker/src/profiles.py
+-rw-r--r--   0        0        0     2280 2024-02-02 20:14:19.331000 maptasker-3.1.8/maptasker/src/progargs.py
+-rw-r--r--   0        0        0    14789 2024-04-04 17:15:09.360212 maptasker-3.1.8/maptasker/src/proginit.py
+-rw-r--r--   0        0        0    29494 2024-04-04 17:15:09.477887 maptasker-3.1.8/maptasker/src/projects.py
+-rw-r--r--   0        0        0     5099 2024-04-02 13:30:45.161179 maptasker-3.1.8/maptasker/src/property.py
+-rw-r--r--   0        0        0    20178 2024-03-28 13:52:59.401283 maptasker-3.1.8/maptasker/src/runcli.py
+-rw-r--r--   0        0        0     7006 2024-04-08 14:23:04.439614 maptasker-3.1.8/maptasker/src/rungui.py
+-rw-r--r--   0        0        0     9758 2024-03-25 17:21:29.645096 maptasker-3.1.8/maptasker/src/scenes.py
+-rw-r--r--   0        0        0    16315 2024-02-02 20:14:14.236000 maptasker-3.1.8/maptasker/src/servicec.py
+-rw-r--r--   0        0        0     6193 2024-02-22 20:13:15.794000 maptasker-3.1.8/maptasker/src/share.py
+-rw-r--r--   0        0        0     3658 2024-02-16 16:36:21.861000 maptasker-3.1.8/maptasker/src/shelsort.py
+-rw-r--r--   0        0        0     7386 2024-04-03 14:49:24.739707 maptasker-3.1.8/maptasker/src/sysconst.py
+-rw-r--r--   0        0        0     6151 2024-02-22 20:13:15.795000 maptasker-3.1.8/maptasker/src/taskactn.py
+-rw-r--r--   0        0        0     6835 2024-03-25 17:21:29.645740 maptasker-3.1.8/maptasker/src/taskerd.py
+-rw-r--r--   0        0        0     2695 2023-11-08 17:54:50.622000 maptasker-3.1.8/maptasker/src/taskflag.py
+-rw-r--r--   0        0        0    20135 2024-03-08 20:16:24.478872 maptasker-3.1.8/maptasker/src/tasks.py
+-rw-r--r--   0        0        0     9946 2024-03-01 19:48:54.083000 maptasker-3.1.8/maptasker/src/taskuniq.py
+-rw-r--r--   0        0        0     2100 2024-02-20 15:01:50.903000 maptasker-3.1.8/maptasker/src/twisty.py
+-rw-r--r--   0        0        0   104581 2024-04-08 18:28:11.307583 maptasker-3.1.8/maptasker/src/userintr.py
+-rw-r--r--   0        0        0    10324 2024-02-22 20:13:25.250000 maptasker-3.1.8/maptasker/src/xmldata.py
+-rw-r--r--   0        0        0     4998 2024-03-28 17:03:02.750060 maptasker-3.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 maptasker-3.1.8/PKG-INFO
```

### Comparing `maptasker-3.1.7/LICENSE.txt` & `maptasker-3.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/README_PyPl.md` & `maptasker-3.1.8/README_PyPl.md`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/assets/Thumbs.db` & `maptasker-3.1.8/maptasker/assets/Thumbs.db`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/assets/maptasker_logo_dark.png` & `maptasker-3.1.8/maptasker/assets/maptasker_logo_dark.png`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/assets/maptasker_logo_light.png` & `maptasker-3.1.8/maptasker/assets/maptasker_logo_light.png`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/main.py` & `maptasker-3.1.8/maptasker/main.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/actargs.py` & `maptasker-3.1.8/maptasker/src/actargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/action.py` & `maptasker-3.1.8/maptasker/src/action.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/actionc.py` & `maptasker-3.1.8/maptasker/src/actionc.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/actiond.py` & `maptasker-3.1.8/maptasker/src/actiond.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/actione.py` & `maptasker-3.1.8/maptasker/src/actione.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                 # Only display up to so many continued lines
                 if count == CONTINUE_LIMIT:
                     # Add comment that we have reached the limit for continued details
                     alist[-1] = f"{alist[-1]}</span>" + format_html(
                         "Red",
                         "",
                         (
-                            f" ... continue limit of {CONTINUE_LIMIT!s} "
+                            f"<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;... continue limit of {CONTINUE_LIMIT!s} "
                             'reached.  See "CONTINUE_LIMIT =" in config.py for '
                             "details"
                         ),
                         True,
                     )
                     # Done with this item...get out of loop.
                     break
```

### Comparing `maptasker-3.1.7/maptasker/src/actionr.py` & `maptasker-3.1.8/maptasker/src/actionr.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/actiont.py` & `maptasker-3.1.8/maptasker/src/actiont.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/addcss.py` & `maptasker-3.1.8/maptasker/src/addcss.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/caveats.py` & `maptasker-3.1.8/maptasker/src/caveats.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/clip.py` & `maptasker-3.1.8/maptasker/src/clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,58 +124,58 @@
 CURSOR_ON = "\033[?25h"  # makes cursor visible
 CURSOR_SAVE_POS = "\033[s"  # saves cursor position
 CURSOR_RESTORE_POS = "\033[u"  # returns cursor to last saved position
 
 PIC = (
     [
         ".......|~......",
-        "....../.\......",
-        ")..|~/___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r")..|~/___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "......~|.......",
-        "(x).../.\......",
-        "..~|./___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"(x).../.\......",
+        r"..~|./___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "...(X).|~......",
-        "....../.\......",
-        "..~|./___\~|...",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r"..~|./___\~|...",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "......~|.(X)...",
-        "....../.\......",
-        "...|~/___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"....../.\......",
+        r"...|~/___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         ".*....~|..*....",
-        "...*../.\....(o",
-        "..~|./___\.|~..",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r"...*../.\....(o",
+        r"..~|./___\.|~..",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
     [
         "...*...|~....*.",
-        ".*..*./.\.*...*",
-        "...|~/___\~|..(",
-        "../_\|::.|/_\..",
-        "..|$||/^\||$|..",
+        r".*..*./.\.*...*",
+        r"...|~/___\~|..(",
+        r"../_\|::.|/_\..",
+        r"..|$||/^\||$|..",
         "..|nnn|I|nnn|..",
     ],
 )
 
 PIC_COLORS = [
     "[0][7] = F_WHT, B_BLU",
     "[0][7] = F_WHT, B_BLU",
```

### Comparing `maptasker-3.1.7/maptasker/src/colors.py` & `maptasker-3.1.8/maptasker/src/colors.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/colrmode.py` & `maptasker-3.1.8/maptasker/src/colrmode.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/condition.py` & `maptasker-3.1.8/maptasker/src/condition.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/config.py` & `maptasker-3.1.8/maptasker/src/config.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/debug.py` & `maptasker-3.1.8/maptasker/src/debug.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/diagram.py` & `maptasker-3.1.8/maptasker/src/diagram.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/diagutil.py` & `maptasker-3.1.8/maptasker/src/diagutil.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/dirout.py` & `maptasker-3.1.8/maptasker/src/dirout.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/error.py` & `maptasker-3.1.8/maptasker/src/error.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/fonts.py` & `maptasker-3.1.8/maptasker/src/fonts.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/format.py` & `maptasker-3.1.8/maptasker/src/format.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/frontmtr.py` & `maptasker-3.1.8/maptasker/src/frontmtr.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/getbakup.py` & `maptasker-3.1.8/maptasker/src/getbakup.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/getids.py` & `maptasker-3.1.8/maptasker/src/getids.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/getputer.py` & `maptasker-3.1.8/maptasker/src/getputer.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/globalvr.py` & `maptasker-3.1.8/maptasker/src/globalvr.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/guiutils.py` & `maptasker-3.1.8/maptasker/src/guiutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,27 @@
 from maptasker.src.sysconst import CHANGELOG_FILE, NOW_TIME, VERSION
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 # TODO Change this 'changelog' with each release!  New lines (\n) must be added.
 CHANGELOG = """
-Version 3.1.7 Change Log\n\n
-- Fixed: Eliminate reading the XML file twice when running from the GUI.\n\n
-- Fixed: The GUI gets a 'Backup File not found' error message if displaying the treeview after having restored the settings.
+Version 3.1.8 Change Log\n
+### Added\n
+- Added: A ruler line has been added to the output as a break to indicate the end of a Project.\n
+- Added: A new button, 'Clear Messages', has been added to the GUI to empty the text message box.\n
+- Added: Display all of the settings that are initially restored with the start of the GUI.\n
+- Added: If the GUI is started along with the '-reset' option then display this in the message box.\n
+### Fixed\n
+- Fixed: The GUI is displaying 'Settings Restored' twice upon entry.\n
+- Fixed: 'SyntaxWarning: invalid escape sequence' error messages if running with Python 3.12 or greater.\n
+- Fixed: The GUI 'Restore Settings' now also includes the display of the colors restored.\n
+## Changed\n
+- Changed: GUI messages were revamped to provide better details.\n
+- Changed: Keep message history in GUI and retain each message's color.\n
 """
 default_font_size = 14
 
 # Set up for access to icons
 CURRENT_PATH = os.path.dirname(os.path.realpath(__file__))
 ICON_DIR = os.path.join(CURRENT_PATH, "../assets", "icons")
 ICON_PATH = {
@@ -208,18 +218,15 @@
         # Ping IP address.
         response = os.system(f"ping -c 1 -t50 > /dev/null {ip_address}")  # noqa: S605
         if response != 0:
             self.backup_error(
                 f"{ip_address} is not reachable (error {response}).  Try again.",
             )
             return False
-        self.display_message_box(
-            "Ping successful.",
-            True,
-        )
+        self.display_message_box("Ping successful.", True)
     else:
         self.backup_error(
             f"Invalid IP address: {ip_address}.  Try again.",
         )
         return False
 
     # Validate port number
@@ -405,14 +412,17 @@
     Parameters:
         - self (object): The object that the function is being called on.
     Returns:
         - None: The function does not return anything, but updates the message attribute of the object.
     Processing Logic:
         - Check if the changelog file exists.
         - If it exists, prepare to display changes and remove the file so we only display the changes once."""
+    # Test changelog before posting to PyPi
+    #self.message = CHANGELOG
+    
     if os.path.isfile(CHANGELOG_FILE):
         self.message = CHANGELOG
         os.remove(CHANGELOG_FILE)
 
 
 # ##################################################################################
 # Initialize the GUI (_init_ method)
@@ -443,16 +453,14 @@
     self.appearance_mode = None
     self.bold = None
     self.color_labels = None
     self.color_lookup = None
     self.color_text_row = None
     self.debug = None
     self.display_detail_level = None
-    self.edit = False
-    self.edit_type = ""
     self.preferences = None
     self.conditions = None
     self.everything = None
     self.taskernet = None
     self.exit = None
     self.fetched_backup_from_android = False
     self.file = None
@@ -765,15 +773,14 @@
         - Creates a grid title and adds it to the sidebar frame.
         - Defines the first grid / column for display detail level.
         - Defines the second grid / column for checkboxes related to display options.
         - Defines the third grid / column for buttons related to program settings.
         - Creates a textbox for displaying help information.
         - Creates a tabview for setting specific names, colors, and debug options.
         - Defines the fourth grid / column for checkboxes related to debug options.
-        - If the program is in edit mode, creates a fifth grid / column for selecting new or existing projects.
         - Defines the sixth grid / column for checkboxes related to runtime settings."""
 
     # Display the frame title
     self.logo_label = add_label(self, self.sidebar_frame, "Display Options", "", 20, "bold", 0, 0, 20, (60, 10), "s")
 
     # Start first grid / column definitions
 
@@ -1144,14 +1151,31 @@
         9,
         1,
         20,
         0,
         "sw",
     )
 
+    # 'Clear Messages' button definition
+    self.reset_button = add_button(
+        self,
+        self,
+        "#246FB6",
+        "",
+        "",
+        self.clear_messages_event,
+        2,
+        "Clear Messages",
+        1,
+        5,
+        1,
+        0,
+        0,
+        "s",
+    )
     # 'Get Backup Settings' button definition
     self.get_backup_button = self.display_backup_button(
         "Get XML from Android Device",
         "#246FB6",
         "#6563ff",
         self.get_backup_event,
     )
@@ -1254,16 +1278,14 @@
     # Start third grid / column definitions
     # create tabview for Name, Color, and Debug
     self.tabview = ctk.CTkTabview(self, width=250, segmented_button_fg_color="#6563ff")
     self.tabview.grid(row=0, column=2, padx=(20, 0), pady=(20, 0), sticky="nsew")
     self.tabview.add("Specific Name")
     self.tabview.add("Colors")
     self.tabview.add("Debug")
-    # if EDIT:
-    #    self.tabview.add("Edit")
 
     self.tabview.tab("Specific Name").grid_columnconfigure(0, weight=1)  # configure grid of individual tabs
     self.tabview.tab("Colors").grid_columnconfigure(0, weight=1)
 
     # Project Name
     self.string_input_button1 = ctk.CTkRadioButton(
         self.tabview.tab("Specific Name"),
@@ -1382,46 +1404,14 @@
         4,
         3,
         20,
         10,
         "w",
         "#6563ff",
     )
-
-    ## Edit Section Prompts
-    # if EDIT:
-    #    # TODO Clean up the geometry
-    #    self.edit_label = add_label(
-    #        self,
-    #        self.tabview.tab("Edit"),
-    #        "New or existing?",
-    #        0,
-    #        "",
-    #        "normal",
-    #        10,
-    #        2,
-    #        (20, 20),
-    #        (20, 20),
-    #        "e",
-    #    )
-    #    self.edit_optionemenu = add_option_menu(
-    #        self,
-    #        self.tabview.tab("Edit"),
-    #        self.edit_event,
-    #        [
-    #            "Create New",
-    #            "Edit Existing",
-    #        ],
-    #        3,
-    #        3,
-    #        (20, 20),
-    #        (20, 20),
-    #        "e",
-    #    )
-
     # Runtime
     self.runtime_checkbox = add_checkbox(
         self,
         self.tabview.tab("Debug"),
         self.runtime_checkbox_event,
         "Display Runtime Settings",
         3,
```

### Comparing `maptasker-3.1.7/maptasker/src/initparg.py` & `maptasker-3.1.8/maptasker/src/initparg.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,10 +50,8 @@
         "reset": False,  # Reset settings to default values
         "runtime": False,  # Display the runtime arguments/settings
         "single_profile_name": "",  # Display single Profile name only
         "single_project_name": "",  # Display single Project name only
         "single_task_name": "",  # Display single Task name only
         "twisty": False,  # Add Task twisty "▶︎" clickable icons for Task details
         "underline": False,  # Underline Project/Profile?Task/Scene names
-        "edit": False,  # Edit mode
-        "edit_type": "",  # Edit type: Create New or Edit Existing
     }
```

### Comparing `maptasker-3.1.7/maptasker/src/kidapp.py` & `maptasker-3.1.8/maptasker/src/kidapp.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/lineout.py` & `maptasker-3.1.8/maptasker/src/lineout.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,33 +58,33 @@
 
     def refresh_our_output(
         self,
         include_the_profile: bool,
         project_name: str,
         profile_name: str,
     ) -> None:
-        """        self.add_line_to_output(
-                    2,
-                    f"Project: {project_name}",
-                    ["", "project_color", FormatLine.add_end_span],
-                )
-            Refreshes the output by clearing existing output and starting anew.
-            Parameters:
-                include_the_profile (bool): Flag to indicate whether this is a Profile to be included.
-                project_name (str): Name of the Project, if any.
-                profile_name (str): Name of the Profile, if any.
-            Returns:
-                - None: No return value.
-            Processing Logic:
-                - Clears existing output and starts anew.
-                - Adds directory item.
-                - Starts Project list.
-                - Checks if Profile is to be included.
-                - Starts Profile list.
-                - Starts Project list."""
+        """self.add_line_to_output(
+                2,
+                f"Project: {project_name}",
+                ["", "project_color", FormatLine.add_end_span],
+            )
+        Refreshes the output by clearing existing output and starting anew.
+        Parameters:
+            include_the_profile (bool): Flag to indicate whether this is a Profile to be included.
+            project_name (str): Name of the Project, if any.
+            profile_name (str): Name of the Profile, if any.
+        Returns:
+            - None: No return value.
+        Processing Logic:
+            - Clears existing output and starts anew.
+            - Adds directory item.
+            - Starts Project list.
+            - Checks if Profile is to be included.
+            - Starts Profile list.
+            - Starts Project list."""
         """
         For whatever reason, we need to clear out the existing output and start anew.
 
                 :param include_the_profile: Boolean flag to indicate whether this is
                     a Profile to be included
                 :param project_name: name of the Project, if any
                 :param profile_name: name of the Profile, if any
```

### Comparing `maptasker-3.1.7/maptasker/src/mapit.py` & `maptasker-3.1.8/maptasker/src/mapit.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/maputils.py` & `maptasker-3.1.8/maptasker/src/maputils.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/nameattr.py` & `maptasker-3.1.8/maptasker/src/nameattr.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/outline.py` & `maptasker-3.1.8/maptasker/src/outline.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/parsearg.py` & `maptasker-3.1.8/maptasker/src/parsearg.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/prefers.py` & `maptasker-3.1.8/maptasker/src/prefers.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/primitem.py` & `maptasker-3.1.8/maptasker/src/primitem.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/proclist.py` & `maptasker-3.1.8/maptasker/src/proclist.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/profiles.py` & `maptasker-3.1.8/maptasker/src/profiles.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/progargs.py` & `maptasker-3.1.8/maptasker/src/progargs.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/proginit.py` & `maptasker-3.1.8/maptasker/src/proginit.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,20 @@
     - Extracts all the XML data from the file
     - Closes the file after reading
     - Outputs initial information like header and source to the user
     """
     # Only get the XML if we don't already have it.
     tasker_root_elements = PrimeItems.tasker_root_elements
     return_code = 0
-    if not tasker_root_elements["all_projects"] and not tasker_root_elements["all_profiles"] and not tasker_root_elements["all_tasks"] and not tasker_root_elements["all_scenes"]:
+    if (
+        not tasker_root_elements["all_projects"]
+        and not tasker_root_elements["all_profiles"]
+        and not tasker_root_elements["all_tasks"]
+        and not tasker_root_elements["all_scenes"]
+    ):
 
         # We don't yet have the data.  Let's get it.
         if not PrimeItems.program_arguments["file"]:
             PrimeItems.program_arguments["file"] = PrimeItems.file_to_get
 
         # Only display message box if we don't yet have the file name,if this is not the first time ever that we have run,
         # and not running from the GUI.
```

### Comparing `maptasker-3.1.7/maptasker/src/projects.py` & `maptasker-3.1.8/maptasker/src/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         task_list = []
         task_output_lines = []
         for task in PrimeItems.tasker_root_elements["all_tasks"]:
             task_list.append(
                 {
                     "xml": PrimeItems.tasker_root_elements["all_tasks"][task]["xml"],
                     "name": PrimeItems.tasker_root_elements["all_tasks"][task]["name"],
-                }
+                },
             )
             task_output_lines.append(" ")
             if PrimeItems.tasker_root_elements["all_tasks"][task]["name"]:
                 PrimeItems.grand_totals["named_tasks"] += 1
             else:
                 PrimeItems.grand_totals["unnamed_tasks"] += 1
         tasks.output_task_list(
@@ -113,19 +113,19 @@
         process_list(
             "Scene:",
             scene_list,
             "",
             found_tasks,
         )
 
-    PrimeItems.output_lines.add_line_to_output(
-        3,
-        "",
-        FormatLine.dont_format_line,
-    )  # Close Project list
+    # PrimeItems.output_lines.add_line_to_output(
+    #    3,
+    #    "",
+    #    FormatLine.dont_format_line,
+    # )  # Close Project list
 
     # Return a list of Tasks found thus far with duplicates remove
     # Reference: https://www.pythonmorsels.com/deduplicate-lists/
     # return list(dict.fromkeys(found_tasks).keys())
     return list(set(found_tasks))
 
 
@@ -439,14 +439,21 @@
             f" not in any Profile, {named_task_count_total} named Tasks out of"
             f" {task_count_unnamed + named_task_count_total} total Tasks,"
             f" and {scene_count} Scenes</DIV><br><br>"
         ),
         ["", "project_color", FormatLine.add_end_span],
     )
 
+    # Print a ruler
+    PrimeItems.output_lines.add_line_to_output(
+        5,
+        "<hr>",
+        FormatLine.dont_format_line,
+    )
+
 
 # ##################################################################################
 # Output the remaining components related to the Project
 # ##################################################################################
 def finish_up(
     project: defusedxml.ElementTree.XML,
     project_name: str,
```

### Comparing `maptasker-3.1.7/maptasker/src/property.py` & `maptasker-3.1.8/maptasker/src/property.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/runcli.py` & `maptasker-3.1.8/maptasker/src/runcli.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/rungui.py` & `maptasker-3.1.8/maptasker/src/rungui.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # GNU General Public License v3.0                                                      #
 # Permissions of this strong copyleft license are conditioned on making available      #
 # complete source code of licensed works and modifications, which include larger works #
 # using a licensed work, under the same license. Copyright and license notices must be #
 # preserved. Contributors provide an express grant of patent rights.                   #
 #                                                                                      #
 # #################################################################################### #
+from __future__ import annotations
+
 import contextlib
 import sys
 
 from maptasker.src.colrmode import set_color_mode
 from maptasker.src.error import error_handler
 from maptasker.src.getputer import save_restore_args
 from maptasker.src.initparg import initialize_runtime_arguments
@@ -42,23 +44,62 @@
     try:
         return int(value_to_convert)
     except (ValueError, TypeError):
         return default_value
 
 
 # ##################################################################################
+# Get the colors to use.
+# ##################################################################################
+def do_colors(user_input: dict) -> dict:
+    """Sets color mode and processes colors.
+    Parameters:
+        - user_input (dict): User input dictionary containing appearance mode and color lookup.
+    Returns:
+        - colormap (dict): Dictionary of colors after processing.
+    Processing Logic:
+        - Set color mode based on user input.
+        - Process color lookup if provided.
+        - Set flag for GUI usage."""
+
+    # Appearance change: Dark or Light mode?
+    colormap = set_color_mode(user_input.appearance_mode)
+
+    # Process the colors
+    if user_input.color_lookup:
+        for key, value in user_input.color_lookup.items():
+            colormap[key] = value
+
+    PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
+
+    return colormap
+
+
+# ##################################################################################
 # Get the program arguments from GUI
 # ##################################################################################
 def process_gui(use_gui: bool) -> tuple[dict, dict]:
-    """
-    Present the GUI and get the runtime details
-        :param use_gui: flag if usijng the GUI, make sure we import it
-        :return: program runtime arguments and colors to use in the output
-    """
     # global MyGui
+    """Parameters:
+        - use_gui (bool): Flag to indicate whether to use GUI or not.
+    Returns:
+        - tuple[dict, dict]: Tuple containing program arguments and colors to use.
+    Processing Logic:
+        - Import MyGui if use_gui is True.
+        - Set flag to indicate GUI usage.
+        - Delete previous Tkinter window if it exists.
+        - Display GUI and get user input.
+        - Initialize runtime arguments if not already set.
+        - If user clicks "Exit" button, save settings and exit program.
+        - If user closes window, cancel program.
+        - If user clicks "Run" button, get input from GUI variables.
+        - Set program arguments in dictionary.
+        - Convert display_detail_level and indent to integers.
+        - Get font from GUI.
+        - Return program arguments and colors to use."""
     if use_gui:
         from maptasker.src.userintr import MyGui
 
     PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
 
     # Get rid of any previous Tkinter window
     if PrimeItems.tkroot is not None:
@@ -103,21 +144,9 @@
     )
     # Convert indent to integer
     PrimeItems.program_arguments["indent"] = convert_to_integer(PrimeItems.program_arguments["indent"], 4)
     # Get the font
     if the_font := user_input.font:
         PrimeItems.program_arguments["font"] = the_font
 
-    # Appearance change: Dark or Light mode?
-    colormap = set_color_mode(user_input.appearance_mode)
-
-    # Process the colors
-    if user_input.color_lookup:
-        for key, value in user_input.color_lookup.items():
-            colormap[key] = value
-
-    PrimeItems.program_arguments["gui"] = True  # Set flag to indicate we are using GUI
-
-    return (
-        PrimeItems.program_arguments,
-        colormap,
-    )
+    # Return the program arguments and colors to use.
+    return (PrimeItems.program_arguments, do_colors(user_input))
```

### Comparing `maptasker-3.1.7/maptasker/src/scenes.py` & `maptasker-3.1.8/maptasker/src/scenes.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/servicec.py` & `maptasker-3.1.8/maptasker/src/servicec.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/share.py` & `maptasker-3.1.8/maptasker/src/share.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/shelsort.py` & `maptasker-3.1.8/maptasker/src/shelsort.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/sysconst.py` & `maptasker-3.1.8/maptasker/src/sysconst.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import ClassVar
 
 import darkdetect
 
 # Global constants
 UNKNOWN_TASK_NAME = "Unnamed/Anonymous."
 
-VERSION = "3.1.7"
+VERSION = "3.1.8"
 MY_VERSION = f"MapTasker version {VERSION}"
 
 MY_LICENSE = "MIT License"
 NO_PROJECT = "-none found."
 COUNTER_FILE = ".MapTasker_RunCount.txt"
 OLD_ARGUMENTS_FILE = ".MapTasker_arguments.json"
 ARGUMENTS_FILE = "MapTasker_Settings.toml"
@@ -126,16 +126,14 @@
     "rerun": "ReRun Program",
     "runtime": "Display Runtime Arguments/Settings",
     "single_profile_name": "Single Profile Name",
     "single_project_name": "Single Project Name",
     "single_task_name": "Single Task Name",
     "twisty": "Hide Task Details under Twisty",
     "underline": "Underline Names",
-    "edit": "Edit",
-    "edit_type": "Edit Type",
 }
 
 # Debug stuff
 logger = logging.getLogger("MapTasker")
 debug_out = False  # Prints the line to be added to the output
 DEBUG_PROGRAM = False
 debug_file = "maptasker_debug.log"
@@ -147,15 +145,15 @@
 pattern3 = re.compile("<")
 pattern4 = re.compile(">")
 
 pattern8 = re.compile("<br>")
 pattern9 = re.compile("</span></span>")
 pattern10 = re.compile("</p></p>")
 pattern11 = re.compile(".*[A-Z].*")
-pattern12 = re.compile("[%]\w+")  # matches any word-constituent character.   # noqa: W605
+pattern12 = re.compile(r"[%]\w+")  # matches any word-constituent character.
 RE_FONT = re.compile(r"</font>")
 
 clean = re.compile("<.*?>")
 
 
 # ASCII Color Definitions
 class Colors:
```

### Comparing `maptasker-3.1.7/maptasker/src/taskactn.py` & `maptasker-3.1.8/maptasker/src/taskactn.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/taskerd.py` & `maptasker-3.1.8/maptasker/src/taskerd.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/taskflag.py` & `maptasker-3.1.8/maptasker/src/taskflag.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/tasks.py` & `maptasker-3.1.8/maptasker/src/tasks.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/taskuniq.py` & `maptasker-3.1.8/maptasker/src/taskuniq.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/twisty.py` & `maptasker-3.1.8/maptasker/src/twisty.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/maptasker/src/userintr.py` & `maptasker-3.1.8/maptasker/src/userintr.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 from maptasker.src.taskerd import get_the_xml_data
 
 # Color Modes: "System" (standard), "Dark", "Light"
 customtkinter.set_appearance_mode("System")
 # Themes: "blue" (standard), "green", "dark-blue"
 customtkinter.set_default_color_theme("blue")
 
+# NOTE: The textbox is used for help information via new_message_box, normal one-liner messages via display_message_box
+#       and multi-line messages via display_multiple_message.
 # Help Text
 INFO_TEXT = (
     "MapTasker displays your Android Tasker configuration based on your uploaded Tasker XML "
     "file (e.g. 'backup.xml'). The display will optionally include all Projects, Profiles, Tasks "
     "and their actions, Profile/Task conditions and other Profile/Task related information.\n\n"
     "* Display options are:\n"
     "    Level 0: display first Task action only, for unnamed Tasks only (silent).\n"
@@ -83,14 +85,15 @@
     "* Save Settings - Save these settings for later use.\n\n"
     "* Restore Settings - Restore the settings from a previously saved session.\n\n"
     "* Report Issue - This will bring up your browser to the issue reporting site, and you can use this to "
     "either report a bug or request a new feature ( [Feature Request] )\n\n"
     "* Appearance Mode: Dark, Light, or System default.\n\n"
     "* Tree View: Display a tree of your Projects/Profiles/Tasks.\n\n"
     "* Reset Options: Clear everything and start anew.\n\n"
+    "* Clear Messages: Clear any messages in the textbox.\n\n"
     "* Font To Use: Change the monospace font used for the output.\n\n"
     "* Display Outline: Display Projects/Profiles/Tasks/Scenes configuration outline.\n\n"
     "* Get XML from Android Device: fetch the backup/exported "
     "XML file from Androiddevice.  You will be asked for the IP address and port number for your"
     " Android device, as well as the file location on the device.\n\n"
     "* Run and Exit: Run the program with the settings provided and then exit.\n"
     "* ReRun: Run multiple times (each time with new settings) without exiting.\n\n"
@@ -147,15 +150,15 @@
     "input to the program once you subsequently click on the 'Run' or 'ReRun' button.\n\n"
     "In order for this to work, you MUST have already imported the 'MapTasker List' profile into Tasker running "
     "on your Android device.  This profile can be found at the following URL:\n\n"
     "    https://shorturl.at/buvK6\n\n"
 )
 
 TREEVIEW_HELP_TEXT = (
-    "The Treeview is experimental and has the following limitations/behavior:\n\n"
+    "The Treeview has the following limitations/behavior:\n\n"
     "- Huge configurations that scroll beyond the bottom of the screen are not viewable in their entirety yet.\n\n"
     "- Only Projects can be displayed. XML consisting of only a single Profile or Task will not be displayed.\n\n"
     "- If the XML has already been fetched, it will be used as input to the treeview.  Hitting the 'Reset' button will clear the treeview data."
     " In otherwords, the treeview will remain the same until either the 'Reset' button is hit, or a new XML file is fetched from the"
     " Android device or the program is run with the '-reset' option."
 )
 
@@ -189,32 +192,31 @@
 
         # set default values
         self.set_defaults(True)
 
         # Now restore the settings and update the fields if not resetting.
         if not PrimeItems.program_arguments["reset"]:
             self.restore_settings_event()
-
-            self.display_message_box("Settings restored.", True)
-
-            self.message = "Settings restored."  # self.message set to "" in set_defaults, above.
+        else:
+            self.display_message_box("GUI started with the '-reset' option.\n", True)
 
             if self.android_ipaddr:
                 # Display backup details as a label
                 self.display_backup_details()
 
             # Check for single item only to be displayed
             if self.single_project_name:
                 self.single_name_status(f"Display only Project '{self.single_project_name}'.", "#3f99ff")
             if self.single_profile_name:
                 self.single_name_status(f"Display only Profile '{self.single_profile_name}'.", "#3f99ff")
             if self.single_task_name:
                 self.single_name_status(f"Display only Task '{self.single_task_name}'.", "#3f99ff")
 
         # Check if newer version of our code is available on Pypi (only check every 24 hours).
+        # If so, add a button to enable user to update.
         if is_new_version():
             self.new_version = True
             # We have a new version.  Let user upgrade.
             self.upgrade_button = add_button(
                 self,
                 self,
                 "",
@@ -279,22 +281,19 @@
         self.indent = 4
         self.color_labels = []
         self.android_ipaddr = ""
         self.android_port = ""
         self.android_file = ""
         if first_time:
             # self.textbox.insert("0.0", HELP)
-            self.all_messages = ""
+            self.all_messages = {}
         self.color_lookup = {}  # Setup default dictionary as empty list
         self.font = OUTPUT_FONT
         self.gui = True
         self.color_row = 4
-        self.edit = False
-        self.edit_type = ""
-
         self.message = ""
 
         # Display current Items setting.
         self.single_name_status("Display all Projects, Profiles, and Tasks.", "#3f99ff")
 
     # ##################################################################################
     # Display the Backup button
@@ -332,53 +331,56 @@
         )
         return self.get_backup_button
 
     # ##################################################################################
     # Display Message Box
     # ##################################################################################
     def display_message_box(self, message: str, good: bool) -> None:
-        # If "good", display in green.  Otherwise, must be bad and display in red.
-        r"""
-        Displays a message box with the given message and color.
-
+        """Display Message Box
         Args:
-            message: The message to display in one line.
-            good: Whether the message is good or bad in one line.
-        Returns:
-            None: No return value in one line.
-
-        - Deletes prior textbox contents
-        - Recreates the textbox
-        - Sets the color based on good/bad
-        - Inserts the accumulated messages
-        - Configures textbox properties
+            message (str): The text to display in the textbox.
+            good (bool): True = No Problem = Green, False = Error = Red
         """
-        color = "Green" if good else "Red"
+
+        # If "good", display in green.  Otherwise, must be bad and display in red.
+        # color = "Green" if good else "Red"
+        bad_color = "red"
+        good_color = "green"
         # Delete prior contents
         self.textbox.destroy()
 
-        # Delete message history if this is foran error
-        if not good:
-            self.all_messages = ""
-
         # Recreate text box
         self.textbox = customtkinter.CTkTextbox(self, height=500, width=600)
         self.textbox.grid(row=0, column=1, padx=20, pady=40, sticky="nsew")
 
-        # Display some colored text
-        # self.textbox.insert('end', 'This is some colored text.\n')
-        # self.textbox.tag_add('color', '1.5', '1.11')  # '1.5' means first line, 5th character; '1.11' means first line, 11th character
-        # self.textbox.tag_config('color', foreground='red')
+        line_num = 0
+
+        # Go through our messages and add each to the text box.
+        for num, key in enumerate(self.all_messages):
+            line_num = num + 1
+            line_num_str = str(line_num)
+            line_detail = self.all_messages[key]
+            # fmt: off
+            self.textbox.insert(f"{line_num_str}.0", line_detail["text"], (line_num_str))
+            self.textbox.tag_add(line_num_str, f"{line_num_str}.0", f"{line_num_str}.{len(line_detail["text"])!s}") # fmt: skip
+            # fmt: on
+            self.textbox.tag_config(line_num_str, foreground=line_detail["color"])
+
+        # Insert the text with our new message into the text box.
+        line_num += 1
+        line_num_str = str(line_num)
+        # Add this message to our dictionary of messages.
+        self.all_messages[line_num] = {"text": f"{message}\n", "color": good_color if good else bad_color}
+        # Add the test and color to the text box.
+        # fmt: off
+        self.textbox.insert(f"{line_num_str}.0", f"{message}\n", (line_num_str))
+        self.textbox.tag_add(line_num_str, f"{line_num_str}.0", f"{line_num_str}.{len(message)!s}")
+        # fmt: on
+        self.textbox.tag_config(line_num_str, foreground=self.all_messages[line_num]["color"])
 
-        self.all_messages = f"{self.all_messages}{message}\n"
-        # self.all_messages = f"{message}\n"
-        # insert at line 0 character 0
-        self.textbox.insert("0.0", self.all_messages)
-        # Set read-only, color, wrap around and font
-        self.textbox.configure(state="disabled", text_color=color, wrap="word", font=(self.font, 14))
         self.textbox.focus_set()
 
     # ##################################################################################
     # Validate name entered
     # ##################################################################################
     def check_name(self, the_name: str, element_name: str) -> bool:
         """
@@ -394,50 +396,49 @@
             3. Check that named item exists in valid items
             4. If error, display message and clear individual names
             5. If valid, display confirmation message and return True
         """
         error_message = ""
         # Check for missing name
         if not the_name:
-            error_message = (
-                f"\n\nEither the name entered for the {element_name} is blank or the"
-                f" 'Cancel' button was clicked.\n\nAll {element_name}s will be"
-                " displayed."
-            )
+            error_message = [
+                f"Either the name entered for the {element_name} is blank or the"
+                f" 'Cancel' button was clicked.\n",
+                "All Projects, Profiles, and Tasks will be displayed.\n",
+                ]
+
             self.named_item = False
         # Check to make sure only one named item has been entered
         elif self.single_project_name and self.single_profile_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Project and a Profile name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n", "You have entered both a Project and a Profile name!\n", "Try again and only select one.",
+            ]
         elif self.single_project_name and self.single_task_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Project and a Task name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n", "You have entered both a Project and a Task name!\n", "Try again and only select one.",
+            ]
         elif self.single_profile_name and self.single_task_name:
-            error_message = (
-                "Error:\n\nYou have entered both a Profile and a Task name!\n\nTry again and only select one."
-            )
+            error_message = [
+                "Error:\n\n", "You have entered both a Profile and a Task name!\n", "Try again and only select one.",
+            ]
         # Make sure the named item exists
         elif not valid_item(the_name, element_name, self.debug, self.appearance_mode):
-            error_message = f'Error: "{the_name}" {element_name} not found!!  Try again.\n{PrimeItems.error_msg}'
+            error_message = [f'Error: "{the_name}" {element_name} not found!  Try again.\n']
 
         # If we have an error, display it and blank out the various individual names
         if error_message:
-            # Delete prior contents
-            self.all_messages = ""
-
-            self.display_message_box(error_message, False)
+            self.display_multiple_messages(error_message, False)
             (
                 self.single_project_name,
                 self.single_profile_name,
                 self.single_task_name,
             ) = ("", "", "")
             return False
 
+        # No error.
         self.display_message_box(
             f"Display only the '{the_name}' {element_name} (overrides any previous set name).",
             True,
         )
         return True
 
     # ##################################################################################
@@ -675,14 +676,30 @@
             anchor="sw",
             font=(font_selected, 14),
         )
         self.font_out_label.grid(row=6, column=1, padx=10, pady=10, sticky="sw")
         self.display_message_box(f"Font To Use set to {font_selected}", True)
 
     # ##################################################################################
+    # Clear the message text box.
+    # ##################################################################################
+    def clear_messages_event(self) -> None:
+        """
+        Clears the message box
+        Args:
+            None
+        Returns:
+            None
+        Processing Logic:
+            - Destroys the message box
+        """
+        self.all_messages = {}
+        self.textbox.destroy()
+
+    # ##################################################################################
     # Process the Display Detail Level selection
     # ##################################################################################
     def detail_selected_event(self, display_detail: str) -> None:
         """
         Set display detail level and update UI
         Args:
             display_detail (str): The selected display detail level
@@ -737,37 +754,14 @@
         - Update the indent option dropdown to the selected amount
         - Display confirmation message of indentation amount"""
         self.indent = ident_amount
         self.indent_option.set(ident_amount)
         self.inform_message("Indentation Amount", True, ident_amount)
 
     # ##################################################################################
-    # Edit selection
-    # ##################################################################################
-    def edit_event(self, edit_type: str) -> None:
-        """
-        Edit an event by setting the edit type.
-
-        :param edit_type: A string representing the type of edit.
-        :return: None
-        """
-
-        self.edit_type = edit_type
-        self.edit = True
-
-        from edittasker.src.edtnewui import ToplevelWindow
-
-        self.edit_type = edit_type
-        self.edit = True
-        if self.toplevel_window is None or not self.toplevel_window.winfo_exists():
-            self.toplevel_window = ToplevelWindow(self)  # create window if its None or destroyed
-        else:
-            self.toplevel_window.focus()  # if window exists focus it
-
-    # ##################################################################################
     # Process color selection
     # ##################################################################################
     def colors_event(self, color_selected_item: str) -> None:
         """
         Changes the color for a selected item
         Args:
             color_selected_item (str): The item whose color is to be changed
@@ -929,30 +923,31 @@
             ),
             "display_detail_level": lambda: self.detail_selected_event("4"),
         }
 
         self.everything = self.everything_checkbox.get()
         value = self.everything
 
-        new_message = all_messages = ""
+        #new_message = all_messages = ""
         for key in message_map:
             if message_func := message_map.get(key):
-                new_message = f"{message_func()}"
+                # Display detail level requires special handling.
                 if key == "display_detail_level":
-                    new_message = f"Display Detail Level: {self.display_detail_level}"
-                all_messages = f"{all_messages}{new_message}"
+                    self.display_message_box(f"Display Detail Level: {self.display_detail_level}", True)
+                else:
+                    # Handle toggle: select/deselect checkbox and set/unset setting.
+                    self.display_message_box(f"{message_func()}", True)
+
             # Check if key is an attribute on self before setting
             if hasattr(self, key) and key != "display_detail_level":
                 setattr(self, key, value)
 
         # Handle Display Detail Level
         self.display_detail_level = 4
 
-        self.display_message_box(all_messages, True)
-
     # ##################################################################################
     # Process the 'Tasker Preferences' checkbox
     # ##################################################################################
     def preferences_event(self) -> None:
         """
         Get user input on whether to display tasker preferences
         Args:
@@ -1124,23 +1119,23 @@
         self.textbox = customtkinter.CTkTextbox(self, height=600, width=250)
         self.textbox.configure(scrollbar_button_color="#6563ff", wrap="word")
         self.textbox.grid(row=0, column=1, padx=(20, 0), pady=(20, 0), sticky="ew")
         # Insert the text.
         self.textbox.insert("0.0", message)
         # Set read-only, color, wrap around and font
         self.textbox.configure(state="disabled", font=(self.font, 14), wrap="word")
-        # Display some colored text
+        # Display some colored text: the heading
         # self.textbox.insert('end', 'This is some colored text.\n')
         self.textbox.tag_add(
             "color",
             "1.0",
             f"1.{len(message)}",
         )  # '1.5' means first line, 5th character; '1.11' means first line, 11th character
         self.textbox.tag_config("color", foreground="green")
-        self.all_messages = ""
+        self.all_messages = {}
 
     # ##################################################################################
     # Process the 'Display Help' button
     # ##################################################################################
     def help_event(self) -> None:
         """Displays help information in a message box.
         Args:
@@ -1362,14 +1357,26 @@
                 setattr(self, key, value)
         else:
             # Use dictionary lookup anmd lambda funtion to process key/value
             message_func = message_map.get(key)
             if message_func:
                 message = message_func()
 
+        # Cleanup the end of the message if it is not set.
+        the_empty_ending = "set to \n"
+        the_empty_ending_length = len(the_empty_ending)
+        named_ending = "named ''.\n"
+        named_ending_length = len(named_ending)
+        if message is None or message == "":
+            return ""
+        if message.endswith(the_empty_ending):
+            message = f"{message[:-the_empty_ending_length]} is not set.\n"
+        elif message.endswith(named_ending):
+            message = f"{message[:-named_ending_length]} is not named.\n"
+
         return message
 
     # ##################################################################################
     # Process the 'Restore Settings' checkbox
     # ##################################################################################
     def restore_settings_event(self) -> None:
         """
@@ -1391,22 +1398,25 @@
         temp_args, self.color_lookup = save_restore_args(temp_args, self.color_lookup, False)
         # Check for errors
         with contextlib.suppress(KeyError):
             if temp_args["msg"]:
                 self.display_message_box(temp_args["msg"], False)
                 temp_args["msg"] = ""
                 return
+
+        # If no colors restored, let user know.
+        if not self.color_lookup:
+            self.display_message_box("Colors set to defaults.", True)
         # Restore progargs values
         if temp_args or self.color_lookup:
             self.extract_settings(temp_args)
             self.restore = True
+
         else:  # Empty?
             self.display_message_box("No settings file found.", False)
-        # Empty message queue so we don't fill it up (causes as display text problem)
-        self.all_messages = ""
 
     # ##################################################################################
     # We have read colors and runtime args from backup file.  Now extract them for use.
     # ##################################################################################
     def extract_settings(self, temp_args: dict) -> None:
         """
         Extract settings from arguments dictionary
@@ -1415,34 +1425,32 @@
         Returns:
             None: Does not return anything
         - Loops through dictionary and sets attributes on object
         - Calls restore_display to get message for setting change
         - Loops through color lookup and builds message of color changes
         - Displays message box with all setting changes
         """
-        all_messages, new_message = "", ""
-        self.all_messages = ""
         for key, value in temp_args.items():
             if key is not None:
                 setattr(self, key, value)
                 if new_message := self.restore_display(key, value):
-                    all_messages = f"{all_messages}{new_message}"
+                    self.display_message_box(f"{new_message}\n", True)
         # Display the restored color changes, using the reverse dictionary of
         #   TYPES_OF_COLOR_NAMES (found in sysconst.py)
         inv_color_names = {v: k for k, v in TYPES_OF_COLOR_NAMES.items()}
         for key, value in self.color_lookup.items():
             if key is not None:
                 if key == "msg":
                     inv_color_names[key] = ""
                 else:
                     with contextlib.suppress(KeyError):
-                        all_messages = f"{all_messages} {inv_color_names[key]} color set to {value}\n"
+                        self.display_message_box(f"{inv_color_names[key]} color set to {value}\n", True)
 
         # Display the queue of messages
-        self.display_message_box(f"{all_messages}\nSettings restored.", True)
+        self.display_message_box("Settings restored.\n", True)
 
     # ##################################################################################
     # Display an input field and a label for the user to input a value
     # ##################################################################################
     def display_label_and_input(
         self,
         label: str,
@@ -1682,14 +1690,29 @@
         if error_message:
             self.display_message_box(
                 error_message,
                 False,
             )
 
     # ##################################################################################
+    # Get list of lines and output them.
+    # ##################################################################################
+    def display_multiple_messages(self, details: list, good_or_bad: bool) -> None:
+        """
+        Display Android settings based on the given details list.
+
+        :param self: The instance of the class.
+        :param details: A list containing the details to be displayed.
+        :param good_or_bad: True = good (green), False = bad (red).
+        :return: None
+        """
+        for line in details:
+            self.display_message_box(line, good_or_bad)
+
+    # ##################################################################################
     # Fetch the backup ip and file details, and validate.
     # This function can be entered through two paths:
     # 1- User clicked on the 'Get Backup Settings' button
     # 2- User clicked on the 'List XML Files' button
     # ##################################################################################
     def fetch_backup_event(self) -> None:
         """Fetches backup event details from user input
@@ -1751,22 +1774,21 @@
 
         # All is well.  Save the info, restore the button and get rid of the input fields.
         self.android_ipaddr = android_ipaddr
         self.android_port = android_port
         if not self.list_files:
             self.android_file = android_file
         clear_android_buttons(self)
-        self.display_message_box(
-            (
-                f"\n\nGet XML IP Address set to: {self.android_ipaddr}\n\nPort"
-                f" Number set to: {self.android_port}\n\nGet"
-                f" Location set to: {self.android_file}"
-                f"\n\nXML file will be fetched when 'Run' is selected."
-            ),
-            True,
+        self.display_multiple_messages(
+            [
+                f"Get XML IP Address set to: {self.android_ipaddr}\n",
+                f"Port Number set to: {self.android_port}\n",
+                f"Get Location set to: {self.android_file}\n",
+                "XML file acquired.\n",
+            ], True,
         )
 
         # Display backup details as a label again.
         self.display_backup_details()
 
     # ##################################################################################
     # Fetching backup from Android.  Let the user know the specific details.
@@ -1779,15 +1801,14 @@
         Returns:
             None: Does not return anything.
         Processing Logic:
             - Displays label and input for getting backup.xml file from Android device
             - Displays label and input for TCP/IP Address and Port of Android device
             - Displays label and input for location of backup file on Android device
         """
-        self.ip_label = self.port_label = self.file_label = None
         self.ip_label = add_label(
             self,
             self,
             "Getting XML file from Android device:",
             "",
             12,
             "normal",
@@ -1840,15 +1861,15 @@
             None
         """
         clear_android_buttons(self)
         self.fetched_backup_from_android = False
         self.android_file = ""
         self.android_ipaddr = ""
         self.android_port = ""
-        self.display_message_box("Get XML Details Cancelled.", True)
+        self.display_message_box("Get XML Details Cancelled.", False)
 
     # ##################################################################################
     # List files event
     # ##################################################################################
     def list_files_event(self) -> None:
         """
         Closes the backup details window.
@@ -1866,28 +1887,26 @@
     # ##################################################################################
     def file_selected_event(self, android_file: str) -> None:
         """User has selected a specific XML file from pulldown menu.
         Returns:
             - None: Adds android_file to file_list."""
         self.android_file = android_file
         clear_android_buttons(self)
-        self.display_message_box(
-            (
-                f"\n\nGet XML IP Address set to: {self.android_ipaddr}\n\nPort"
-                f" Number set to: {self.android_port}\n\nGet"
-                f" Location set to: {self.android_file}"
-                f"\n\nXML file will be fetched when 'Run' is selected."
-            ),
-            True,
+        self.display_multiple_messages(
+            [
+                f"Get XML IP Address set to: {self.android_ipaddr}\n",
+                f"Port Number set to: {self.android_port}\n",
+                f"Get Location set to: {self.android_file}\n",
+                "XML file acquired.\n",
+            ], True,
         )
 
-        # Validate XML file.add
+        # Validate XML file.
         PrimeItems.program_arguments["gui"] = True
         return_code, error_message = validate_xml_file(self.android_ipaddr, self.android_port, android_file)
-
         if return_code > 0:
             self.display_message_box(error_message, False)  # Error out and exit
             return
 
         # Display backup details as a label again.
         self.display_backup_details()
 
@@ -1959,15 +1978,15 @@
         """
         self.debug = self.debug_checkbox.get()
         if self.debug:
             if Path("backup.xml").is_file():
                 self.display_message_box("Debug mode enabled.", True)
             else:
                 self.display_message_box(
-                    ("Debug mode requires Tasker XML file to be named: 'backup.xml', which is missing!"),
+                    ("Debug mode requires Tasker XML file to be named: 'backup.xml', which is missing.  No change."),
                     False,
                 )
                 self.debug = False
         else:
             self.display_message_box("Debug mode disabled.", True)
 
     # ##################################################################################
@@ -2162,18 +2181,19 @@
             or self.android_ipaddr
         ):
             if self.android_ipaddr == "":
                 return_code = get_xml(self.debug, self.appearance_mode)
                 # Did we get an error reading the backup file?
                 if return_code > 0:
                     if return_code == 6:
-                        self.display_message_box("Cancel button pressed.", False)
+                        self.display_message_box("Cancel button pressed.\n", False)
                     else:
-                        self.display_message_box(
-                            f"{PrimeItems.error_msg}\n\nClick 'Reset Options' to try a different XML file.", False,
+                        self.display_multiple_messages(
+                            [f"{PrimeItems.error_msg}\n", "Click 'Reset Options' to try a different XML file."],
+                            False,
                         )
                     return False
 
             # We have a file identified.  We now have to read it in.
             else:
                 filename_location = self.android_file.rfind(PrimeItems.slash) + 1
                 file_to_use = PrimeItems.program_arguments["android_file"][filename_location:]
@@ -2211,15 +2231,14 @@
             - Calls the build_the_tree function to build the tree.
             - Calls the display_tree function to display the tree."""
         PrimeItems.error_code = 0  # Clear any previous error.
 
         # Do we already have the XML?
         # If we don't have any data, get it.
         if self.load_xml():
-
             # Ok, we have our root Tasker elements.  Build the tree
             self.toplevel_window = None
 
             # Build our tree from XML data
             tree_data = self.build_the_tree()
 
             # Display the tree
@@ -2249,15 +2268,14 @@
         projects = root["all_projects"]
         if projects:
             for project in projects:
                 project_name = projects[project]["name"]
 
                 # Retrieves profile IDs for a given project and project name, excluding projects without profiles.
                 if profile_ids := get_ids(True, projects[project]["xml"], project_name, []):
-
                     # Build our list of Profiles in this Project.
                     profile_list = build_profiles(root, profile_ids)
 
                 # Project has no Profiles
                 else:
                     profile_list = ["No Profiles Found"]
 
@@ -2323,15 +2341,14 @@
         - Get the name of the current profile.
         - If no name is found, add a default message to the profile name.
         - Combine the profile name and task list into a dictionary and add it to the profile list.
         - Return the profile list."""
     profiles = root["all_profiles"]
     profile_list = []
     for profile in profile_ids:
-
         # Get the Profile's Tasks
         PrimeItems.task_count_unnamed = 0  # Avoid an error in get_profile_tasks
         if the_tasks := get_profile_tasks(profiles[profile]["xml"], [], []):
             task_list = []
             # Process each Task.  Tasks are simply a flat list of names.
             for task in the_tasks:
                 if task["name"] == "":
```

### Comparing `maptasker-3.1.7/maptasker/src/xmldata.py` & `maptasker-3.1.8/maptasker/src/xmldata.py`

 * *Files identical despite different names*

### Comparing `maptasker-3.1.7/pyproject.toml` & `maptasker-3.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "maptasker"
 
-version = "3.1.7"
+version = "3.1.8"
 
 description = "Utility to display your entire Android 'Tasker' configuration on your MAC."
 authors = ["Michael Rubin <mikrubin@gmail.com>"]
 readme = "README_PyPl.md"
 license = "MIT License (MIT)"
 repository = "https://github.com/mctinker/Map-Tasker"
 # changelog = "https://github.com/mctinker/Map-Tasker/blob/Master/Changelog.md"
```

### Comparing `maptasker-3.1.7/PKG-INFO` & `maptasker-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maptasker
-Version: 3.1.7
+Version: 3.1.8
 Summary: Utility to display your entire Android 'Tasker' configuration on your MAC.
 Home-page: https://github.com/mctinker/Map-Tasker
 License: MIT License (MIT)
 Keywords: tasker,Tasker,map tasker
 Author: Michael Rubin
 Author-email: mikrubin@gmail.com
 Requires-Python: >=3.11,<=3.13
```

