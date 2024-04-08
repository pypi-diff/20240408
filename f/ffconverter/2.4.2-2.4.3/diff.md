# Comparing `tmp/ffconverter-2.4.2.tar.gz` & `tmp/ffconverter-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffconverter-2.4.2.tar", last modified: Sun Apr  7 09:22:48 2024, max compression
+gzip compressed data, was "ffconverter-2.4.3.tar", last modified: Mon Apr  8 20:07:22 2024, max compression
```

## Comparing `ffconverter-2.4.2.tar` & `ffconverter-2.4.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.399448 ffconverter-2.4.2/
--rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.2/AUTHORS
--rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.2/COPYING
--rw-r--r--   0 luna      (1000) luna      (1000)     6677 2024-04-07 09:12:20.000000 ffconverter-2.4.2/ChangeLog
--rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.2/MANIFEST.in
--rw-r--r--   0 luna      (1000) luna      (1000)     2575 2024-04-07 09:22:48.399448 ffconverter-2.4.2/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     3874 2024-04-07 09:04:58.000000 ffconverter-2.4.2/README.md
--rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.2/TRANSLATORS
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.392781 ffconverter-2.4.2/bin/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.2/bin/ffconverter
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.396115 ffconverter-2.4.2/ffconverter/
--rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-07 09:12:37.000000 ffconverter-2.4.2/ffconverter/__init__.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/about_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/audiovideotab.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/config.py
--rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.2/ffconverter/dynamictab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    29255 2024-04-06 19:26:17.000000 ffconverter-2.4.2/ffconverter/ffconverter.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/imagetab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/preferences_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/presets_dlgs.py
--rw-r--r--   0 luna      (1000) luna      (1000)    26813 2024-04-04 19:50:46.000000 ffconverter-2.4.2/ffconverter/progress.py
--rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.2/ffconverter/qrc_resources.py
--rw-r--r--   0 luna      (1000) luna      (1000)    27291 2024-04-07 09:10:16.000000 ffconverter-2.4.2/ffconverter/utils.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.399448 ffconverter-2.4.2/ffconverter.egg-info/
--rw-r--r--   0 luna      (1000) luna      (1000)     2575 2024-04-07 09:22:48.000000 ffconverter-2.4.2/ffconverter.egg-info/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     1296 2024-04-07 09:22:48.000000 ffconverter-2.4.2/ffconverter.egg-info/SOURCES.txt
--rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-07 09:22:48.000000 ffconverter-2.4.2/ffconverter.egg-info/dependency_links.txt
--rw-r--r--   0 luna      (1000) luna      (1000)       19 2024-04-07 09:22:48.000000 ffconverter-2.4.2/ffconverter.egg-info/requires.txt
--rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-07 09:22:48.000000 ffconverter-2.4.2/ffconverter.egg-info/top_level.txt
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.2/launcher
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.396115 ffconverter-2.4.2/locale/
--rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter.pro
--rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_bg.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_ca.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_cs.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_de_DE.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_el.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_en.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_es.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_fr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_gl.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_gl_ES.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_hu.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_it.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_ms_MY.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_pl_PL.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_pt.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_pt_BR.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_ro_RO.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_ru.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_tr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_vi.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_zh_CN.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.2/locale/ffconverter_zh_TW.ts
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.396115 ffconverter-2.4.2/man/
--rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.2/man/ffconverter.1.gz
--rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.2/resources.qrc
--rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-07 09:22:48.399448 ffconverter-2.4.2/setup.cfg
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3481 2024-04-07 09:02:56.000000 ffconverter-2.4.2/setup.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.399448 ffconverter-2.4.2/share/
--rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-07 09:12:56.000000 ffconverter-2.4.2/share/ffconverter.desktop
--rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.2/share/ffconverter.png
--rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.2/share/presets.xml
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-07 09:22:48.399448 ffconverter-2.4.2/test/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.2/test/test_dialogs.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/
+-rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.3/AUTHORS
+-rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.3/COPYING
+-rw-r--r--   0 luna      (1000) luna      (1000)     6895 2024-04-08 19:51:36.000000 ffconverter-2.4.3/ChangeLog
+-rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.3/MANIFEST.in
+-rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-08 20:07:22.700591 ffconverter-2.4.3/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     4765 2024-04-08 19:17:41.000000 ffconverter-2.4.3/README.md
+-rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.3/TRANSLATORS
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.693924 ffconverter-2.4.3/bin/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.3/bin/ffconverter
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.697257 ffconverter-2.4.3/ffconverter/
+-rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-08 19:21:32.000000 ffconverter-2.4.3/ffconverter/__init__.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/about_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/audiovideotab.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/config.py
+-rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.3/ffconverter/dynamictab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    29489 2024-04-08 19:33:48.000000 ffconverter-2.4.3/ffconverter/ffconverter.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/imagetab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/preferences_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/presets_dlgs.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27485 2024-04-08 19:49:28.000000 ffconverter-2.4.3/ffconverter/progress.py
+-rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.3/ffconverter/qrc_resources.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27485 2024-04-08 19:41:28.000000 ffconverter-2.4.3/ffconverter/utils.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/ffconverter.egg-info/
+-rw-r--r--   0 luna      (1000) luna      (1000)     2639 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     1296 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       30 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/requires.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-08 20:07:22.000000 ffconverter-2.4.3/ffconverter.egg-info/top_level.txt
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.3/launcher
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.697257 ffconverter-2.4.3/locale/
+-rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter.pro
+-rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_bg.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ca.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_cs.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_de_DE.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_el.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_en.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_es.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_fr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_gl.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_gl_ES.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_hu.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_it.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ms_MY.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pl_PL.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pt.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_pt_BR.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ro_RO.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_ru.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_tr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_vi.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_zh_CN.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.3/locale/ffconverter_zh_TW.ts
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/man/
+-rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.3/man/ffconverter.1.gz
+-rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.3/resources.qrc
+-rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-08 20:07:22.700591 ffconverter-2.4.3/setup.cfg
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3652 2024-04-08 19:20:09.000000 ffconverter-2.4.3/setup.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/share/
+-rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-08 19:21:37.000000 ffconverter-2.4.3/share/ffconverter.desktop
+-rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.3/share/ffconverter.png
+-rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.3/share/presets.xml
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-08 20:07:22.700591 ffconverter-2.4.3/test/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.3/test/test_dialogs.py
```

### Comparing `ffconverter-2.4.2/COPYING` & `ffconverter-2.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ChangeLog` & `ffconverter-2.4.3/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Version 2.4.3
+-------------
+
+* Move trimesh/gmsh to optional dependencies
+
+* Add missing 3D Formats
+
+* Add instructions for ARM users on how to install (compile) GMSH
+
+* Add proper handling of unexpected missing gmsh
+
 Version 2.4.2
 -------------
 
 * Fix dependency checking for trimesh
 
 * Add trimesh (and gmsh) as dependencies in setup.py,
   users can choose to remove these afterwards.
```

### Comparing `ffconverter-2.4.2/PKG-INFO` & `ffconverter-2.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.2
+Version: 2.4.3
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
@@ -42,16 +42,17 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Utilities
 License-File: COPYING
 License-File: AUTHORS
 Requires-Dist: pyqt5
-Requires-Dist: trimesh
-Requires-Dist: gmsh
+Provides-Extra: trimesh
+Requires-Dist: trimesh; extra == "trimesh"
+Requires-Dist: gmsh; extra == "trimesh"
 
 
 FF Converter
 -------------------
 
 Graphical application which enables you to convert audio, video, image and
 document files between all popular formats using ffmpeg, unoconv, and ImageMagick.
```

### Comparing `ffconverter-2.4.2/README.md` & `ffconverter-2.4.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,38 @@
 ```
 
 #### Troubleshooting
 If a optional dependency is installed after the program, you might  
 need to restart the program twice to ensure the cache gets overwritten.  
 If this does not work, delete the cache (Preferences -> Delete Cache).  
 
+#### Troubleshooting (ARM CPUs)
+For converting 3D Models, the python packages `trimesh` and `gmsh` are  
+required. Sadly, `gmsh` is not available on PyPi for ARM devices. You can  
+compile it yourself by using the script below.  
+__WARNING: You won't be able to uninstall gmsh using pip__  
+and any scripts using it must first run `sys.path.append('/usr/local/lib')`.  
+This will take a while. I only have a rapidly overheating phone  
+for testing ARM, so I am not that sure about compile time on other  
+devices, but expect *upwards of 2 hours compile time*.  
+```bash
+git clone https://gitlab.onelab.info/gmsh/gmsh.git # 200+ MiB size
+mkdir ./gmsh/build
+cd ./gmsh/build
+
+# You can probably replace `gcc` and `g++` with any other C/C++ Compiler.
+CC=gcc CXX=g++ cmake -DENABLE_BUILD_DYNAMIC=1 ..
+make
+sudo make install
+
+# optional, you no longer need the git repo
+cd ../..
+rm -r ./gmsh
+```
+
 #### Troubleshooting (Linux)
 On some distros ("externally managed environments", like Arch and Debian),  
 `pip` will not work. In this case, you should use `pipx`.  
 
 ```sh
 sudo PIPX_HOME=/usr/local/pipx PIPX_BIN_DIR=/usr/local/bin pipx install --system-site-packages ffconverter
 sudo ln -sf /usr/local/pipx/venvs/ffconverter/share/applications/ffconverter.desktop /usr/local/share/applications/ffconverter.desktop
```

### Comparing `ffconverter-2.4.2/TRANSLATORS` & `ffconverter-2.4.3/TRANSLATORS`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/__init__.py` & `ffconverter-2.4.3/ffconverter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 GUI File Format Converter
 """
 
 # version
 __major__ = 2
 __minor__ = 4
-__patch__ = 2
+__patch__ = 3
 __prerelease__ = "" # alpha, beta, rc etc.
 
 # package information
 __name__ = "ffconverter"
 __version__ = "{0}.{1}.{2}".format(__major__, __minor__, __patch__)
 __version__ += __prerelease__
 __description__ = "File Format Converter with Qt GUI"
```

### Comparing `ffconverter-2.4.2/ffconverter/about_dlg.py` & `ffconverter-2.4.3/ffconverter/about_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/audiovideotab.py` & `ffconverter-2.4.3/ffconverter/audiovideotab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/config.py` & `ffconverter-2.4.3/ffconverter/config.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/dynamictab.py` & `ffconverter-2.4.3/ffconverter/dynamictab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/ffconverter.py` & `ffconverter-2.4.3/ffconverter/ffconverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,16 @@
         self.compress_zip = utils.is_installed('zip', use_wsl)
         self.compress_unzip = utils.is_installed('unzip', use_wsl)
         self.compress_tar = utils.is_installed('tar', use_wsl)
         self.compress_squash = utils.is_installed('mksquashfs', use_wsl) and utils.is_installed('unsquashfs', use_wsl)
         self.compress_ar = utils.is_installed('ar', use_wsl)
         self.compress_gzip = utils.is_installed('gzip', use_wsl)
         self.compress_bzip2 = utils.is_installed('bzip2', use_wsl)
-        self.trimesh = utils.is_installed('trimesh', use_wsl)
+        self.trimesh = utils.is_installed('trimesh', False, is_import=True)
+        self.gmsh = utils.is_installed('gmsh', False, is_import=True)
 
         self.missing = []
         if not self.ffmpeg_path:
             self.missing.append('ffmpeg')
         if not self.unoconv:
             self.missing.append('unoconv')
         if not self.imagemagick:
@@ -408,16 +409,19 @@
             self.missing.append('squashfs-tools')
         if not self.compress_ar:
             self.missing.append('binutils/ar')
         if not self.compress_gzip:
             self.missing.append('gzip')
         if not self.compress_bzip2:
             self.missing.append('bzip2')
+        # if trimesh is missing, we won't use gmsh anyways
         if not self.trimesh:
             self.missing.append('trimesh')
+        if not self.trimesh and not self.gmsh:
+            self.missing.append('and gmsh')
 
         if self.missing:
             status = ', '.join(self.missing)
             status = self.tr('Missing dependencies:') + ' ' + status
             if mobile_ui:
                 print(status)
             else:
```

### Comparing `ffconverter-2.4.2/ffconverter/imagetab.py` & `ffconverter-2.4.3/ffconverter/imagetab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/preferences_dlg.py` & `ffconverter-2.4.3/ffconverter/preferences_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/presets_dlgs.py` & `ffconverter-2.4.3/ffconverter/presets_dlgs.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/progress.py` & `ffconverter-2.4.3/ffconverter/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,17 +623,28 @@
     def convert_model(self, from_file, to_file):
         # can't be imported at the start because its a optional dependency
         import trimesh
         # python library doesn't need escaped paths, we can undo that
         from_file = from_file.replace('"', '').replace('\\', '')
         to_file   =   to_file.replace('"', '').replace('\\', '')
         
-        needs_gmsh = utils.get_extension(from_file) in ['iges', 'stp', 'step', 'brep']
+        # these formats require gmsh in addition to trimesh
+        needs_gmsh = utils.get_extension(from_file) in ['brep', 'step', 'iges', 'inp', 'bdf'] or utils.get_extension(to_file) in ['inp', 'bdf']
+        # check that GMSH is installed, append to sys.path if needed
+        if needs_gmsh and not utils.is_installed('gmsh', False, is_import=True):
+            self.update_text_edit_signal.emit("Would fail to load GMSH, retrying with /usr/local/lib\n")
+            if not '/usr/local/lib' in sys.path:
+                sys.path.append('/usr/local/lib')
+            # retry with the new sys.path
+            if not utils.is_installed('gmsh', False, is_import=True):
+                self.update_text_edit_signal.emit("Unable to locate GMSH, please install it. (using PyPi/pip)\n")
+                return False
+
         try:
-            if utils.get_extension(from_file) in ['iges', 'stp', 'step', 'brep']:
+            if needs_gmsh:
                 self.update_text_edit_signal.emit(f"Loading file from {from_file} using trimesh.gmsh\n")
                 mesh = trimesh.Trimesh(**trimesh.interfaces.gmsh.load_gmsh(file_name=from_file))
             else:
                 self.update_text_edit_signal.emit(f"Loading file from {from_file} using trimesh.default\n")
                 mesh = trimesh.load(from_file)
             self.update_text_edit_signal.emit(f"Saving File to {to_file}\n")
             mesh.export(to_file)
```

### Comparing `ffconverter-2.4.2/ffconverter/qrc_resources.py` & `ffconverter-2.4.3/ffconverter/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/ffconverter/utils.py` & `ffconverter-2.4.3/ffconverter/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,27 @@
     Return the number of seconds of duration, an integer.
     Duration is a string of type hh:mm:ss.ts
     """
     duration = duration.split('.')[0] # get rid of milliseconds
     hours, mins, secs = [int(i) for i in duration.split(':')]
     return secs + (hours * 3600) + (mins * 60)
 
-def is_installed(program, use_wsl, wsl_only=False):
+def is_installed(program, use_wsl, wsl_only=False, is_import=False):
     """
     If program is a program name, returns the absolute path to this program if
     included in the PATH enviromental variable, else empty string.
 
     If program is an absolute path, returns the path if it's executable, else
     empty string.
     """
 
     if program.startswith('wsl'): return program # do not resolve WSL paths
 
     # python packages
-    if program == 'trimesh':
+    if is_import:
         is_installed = False
         if importlib.util.find_spec(program) is not None:
             is_installed = importlib.util.find_spec(program).loader is not None
         return is_installed
 
     # wsl_only is used to not get "convert" on a windows system
     if wsl_only == False:
@@ -300,17 +300,20 @@
     if compression_exts != [[], []]: # if any of the tools work
         compression_exts[0] += extraformats_compression
         compression_exts[1] += extraformats_compression + ['[Folder]']
     supported_tmp.append(compression_exts)
 
     model_exts = [[], []]
     if 'trimesh' not in missing:
-        # TODO: trimesh can load/export far more types, add these
-        model_exts[0] += ['step']
-        model_exts[1] += ['stl']
+        model_exts[0] += ['stl', 'stl_ascii', 'off', 'ply', 'obj', 'glb', '3mf', '3dxml', 'gtlf']
+        model_exts[1] += ['stl', 'ply', 'off', 'obj', 'glb', 'gtlf', 'dae']
+        if 'gmsh' not in missing:
+            model_exts[0] += ['brep', 'step', 'iges', 'inp', 'bdf']
+            model_exts[1] += ['inp', 'bdf']
+
     supported_tmp.append(model_exts)
 
     # if the function is meant to return a converter for a in/output pair
     if get_conv_for_ext:
         if ext[0] in ffmpeg_conversions[0] and ext[1] in ffmpeg_conversions[1]:
             return "ffmpeg"
         elif ext[0] in pandoc_conversions[0] and ext[1] in pandoc_conversions[1]:
```

### Comparing `ffconverter-2.4.2/ffconverter.egg-info/PKG-INFO` & `ffconverter-2.4.3/ffconverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.2
+Version: 2.4.3
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
@@ -42,16 +42,17 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Utilities
 License-File: COPYING
 License-File: AUTHORS
 Requires-Dist: pyqt5
-Requires-Dist: trimesh
-Requires-Dist: gmsh
+Provides-Extra: trimesh
+Requires-Dist: trimesh; extra == "trimesh"
+Requires-Dist: gmsh; extra == "trimesh"
 
 
 FF Converter
 -------------------
 
 Graphical application which enables you to convert audio, video, image and
 document files between all popular formats using ffmpeg, unoconv, and ImageMagick.
```

### Comparing `ffconverter-2.4.2/ffconverter.egg-info/SOURCES.txt` & `ffconverter-2.4.3/ffconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter.pro` & `ffconverter-2.4.3/locale/ffconverter.pro`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_bg.ts` & `ffconverter-2.4.3/locale/ffconverter_bg.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_ca.ts` & `ffconverter-2.4.3/locale/ffconverter_ca.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_cs.ts` & `ffconverter-2.4.3/locale/ffconverter_cs.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_de_DE.ts` & `ffconverter-2.4.3/locale/ffconverter_de_DE.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_el.ts` & `ffconverter-2.4.3/locale/ffconverter_el.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_en.ts` & `ffconverter-2.4.3/locale/ffconverter_en.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_es.ts` & `ffconverter-2.4.3/locale/ffconverter_es.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_fr.ts` & `ffconverter-2.4.3/locale/ffconverter_fr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_gl.ts` & `ffconverter-2.4.3/locale/ffconverter_gl.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_gl_ES.ts` & `ffconverter-2.4.3/locale/ffconverter_gl_ES.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_hu.ts` & `ffconverter-2.4.3/locale/ffconverter_hu.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_it.ts` & `ffconverter-2.4.3/locale/ffconverter_it.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_ms_MY.ts` & `ffconverter-2.4.3/locale/ffconverter_ms_MY.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_pl_PL.ts` & `ffconverter-2.4.3/locale/ffconverter_pl_PL.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_pt.ts` & `ffconverter-2.4.3/locale/ffconverter_pt.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_pt_BR.ts` & `ffconverter-2.4.3/locale/ffconverter_pt_BR.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_ro_RO.ts` & `ffconverter-2.4.3/locale/ffconverter_ro_RO.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_ru.ts` & `ffconverter-2.4.3/locale/ffconverter_ru.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_tr.ts` & `ffconverter-2.4.3/locale/ffconverter_tr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_vi.ts` & `ffconverter-2.4.3/locale/ffconverter_vi.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_zh_CN.ts` & `ffconverter-2.4.3/locale/ffconverter_zh_CN.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/locale/ffconverter_zh_TW.ts` & `ffconverter-2.4.3/locale/ffconverter_zh_TW.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/man/ffconverter.1.gz` & `ffconverter-2.4.3/man/ffconverter.1.gz`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/resources.qrc` & `ffconverter-2.4.3/resources.qrc`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/setup.py` & `ffconverter-2.4.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import ffconverter
 from distutils.core import setup
+from distutils.util import get_platform
 import os
 
 if os.name == 'nt':
     data_files = [('share/applications', ['share/ffconverter.desktop']),
                 ('share/pixmaps', ['share/ffconverter.png']),
                 ('share/ffconverter', ['share/presets.xml']),
                 ('share/man/man1', ['man/ffconverter.1.gz'])]
@@ -15,18 +16,21 @@
                 ('share/ffconverter', ['share/presets.xml']),
                 ('share/man/man1', ['man/ffconverter.1.gz'])]
 
 setup(
     name = ffconverter.__name__,
     packages = [ffconverter.__name__],
     install_requires=[
-          'pyqt5',
-          'trimesh',
-          'gmsh'
+          'pyqt5'
       ],
+    extras_require={
+        "trimesh": (
+            [] if 'arm' in get_platform().lower() else # gmsh not available for ARM
+            ["trimesh", "gmsh"])
+        },
     scripts = ['bin/ffconverter'],
     data_files = data_files,
     version = ffconverter.__version__,
     description = ffconverter.__description__,
     author = ffconverter.__author__,
     author_email = ffconverter.__author_email__,
     maintainer = ffconverter.__maintainer__,
```

### Comparing `ffconverter-2.4.2/share/ffconverter.png` & `ffconverter-2.4.3/share/ffconverter.png`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/share/presets.xml` & `ffconverter-2.4.3/share/presets.xml`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.2/test/test_dialogs.py` & `ffconverter-2.4.3/test/test_dialogs.py`

 * *Files identical despite different names*

