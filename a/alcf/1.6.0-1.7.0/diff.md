# Comparing `tmp/alcf-1.6.0.tar.gz` & `tmp/alcf-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcf-1.6.0.tar", last modified: Wed Feb 28 14:52:25 2024, max compression
+gzip compressed data, was "alcf-1.7.0.tar", last modified: Mon Apr  8 13:07:21 2024, max compression
```

## Comparing `alcf-1.6.0.tar` & `alcf-1.7.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.057348 alcf-1.6.0/
--rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-02-28 14:48:11.000000 alcf-1.6.0/.editorconfig
--rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-02-28 14:48:11.000000 alcf-1.6.0/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-02-28 14:48:11.000000 alcf-1.6.0/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-02-28 14:48:11.000000 alcf-1.6.0/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-02-28 14:52:25.057348 alcf-1.6.0/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-02-28 14:48:11.000000 alcf-1.6.0/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/algorithms/
--rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/algorithms/calibration/
--rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/calibration/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/calibration/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/algorithms/cloud_base_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/cloud_base_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/cloud_base_detection/default.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/algorithms/cloud_detection/
--rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/cloud_detection/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/cloud_detection/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/couple.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/interp.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)      781 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/lidar_ratio.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/algorithms/noise_removal/
--rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/noise_removal/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/noise_removal/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/output_sample.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10602 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1196 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/tsample.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/algorithms/zsample.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/bin/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/bin/__init__.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)      319 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/bin/alcf.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf/cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      408 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3621 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/auto.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.045348 alcf-1.6.0/alcf/cmds/auto_cmds/
--rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/auto_cmds/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/auto_cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1671 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/auto_cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/auto_cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/calibrate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/compare.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/convert.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12318 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/lidar.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1395 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8639 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/model.py
--rw-r--r--   0 peter     (1000) peter     (1000)    18068 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/plot.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6424 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/simulate.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4975 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/cmds/stats.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.045348 alcf-1.6.0/alcf/fonts/
--rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/fonts/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/fonts/PublicSans-Bold.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/fonts/PublicSans-BoldItalic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/fonts/PublicSans-Italic.otf
--rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/fonts/PublicSans-Regular.otf
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.045348 alcf-1.6.0/alcf/lidars/
--rw-r--r--   0 peter     (1000) peter     (1000)     1426 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/blview.py
--rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/caliop.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1742 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/chm15k.py
--rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/cl31.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/cl51.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1865 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/cl61.py
--rw-r--r--   0 peter     (1000) peter     (1000)      985 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/default.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3545 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/mpl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2195 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/lidars/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4659 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/misc.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.045348 alcf-1.6.0/alcf/models/
--rw-r--r--   0 peter     (1000) peter     (1000)     2235 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4179 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/amps.py
--rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/cmip5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2577 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/era5.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2521 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/icon.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/icon_intake_healpix.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2559 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/jra55.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1650 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/merra2.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1854 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/nzcsm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2939 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/nzesm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-02-28 14:48:11.000000 alcf-1.6.0/alcf/models/um.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.041348 alcf-1.6.0/alcf.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     4562 2024-02-28 14:52:25.000000 alcf-1.6.0/alcf.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)      173 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-02-28 14:52:24.000000 alcf-1.6.0/alcf.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-02-28 14:48:11.000000 alcf-1.6.0/build_doc
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.049348 alcf-1.6.0/cosp/
--rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/.editorconfig
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.049348 alcf-1.6.0/cosp/MISR_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/MISR_simulator/MISR_simulator.f
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.049348 alcf-1.6.0/cosp/MODIS_simulator/
--rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/MODIS_simulator/modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/MODIS_simulator/test_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/Makefile.cmor1
--rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/Makefile.ibm
--rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/README.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/README_v1.4.1.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.049348 alcf-1.6.0/cosp/actsim/
--rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/actsim/lidar_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/actsim/lmd_ipsl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/actsim/mie_backscatter_1064.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/actsim/mie_backscatter_532.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/actsim/mie_backscatter_910.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.049348 alcf-1.6.0/cosp/cfmip2/
--rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_constants.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_defs.h
--rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_htfrtc.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_input_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_io.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_isccp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_lidar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_misr_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_modis_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_output_nl.txt
--rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_rttov.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_rttov_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_simulator.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_types.F90
--rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/cosp_utils.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.053348 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/
--rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/Makefile
--rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/README
--rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/congvec.expected
--rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/congvec.f
--rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/icarus.f
--rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/input.data
--rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/input.data.halved
--rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
--rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/license
--rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/rcsid
--rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
--rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.053348 alcf-1.6.0/cosp/llnl/
--rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/llnl/cosp_radar.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/llnl/llnl_stats.F90
--rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/llnl/pf_to_mr.f
--rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/llnl/prec_scops.f
--rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/mac_info.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/predict_mom07.F90
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.053348 alcf-1.6.0/cosp/quickbeam/
--rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/README
--rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/array_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/atmos_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/calc_Re.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/dsd.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/format_input.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/gases.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/load_hydrometeor_classes.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/load_mie_table.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/math_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/mrgrnk.f90
--rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/optics_lib.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/predict_psd07.f
--rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/radar_simulator.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/radar_simulator_init.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/radar_simulator_types.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/scale_LUTs_io.f90
--rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/quickbeam/zeff.f90
--rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/replace_tabs.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/tests.sh
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.053348 alcf-1.6.0/cosp/utils/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/utils/COSP_plots.py
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.6.0/cosp/utils/append_cf3hr_files.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-02-28 14:48:11.000000 alcf-1.6.0/download_cosp
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.057348 alcf-1.6.0/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     4194 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-auto.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2264 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-calibrate.1
--rw-r--r--   0 peter     (1000) peter     (1000)      795 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-compare.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2292 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-convert.1
--rw-r--r--   0 peter     (1000) peter     (1000)     6969 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-lidar.1
--rw-r--r--   0 peter     (1000) peter     (1000)     4281 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-model.1
--rw-r--r--   0 peter     (1000) peter     (1000)     5418 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-plot.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1965 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-simulate.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3928 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1393 2024-02-28 14:48:11.000000 alcf-1.6.0/man/alcf.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-02-28 14:52:25.057348 alcf-1.6.0/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2220 2024-02-28 14:48:11.000000 alcf-1.6.0/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-02-28 14:52:25.057348 alcf-1.6.0/src/
--rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-02-28 14:48:11.000000 alcf-1.6.0/src/cosp_run.f03
--rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-02-28 14:48:11.000000 alcf-1.6.0/src/main.f03
--rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-02-28 14:48:11.000000 alcf-1.6.0/src/nc_utils.f03
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      239 2024-04-08 13:01:39.000000 alcf-1.7.0/.editorconfig
+-rw-r--r--   0 peter     (1000) peter     (1000)     1144 2024-04-08 13:01:39.000000 alcf-1.7.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)      181 2024-04-08 13:01:39.000000 alcf-1.7.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2024-04-08 13:01:39.000000 alcf-1.7.0/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-08 13:07:21.983892 alcf-1.7.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      764 2024-04-08 13:01:39.000000 alcf-1.7.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/algorithms/
+-rw-r--r--   0 peter     (1000) peter     (1000)       27 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf/algorithms/calibration/
+-rw-r--r--   0 peter     (1000) peter     (1000)       62 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/calibration/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/calibration/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/cloud_base_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       71 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_base_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      930 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_base_detection/default.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/cloud_detection/
+-rw-r--r--   0 peter     (1000) peter     (1000)       66 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_detection/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1533 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/cloud_detection/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1871 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/couple.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1018 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/interp.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)      781 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/lidar_ratio.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/algorithms/noise_removal/
+-rw-r--r--   0 peter     (1000) peter     (1000)       64 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/noise_removal/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1366 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/noise_removal/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1812 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/output_sample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10602 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1196 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/tsample.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1365 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/algorithms/zsample.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/bin/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/bin/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      319 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/bin/alcf.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      408 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3658 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/cmds/auto_cmds/
+-rw-r--r--   0 peter     (1000) peter     (1000)      141 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      843 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1671 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1086 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/auto_cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2804 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/calibrate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2148 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/compare.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4512 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/convert.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12355 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/lidar.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1395 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9347 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/model.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    18068 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/plot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6424 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/simulate.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4939 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/cmds/stats.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.967893 alcf-1.7.0/alcf/fonts/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6709 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    56032 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Bold.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60100 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-BoldItalic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    60316 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Italic.otf
+-rw-r--r--   0 peter     (1000) peter     (1000)    56792 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/fonts/PublicSans-Regular.otf
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.971892 alcf-1.7.0/alcf/lidars/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1426 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/blview.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      101 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/caliop.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1742 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/chm15k.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      410 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl31.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2278 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl51.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1865 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/cl61.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      985 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/default.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3545 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/mpl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2195 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/lidars/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4659 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/misc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.971892 alcf-1.7.0/alcf/models/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2235 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4179 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/amps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      359 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/cmip5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2577 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/era5.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2521 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/icon.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1783 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/icon_intake_healpix.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2559 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/jra55.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1650 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/merra2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1854 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/nzcsm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2939 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/nzesm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2181 2024-04-08 13:01:39.000000 alcf-1.7.0/alcf/models/um.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.963892 alcf-1.7.0/alcf.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1002 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     4562 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       52 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)      173 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        5 2024-04-08 13:07:21.000000 alcf-1.7.0/alcf.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1677 2024-04-08 13:01:39.000000 alcf-1.7.0/build_doc
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      260 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/.editorconfig
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/MISR_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MISR_simulator/MISR_simulator.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/MODIS_simulator/
+-rw-r--r--   0 peter     (1000) peter     (1000)    64835 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MODIS_simulator/modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7387 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/MODIS_simulator/test_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5167 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)     7506 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile.cmor1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7515 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/Makefile.ibm
+-rw-r--r--   0 peter     (1000) peter     (1000)      936 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README.md
+-rw-r--r--   0 peter     (1000) peter     (1000)    48320 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/README_v1.4.1.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/actsim/
+-rw-r--r--   0 peter     (1000) peter     (1000)    35248 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/lidar_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    38101 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/lmd_ipsl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11672 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_1064.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11571 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_532.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    11642 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/actsim/mie_backscatter_910.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.975892 alcf-1.7.0/cosp/cfmip2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2508 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7271 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     7400 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3320 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     3261 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    31979 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    15220 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_constants.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1881 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_defs.h
+-rw-r--r--   0 peter     (1000) peter     (1000)     2644 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_htfrtc.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6934 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_input_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    40704 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_io.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4292 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_isccp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4123 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_lidar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3561 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_misr_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    25019 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_modis_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     3646 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_output_nl.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)    26091 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_rttov.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5694 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_rttov_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9657 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_simulator.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13744 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    70109 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_types.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)    13287 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/cosp_utils.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2957 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/Makefile
+-rw-r--r--   0 peter     (1000) peter     (1000)    59127 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/README
+-rw-r--r--   0 peter     (1000) peter     (1000)      165 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.expected
+-rw-r--r--   0 peter     (1000) peter     (1000)     2545 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    43978 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/icarus.f
+-rw-r--r--   0 peter     (1000) peter     (1000)      869 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data
+-rw-r--r--   0 peter     (1000) peter     (1000)     1042 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data.halved
+-rw-r--r--   0 peter     (1000) peter     (1000)    13495 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     1845 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/license
+-rwxr-xr-x   0 peter     (1000) peter     (1000)       15 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/rcsid
+-rw-r--r--   0 peter     (1000) peter     (1000)    11849 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     2539 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2660 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh
+-rw-r--r--   0 peter     (1000) peter     (1000)    13385 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3095 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/llnl/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7918 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/cosp_radar.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     6082 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/llnl_stats.F90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5703 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/pf_to_mr.f
+-rw-r--r--   0 peter     (1000) peter     (1000)     9585 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/llnl/prec_scops.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    75040 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/mac_info.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)     1317 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/predict_mom07.F90
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/quickbeam/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/README
+-rw-r--r--   0 peter     (1000) peter     (1000)     4166 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/array_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     5500 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/atmos_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7260 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/calc_Re.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    10671 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/dsd.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4282 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/format_input.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     7774 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/gases.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1665 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/load_hydrometeor_classes.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     1761 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/load_mie_table.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     9299 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/math_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    17248 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/mrgrnk.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)    36058 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/optics_lib.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4211 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/predict_psd07.f
+-rw-r--r--   0 peter     (1000) peter     (1000)    18284 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4867 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator_init.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     2934 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/radar_simulator_types.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4039 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/scale_LUTs_io.f90
+-rw-r--r--   0 peter     (1000) peter     (1000)     4852 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/quickbeam/zeff.f90
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      143 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/replace_tabs.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      196 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/tests.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.979892 alcf-1.7.0/cosp/utils/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     8682 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/utils/COSP_plots.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3379 2023-04-22 09:28:05.000000 alcf-1.7.0/cosp/utils/append_cf3hr_files.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      333 2024-04-08 13:01:39.000000 alcf-1.7.0/download_cosp
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     4228 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-auto.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2261 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-calibrate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      792 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-compare.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2289 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-convert.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     7003 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-lidar.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     4711 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-model.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     5415 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-plot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1962 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-simulate.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3925 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1390 2024-04-08 13:01:39.000000 alcf-1.7.0/man/alcf.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-08 13:07:21.983892 alcf-1.7.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2220 2024-04-08 13:01:39.000000 alcf-1.7.0/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-08 13:07:21.983892 alcf-1.7.0/src/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12585 2024-04-08 13:01:39.000000 alcf-1.7.0/src/cosp_run.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)    11128 2024-04-08 13:01:39.000000 alcf-1.7.0/src/main.f03
+-rw-r--r--   0 peter     (1000) peter     (1000)     8501 2024-04-08 13:01:39.000000 alcf-1.7.0/src/nc_utils.f03
```

### Comparing `alcf-1.6.0/LICENSE.md` & `alcf-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/Makefile` & `alcf-1.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/PKG-INFO` & `alcf-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.6.0
+Version: 1.7.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.6.0/README.md` & `alcf-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/cloud_base_detection/default.py` & `alcf-1.7.0/alcf/algorithms/cloud_base_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/cloud_detection/default.py` & `alcf-1.7.0/alcf/algorithms/cloud_detection/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/couple.py` & `alcf-1.7.0/alcf/algorithms/couple.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/interp.pyx` & `alcf-1.7.0/alcf/algorithms/interp.pyx`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/lidar_ratio.py` & `alcf-1.7.0/alcf/algorithms/lidar_ratio.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/noise_removal/default.py` & `alcf-1.7.0/alcf/algorithms/noise_removal/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/output_sample.py` & `alcf-1.7.0/alcf/algorithms/output_sample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/stats.py` & `alcf-1.7.0/alcf/algorithms/stats.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/tsample.py` & `alcf-1.7.0/alcf/algorithms/tsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/algorithms/zsample.py` & `alcf-1.7.0/alcf/algorithms/zsample.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/auto.py` & `alcf-1.7.0/alcf/cmds/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,17 @@
 - `blview`: Vaisala BL-VIEW L2 product.
 - `caliop`: CALIPSO/CALIOP (`alcf auto model` only).
 - `chm15k`: Lufft CHM 15k.
 - `cl31`: Vaisala CL31.
 - `cl51`: Vaisala CL51.
 - `cl61`: Vaisala CL61.
 - `cosp`: COSP simulated lidar.
-- `minimpl`: Sigma Space MiniMPL.
+- `minimpl`: Sigma Space MiniMPL (converted via SigmaMPL).
 - `mpl`: Sigma Space MPL (converted via SigmaMPL).
-- `mpl2nc`: Sigma Space MPL (converted via mpl2nc).
+- `mpl2nc`: Sigma Space MPL and MiniMPL (converted via mpl2nc).
 
 Time format
 -----------
 
 `YYYY-MM-DD[THH:MM[:SS]]`, where `YYYY` is year, `MM` is month, `DD` is day,
 `HH` is hour, `MM` is minute, `SS` is second. Example: 2000-01-01T00:00:00.
```

### Comparing `alcf-1.6.0/alcf/cmds/auto_cmds/compare.py` & `alcf-1.7.0/alcf/cmds/auto_cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/auto_cmds/lidar.py` & `alcf-1.7.0/alcf/cmds/auto_cmds/lidar.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/auto_cmds/model.py` & `alcf-1.7.0/alcf/cmds/auto_cmds/model.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/calibrate.py` & `alcf-1.7.0/alcf/cmds/calibrate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/compare.py` & `alcf-1.7.0/alcf/cmds/compare.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/convert.py` & `alcf-1.7.0/alcf/cmds/convert.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/lidar.py` & `alcf-1.7.0/alcf/cmds/lidar.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
 - `blview`: Vaisala BL-VIEW L2 product.
 - `chm15k`: Lufft CHM 15k.
 - `cl31`: Vaisala CL31.
 - `cl51`: Vaisala CL51.
 - `cl61`: Vaisala CL61.
 - `cosp`: COSP simulated lidar.
 - `default`: The same format as the output of `alcf lidar`.
-- `minimpl`: Sigma Space MiniMPL.
+- `minimpl`: Sigma Space MiniMPL (converted via SigmaMPL).
 - `mpl`: Sigma Space MPL (converted via SigmaMPL).
-- `mpl2nc`: Sigma Space MPL (converted via mpl2nc).
+- `mpl2nc`: Sigma Space MPL and MiniMPL (converted via mpl2nc).
 
 Options
 -------
 
 - `align_output: <value>`: Align output time periods to the nearest multiple of output_sampling. Default: `true`.
 - `altitude: <altitude>`: Altitude of the instrument (m). Default: Taken from lidar data or `0` if not available.
 - `bsd: <value>`: Assume a given standard deviation of backscatter noise when detecting clouds or `none` to use the value calculated by the noise removal algorithm from observed backscatter if available (m^-1.sr^-1). The value applies at height `bsd_z` and is range-scaled for other heights. A suitable value can be taken from a plot generated by `alcf plot backscatter_sd_hist`. Default: `none`.
```

### Comparing `alcf-1.6.0/alcf/cmds/main.py` & `alcf-1.7.0/alcf/cmds/main.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/model.py` & `alcf-1.7.0/alcf/cmds/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,36 +14,42 @@
 		'lon': np.array([point[0], point[0]], dtype=np.float64),
 		'lat': np.array([point[1], point[1]], dtype=np.float64),
 		'time': np.array([time[0], time[1]], dtype=np.float64),
 		'time_bnds': np.array([[time[0], time_mid], [time_mid, time[1]]],
 			dtype=np.float64),
 	}
 
-def track_auto_time_bnds(time):
+def track_auto_time_bnds(time, track_gap=0):
 	n = len(time)
 	time_bnds = np.full((n, 2), np.nan, np.float64)
 	time_bnds[0,0] = time[0]
 	time_bnds[-1,1] = time[-1]
 	time_avg = 0.5*(time[:-1] + time[1:])
 	time_bnds[1:,0] = time_avg
 	time_bnds[:-1,1] = time_avg
+	if track_gap != 0:
+		time_diff = time[1:] - time[:-1]
+		mask1 = np.full(n, False, bool)
+		mask2 = np.full(n, False, bool)
+		mask1[:-1] = time_diff > track_gap
+		mask2[1:] = time_diff > track_gap
+		time_bnds[mask1,1] = time[mask1]
+		time_bnds[mask2,0] = time[mask2]
 	return time_bnds
 
-def read_track(filenames, lon_180=False):
-	iterable = False
-	try: iterable = iter(filenames)
-	except Exception: pass
-	else: filenames = [filenames]
+def read_track(filenames, lon_180=False, track_gap=0):
+	if type(filenames) not in [list, tuple]:
+		filenames = [filenames]
 	dd = []
 	for filename in filenames:
 		d = ds.read(filename, jd=True)
 		if len(d['time']) < 2:
 			raise ValueError('%s: Track must contain at least two records', filename)
 		if 'time_bnds' not in d:
-			d['time_bnds'] = track_auto_time_bnds(d['time'])
+			d['time_bnds'] = track_auto_time_bnds(d['time'], track_gap)
 			d['.']['time_bnds'] = {
 				'.dims': ['time', 'bnds'],
 				'long_name': 'time bounds',
 				'standard_name': 'time',
 				'units': 'days since -4713-11-24 12:00 UTC',
 				'calendar': 'proleptic_gregorian',
 			}
@@ -118,14 +124,15 @@
 		if debug: print(traceback.format_exc(), file=sys.stderr)
 		else: print('Use --debug to print debugging information.', file=sys.stderr)
 
 def run(type_, input_, output,
 	point=None,
 	time=None,
 	track=None,
+	track_gap=21600,
 	override_year=None,
 	track_lon_180=False,
 	debug=False,
 	r=False,
 	njobs=None,
 	**kwargs
 ):
@@ -147,19 +154,20 @@
 
 Arguments
 ---------
 
 - `type`: Input data type (see Types below).
 - `input`: Input directory.
 - `output`: Output directory.
-- `lon`: Point longitude.
-- `lat`: Point latitutde.
+- `lon`: Point longitude (degrees East).
+- `lat`: Point latitutde (degrees North).
 - `start`: Start time (see Time format below).
 - `end`: End time (see Time format below).
 - `track: <file>`, `track: { <file>... }`: One or more track NetCDF files (see Files below). If multiple files are supplied and `time_bnds` is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same.
+- `track_gap: <interval>`: If the interval is not 0, a track file is supplied, the `time_bnds` variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points. Default: `21600` (6 hours).
 - `options`: See Options below.
 
 Options
 -------
 
 - `njobs: <n>`: Number of parallel jobs. Default: number of CPU cores.
 - `-r`: Process the input directory recursively.
@@ -201,15 +209,15 @@
 		for i in [0, 1]:
 			time_lim[i] = aq.from_iso(time[i])
 			if time_lim[i] is None:
 				raise ValueError('Invalid time format: %s' % time[i])
 
 	d_track = None
 	if track is not None:
-		d_track = read_track(track, track_lon_180)
+		d_track = read_track(track, track_lon_180, track_gap/86400.)
 	elif point is not None and time is not None:
 		d_track = point_to_track(point, time_lim)
 	else:
 		raise ValueError('Point and time or track is required')
 
 	time_start = max(d_track['time_bnds'][0,0], time_lim[0])
 	time_end = min(d_track['time_bnds'][-1,1], time_lim[1])
```

### Comparing `alcf-1.6.0/alcf/cmds/plot.py` & `alcf-1.7.0/alcf/cmds/plot.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/simulate.py` & `alcf-1.7.0/alcf/cmds/simulate.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/cmds/stats.py` & `alcf-1.7.0/alcf/cmds/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-from collections.abc import Iterable
 import numpy as np
 import ds_format as ds
 from alcf.algorithms import interp
 from alcf.algorithms import stats
 from alcf.misc import parse_time
 
 VARIABLES = [
@@ -16,15 +15,15 @@
 	'backscatter_sd',
 	'backscatter_mol',
 	'lon',
 	'lat',
 ]
 
 def read_filters(filters):
-	if isinstance(filters, Iterable):
+	if type(filters) in [list, tuple]:
 		return [ds.read(filename) for filename in filters]
 	else:
 		return [ds.read(filters)]
 
 def run(input_, output,
 	tlim=None,
 	blim=[5., 200.],
```

### Comparing `alcf-1.6.0/alcf/fonts/LICENSE.md` & `alcf-1.7.0/alcf/fonts/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/fonts/PublicSans-Bold.otf` & `alcf-1.7.0/alcf/fonts/PublicSans-Bold.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/fonts/PublicSans-BoldItalic.otf` & `alcf-1.7.0/alcf/fonts/PublicSans-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/fonts/PublicSans-Italic.otf` & `alcf-1.7.0/alcf/fonts/PublicSans-Italic.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/fonts/PublicSans-Regular.otf` & `alcf-1.7.0/alcf/fonts/PublicSans-Regular.otf`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/__init__.py` & `alcf-1.7.0/alcf/lidars/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/blview.py` & `alcf-1.7.0/alcf/lidars/blview.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/chm15k.py` & `alcf-1.7.0/alcf/lidars/chm15k.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/cl51.py` & `alcf-1.7.0/alcf/lidars/cl51.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/cl61.py` & `alcf-1.7.0/alcf/lidars/cl61.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/default.py` & `alcf-1.7.0/alcf/lidars/default.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/mpl.py` & `alcf-1.7.0/alcf/lidars/mpl.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/lidars/mpl2nc.py` & `alcf-1.7.0/alcf/lidars/mpl2nc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/misc.py` & `alcf-1.7.0/alcf/misc.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/__init__.py` & `alcf-1.7.0/alcf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/amps.py` & `alcf-1.7.0/alcf/models/amps.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/era5.py` & `alcf-1.7.0/alcf/models/era5.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/icon.py` & `alcf-1.7.0/alcf/models/icon.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/icon_intake_healpix.py` & `alcf-1.7.0/alcf/models/icon_intake_healpix.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/jra55.py` & `alcf-1.7.0/alcf/models/jra55.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/merra2.py` & `alcf-1.7.0/alcf/models/merra2.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/nzcsm.py` & `alcf-1.7.0/alcf/models/nzcsm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/nzesm.py` & `alcf-1.7.0/alcf/models/nzesm.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf/models/um.py` & `alcf-1.7.0/alcf/models/um.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/alcf.egg-info/PKG-INFO` & `alcf-1.7.0/alcf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcf
-Version: 1.6.0
+Version: 1.7.0
 Summary: Automatic Lidar and Ceilometer Framework (ALCF)
 Home-page: https://alcf.peterkuma.net
 Author: Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: alc,ceilometer,lidar,atmosphere,model,simulator,nwp,gcm,cosp,actsim,vaisala,cl51,cl31,lufft,chm-15k,minimpl,amps,merra-2,um
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alcf-1.6.0/alcf.egg-info/SOURCES.txt` & `alcf-1.7.0/alcf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/build_doc` & `alcf-1.7.0/build_doc`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/MISR_simulator/MISR_simulator.f` & `alcf-1.7.0/cosp/MISR_simulator/MISR_simulator.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/MODIS_simulator/modis_simulator.F90` & `alcf-1.7.0/cosp/MODIS_simulator/modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/MODIS_simulator/test_modis_simulator.F90` & `alcf-1.7.0/cosp/MODIS_simulator/test_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/Makefile` & `alcf-1.7.0/cosp/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/Makefile.cmor1` & `alcf-1.7.0/cosp/Makefile.cmor1`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/Makefile.ibm` & `alcf-1.7.0/cosp/Makefile.ibm`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/README.md` & `alcf-1.7.0/cosp/README.md`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/README.txt` & `alcf-1.7.0/cosp/README.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/actsim/lidar_simulator.F90` & `alcf-1.7.0/cosp/actsim/lidar_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/actsim/lmd_ipsl_stats.F90` & `alcf-1.7.0/cosp/actsim/lmd_ipsl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/actsim/mie_backscatter_1064.F90` & `alcf-1.7.0/cosp/actsim/mie_backscatter_1064.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/actsim/mie_backscatter_532.F90` & `alcf-1.7.0/cosp/actsim/mie_backscatter_532.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/actsim/mie_backscatter_910.F90` & `alcf-1.7.0/cosp/actsim/mie_backscatter_910.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_cmor_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_input_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_long_inline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt` & `alcf-1.7.0/cosp/cfmip2/cosp_output_cfmip2_short_offline.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp.F90` & `alcf-1.7.0/cosp/cosp.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_constants.F90` & `alcf-1.7.0/cosp/cosp_constants.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_defs.h` & `alcf-1.7.0/cosp/cosp_defs.h`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_htfrtc.F90` & `alcf-1.7.0/cosp/cosp_htfrtc.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_input_nl.txt` & `alcf-1.7.0/cosp/cosp_input_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_io.F90` & `alcf-1.7.0/cosp/cosp_io.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_isccp_simulator.F90` & `alcf-1.7.0/cosp/cosp_isccp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_lidar.F90` & `alcf-1.7.0/cosp/cosp_lidar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_misr_simulator.F90` & `alcf-1.7.0/cosp/cosp_misr_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_modis_simulator.F90` & `alcf-1.7.0/cosp/cosp_modis_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_output_nl.txt` & `alcf-1.7.0/cosp/cosp_output_nl.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_rttov.F90` & `alcf-1.7.0/cosp/cosp_rttov.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_rttov_simulator.F90` & `alcf-1.7.0/cosp/cosp_rttov_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_simulator.F90` & `alcf-1.7.0/cosp/cosp_simulator.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_stats.F90` & `alcf-1.7.0/cosp/cosp_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_types.F90` & `alcf-1.7.0/cosp/cosp_types.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/cosp_utils.F90` & `alcf-1.7.0/cosp/cosp_utils.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/Makefile` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/Makefile`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/README` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/README`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/congvec.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/icarus.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/icarus.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/input.data` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/input.data.halved` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/input.data.halved`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/license` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/license`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/scops.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_congvec.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_congvec.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh` & `alcf-1.7.0/cosp/icarus-scops-4.1-bsd/test_isccp_cloud_types.ksh`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/llnl/cosp_radar.F90` & `alcf-1.7.0/cosp/llnl/cosp_radar.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/llnl/llnl_stats.F90` & `alcf-1.7.0/cosp/llnl/llnl_stats.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/llnl/pf_to_mr.f` & `alcf-1.7.0/cosp/llnl/pf_to_mr.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/llnl/prec_scops.f` & `alcf-1.7.0/cosp/llnl/prec_scops.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/mac_info.txt` & `alcf-1.7.0/cosp/mac_info.txt`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/predict_mom07.F90` & `alcf-1.7.0/cosp/predict_mom07.F90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/README` & `alcf-1.7.0/cosp/quickbeam/README`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/array_lib.f90` & `alcf-1.7.0/cosp/quickbeam/array_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/atmos_lib.f90` & `alcf-1.7.0/cosp/quickbeam/atmos_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/calc_Re.f90` & `alcf-1.7.0/cosp/quickbeam/calc_Re.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/dsd.f90` & `alcf-1.7.0/cosp/quickbeam/dsd.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/format_input.f90` & `alcf-1.7.0/cosp/quickbeam/format_input.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/gases.f90` & `alcf-1.7.0/cosp/quickbeam/gases.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/load_hydrometeor_classes.f90` & `alcf-1.7.0/cosp/quickbeam/load_hydrometeor_classes.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/load_mie_table.f90` & `alcf-1.7.0/cosp/quickbeam/load_mie_table.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/math_lib.f90` & `alcf-1.7.0/cosp/quickbeam/math_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/mrgrnk.f90` & `alcf-1.7.0/cosp/quickbeam/mrgrnk.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/optics_lib.f90` & `alcf-1.7.0/cosp/quickbeam/optics_lib.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/predict_psd07.f` & `alcf-1.7.0/cosp/quickbeam/predict_psd07.f`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/radar_simulator.f90` & `alcf-1.7.0/cosp/quickbeam/radar_simulator.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/radar_simulator_init.f90` & `alcf-1.7.0/cosp/quickbeam/radar_simulator_init.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/radar_simulator_types.f90` & `alcf-1.7.0/cosp/quickbeam/radar_simulator_types.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/scale_LUTs_io.f90` & `alcf-1.7.0/cosp/quickbeam/scale_LUTs_io.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/quickbeam/zeff.f90` & `alcf-1.7.0/cosp/quickbeam/zeff.f90`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/utils/COSP_plots.py` & `alcf-1.7.0/cosp/utils/COSP_plots.py`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/cosp/utils/append_cf3hr_files.sh` & `alcf-1.7.0/cosp/utils/append_cf3hr_files.sh`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/man/alcf-auto.1` & `alcf-1.7.0/man/alcf-auto.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-AUTO" "1" "February 2024" ""
+.TH "ALCF\-AUTO" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-auto\fR \- Peform automatic processing of model or lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf auto model <model_type> <lidar_type> point: { <lon> <lat> } time: { <start> <end> } [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
 
 alcf auto model <model_type> <lidar_type> track: <track> [<options>] [<model_options>] [<lidar_options>] [\-\-] <input> <output>
@@ -126,21 +126,21 @@
 \fBcl61\fR
 Vaisala CL61\.
 .TP
 \fBcosp\fR
 COSP simulated lidar\.
 .TP
 \fBminimpl\fR
-Sigma Space MiniMPL\.
+Sigma Space MiniMPL (converted via SigmaMPL)\.
 .TP
 \fBmpl\fR
 Sigma Space MPL (converted via SigmaMPL)\.
 .TP
 \fBmpl2nc\fR
-Sigma Space MPL (converted via mpl2nc)\.
+Sigma Space MPL and MiniMPL (converted via mpl2nc)\.
 .SH "TIME FORMAT"
 \fBYYYY\-MM\-DD[THH:MM[:SS]]\fR, where \fBYYYY\fR is year, \fBMM\fR is month, \fBDD\fR is day, \fBHH\fR is hour, \fBMM\fR is minute, \fBSS\fR is second\. Example: 2000\-01\-01T00:00:00\.
 .SH "EXAMPLES"
 Simulate a Vaisala CL51 instrument from MERRA\-2 data in \fBM2I3NVASM\.5\.12\.4\fR at 45 S, 170 E between 1 and 2 January 2020 and store the output in \fBalcf_merra2\fR\.
 .IP "" 4
 .nf
 alcf auto model merra2 cl51 point: { \-45\.0 170\.0 } time: { 2020\-01\-01 2020\-01\-02 } M2I3NVASM\.5\.12\.4 alcf_merra2
```

### Comparing `alcf-1.6.0/man/alcf-calibrate.1` & `alcf-1.7.0/man/alcf-calibrate.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CALIBRATE" "1" "February 2024" ""
+.TH "ALCF\-CALIBRATE" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-calibrate\fR \- Calibrate ALC backscatter\.
 .SH "SYNOPSIS"
 .nf
 alcf calibrate <type> [\-\-] <time_periods> <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.6.0/man/alcf-compare.1` & `alcf-1.7.0/man/alcf-compare.1`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-COMPARE" "1" "February 2024" ""
+.TH "ALCF\-COMPARE" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-compare\fR \- Calculate comparison statistics from multiple lidar time series\.
 .SH "SYNOPSIS"
 .nf
 alcf compare <input_1> <input_2> [<input_n>\|\.\|\.\|\.] <output>
 .fi
 .SH "ARGUMENTS"
```

### Comparing `alcf-1.6.0/man/alcf-convert.1` & `alcf-1.7.0/man/alcf-convert.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-CONVERT" "1" "February 2024" ""
+.TH "ALCF\-CONVERT" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-convert\fR \- Convert input instrument or model data to NetCDF\.
 .SH "SYNOPSIS"
 .nf
 alcf convert [options] <type> [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.6.0/man/alcf-lidar.1` & `alcf-1.7.0/man/alcf-lidar.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-LIDAR" "1" "February 2024" ""
+.TH "ALCF\-LIDAR" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-lidar\fR \- Process lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf lidar <type> [<options>] [<algorithm_options>] [\-\-] <lidar> <output>
 .fi
 .SH "DESCRIPTION"
@@ -60,21 +60,21 @@
 \fBcosp\fR
 COSP simulated lidar\.
 .TP
 \fBdefault\fR
 The same format as the output of \fBalcf lidar\fR\.
 .TP
 \fBminimpl\fR
-Sigma Space MiniMPL\.
+Sigma Space MiniMPL (converted via SigmaMPL)\.
 .TP
 \fBmpl\fR
 Sigma Space MPL (converted via SigmaMPL)\.
 .TP
 \fBmpl2nc\fR
-Sigma Space MPL (converted via mpl2nc)\.
+Sigma Space MPL and MiniMPL (converted via mpl2nc)\.
 .SH "OPTIONS"
 .TP
 \fBalign_output: <value>\fR
 Align output time periods to the nearest multiple of output_sampling\. Default: \fBtrue\fR\.
 .TP
 \fBaltitude: <altitude>\fR
 Altitude of the instrument (m)\. Default: Taken from lidar data or \fB0\fR if not available\.
```

### Comparing `alcf-1.6.0/man/alcf-model.1` & `alcf-1.7.0/man/alcf-model.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-MODEL" "1" "February 2024" ""
+.TH "ALCF\-MODEL" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-model\fR \- Extract model data at a point or along a track\.
 .SH "SYNOPSIS"
 .nf
 alcf model <type> point: { <lon> <lat> } time: { <start> <end> } [options] [\-\-] <input> <output>
 
 alcf model <type> track: <track> [\-\-] <input> <output>
@@ -15,24 +15,26 @@
 .IP "\[ci]" 4
 \fBtype\fR: Input data type (see Types below)\.
 .IP "\[ci]" 4
 \fBinput\fR: Input directory\.
 .IP "\[ci]" 4
 \fBoutput\fR: Output directory\.
 .IP "\[ci]" 4
-\fBlon\fR: Point longitude\.
+\fBlon\fR: Point longitude (degrees East)\.
 .IP "\[ci]" 4
-\fBlat\fR: Point latitutde\.
+\fBlat\fR: Point latitutde (degrees North)\.
 .IP "\[ci]" 4
 \fBstart\fR: Start time (see Time format below)\.
 .IP "\[ci]" 4
 \fBend\fR: End time (see Time format below)\.
 .IP "\[ci]" 4
 \fBtrack: <file>\fR, \fBtrack: { <file>\|\.\|\.\|\. }\fR: One or more track NetCDF files (see Files below)\. If multiple files are supplied and \fBtime_bnds\fR is not present in the files, they are assumed to be multiple segments of a discontinous track unless the last and first time of adjacent tracks are the same\.
 .IP "\[ci]" 4
+\fBtrack_gap: <interval>\fR: If the interval is not 0, a track file is supplied, the \fBtime_bnds\fR variable is not defined in the file and any two adjacent points are separated by more than the specified time interval (seconds), then a gap is assumed to be present between the two data points, instead of interpolating location between the two points\. Default: \fB21600\fR (6 hours)\.
+.IP "\[ci]" 4
 \fBoptions\fR: See Options below\.
 .IP "" 0
 .SH "OPTIONS"
 .TP
 \fBnjobs: <n>\fR
 Number of parallel jobs\. Default: number of CPU cores\.
 .TP
```

### Comparing `alcf-1.6.0/man/alcf-plot.1` & `alcf-1.7.0/man/alcf-plot.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-PLOT" "1" "February 2024" ""
+.TH "ALCF\-PLOT" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-plot\fR \- Plot lidar data\.
 .SH "SYNOPSIS"
 .nf
 alcf plot <plot_type> [<options>] [<plot_options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.6.0/man/alcf-simulate.1` & `alcf-1.7.0/man/alcf-simulate.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-SIMULATE" "1" "February 2024" ""
+.TH "ALCF\-SIMULATE" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-simulate\fR \- Simulate lidar measurements from model data using COSP\.
 .SH "SYNOPSIS"
 .nf
 alcf simulate <type> [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.6.0/man/alcf-stats.1` & `alcf-1.7.0/man/alcf-stats.1`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF\-STATS" "1" "February 2024" ""
+.TH "ALCF\-STATS" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\-stats\fR \- Calculate cloud occurrence statistics\.
 .SH "SYNOPSIS"
 .nf
 alcf stats [<options>] [\-\-] <input> <output>
 .fi
 .SH "DESCRIPTION"
```

### Comparing `alcf-1.6.0/man/alcf.1` & `alcf-1.7.0/man/alcf.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" generated with Ronn-NG/v0.9.1
 .\" http://github.com/apjanke/ronn-ng/tree/0.9.1
-.TH "ALCF" "1" "February 2024" ""
+.TH "ALCF" "1" "April 2024" ""
 .SH "NAME"
 \fBalcf\fR \- Tool for processing of automatic lidar and ceilometer (ALC) data and intercomparison with atmospheric models\.
 .SH "SYNOPSIS"
 .nf
 alcf <cmd> [<options>]
 alcf <cmd> \-\-help
 .fi
```

### Comparing `alcf-1.6.0/setup.py` & `alcf-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	def run(self):
 		subprocess.run('make', cwd='cosp', check=True)
 		subprocess.run('make', check=True)
 		build_py.run(self)
 
 setup(
 	name='alcf',
-	version='1.6.0',
+	version='1.7.0',
 	description='Automatic Lidar and Ceilometer Framework (ALCF)',
 	author='Peter Kuma, Adrian J. McDonald, Olaf Morgenstern, Richard Querel, Israel Silber, Connor J. Flynn',
 	author_email='peter@peterkuma.net',
 	license='MIT',
 	entry_points={
 		'console_scripts': 'alcf = alcf.bin.alcf:main_wrapper',
 	},
```

### Comparing `alcf-1.6.0/src/cosp_run.f03` & `alcf-1.7.0/src/cosp_run.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/src/main.f03` & `alcf-1.7.0/src/main.f03`

 * *Files identical despite different names*

### Comparing `alcf-1.6.0/src/nc_utils.f03` & `alcf-1.7.0/src/nc_utils.f03`

 * *Files identical despite different names*

