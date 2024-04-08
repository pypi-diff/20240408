# Comparing `tmp/imagedata_format_biff-0.0.6.tar.gz` & `tmp/imagedata_format_biff-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagedata_format_biff-0.0.6.tar", last modified: Fri Mar  1 13:35:37 2024, max compression
+gzip compressed data, was "imagedata_format_biff-0.0.8.tar", last modified: Mon Apr  8 12:24:00 2024, max compression
```

## Comparing `imagedata_format_biff-0.0.6.tar` & `imagedata_format_biff-0.0.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)      335 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/.travis.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1124 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.380327 imagedata_format_biff-0.0.6/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.384327 imagedata_format_biff-0.0.6/data/biff/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.384327 imagedata_format_biff-0.0.6/data/biff/time/
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/biff/time/time00.biff
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/biff/time/time01.biff
--rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/biff/time/time02.biff
--rw-r--r--   0 runner    (1001) docker     (127)   120985 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/biff/time.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.380327 imagedata_format_biff-0.0.6/data/dicom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.388327 imagedata_format_biff-0.0.6/data/dicom/template/
--rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00000.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00001.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00002.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00003.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00004.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00005.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00006.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00007.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00008.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00009.dcm
--rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/template/Image_00010.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.384327 imagedata_format_biff-0.0.6/data/dicom/time/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.388327 imagedata_format_biff-0.0.6/data/dicom/time/time00/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00021.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.388327 imagedata_format_biff-0.0.6/data/dicom/time/time01/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00021.dcm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/data/dicom/time/time02/
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00019.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00020.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00021.dcm
--rwxr-xr-x   0 runner    (1001) docker     (127)    16444 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1605 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.384327 imagedata_format_biff-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/src/imagedata_format_biff/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33217 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff/biffplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 13:35:37.000000 imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/techstack.md
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/techstack.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:37.392327 imagedata_format_biff-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/tests/compare_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/tests/test_formats_biff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/tests/test_formats_biff_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-01 13:35:07.000000 imagedata_format_biff-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      335 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/.travis.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1124 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      515 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.018571 imagedata_format_biff-0.0.8/data/biff/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.018571 imagedata_format_biff-0.0.8/data/biff/time/
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time00.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time01.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   176128 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time/time02.biff
+-rw-r--r--   0 runner    (1001) docker     (127)   120985 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/biff/time.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/dicom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.022570 imagedata_format_biff-0.0.8/data/dicom/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00000.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00001.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00002.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39730 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00003.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00004.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00005.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00006.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00007.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00008.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00009.dcm
+-rw-r--r--   0 runner    (1001) docker     (127)    39728 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/template/Image_00010.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/data/dicom/time/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.022570 imagedata_format_biff-0.0.8/data/dicom/time/time00/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00021.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/data/dicom/time/time01/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00021.dcm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/data/dicom/time/time02/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00019.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00020.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179780 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00021.dcm
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16444 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1605 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.014570 imagedata_format_biff-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.026570 imagedata_format_biff-0.0.8/src/imagedata_format_biff/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-08 12:23:29.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff/biffplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-08 12:23:59.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:23:59.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 12:24:00.000000 imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/techstack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/techstack.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:24:00.030571 imagedata_format_biff-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/compare_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/test_formats_biff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tests/test_formats_biff_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-08 12:23:30.000000 imagedata_format_biff-0.0.8/tox.ini
```

### Comparing `imagedata_format_biff-0.0.6/LICENSE.txt` & `imagedata_format_biff-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/MANIFEST.in` & `imagedata_format_biff-0.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/Makefile` & `imagedata_format_biff-0.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/PKG-INFO` & `imagedata_format_biff-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagedata_format_biff
-Version: 0.0.6
+Version: 0.0.8
 Summary: Imagedata format plugin for biff image data
 Home-page: https://github.com/erling6232/imagedata_format_biff
 Author: Erling Andersen
 Author-email: Erling.Andersen@Helse-Bergen.NO
 License: MIT
 Project-URL: Documentation, https://imagedata.readthedocs.io
 Project-URL: Source Code, https://github.com/erling6232/imagedata_format_biff
```

### Comparing `imagedata_format_biff-0.0.6/README.rst` & `imagedata_format_biff-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/biff/time/time00.biff` & `imagedata_format_biff-0.0.8/data/biff/time/time00.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/biff/time/time01.biff` & `imagedata_format_biff-0.0.8/data/biff/time/time01.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/biff/time/time02.biff` & `imagedata_format_biff-0.0.8/data/biff/time/time02.biff`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/biff/time.zip` & `imagedata_format_biff-0.0.8/data/biff/time.zip`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00000.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00000.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00001.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00001.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00002.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00002.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00003.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00003.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00004.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00004.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00005.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00005.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00006.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00006.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00007.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00007.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00008.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00008.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00009.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00009.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/template/Image_00010.dcm` & `imagedata_format_biff-0.0.8/data/dicom/template/Image_00010.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00019.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00020.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time00/Image_00021.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time00/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00019.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00020.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time01/Image_00021.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time01/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00019.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00019.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00020.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00020.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/data/dicom/time/time02/Image_00021.dcm` & `imagedata_format_biff-0.0.8/data/dicom/time/time02/Image_00021.dcm`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/pylintrc` & `imagedata_format_biff-0.0.8/pylintrc`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/setup.cfg` & `imagedata_format_biff-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/src/imagedata_format_biff/__init__.py` & `imagedata_format_biff-0.0.8/src/imagedata_format_biff/__init__.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/src/imagedata_format_biff/biffplugin.py` & `imagedata_format_biff-0.0.8/src/imagedata_format_biff/biffplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,7 +916,8 @@
             struct.pack(endian + str(n) + dformat[0], *arr.flatten(order='C'))
         )
 
         rest = struct.calcsize(endian + str(n) + dformat[0]) % 512
         if rest != 0:
             logging.debug('_write_band: filling %d bytes' % (512 - rest))
             self.f.write((512 - rest) * b'\x00')
+        self.f.flush()
```

### Comparing `imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/PKG-INFO` & `imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagedata_format_biff
-Version: 0.0.6
+Version: 0.0.8
 Summary: Imagedata format plugin for biff image data
 Home-page: https://github.com/erling6232/imagedata_format_biff
 Author: Erling Andersen
 Author-email: Erling.Andersen@Helse-Bergen.NO
 License: MIT
 Project-URL: Documentation, https://imagedata.readthedocs.io
 Project-URL: Source Code, https://github.com/erling6232/imagedata_format_biff
```

### Comparing `imagedata_format_biff-0.0.6/src/imagedata_format_biff.egg-info/SOURCES.txt` & `imagedata_format_biff-0.0.8/src/imagedata_format_biff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/techstack.md` & `imagedata_format_biff-0.0.8/techstack.md`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/techstack.yml` & `imagedata_format_biff-0.0.8/techstack.yml`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/tests/compare_headers.py` & `imagedata_format_biff-0.0.8/tests/compare_headers.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/tests/test_formats_biff.py` & `imagedata_format_biff-0.0.8/tests/test_formats_biff.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/tests/test_formats_biff_template.py` & `imagedata_format_biff-0.0.8/tests/test_formats_biff_template.py`

 * *Files identical despite different names*

### Comparing `imagedata_format_biff-0.0.6/tox.ini` & `imagedata_format_biff-0.0.8/tox.ini`

 * *Files identical despite different names*

