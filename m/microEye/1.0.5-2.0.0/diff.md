# Comparing `tmp/microEye-1.0.5.tar.gz` & `tmp/microEye-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microEye-1.0.5.tar", last modified: Tue Jan  2 08:21:49 2024, max compression
+gzip compressed data, was "microEye-2.0.0.tar", last modified: Mon Apr  8 15:25:11 2024, max compression
```

## Comparing `microEye-1.0.5.tar` & `microEye-2.0.0.tar`

### file list

```diff
@@ -1,121 +1,128 @@
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.971308 microEye-1.0.5/
--rw-rw-rw-   0        0        0    35823 2021-10-04 21:46:20.000000 microEye-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       32 2021-10-04 21:46:20.000000 microEye-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    11653 2024-01-02 08:21:49.970307 microEye-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10084 2023-12-29 14:04:28.000000 microEye-1.0.5/README.md
--rw-rw-rw-   0        0        0      525 2023-12-17 12:51:53.000000 microEye-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-02 08:21:49.971308 microEye-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1959 2024-01-02 08:09:50.000000 microEye-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.815430 microEye-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.842484 microEye-1.0.5/src/microEye/
--rw-rw-rw-   0        0        0       49 2023-12-07 17:11:30.000000 microEye-1.0.5/src/microEye/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.867549 microEye-1.0.5/src/microEye/analysis/
--rw-rw-rw-   0        0        0       75 2023-12-01 21:47:51.000000 microEye-1.0.5/src/microEye/analysis/__init__.py
--rw-rw-rw-   0        0        0     4357 2023-11-09 14:24:59.000000 microEye-1.0.5/src/microEye/analysis/checklist_dialog.py
--rw-rw-rw-   0        0        0     7913 2023-11-09 14:25:26.000000 microEye-1.0.5/src/microEye/analysis/cmosMaps.py
--rw-rw-rw-   0        0        0    73807 2023-12-12 12:03:13.000000 microEye-1.0.5/src/microEye/analysis/file_sys.py
--rw-rw-rw-   0        0        0    17227 2023-12-13 17:51:40.000000 microEye-1.0.5/src/microEye/analysis/filters.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.876569 microEye-1.0.5/src/microEye/analysis/fitting/
--rw-rw-rw-   0        0        0        0 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/analysis/fitting/__init__.py
--rw-rw-rw-   0        0        0    19375 2023-12-13 18:47:15.000000 microEye-1.0.5/src/microEye/analysis/fitting/fit.py
--rw-rw-rw-   0        0        0    11506 2023-11-09 14:22:09.000000 microEye-1.0.5/src/microEye/analysis/fitting/nena.py
--rw-rw-rw-   0        0        0     2632 2023-10-22 12:20:11.000000 microEye-1.0.5/src/microEye/analysis/fitting/phasor_fit.py
--rw-rw-rw-   0        0        0     8412 2023-12-11 17:29:36.000000 microEye-1.0.5/src/microEye/analysis/fitting/processing.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.881574 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.886670 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/
--rw-rw-rw-   0        0        0    14681 2023-11-14 14:34:42.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUfunctions.py
--rw-rw-rw-   0        0        0    44525 2023-11-14 14:35:50.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUmleFit_LM.py
--rw-rw-rw-   0        0        0     5425 2023-11-14 14:35:58.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUsplineLib.py
--rw-rw-rw-   0        0        0       29 2022-08-26 14:54:16.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.891597 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/
--rw-rw-rw-   0        0        0    14796 2023-11-14 14:36:18.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUfunctions.py
--rw-rw-rw-   0        0        0    47360 2023-11-14 14:37:00.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_EMCCD.py
--rw-rw-rw-   0        0        0    48840 2023-11-14 14:37:37.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_sCMOS.py
--rw-rw-rw-   0        0        0     5475 2023-11-14 14:37:53.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUsplineLib.py
--rw-rw-rw-   0        0        0       70 2022-08-26 14:55:36.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/__init__.py
--rw-rw-rw-   0        0        0      166 2023-11-29 21:09:22.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/__init__.py
--rw-rw-rw-   0        0        0      798 2022-10-14 09:21:45.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/constants.py
--rw-rw-rw-   0        0        0    25038 2023-12-12 12:17:12.000000 microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/mainfunctions.py
--rw-rw-rw-   0        0        0    25249 2023-12-15 12:32:27.000000 microEye-1.0.5/src/microEye/analysis/fitting/results.py
--rw-rw-rw-   0        0        0     4407 2023-12-15 09:50:23.000000 microEye-1.0.5/src/microEye/analysis/fitting/results_stats.py
--rw-rw-rw-   0        0        0     6768 2023-11-29 21:19:03.000000 microEye-1.0.5/src/microEye/analysis/fitting/tardis.py
--rw-rw-rw-   0        0        0    15946 2023-12-19 12:03:52.000000 microEye-1.0.5/src/microEye/analysis/multi_viewer.py
--rw-rw-rw-   0        0        0    18313 2023-11-09 14:24:15.000000 microEye-1.0.5/src/microEye/analysis/rendering.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.896616 microEye-1.0.5/src/microEye/analysis/tools/
--rw-rw-rw-   0        0        0        0 2023-11-14 17:41:06.000000 microEye-1.0.5/src/microEye/analysis/tools/__init__.py
--rw-rw-rw-   0        0        0    37298 2023-12-07 19:53:16.000000 microEye-1.0.5/src/microEye/analysis/tools/kymograms.py
--rw-rw-rw-   0        0        0    21257 2023-12-20 17:01:24.000000 microEye-1.0.5/src/microEye/analysis/tools/roi_selectors.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.904639 microEye-1.0.5/src/microEye/analysis/viewer/
--rw-rw-rw-   0        0        0        0 2023-12-01 20:21:51.000000 microEye-1.0.5/src/microEye/analysis/viewer/__init__.py
--rw-rw-rw-   0        0        0    14694 2023-12-15 14:46:23.000000 microEye-1.0.5/src/microEye/analysis/viewer/image_options_widget.py
--rw-rw-rw-   0        0        0    42436 2023-12-29 13:28:26.000000 microEye-1.0.5/src/microEye/analysis/viewer/images.py
--rw-rw-rw-   0        0        0     3836 2023-12-09 14:28:24.000000 microEye-1.0.5/src/microEye/analysis/viewer/layers_widget.py
--rw-rw-rw-   0        0        0    28599 2023-12-12 15:18:20.000000 microEye-1.0.5/src/microEye/analysis/viewer/localizations.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.909645 microEye-1.0.5/src/microEye/hardware/
--rw-rw-rw-   0        0        0      219 2023-11-10 21:51:40.000000 microEye-1.0.5/src/microEye/hardware/__init__.py
--rw-rw-rw-   0        0        0    32786 2023-11-29 21:27:03.000000 microEye-1.0.5/src/microEye/hardware/acquisition_module.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.927192 microEye-1.0.5/src/microEye/hardware/cams/
--rw-rw-rw-   0        0        0     4787 2023-11-29 21:18:35.000000 microEye-1.0.5/src/microEye/hardware/cams/CameraListWidget.py
--rw-rw-rw-   0        0        0     3871 2023-11-14 14:25:51.000000 microEye-1.0.5/src/microEye/hardware/cams/IR_Cam.py
--rw-rw-rw-   0        0        0      682 2023-09-15 09:05:28.000000 microEye-1.0.5/src/microEye/hardware/cams/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-11-14 14:27:24.000000 microEye-1.0.5/src/microEye/hardware/cams/camera_calibration.py
--rw-rw-rw-   0        0        0    23436 2023-12-20 16:39:12.000000 microEye-1.0.5/src/microEye/hardware/cams/camera_options.py
--rw-rw-rw-   0        0        0    27144 2023-12-22 21:23:24.000000 microEye-1.0.5/src/microEye/hardware/cams/camera_panel.py
--rw-rw-rw-   0        0        0    18474 2023-12-20 22:41:12.000000 microEye-1.0.5/src/microEye/hardware/cams/jobs.py
--rw-rw-rw-   0        0        0     3109 2023-11-14 14:17:40.000000 microEye-1.0.5/src/microEye/hardware/cams/line_profiler.py
--rw-rw-rw-   0        0        0     1021 2023-09-14 07:18:37.000000 microEye-1.0.5/src/microEye/hardware/cams/micam.py
--rw-rw-rw-   0        0        0    55915 2023-12-19 13:17:13.000000 microEye-1.0.5/src/microEye/hardware/cams/thorlabs.py
--rw-rw-rw-   0        0        0    29918 2023-12-28 09:25:15.000000 microEye-1.0.5/src/microEye/hardware/cams/thorlabs_panel.py
--rw-rw-rw-   0        0        0    35360 2023-12-22 20:58:55.000000 microEye-1.0.5/src/microEye/hardware/cams/ueye_camera.py
--rw-rw-rw-   0        0        0    29635 2023-12-28 09:04:01.000000 microEye-1.0.5/src/microEye/hardware/cams/ueye_panel.py
--rw-rw-rw-   0        0        0    31524 2023-12-18 23:02:38.000000 microEye-1.0.5/src/microEye/hardware/cams/vimba_cam.py
--rw-rw-rw-   0        0        0    29877 2023-12-22 21:05:39.000000 microEye-1.0.5/src/microEye/hardware/cams/vimba_panel.py
--rw-rw-rw-   0        0        0    36965 2023-12-17 12:57:19.000000 microEye-1.0.5/src/microEye/hardware/control_module.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.933206 microEye-1.0.5/src/microEye/hardware/lasers/
--rw-rw-rw-   0        0        0      139 2023-09-13 10:52:47.000000 microEye-1.0.5/src/microEye/hardware/lasers/__init__.py
--rw-rw-rw-   0        0        0    18187 2023-11-14 14:25:28.000000 microEye-1.0.5/src/microEye/hardware/lasers/io_matchbox.py
--rw-rw-rw-   0        0        0    14610 2023-11-14 14:25:06.000000 microEye-1.0.5/src/microEye/hardware/lasers/io_single_laser.py
--rw-rw-rw-   0        0        0    67442 2023-12-29 13:43:24.000000 microEye-1.0.5/src/microEye/hardware/miEye.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.937222 microEye-1.0.5/src/microEye/hardware/misc/
--rw-rw-rw-   0        0        0        0 2023-11-10 21:51:29.000000 microEye-1.0.5/src/microEye/hardware/misc/__init__.py
--rw-rw-rw-   0        0        0     2045 2023-11-14 14:24:31.000000 microEye-1.0.5/src/microEye/hardware/misc/acquisition_view.py
--rw-rw-rw-   0        0        0    29301 2023-11-14 14:24:15.000000 microEye-1.0.5/src/microEye/hardware/misc/reglo.py
--rw-rw-rw-   0        0        0     7915 2023-11-14 14:23:43.000000 microEye-1.0.5/src/microEye/hardware/misc/temp.py
--rw-rw-rw-   0        0        0     3969 2023-11-14 14:19:31.000000 microEye-1.0.5/src/microEye/hardware/port_config.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.939224 microEye-1.0.5/src/microEye/hardware/protocols/
--rw-rw-rw-   0        0        0        2 2023-12-28 20:04:25.000000 microEye-1.0.5/src/microEye/hardware/protocols/__init__.py
--rw-rw-rw-   0        0        0    21600 2023-12-29 09:53:15.000000 microEye-1.0.5/src/microEye/hardware/protocols/actions.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.944244 microEye-1.0.5/src/microEye/hardware/stages/
--rw-rw-rw-   0        0        0      124 2023-09-13 10:41:31.000000 microEye-1.0.5/src/microEye/hardware/stages/__init__.py
--rw-rw-rw-   0        0        0     7353 2023-11-14 14:23:34.000000 microEye-1.0.5/src/microEye/hardware/stages/elliptec.py
--rw-rw-rw-   0        0        0    13023 2023-11-29 21:19:21.000000 microEye-1.0.5/src/microEye/hardware/stages/kinesis.py
--rw-rw-rw-   0        0        0    12515 2023-11-14 14:23:18.000000 microEye-1.0.5/src/microEye/hardware/stages/piezo_concept.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.948248 microEye-1.0.5/src/microEye/hardware/widgets/
--rw-rw-rw-   0        0        0       71 2023-09-13 10:44:41.000000 microEye-1.0.5/src/microEye/hardware/widgets/__init__.py
--rw-rw-rw-   0        0        0     6839 2023-11-14 14:22:48.000000 microEye-1.0.5/src/microEye/hardware/widgets/focusWidget.py
--rw-rw-rw-   0        0        0     3345 2023-11-29 21:22:29.000000 microEye-1.0.5/src/microEye/hardware/widgets/qlist_slider.py
--rw-rw-rw-   0        0        0     9762 2023-11-29 21:26:59.000000 microEye-1.0.5/src/microEye/hardware/widgets/scan_acquisition.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.956277 microEye-1.0.5/src/microEye/icons/
--rw-rw-rw-   0        0        0   177771 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/1024.png
--rw-rw-rw-   0        0        0    15888 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/128.png
--rw-rw-rw-   0        0        0      956 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/16.png
--rw-rw-rw-   0        0        0    35513 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/256.png
--rw-rw-rw-   0        0        0     2553 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/32.png
--rw-rw-rw-   0        0        0    79151 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/512.png
--rw-rw-rw-   0        0        0     6562 2022-04-24 18:32:42.000000 microEye-1.0.5/src/microEye/icons/64.png
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.967305 microEye-1.0.5/src/microEye/shared/
--rw-rw-rw-   0        0        0        0 2023-11-29 21:10:46.000000 microEye-1.0.5/src/microEye/shared/__init__.py
--rw-rw-rw-   0        0        0     2955 2023-12-19 11:47:43.000000 microEye-1.0.5/src/microEye/shared/expandable_groupbox.py
--rw-rw-rw-   0        0        0    11556 2023-12-17 14:58:44.000000 microEye-1.0.5/src/microEye/shared/gui_helper.py
--rw-rw-rw-   0        0        0     7771 2023-12-17 12:45:57.000000 microEye-1.0.5/src/microEye/shared/hid_controller.py
--rw-rw-rw-   0        0        0     4074 2023-12-17 12:47:32.000000 microEye-1.0.5/src/microEye/shared/labelled_slider.py
--rw-rw-rw-   0        0        0    23861 2023-12-18 12:44:45.000000 microEye-1.0.5/src/microEye/shared/metadata.py
--rw-rw-rw-   0        0        0    35622 2023-12-19 12:46:02.000000 microEye-1.0.5/src/microEye/shared/metadata_tree.py
--rw-rw-rw-   0        0        0    10409 2023-12-17 12:54:46.000000 microEye-1.0.5/src/microEye/shared/pyscripting.py
--rw-rw-rw-   0        0        0     2354 2023-12-17 12:57:39.000000 microEye-1.0.5/src/microEye/shared/thread_worker.py
--rw-rw-rw-   0        0        0    44312 2023-12-20 23:00:00.000000 microEye-1.0.5/src/microEye/shared/uImage.py
-drwxrwxrwx   0        0        0        0 2024-01-02 08:21:49.969307 microEye-1.0.5/src/microEye.egg-info/
--rw-rw-rw-   0        0        0    11653 2024-01-02 08:21:49.000000 microEye-1.0.5/src/microEye.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4004 2024-01-02 08:21:49.000000 microEye-1.0.5/src/microEye.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-02 08:21:49.000000 microEye-1.0.5/src/microEye.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-02 08:21:49.000000 microEye-1.0.5/src/microEye.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:11.012312 microEye-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2021-10-04 21:46:20.000000 microEye-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       32 2021-10-04 21:46:20.000000 microEye-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12636 2024-04-08 15:25:11.011311 microEye-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10916 2024-04-08 15:12:18.000000 microEye-2.0.0/README.md
+-rw-rw-rw-   0        0        0      525 2023-12-17 12:51:53.000000 microEye-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:25:11.012312 microEye-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2071 2024-04-08 15:24:14.000000 microEye-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.436733 microEye-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.456616 microEye-2.0.0/src/microEye/
+-rw-rw-rw-   0        0        0       49 2023-12-07 17:11:30.000000 microEye-2.0.0/src/microEye/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.514727 microEye-2.0.0/src/microEye/analysis/
+-rw-rw-rw-   0        0        0       75 2023-12-01 21:47:51.000000 microEye-2.0.0/src/microEye/analysis/__init__.py
+-rw-rw-rw-   0        0        0     4357 2023-11-09 14:24:59.000000 microEye-2.0.0/src/microEye/analysis/checklist_dialog.py
+-rw-rw-rw-   0        0        0     7913 2023-11-09 14:25:26.000000 microEye-2.0.0/src/microEye/analysis/cmosMaps.py
+-rw-rw-rw-   0        0        0    72725 2024-03-13 17:14:53.000000 microEye-2.0.0/src/microEye/analysis/file_sys.py
+-rw-rw-rw-   0        0        0    18184 2024-01-29 09:21:15.000000 microEye-2.0.0/src/microEye/analysis/filters.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.563078 microEye-2.0.0/src/microEye/analysis/fitting/
+-rw-rw-rw-   0        0        0        0 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/analysis/fitting/__init__.py
+-rw-rw-rw-   0        0        0    19381 2024-02-07 15:18:39.000000 microEye-2.0.0/src/microEye/analysis/fitting/fit.py
+-rw-rw-rw-   0        0        0    11506 2023-11-09 14:22:09.000000 microEye-2.0.0/src/microEye/analysis/fitting/nena.py
+-rw-rw-rw-   0        0        0     2632 2023-10-22 12:20:11.000000 microEye-2.0.0/src/microEye/analysis/fitting/phasor_fit.py
+-rw-rw-rw-   0        0        0     8412 2023-12-11 17:29:36.000000 microEye-2.0.0/src/microEye/analysis/fitting/processing.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.585305 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.611218 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/
+-rw-rw-rw-   0        0        0    14681 2023-11-14 14:34:42.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUfunctions.py
+-rw-rw-rw-   0        0        0    44525 2023-11-14 14:35:50.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUmleFit_LM.py
+-rw-rw-rw-   0        0        0     5425 2023-11-14 14:35:58.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUsplineLib.py
+-rw-rw-rw-   0        0        0       29 2022-08-26 14:54:16.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.645873 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/
+-rw-rw-rw-   0        0        0    14796 2023-11-14 14:36:18.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUfunctions.py
+-rw-rw-rw-   0        0        0    47360 2023-11-14 14:37:00.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_EMCCD.py
+-rw-rw-rw-   0        0        0    48840 2023-11-14 14:37:37.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_sCMOS.py
+-rw-rw-rw-   0        0        0     5475 2023-11-14 14:37:53.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUsplineLib.py
+-rw-rw-rw-   0        0        0       70 2022-08-26 14:55:36.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-11-29 21:09:22.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/__init__.py
+-rw-rw-rw-   0        0        0      798 2022-10-14 09:21:45.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/constants.py
+-rw-rw-rw-   0        0        0    25038 2023-12-12 12:17:12.000000 microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/mainfunctions.py
+-rw-rw-rw-   0        0        0    25249 2023-12-15 12:32:27.000000 microEye-2.0.0/src/microEye/analysis/fitting/results.py
+-rw-rw-rw-   0        0        0     4407 2023-12-15 09:50:23.000000 microEye-2.0.0/src/microEye/analysis/fitting/results_stats.py
+-rw-rw-rw-   0        0        0     6768 2023-11-29 21:19:03.000000 microEye-2.0.0/src/microEye/analysis/fitting/tardis.py
+-rw-rw-rw-   0        0        0    14857 2024-03-13 17:13:09.000000 microEye-2.0.0/src/microEye/analysis/multi_viewer.py
+-rw-rw-rw-   0        0        0    18313 2023-11-09 14:24:15.000000 microEye-2.0.0/src/microEye/analysis/rendering.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.659075 microEye-2.0.0/src/microEye/analysis/tools/
+-rw-rw-rw-   0        0        0        0 2023-11-14 17:41:06.000000 microEye-2.0.0/src/microEye/analysis/tools/__init__.py
+-rw-rw-rw-   0        0        0    37407 2024-03-25 12:43:40.000000 microEye-2.0.0/src/microEye/analysis/tools/kymograms.py
+-rw-rw-rw-   0        0        0    21257 2023-12-20 17:01:24.000000 microEye-2.0.0/src/microEye/analysis/tools/roi_selectors.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.686501 microEye-2.0.0/src/microEye/analysis/viewer/
+-rw-rw-rw-   0        0        0        0 2023-12-01 20:21:51.000000 microEye-2.0.0/src/microEye/analysis/viewer/__init__.py
+-rw-rw-rw-   0        0        0    14694 2023-12-15 14:46:23.000000 microEye-2.0.0/src/microEye/analysis/viewer/image_options_widget.py
+-rw-rw-rw-   0        0        0    42209 2024-03-06 12:06:06.000000 microEye-2.0.0/src/microEye/analysis/viewer/images.py
+-rw-rw-rw-   0        0        0     3836 2023-12-09 14:28:24.000000 microEye-2.0.0/src/microEye/analysis/viewer/layers_widget.py
+-rw-rw-rw-   0        0        0    28493 2024-03-06 12:06:03.000000 microEye-2.0.0/src/microEye/analysis/viewer/localizations.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.707812 microEye-2.0.0/src/microEye/hardware/
+-rw-rw-rw-   0        0        0      123 2024-03-13 15:57:54.000000 microEye-2.0.0/src/microEye/hardware/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.815141 microEye-2.0.0/src/microEye/hardware/cams/
+-rw-rw-rw-   0        0        0     3871 2023-11-14 14:25:51.000000 microEye-2.0.0/src/microEye/hardware/cams/IR_Cam.py
+-rw-rw-rw-   0        0        0      668 2024-03-07 13:23:18.000000 microEye-2.0.0/src/microEye/hardware/cams/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-11-14 14:27:24.000000 microEye-2.0.0/src/microEye/hardware/cams/camera_calibration.py
+-rw-rw-rw-   0        0        0    14333 2024-03-20 10:32:59.000000 microEye-2.0.0/src/microEye/hardware/cams/camera_list.py
+-rw-rw-rw-   0        0        0    18177 2024-03-18 14:20:37.000000 microEye-2.0.0/src/microEye/hardware/cams/camera_options.py
+-rw-rw-rw-   0        0        0    28421 2024-03-25 22:31:11.000000 microEye-2.0.0/src/microEye/hardware/cams/camera_panel.py
+-rw-rw-rw-   0        0        0    24293 2024-03-17 10:36:33.000000 microEye-2.0.0/src/microEye/hardware/cams/dummy_panel.py
+-rw-rw-rw-   0        0        0    18167 2024-03-18 14:28:24.000000 microEye-2.0.0/src/microEye/hardware/cams/jobs.py
+-rw-rw-rw-   0        0        0     3109 2023-11-14 14:17:40.000000 microEye-2.0.0/src/microEye/hardware/cams/line_profiler.py
+-rw-rw-rw-   0        0        0    12843 2024-03-08 13:36:48.000000 microEye-2.0.0/src/microEye/hardware/cams/micam.py
+-rw-rw-rw-   0        0        0    55939 2024-03-06 11:13:29.000000 microEye-2.0.0/src/microEye/hardware/cams/thorlabs.py
+-rw-rw-rw-   0        0        0    29365 2024-03-18 14:19:02.000000 microEye-2.0.0/src/microEye/hardware/cams/thorlabs_panel.py
+-rw-rw-rw-   0        0        0    35384 2024-03-06 11:24:41.000000 microEye-2.0.0/src/microEye/hardware/cams/ueye_camera.py
+-rw-rw-rw-   0        0        0    29098 2024-03-18 14:18:14.000000 microEye-2.0.0/src/microEye/hardware/cams/ueye_panel.py
+-rw-rw-rw-   0        0        0    33951 2024-03-08 13:49:59.000000 microEye-2.0.0/src/microEye/hardware/cams/vimba_cam.py
+-rw-rw-rw-   0        0        0    29856 2024-03-17 10:36:28.000000 microEye-2.0.0/src/microEye/hardware/cams/vimba_panel.py
+-rw-rw-rw-   0        0        0     1726 2024-03-13 10:55:31.000000 microEye-2.0.0/src/microEye/hardware/device.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.845311 microEye-2.0.0/src/microEye/hardware/lasers/
+-rw-rw-rw-   0        0        0      190 2024-03-19 09:00:56.000000 microEye-2.0.0/src/microEye/hardware/lasers/__init__.py
+-rw-rw-rw-   0        0        0    23054 2024-03-21 23:42:03.000000 microEye-2.0.0/src/microEye/hardware/lasers/io_matchbox.py
+-rw-rw-rw-   0        0        0     2386 2024-03-13 22:44:59.000000 microEye-2.0.0/src/microEye/hardware/lasers/io_params.py
+-rw-rw-rw-   0        0        0    21943 2024-03-19 20:59:34.000000 microEye-2.0.0/src/microEye/hardware/lasers/io_single_laser.py
+-rw-rw-rw-   0        0        0    15037 2024-03-25 15:25:46.000000 microEye-2.0.0/src/microEye/hardware/lasers/laser_relay.py
+-rw-rw-rw-   0        0        0    44864 2024-03-27 12:44:06.000000 microEye-2.0.0/src/microEye/hardware/miEye.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.864193 microEye-2.0.0/src/microEye/hardware/misc/
+-rw-rw-rw-   0        0        0        0 2023-11-10 21:51:29.000000 microEye-2.0.0/src/microEye/hardware/misc/__init__.py
+-rw-rw-rw-   0        0        0     2045 2023-11-14 14:24:31.000000 microEye-2.0.0/src/microEye/hardware/misc/acquisition_view.py
+-rw-rw-rw-   0        0        0    27835 2024-03-13 17:09:01.000000 microEye-2.0.0/src/microEye/hardware/misc/reglo.py
+-rw-rw-rw-   0        0        0     6538 2024-03-13 17:09:08.000000 microEye-2.0.0/src/microEye/hardware/misc/temp.py
+-rw-rw-rw-   0        0        0     1962 2024-03-16 12:12:33.000000 microEye-2.0.0/src/microEye/hardware/port_config.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.872711 microEye-2.0.0/src/microEye/hardware/protocols/
+-rw-rw-rw-   0        0        0        2 2023-12-28 20:04:25.000000 microEye-2.0.0/src/microEye/hardware/protocols/__init__.py
+-rw-rw-rw-   0        0        0    21600 2023-12-29 09:53:15.000000 microEye-2.0.0/src/microEye/hardware/protocols/actions.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.900840 microEye-2.0.0/src/microEye/hardware/stages/
+-rw-rw-rw-   0        0        0      132 2024-03-21 08:12:48.000000 microEye-2.0.0/src/microEye/hardware/stages/__init__.py
+-rw-rw-rw-   0        0        0     7353 2023-11-14 14:23:34.000000 microEye-2.0.0/src/microEye/hardware/stages/elliptec.py
+-rw-rw-rw-   0        0        0    13000 2024-03-17 11:16:28.000000 microEye-2.0.0/src/microEye/hardware/stages/kinesis.py
+-rw-rw-rw-   0        0        0    16331 2024-03-27 12:44:06.000000 microEye-2.0.0/src/microEye/hardware/stages/piezo_concept.py
+-rw-rw-rw-   0        0        0    22941 2024-03-27 12:44:00.000000 microEye-2.0.0/src/microEye/hardware/stages/stabilizer.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.928393 microEye-2.0.0/src/microEye/hardware/widgets/
+-rw-rw-rw-   0        0        0      124 2024-03-20 08:51:04.000000 microEye-2.0.0/src/microEye/hardware/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3824 2024-03-25 15:33:18.000000 microEye-2.0.0/src/microEye/hardware/widgets/devices.py
+-rw-rw-rw-   0        0        0     9414 2024-03-27 12:44:06.000000 microEye-2.0.0/src/microEye/hardware/widgets/focusWidget.py
+-rw-rw-rw-   0        0        0     3345 2023-11-29 21:22:29.000000 microEye-2.0.0/src/microEye/hardware/widgets/qlist_slider.py
+-rw-rw-rw-   0        0        0    12450 2024-03-25 23:19:53.000000 microEye-2.0.0/src/microEye/hardware/widgets/scan_acquisition.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:10.936422 microEye-2.0.0/src/microEye/icons/
+-rw-rw-rw-   0        0        0   177771 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/1024.png
+-rw-rw-rw-   0        0        0    15888 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/128.png
+-rw-rw-rw-   0        0        0      956 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/16.png
+-rw-rw-rw-   0        0        0    35513 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/256.png
+-rw-rw-rw-   0        0        0     2553 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/32.png
+-rw-rw-rw-   0        0        0    79151 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/512.png
+-rw-rw-rw-   0        0        0     6562 2022-04-24 18:32:42.000000 microEye-2.0.0/src/microEye/icons/64.png
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:11.009309 microEye-2.0.0/src/microEye/shared/
+-rw-rw-rw-   0        0        0       67 2024-03-13 17:11:32.000000 microEye-2.0.0/src/microEye/shared/__init__.py
+-rw-rw-rw-   0        0        0     2955 2023-12-19 11:47:43.000000 microEye-2.0.0/src/microEye/shared/expandable_groupbox.py
+-rw-rw-rw-   0        0        0    11546 2024-03-25 23:12:21.000000 microEye-2.0.0/src/microEye/shared/gui_helper.py
+-rw-rw-rw-   0        0        0    14547 2024-03-20 08:21:38.000000 microEye-2.0.0/src/microEye/shared/hid_controller.py
+-rw-rw-rw-   0        0        0     4074 2023-12-17 12:47:32.000000 microEye-2.0.0/src/microEye/shared/labelled_slider.py
+-rw-rw-rw-   0        0        0    23861 2023-12-18 12:44:45.000000 microEye-2.0.0/src/microEye/shared/metadata.py
+-rw-rw-rw-   0        0        0    31681 2024-03-13 22:57:38.000000 microEye-2.0.0/src/microEye/shared/metadata_tree.py
+-rw-rw-rw-   0        0        0     7152 2024-03-18 14:07:57.000000 microEye-2.0.0/src/microEye/shared/parameter_tree.py
+-rw-rw-rw-   0        0        0    10409 2023-12-17 12:54:46.000000 microEye-2.0.0/src/microEye/shared/pyscripting.py
+-rw-rw-rw-   0        0        0     3021 2024-04-08 15:05:40.000000 microEye-2.0.0/src/microEye/shared/start_gui.py
+-rw-rw-rw-   0        0        0     2354 2024-03-08 11:24:14.000000 microEye-2.0.0/src/microEye/shared/thread_worker.py
+-rw-rw-rw-   0        0        0    44509 2024-01-29 08:52:13.000000 microEye-2.0.0/src/microEye/shared/uImage.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:25:11.010311 microEye-2.0.0/src/microEye.egg-info/
+-rw-rw-rw-   0        0        0    12636 2024-04-08 15:25:10.000000 microEye-2.0.0/src/microEye.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4265 2024-04-08 15:25:10.000000 microEye-2.0.0/src/microEye.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:25:10.000000 microEye-2.0.0/src/microEye.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      464 2024-04-08 15:25:10.000000 microEye-2.0.0/src/microEye.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 15:25:10.000000 microEye-2.0.0/src/microEye.egg-info/top_level.txt
```

### Comparing `microEye-1.0.5/LICENSE` & `microEye-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/PKG-INFO` & `microEye-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,39 @@
-Metadata-Version: 2.1
-Name: microEye
-Version: 1.0.5
-Summary: A python toolkit for fluorescence microscopy         that features hardware control, data analysis and vizualization         for super-resolution single-molecule localization microscopy and         single-partical tracking.
-Home-page: https://github.com/samhitech/microEye
-Author: Mohammad Nour Alsamsam
-Author-email: nour.alsamsam@gmail.com
-Project-URL: miEye Paper, https://doi.org/10.1016/j.ohx.2022.e00368
-Project-URL: miEye OSF, http://doi.org/10.17605/osf.io/j2fqy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires: autopep8 (==2.0.4)
-Requires: dask (==2022.1.0)
-Requires: h5py (==3.10.0)
-Requires: hidapi (==0.14.0)
-Requires: matplotlib (==3.6.3)
-Requires: numba (==0.57.1)
-Requires: numpy (==1.24.4)
-Requires: ome_types (==0.4.3)
-Requires: opencv_python (==4.5.3)
-Requires: pandas (==1.3.3)
-Requires: pyflakes (==2.4.0)
-Requires: PyQt5 (==5.15.10)
-Requires: PyQt5_sip (==12.11.1)
-Requires: pyqtgraph (==0.13.3)
-Requires: pyserial (==3.5)
-Requires: pyueye (==4.96.952)
-Requires: QDarkStyle (==3.1)
-Requires: QScintilla (==2.13.4)
-Requires: scikit_image (==0.18.3)
-Requires: scikit_learn (==1.1.3)
-Requires: scipy (==1.11.4)
-Requires: setuptools (==69.0.2)
-Requires: tables (==3.9.1)
-Requires: tifffile (==2022.2.2)
-Requires: zarr (==2.10.3)
-Requires-Python: >=3.9.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# The microEye
 
-# microEye
-
-**microEye** is a python toolkit for fluorescence microscopy that features hardware control, data analysis and vizualization for super-resolution single-molecule localization microscopy and single-partical tracking.
-
-## Modules
-
-- **miEye Module:** Provides the primary GUI for microscope control and data acquisition, combining previous functionalities implemented within *Acquisition* and *Control* modules.
-
-- **Multi Viewer Module:** An improved GUI replacing *Tiff Viewer* module that allows processing multiple files providing data analysis and visualization tools.
-
-**Note: The following modules are deprecated, and support has been halted. Please consider the alternatives above.**
-
-- **Acquisition Module:** Enables multi-camera image acquisition within a unified graphical user interface.
-
-- **Control Module:** Allows users to set laser excitation presets, manually focus, and perform automatic focus stabilization by monitoring the peak position of a totally internally reflected IR beam and adjusting the piezo stage accordingly.
-
-- **Tiff Viewer Module:** Provides access to TIFF images (single files and sequences) of order TYX (2D SMLM) and facilitates visualizing the filtering-localization process (*WYSIWYG*).
+The **`microEye`** is a Python toolkit for fluorescence microscopy that supports super-resolution single-molecule localization microscopy and single-particle tracking. It features hardware control, data analysis, and visualization.
 
 This toolkit is compatible with the [hardware](#hardware) used in our microscope. For further details, refer to the [miEye microscope paper](https://doi.org/10.1016/j.ohx.2022.e00368) and [OSF project](http://doi.org/10.17605/osf.io/j2fqy).
 
-## Uses Packages
-
-- autopep8
-- dask
-- h5py
-- hidapi
-- matplotlib
-- numba
-- numpy
-- ome_types
-- opencv_python
-- pandas
-- pyflakes
-- PyQt5
-- PyQt5_sip
-- pyqtgraph
-- pyserial
-- pyueye
-- QDarkStyle
-- QScintilla
-- scikit_image
-- scikit_learn
-- scipy
-- setuptools
-- tables
-- tifffile
-- VimbaPython (Included in [Vimba SDK](https://www.alliedvision.com/en/products/vimba-sdk/) and installed manually)
-- zarr
-
-## How to Install [Package](https://pypi.org/project/microEye/)
-
-1. Download and install the latest [*Python*](https://www.python.org/downloads/) 3.9 stable release.
-
-2. Open a terminal and install the [*microEye*](https://pypi.org/project/microEye/) package using *pip*.
-
-    ```bash
-    pip install microEye
-    ```
-
-3. Download the [requirements.txt](https://github.com/samhitech/microEye/blob/main/requirements.txt) file and install the required packages for *microEye* by executing: (This may take a while)
-
-    ```bash
-    pip install -r /path/to/requirements.txt
-    ```
-
-4. Install the specific hardware drivers for the cameras:
-
-   - **Integrated Optics** [Laser control software](https://integratedoptics.com/downloads).
-
-   - **IDS uEye CMOS cameras:** Install [IDS Software Suite 4.96.1](https://en.ids-imaging.com/download-details/AB00604.html?os=windows&version=win10&bus=64&floatcalc=) for Windows 32/64-bit.
-
-   - **Allied Vision CMOS cameras:** Install [Vimba SDK](https://www.alliedvision.com/en/products/vimba-sdk) 5.0 or 6.0 outside the Program Files to skip the run-as-admin requirement. In a terminal navigate to directory [*.../Allied Vision/Vimba_5.0/VimbaPython/*] where [*setup.py*] is located and execute:
-
-        ```bash
-        python -m pip install .
-        ```
-
-   - **Thorlabs CMOS cameras:** Install [Thorcam](https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ThorCam) in its default directory. Note, some *Thorlabs* cameras can get identified by *Windows* as *IDS uEye* cameras and run without this software.
-
-5. Other hardware used by the miEye microscope:
-
-   - Thorlabs [Kinesis® Software](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=10285) and [Elliptec™ Software](https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ELL).
-
-6. Download and run examples to start using microEye! :partying_face:
-
-**Note:** *microEye* might not function as expected in case drivers are missing.
-
-## Microscope Scheme
-
-Schematic overview of the miEye instrument. A) The excitation path via single-mode fiber (SMF) for TIRF-, HILO-, and Epi-mode. B) The excitation path via multi-mode fiber (MMF) for Epi-mode when imaging MMF output on the sample plane. C) The fluorescence emission path. D) IR laser-based autofocusing path. AC: achromat lens, AS: aspheric lens, BFP: back-focal plane, TL: tube lens, B: B-coated N-BK7 optics, BS: beamsplitter.
-
-| Scheme 1 | Scheme 2 |
-|----------| ---------|
-| ![quadScheme_4](https://user-images.githubusercontent.com/89871015/182302644-9fdf8615-75c3-4702-9913-d1a535f60e22.png) | ![scheme_git_0](https://user-images.githubusercontent.com/89871015/182302694-3f70d058-b1b6-4ef5-9cc2-aec9b58a05f0.png)|
-
-## Hardware
-
-### Supported Cameras
-
-- IDS uEye industrial-grade CMOS cameras, specifically [UI-3060CP Rev. 2](https://en.ids-imaging.com/store/products/cameras/ui-3060cp-rev-2.html).
-
-- Thorlabs DCx cameras using the UC480 driver, specifically [DCC1545M](https://www.thorlabs.com/thorProduct.cfm?partNumber=DCC1545M).
-
-- Allied Vision cameras using Vimba SDK, specifically [Alvium 1800 U-158m](https://www.alliedvision.com/en/products/alvium-configurator/alvium-1800-u/158/#_configurator).
-
-### Additional Hardware
-
-- Integrated Optics Multi-wavelength Laser Combiner [MatchBox](https://integratedoptics.com/products/wavelength-combiners).
-
-- Piezo Concept nanopositioner for microscope objectives [FOC](https://piezoconcept-store.squarespace.com/1-axis/p/foc).
-
-- Thorlab's Elliptec Dual-Position/Four-Position ([ELL6](https://www.thorlabs.com/thorproduct.cfm?partnumber=ELL6)/[ELL9](https://www.thorlabs.com/thorproduct.cfm?partnumber=ELL9)) support.
-
-- Thorlab's Kinesis [KDC101](https://www.thorlabs.com/thorproduct.cfm?partnumber=KDC101) controller for [Z825B](https://www.thorlabs.com/thorproduct.cfm?partnumber=Z825B) 25mm motorized actuators used for the XY stage instead of manual micrometers. (Requires activating USB VCP to access the COM port from device manager)
-
-- Parallax Linescan Camera Module used for IR autofocus stabilization tracking [TSL1401-DB (#28317)](https://eu.mouser.com/ProductDetail/Parallax/28317?qs=%2Fha2pyFaduiCRhuOAXMuCmQIeG1Q3R01m6Y1EH%252BmN80%3D) acquisition done by an Arduino [LineScanner](https://github.com/samhitech/LineScanner).
+![Package Health](https://snyk.io/advisor/python/microEye/badge.svg)
+![Python Version](https://img.shields.io/badge/Python-version_3.9-blue)
+![Package Version](https://img.shields.io/badge/version-2.0.0-gold)
+![Package Version](https://img.shields.io/badge/GUI_Platform-PyQt5-navy)
+![Package Version](https://img.shields.io/badge/OS-Windows-cyan)
+[![DOI](https://img.shields.io/badge/HardwareX-10.1016/j.ohx.2022.e00368-orange)](https://doi.org/10.1016/j.ohx.2022.e00368)
+
+```bash
+   __  ____              ____                ___   ___   ___ 
+  /  |/  (_)__________  / __/_ _____   _  __|_  | / _ \ / _ \
+ / /|_/ / / __/ __/ _ \/ _// // / -_) | |/ / __/_/ // // // /
+/_/  /_/_/\__/_/  \___/___/\_, /\__/  |___/____(_)___(_)___/ 
+                          /___/
+```
 
-- [RelayBox](https://github.com/samhitech/RelayBox) Arduino for laser control using the camera flash signal with different presets.
+## Modules
 
-- Parts list of our [miEye OSF Project](https://osf.io/j2fqy/) – an iteration of [hohlbeinlab miCube](https://hohlbeinlab.github.io/miCube/index.html).
+### The miEye Module
 
-## miEye Module
+The `miEye_module` provides the primary graphical user interface (GUI) for microscope control and data acquisition, combining the functionalities of the deprecated *Acquisition* and *Control* modules.
 
 | miEye module | Acquisition Camera |
 |----------------|----------------|
-| ![miEye](https://github.com/samhitech/microEye/assets/89871015/73211153-6811-4acc-816f-154b1a2c5a32) | ![Cam_acq](https://github.com/samhitech/microEye/assets/89871015/a114fde6-a847-4be5-ab10-95f82190c830) |
+| ![miEye](https://github.com/samhitech/microEye/assets/89871015/20c5573a-e489-478e-adfc-29410bc6d4c2) | ![CamStack](https://github.com/samhitech/microEye/assets/89871015/ead95989-54ce-4643-b5a3-4461c36f6b14) |
 
-### How to use
+**How to use:**
 
 For Vimba SDK to work, the script should be executed as an administrator on Windows and wrapped in a `with` statement:
 
 ```python
 from microEye.hardware import miEye_module
 
 try:
@@ -183,79 +46,130 @@
         app, window = miEye_module.StartGUI()
         app.exec_()
 else:
     app, window = miEye_module.StartGUI()
     app.exec_()
 ```
 
-## Multi Viewer Module
+### The Multi Viewer Module
+
+The `multi_viewer` Module is an improved GUI that replaces the deprecated `tiff_viewer` module. It allows users to process multiple files and provides data analysis and visualization tools for super-resolution single-molecule localization microscopy and single-particle tracking.
 
 | Raw Data | Localizations |
 |----------------|----------------|
-| ![Stack_images](https://github.com/samhitech/microEye/assets/89871015/07479e66-77c6-4d2d-b47f-ade89239dc49) | ![Stack_loc](https://github.com/samhitech/microEye/assets/89871015/beb0981d-a6d9-46d8-ae1c-e0d267f1d10e) |
+| ![imagesStack](https://github.com/samhitech/microEye/assets/89871015/17421117-a633-4a20-ba38-e7adffcd7332) | ![locStack](https://github.com/samhitech/microEye/assets/89871015/713d9fc7-7f92-4341-adb2-17b83ac8fc34) |
 
-### How to use
+**How to use:**
 
 ```python
 from microEye import multi_viewer
 
 app, window = multi_viewer.StartGUI('')
 
 app.exec_()
 ```
 
-## Acquisition Module (Deprecated)
+## Uses Packages
 
-### How to use
+The `microEye` uses the following Python packages:
 
-For Vimba SDK to work, the script should be executed as an administrator on Windows and wrapped in a `with` statement:
+| Data Analysis and Visualization | GUI and UI Development | Code Quality and Formatting | Image and Video Processing | File and Data Storage | Other Utilities |
+|--------------------------------|------------------------|------------------------------|---------------------------|-----------------------|-----------------|
+| dask                           | PyQt5                  | autopep8                     | opencv-python | ome-types             | hidapi          |
+| h5py                           | pyqtdarktheme          | pyflakes                    |                           | tables                | pyfiglet        |
+| matplotlib                     | pyqtgraph              |                              |              | zarr                  | pyserial        |
+| numba                          | QDarkStyle             |                              |                           |                       | pyueye          |
+| numpy                          | QScintilla             |                              |                           |                       | setuptools      |
+| pandas                         |                        |                              |                           |                       | tabulate        |
+| scikit-image                   |                        |                              |                           |                       | VimbaPython     |
+| scikit-learn                   |                        |                              |                           |                       |                 |
+| scipy                          |                        |                              |                           |                       |                 |
+| tifffile                       |                        |                              |                           |                       |                 |
+| vispy                          |                        |                              |                           |                       |                 |
 
-```python
-from microEye.hardware import acquisition_module
+Note: VimbaPython is included in Vimba SDK and needs to be installed manually.
 
-try:
-    import vimba as vb
-except Exception:
-    vb = None
+## How to Install [microEye](https://pypi.org/project/microEye/)
 
-if vb:
-    with vb.Vimba.get_instance() as vimba:
-        app, window = acquisition_module.StartGUI()
-        app.exec_()
-else:
-    app, window = acquisition_module.StartGUI()
-    app.exec_()
-```
+1. **Install Python:**
 
-## Control Module (Deprecated)
+   Download and install the latest [Python 3.9 stable release](https://www.python.org/downloads/).
 
-### How to use
+2. **Install microEye package:**
 
-```python
-from microEye.hardware import control_module
+   Open a terminal and execute the following command to install microEye using pip:
 
-app, window = control_module.StartGUI()
-app.exec_()
-```
+    ```powershell
+    pip install microEye
+    ```
+
+3. **Install required packages:**
 
-## Tiff Viewer Module (Deprecated)
+   Download the [requirements.txt](https://github.com/samhitech/microEye/blob/main/requirements.txt) file. Navigate to the directory containing the requirements file in your terminal and run:
 
-| File System | Data Fitting | Localizations Visualization & Analysis |
-| --------------- | ----------------- | ----------------- |
-| ![Capture Viewer](https://user-images.githubusercontent.com/89871015/150964047-ba4521fa-1ffa-4f76-9e4e-6759fbdc3b8f.PNG) | ![Capture Viewer 2](https://user-images.githubusercontent.com/89871015/150964062-9560b228-5052-40cb-86fc-5617f760a1b1.PNG) | ![Capture Viewer 3](https://user-images.githubusercontent.com/89871015/151448086-0799926d-a4a4-420b-ad12-177145a90c78.png) |
+    ```powershell
+    pip install -r requirements.txt
+    ```
 
-### How to use
+   Note: This step might take a while.
 
-```python
-from microEye import tiff_viewer
+4. **Install specific hardware drivers: (Optional)**
+   - For Integrated Optics: Download and install [Laser control software](https://integratedoptics.com/downloads).
+   - For IDS uEye CMOS cameras: Install [IDS Software Suite 4.96.1](https://en.ids-imaging.com/download-details/AB00604.html?os=windows&version=win10&bus=64&floatcalc=) for Windows 32/64-bit.
+   - For Allied Vision CMOS cameras: Install [Vimba SDK](https://www.alliedvision.com/en/products/vimba-sdk) 5.0 or 6.0 outside the Program Files. Navigate to the directory containing setup.py and run:
 
-app, window = tiff_viewer.StartGUI('')
+        ```powershell
+        python -m pip install .
+        ```
 
-app.exec_()
-```
+   - For Thorlabs CMOS cameras: Install [Thorcam](https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ThorCam) in its default directory. Note: Some Thorlabs cameras may be identified as IDS uEye cameras by Windows and may run without Thorcam.
+
+   - For Thorlabs hardware, install [Kinesis® Software](https://www.thorlabs.com/newgrouppage9.cfm?objectgroup_id=10285) and [Elliptec™ Software](https://www.thorlabs.com/software_pages/ViewSoftwarePage.cfm?Code=ELL).
+
+5. **Download and run examples:**
+   Download examples to start using microEye!
+
+:partying_face: **Note:** Ensure all necessary drivers are installed for microEye to function properly.
+
+## Microscope Scheme
+
+Schematic overview of the miEye instrument:
+
+- **A) Single-Mode Fiber (SMF):** Excitation path for TIRF-, HILO-, and Epi-mode.
+- **B) Multi-Mode Fiber (MMF):** Excitation path for Epi-mode when imaging MMF output on the sample plane.
+- **C) Fluorescence Emission:** Path for fluorescence emission.
+- **D) Automatic Focus Stabilization:** the automatic focus stabilization path using an IR laser in TIRF setting.
+
+| Scheme 1 | Scheme 2 |
+|----------|---------|
+| ![Quad Scheme](https://user-images.githubusercontent.com/89871015/182302644-9fdf8615-75c3-4702-9913-d1a535f60e22.png) | ![Scheme GIT](https://user-images.githubusercontent.com/89871015/182302694-3f70d058-b1b6-4ef5-9cc2-aec9b58a05f0.png) |
+
+**Key Components:** *AC:* Achromat lens, *AS:* Aspheric lens, *BFP:* Back-focal plane, *TL:* Tube lens, *B:* B-coated N-BK7 optics, *BS:* Beamsplitter.
+
+## Hardware
+
+### Supported Cameras
+
+| Camera | Description | Link |
+|--------|-------------|------|
+| IDS uEye UI-3060CP Rev. 2 | IDS industrial-grade CMOS cameras | [Link](https://en.ids-imaging.com/store/products/cameras/ui-3060cp-rev-2.html) |
+| Thorlabs DCC1545M | DCx camera using UC480 driver | [Link](https://www.thorlabs.com/thorProduct.cfm?partNumber=DCC1545M) |
+| Allied Vision Alvium 1800 | Allied Vision industrial-grade CMOS cameras (U-158m, U-511m)  | [Link](https://www.alliedvision.com/en/products/alvium-configurator/alvium-1800-u/158/#_configurator) |
+
+### Additional Hardware
+
+| Hardware | Description | Link |
+|----------|-------------|------|
+| Integrated Optics MatchBox | Multi-wavelength Laser Combiner, Single Laser MatchBox | [Link](https://integratedoptics.com/products/wavelength-combiners) |
+| Piezo Concept FOC | Nanopositioner for microscope objectives | [Link](https://piezoconcept-store.squarespace.com/1-axis/p/foc) |
+| Thorlabs Elliptec ELL6/ELL9 | Dual/Four-Position Support | [ELL6](https://www.thorlabs.com/thorproduct.cfm?partnumber=ELL6), [ELL9](https://www.thorlabs.com/thorproduct.cfm?partnumber=ELL9) |
+| Thorlabs KDC101 | Kinesis Controller for Z825B/[Z925B](https://www.thorlabs.com/thorproduct.cfm?partnumber=Z925B) actuators (Activate USB VCP to access the COM port in device manager) | [Link](https://www.thorlabs.com/thorproduct.cfm?partnumber=KDC101) |
+| Parallax TSL1401-DB (#28317) | Linescan Camera Module | [Link](https://eu.mouser.com/ProductDetail/Parallax/28317?qs=%2Fha2pyFaduiCRhuOAXMuCmQIeG1Q3R01m6Y1EH%252BmN80%3D) |
+| RelayBox Arduino | For laser control using camera GPIO signals | [RelayBox](https://github.com/samhitech/RelayBox) |
+| miEye OSF Project Parts List | Parts list of miEye OSF Project | [Link](https://osf.io/j2fqy/) |
 
 ## Authors
 
 [Mohammad Nour Alsamsam](https://tutkuslab.github.io/team/MNA/), PhD student @ Vilnius University.
 
 [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/samhightech.svg?style=social&label=Follow%20%40samhightech)](https://twitter.com/samhightech)
```

### Comparing `microEye-1.0.5/pyproject.toml` & `microEye-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/setup.py` & `microEye-2.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 import setuptools
 
 with open('README.md', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='microEye',
-    version='1.0.5',
+    version='2.0.0',
     author='Mohammad Nour Alsamsam',
     author_email='nour.alsamsam@gmail.com',
     description='A python toolkit for fluorescence microscopy \
         that features hardware control, data analysis and vizualization \
         for super-resolution single-molecule localization microscopy and \
         single-partical tracking.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/samhitech/microEye',
     project_urls={
         'miEye Paper': 'https://doi.org/10.1016/j.ohx.2022.e00368',
-        'miEye OSF': 'http://doi.org/10.17605/osf.io/j2fqy'},
+        'miEye OSF': 'http://doi.org/10.17605/osf.io/j2fqy',
+    },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     python_requires='>=3.9.4',
     include_package_data=True,
-    requires = [
+    install_requires=[
         'autopep8 (==2.0.4)',
         'dask (==2022.1.0)',
         'h5py (==3.10.0)',
         'hidapi (==0.14.0)',
         'matplotlib (==3.6.3)',
         'numba (==0.57.1)',
         'numpy (==1.24.4)',
-        'ome_types (==0.4.3)',
-        'opencv_python (==4.5.3)',
+        'ome-types (==0.5.1)',
+        'opencv-python (==4.9.0.80)',
         'pandas (==1.3.3)',
+        'pyfiglet (==1.0.2)',
         'pyflakes (==2.4.0)',
         'PyQt5 (==5.15.10)',
-        'PyQt5_sip (==12.11.1)',
+        'pyqtdarktheme (==2.1.0)',
         'pyqtgraph (==0.13.3)',
         'pyserial (==3.5)',
         'pyueye (==4.96.952)',
-        'QDarkStyle (==3.1)',
+        'QDarkStyle (==3.2.3)',
         'QScintilla (==2.13.4)',
-        'scikit_image (==0.18.3)',
-        'scikit_learn (==1.1.3)',
-        'scipy (==1.11.4)',
+        'scikit-image (==0.18.3)',
+        'scikit-learn (==1.1.3)',
+        'scipy (==1.12.0)',
         'setuptools (==69.0.2)',
         'tables (==3.9.1)',
+        'tabulate (==0.9.0)',
         'tifffile (==2022.2.2)',
+        'vispy (==0.14.1)',
         'zarr (==2.10.3)',
-    ]
+    ],
 )
```

### Comparing `microEye-1.0.5/src/microEye/analysis/checklist_dialog.py` & `microEye-2.0.0/src/microEye/analysis/checklist_dialog.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/cmosMaps.py` & `microEye-2.0.0/src/microEye/analysis/cmosMaps.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/file_sys.py` & `microEye-2.0.0/src/microEye/analysis/file_sys.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import tifffile as tf
 from numba import cuda
 from ome_types.model import OME
 from PyQt5.QtCore import *
 from PyQt5.QtGui import QIcon
 from PyQt5.QtWidgets import *
 
+from ..shared import start_gui
+
 if cuda.is_available():
     from .fitting.pyfit3Dcspline.mainfunctions import GPUmleFit_LM
 else:
     def GPUmleFit_LM(*args):
         pass
 
 from ..shared.gui_helper import *
@@ -50,15 +52,15 @@
     CMOS_MAPS = 'CMOS Maps'
     DATA_FILTERS = 'Data Filters'
     METADATA = 'Metadata'
 
 
 class tiff_viewer(QMainWindow):
 
-    def __init__(self, threadpool, path=None):
+    def __init__(self, path=None):
         super().__init__()
         # Set window properties
         self.title = 'microEye tiff viewer'
         self.left = 0
         self.top = 0
         self._width = 1300
         self._height = 650
@@ -68,15 +70,15 @@
         # Initialize variables
         self.fittingResults = None
         self.tiff = None
         self.tiffSequence = None
         self.stack_handler = None
 
         # Threading
-        self._threadpool = threadpool
+        self._threadpool = QThreadPool.globalInstance()
         print('Multithreading with maximum %d threads'
               % self._threadpool.maxThreadCount())
 
         # Set the path
         if path is None:
             path = os.path.dirname(os.path.abspath(__package__))
         self.initialize(path)
@@ -386,16 +388,15 @@
 
     def setupImageToolsTab(self):
         # Creating the Image Stack Processing Tools tab layout
         self.image_tools_layout = self.create_tab(
             DockKeys.IMAGE_TOOLS, QVBoxLayout,
             'LeftDockWidgetArea', widget=None)
 
-        self.kymogram_widget = KymogramWidget(
-            self._threadpool)
+        self.kymogram_widget = KymogramWidget()
 
         self.kymogram_widget.displayClicked.connect(self.kymogram_display_clicked)
         self.kymogram_widget.extractClicked.connect(self.kymogram_btn_clicked)
 
         self.image_tools_layout.addWidget(self.kymogram_widget)
 
     def setupLocalizationTab(self):
@@ -1921,48 +1922,15 @@
             The path to a file to be loaded initially.
 
         Returns
         -------
         tuple of QApplication and tiff_viewer
             Returns a tuple with QApplication and tiff_viewer main window.
         '''
-        # Create a QApplication
-        app = QApplication(sys.argv)
-
-        thread_pool = QThreadPool()
-
-        # Set dark mode from qdarkstyle (not compatible with PyQt6)
-        app.setStyleSheet(qdarkstyle.load_stylesheet(qt_api='pyqt5'))
-
-        # Set the font size for the application
-        font = app.font()
-        font.setPointSize(10)
-        app.setFont(font)
-
-        # Set the app icon
-        dirname = os.path.dirname(os.path.abspath(__file__))
-        app_icon = QIcon()
-        icon_sizes = [16, 24, 32, 48, 64, 128, 256, 512]
-
-        for size in icon_sizes:
-            icon_path = os.path.join(dirname, f'../icons/{size}.png')
-            app_icon.addFile(icon_path, QSize(size, size))
-
-        app.setWindowIcon(app_icon)
-
-        # Set the app user model ID for Windows
-        if sys.platform.startswith('win'):
-            import ctypes
-            my_app_id = 'samhitech.mircoEye.tiff_viewer'  # App ID
-            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(my_app_id)
-
-        # Create the tiff_viewer window
-        window = tiff_viewer(thread_pool, path)
-
-        return app, window
+        return start_gui(tiff_viewer, path)
 
 
 def get_dock_config(dock: QDockWidget):
     '''
     Get the configuration dictionary for a QDockWidget.
 
     Parameters
```

### Comparing `microEye-1.0.5/src/microEye/analysis/filters.py` & `microEye-2.0.0/src/microEye/analysis/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,17 +65,31 @@
 
     def gaussian_kernel(dim, sigma):
         x = cv2.getGaussianKernel(dim, sigma)
         kernel = x.dot(x.T)
         return kernel
 
     def run(self, image: np.ndarray) -> np.ndarray:
-        return cv2.normalize(
-            signal.convolve2d(image, np.rot90(self.dog), mode='same'),
+        rows, cols = image.shape
+        nrows = cv2.getOptimalDFTSize(rows)
+        ncols = cv2.getOptimalDFTSize(cols)
+        pad_rows = nrows - rows
+        pad_cols = ncols - cols
+
+        # Ensure that pad_cols[1] and pad_rows[1] are at least 1
+        pad_rows = (pad_rows // 2, max(1, pad_rows - pad_rows // 2))
+        pad_cols = (pad_cols // 2, max(1, pad_cols - pad_cols // 2))
+
+        nimg = np.pad(image, (pad_rows, pad_cols), mode='reflect')
+
+        res = cv2.normalize(
+            signal.convolve2d(nimg, np.rot90(self.dog), mode='same')[
+                pad_rows[0]:-pad_rows[1], pad_cols[0]:-pad_cols[1]],
             None, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U)
+        return res
 
     def get_metadata(self):
         '''Return metadata about the Difference of Gaussians filter.'''
         return {
             'name': 'Difference of Gaussains Filter',
             'sigma': self.sigma,
             'factor': self.factor
@@ -318,33 +332,41 @@
         '''
 
         # time = QDateTime.currentDateTime()
 
         rows, cols = image.shape
         nrows = cv2.getOptimalDFTSize(rows)
         ncols = cv2.getOptimalDFTSize(cols)
-        nimg = np.zeros((nrows, ncols))
-        nimg[:rows, :cols] = image
+        pad_rows = nrows - rows
+        pad_cols = ncols - cols
+
+        # Ensure that pad_cols[1] and pad_rows[1] are at least 1
+        pad_rows = (pad_rows // 2, max(1, pad_rows - pad_rows // 2))
+        pad_cols = (pad_cols // 2, max(1, pad_cols - pad_cols // 2))
+
+        nimg = np.pad(image, (pad_rows, pad_cols), mode='reflect')
+        # nimg = np.zeros((nrows, ncols))
+        # nimg[:rows, :cols] = image
 
         ft = fftshift(cv2.dft(np.float64(nimg), flags=cv2.DFT_COMPLEX_OUTPUT))
 
         filter = np.ones(ft.shape[:2])
 
         refresh = self._refresh
 
         if self._filter is None:
             refresh = True
         elif self._filter.shape != ft.shape[:2]:
             refresh = True
 
         if refresh:
-            if self._type == BANDPASS_TYPES.Gaussian:
+            if self._type == BANDPASS_TYPES.Gaussian.name:
                 filter = self.gauss_bandpass_filter(
                     ft.shape, self._center, self._width)
-            elif self._type == BANDPASS_TYPES.Butterworth:
+            elif self._type == BANDPASS_TYPES.Butterworth.name:
                 filter = self.butterworth_bandpass_filter(
                     ft.shape, self._center, self._width)
             else:
                 cutoff = int(max(0, self._center - self._width // 2))
                 cuton = int(self._center + self._width // 2)
                 filter = self.ideal_bandpass_filter(ft.shape, cutoff, cuton)
 
@@ -361,15 +383,17 @@
         ft[:, :, 1] *= filter
         idft = cv2.idft(ifftshift(ft))
         idft = cv2.magnitude(idft[:, :, 0], idft[:, :, 1])
         cv2.normalize(
             idft, img, 0, 255, cv2.NORM_MINMAX, cv2.CV_8U)
 
         # exex = time.msecsTo(QDateTime.currentDateTime())
-        return img[:rows, :cols]
+        return img[
+            pad_rows[0]:-pad_rows[1],
+            pad_cols[0]:-pad_cols[1]]
 
     def set_params(
             self,
             center: float, width: float,
             filter_type: BANDPASS_TYPES, show: bool):
         self._center = center
         self._width = width
```

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/fit.py` & `microEye-2.0.0/src/microEye/analysis/fitting/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     if params is None:
         # Setup SimpleBlobDetector parameters.
         params = cv2.SimpleBlobDetector_Params()
 
         params.filterByColor = True
         params.blobColor = 255
 
-        params.minDistBetweenBlobs = 0
+        params.minDistBetweenBlobs = 1
 
         # Change thresholds
         # params.minThreshold = 0
         # params.maxThreshold = 255
 
         # Filter by Area.
         params.filterByArea = True
@@ -78,15 +78,15 @@
         self.set_blob_detector_params(**kwargs)
 
     def set_blob_detector_params(
             self, min_threshold=0, max_threshold=255,
             minArea=1.5, maxArea=80,
             minCircularity=None, minConvexity=None,
             minInertiaRatio=None, blobColor=255,
-            minDistBetweenBlobs=0) -> cv2.SimpleBlobDetector_Params:
+            minDistBetweenBlobs=1) -> cv2.SimpleBlobDetector_Params:
         '''
         Set parameters for the blob detector.
 
         Parameters
         ----------
         min_threshold : float, optional
             Minimum threshold for blob detection (default: 0).
@@ -126,31 +126,31 @@
         self.params.filterByArea = True
         self.params.minArea = minArea
         self.params.maxArea = maxArea
 
         # Filter by Circularity
         if minCircularity is None:
             self.params.filterByCircularity = False
-            self.params.minCircularity = 0
+            # self.params.minCircularity = 0
         else:
             self.params.filterByCircularity = True
             self.params.minCircularity = minCircularity
 
         # Filter by Convexity
         if minConvexity is None:
             self.params.filterByConvexity = False
-            self.params.minConvexity = 0
+            # self.params.minConvexity = 0
         else:
             self.params.filterByConvexity = True
             self.params.minConvexity = minConvexity
 
         # Filter by Inertia
         if minInertiaRatio is None:
             self.params.filterByInertia = False
-            self.params.minInertiaRatio = 0
+            # self.params.minInertiaRatio = 0
         else:
             self.params.filterByInertia = True
             self.params.minInertiaRatio = minInertiaRatio
 
         self.detector = get_blob_detector(self.params)
 
     def find_peaks(self, img: np.ndarray):
```

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/nena.py` & `microEye-2.0.0/src/microEye/analysis/fitting/nena.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/phasor_fit.py` & `microEye-2.0.0/src/microEye/analysis/fitting/phasor_fit.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/processing.py` & `microEye-2.0.0/src/microEye/analysis/fitting/processing.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUfunctions.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUfunctions.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUmleFit_LM.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUmleFit_LM.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUsplineLib.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/CPU/CPUsplineLib.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUfunctions.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUfunctions.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_EMCCD.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_EMCCD.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_sCMOS.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUmleFit_LM_sCMOS.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUsplineLib.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/GPU/GPUsplineLib.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/constants.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/constants.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/pyfit3Dcspline/mainfunctions.py` & `microEye-2.0.0/src/microEye/analysis/fitting/pyfit3Dcspline/mainfunctions.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/results.py` & `microEye-2.0.0/src/microEye/analysis/fitting/results.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/results_stats.py` & `microEye-2.0.0/src/microEye/analysis/fitting/results_stats.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/fitting/tardis.py` & `microEye-2.0.0/src/microEye/analysis/fitting/tardis.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/multi_viewer.py` & `microEye-2.0.0/src/microEye/analysis/multi_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import cv2
 import qdarkstyle
 from PyQt5.QtCore import *
 from PyQt5.QtGui import QIcon
 from PyQt5.QtWidgets import *
 
+from ..shared import StartGUI
 from ..shared.gui_helper import *
 from ..shared.thread_worker import *
 from ..shared.uImage import *
 from .fitting.results import FittingResults
 from .viewer.images import StackView
 from .viewer.localizations import LocalizationsView
 
@@ -23,30 +24,30 @@
     FILE_SYSTEM = 'File System'
     SMLM_ANALYSIS = 'SMLM Analysis'
     DATA_FILTERS = 'Data Filters'
 
 
 class multi_viewer(QMainWindow):
 
-    def __init__(self, threadpool, path=None):
+    def __init__(self, path=None):
         super().__init__()
         # Set window properties
         self.title = 'microEye tiff viewer'
         self.left = 0
         self.top = 0
         self._width = 1600
         self._height = 950
         self._zoom = 1
         self._n_levels = 4096
 
         # Initialize variables
         self.fittingResults = None
 
         # Threading
-        self._threadpool = threadpool
+        self._threadpool = QThreadPool.globalInstance()
         print('Multithreading with maximum %d threads'
               % self._threadpool.maxThreadCount())
 
         # Set the path
         if path is None:
             path = os.path.dirname(os.path.abspath(__package__))
         self.initialize(path)
@@ -278,31 +279,32 @@
 
         if not self.model.isDir(i):
             cv2.destroyAllWindows()
             index = self.model.index(i.row(), 0, i.parent())
             path = self.model.filePath(index)
 
             if path.endswith('.tif') or path.endswith('.tiff'):
-                view = StackView.FromImageSequence(path, None, self._threadpool)
+                view = StackView.FromImageSequence(path, None)
                 view.localizedData.connect(self.localizedData)
             elif path.endswith('.h5') or path.endswith('.tsv'):
                 results = FittingResults.fromFile(path, 1)
                 if results is not None:
-                    view = LocalizationsView(path, results, self._threadpool)
+                    view = LocalizationsView(path, results)
                     print('Done importing results.')
                 else:
                     print('Error importing results.')
         else:
             index = self.model.index(i.row(), 0, i.parent())
             path = self.model.filePath(index)
 
             if path.endswith('.zarr'):
-                view = StackView.FromZarr(path, self._threadpool)
+                view = StackView.FromZarr(path)
             else:
-                view = StackView.FromImageSequence(path, None, self._threadpool)
+                view = StackView.FromImageSequence(
+                    path, self.imsq_pattern.text())
 
             view.localizedData.connect(self.localizedData)
 
         if view:
             window = self.mdi_area.addSubWindow(view, Qt.SubWindow)
             window.show()
 
@@ -320,48 +322,15 @@
             The path to a file to be loaded initially.
 
         Returns
         -------
         tuple of QApplication and multi_viewer
             Returns a tuple with QApplication and multi_viewer main window.
         '''
-        # Create a QApplication
-        app = QApplication(sys.argv)
-
-        thread_pool = QThreadPool()
-
-        # Set dark mode from qdarkstyle (not compatible with PyQt6)
-        app.setStyleSheet(qdarkstyle.load_stylesheet(qt_api='pyqt5'))
-
-        # Set the font size for the application
-        font = app.font()
-        font.setPointSize(10)
-        app.setFont(font)
-
-        # Set the app icon
-        dirname = os.path.dirname(os.path.abspath(__file__))
-        app_icon = QIcon()
-        icon_sizes = [16, 24, 32, 48, 64, 128, 256, 512]
-
-        for size in icon_sizes:
-            icon_path = os.path.join(dirname, f'../icons/{size}.png')
-            app_icon.addFile(icon_path, QSize(size, size))
-
-        app.setWindowIcon(app_icon)
-
-        # Set the app user model ID for Windows
-        if sys.platform.startswith('win'):
-            import ctypes
-            my_app_id = 'samhitech.mircoEye.multi_viewer'  # App ID
-            ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(my_app_id)
-
-        # Create the multi_viewer window
-        window = multi_viewer(thread_pool, path)
-
-        return app, window
+        return StartGUI(multi_viewer, path)
 
 def get_dock_config(dock: QDockWidget):
     '''
     Get the configuration dictionary for a QDockWidget.
 
     Parameters
     ----------
```

### Comparing `microEye-1.0.5/src/microEye/analysis/rendering.py` & `microEye-2.0.0/src/microEye/analysis/rendering.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/tools/kymograms.py` & `microEye-2.0.0/src/microEye/analysis/tools/kymograms.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                     1,
                     cv2.LINE_AA
                 )
 
         cv2.imshow('Select Line ROIs', self.resized_image)
         cv2.setWindowTitle(
             'Select Line ROIs',
-            f'Select Line ROIs \"Mode: {self.current_mode}\"' + \
+            f'Select Line ROIs "Mode: {self.current_mode}"' + \
                 ' (Space: change mode | Q: quit)')
 
     def mouse_callback(self, event, x, y, flags, param):
         '''
         Mouse callback function for handling mouse events.
 
         Parameters
@@ -464,14 +464,16 @@
         dy = dY[idx]
 
         temp = np.zeros(n_points[idx])
         for move_line in move_lines:
             x_idx = np.round(x + move_line * dx).astype(np.int64)
             y_idx = np.round(y + move_line * dy).astype(np.int64)
             with nb.objmode():
+                np.clip(x_idx, 0, Data.shape[1]-1, x_idx)
+                np.clip(y_idx, 0, Data.shape[0]-1, y_idx)
                 if method == 'maximum':
                     temp[:] = np.maximum(temp, Data[y_idx, x_idx])
                 else:
                     temp[:] = temp + Data[y_idx, x_idx]
         if method == 'average' and linewidth > 1:
             Roi[lut[idx]:lut[idx+1]] = temp / len(move_lines)
         else:
@@ -669,17 +671,17 @@
         '<b>I:</b> Insert at segment',
         '<b>R:</b> Remove points',
         '<b>C:</b> Clear all ROIs',
         '<b>Delete:</b> Delete the last added point',
         '<b>Up/Down Arrows:</b> Select active ROI.'
     ]
 
-    def __init__(self, threadpool: QThreadPool, parent=None):
+    def __init__(self, parent=None):
         super().__init__(parent)
-        self._threadpool = threadpool
+        self._threadpool = QThreadPool.globalInstance()
 
         self.kymogram_temporal_window = create_spin_box(0, 100, 1, 50)
         self.kymogram_linewidth = create_spin_box(1, 100, 1, 1)
 
         self.temporal_window_location = QComboBox()
         self.temporal_window_location.addItems(
             ['From Current', 'Current Central', 'To Current'])
```

### Comparing `microEye-1.0.5/src/microEye/analysis/tools/roi_selectors.py` & `microEye-2.0.0/src/microEye/analysis/tools/roi_selectors.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/viewer/image_options_widget.py` & `microEye-2.0.0/src/microEye/analysis/viewer/image_options_widget.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/viewer/images.py` & `microEye-2.0.0/src/microEye/analysis/viewer/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,35 +63,32 @@
     A class for viewing and interacting with image stacks in a PyQt5 application.
     '''
     localizedData = pyqtSignal(str)
 
     def __init__(
             self,
             path: str,
-            stack_handler: Union[ZarrImageSequence, TiffSeqHandler],
-            threadpool: QThreadPool =None):
+            stack_handler: Union[ZarrImageSequence, TiffSeqHandler]):
         '''
         Initialize the StackView.
 
         Parameters
         ----------
         path : str
             The path to the image stack.
         stack_handler : Union[ZarrImageSequence, TiffSeqHandler]
             An image stack handler.
-        threadpool : QThreadPool, optional
-            Thread pool for concurrent processing, by default None.
         '''
         super().__init__()
 
         self.setWindowTitle(path.split('/')[-1])
 
         self.path = path
         self.stack_handler = stack_handler
-        self._threadpool = threadpool
+        self._threadpool = QThreadPool.globalInstance()
 
         self.main_layout = QHBoxLayout()
         self.setLayout(self.main_layout)
 
         # Graphics layout
         self.initGraphics()
 
@@ -328,16 +325,15 @@
             elif parameter == 'CompositionMode':
                 idx = int(parent.split(' ')[-1]) - 1
                 self.image_items[idx][0].setCompositionMode(
                     getattr(QPainter.CompositionMode, 'CompositionMode_' + str(data)))
 
     def setupKymogramTab(self):
         # Creating the kymogram tab layout
-        self.kymogram_widget = KymogramWidget(
-            self._threadpool)
+        self.kymogram_widget = KymogramWidget()
 
         self.kymogram_widget.setMaximum(
             self.stack_handler.shapeTCZYX()[0] - 1)
         self.kymogram_widget.displayClicked.connect(self.kymogram_display_clicked)
         self.kymogram_widget.extractClicked.connect(self.kymogram_btn_clicked)
 
         self.tab_widget.addTab(self.kymogram_widget, 'Kymogram')
@@ -1061,15 +1057,15 @@
             else:
                 event.ignore()
                 QMessageBox.warning(
                     self, 'Warning', 'Cannot close while workers are active!')
 
     @staticmethod
     def FromZarr(
-            path: str, threadpool=None):
+            path: str):
         '''
         Create a StackView instance from a Zarr image sequence.
 
         Parameters
         ----------
         path : str
             The path to the Zarr image sequence.
@@ -1082,22 +1078,22 @@
         if not os.path.isdir(path):
             raise ValueError(
                 "The supplied path should refer to a directory that includes '.zarr'")
 
         zarr_handler = ZarrImageSequence(path)
         zarr_handler.open()
 
-        stack_view = StackView(path, zarr_handler, threadpool)
+        stack_view = StackView(path, zarr_handler)
         stack_view.centerROI()
 
         return stack_view
 
     @staticmethod
     def FromImageSequence(
-            path: str, mask_pattern: str = None, threadpool=None):
+            path: str, mask_pattern: str = None):
         '''
         Create a StackView instance from an image sequence.
 
         Parameters
         ----------
         path : str
             The path to the image sequence.
@@ -1120,15 +1116,15 @@
                 image_sequence = tf.TiffSequence([path])
         except ValueError:
             return None
 
         image_seq_handler = TiffSeqHandler(image_sequence)
         image_seq_handler.open()
 
-        stack_view = StackView(path, image_seq_handler, threadpool)
+        stack_view = StackView(path, image_seq_handler)
         stack_view.centerROI()
 
         with tf.TiffFile(image_sequence.files[0]) as fl:
             if fl.is_ome:
                 ome = OME.from_xml(fl.ome_metadata)
                 stack_view.load_ome_metadata(ome)
```

### Comparing `microEye-1.0.5/src/microEye/analysis/viewer/layers_widget.py` & `microEye-2.0.0/src/microEye/analysis/viewer/layers_widget.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/analysis/viewer/localizations.py` & `microEye-2.0.0/src/microEye/analysis/viewer/localizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import traceback
 
 import cv2
 import numpy as np
 import pandas as pd
 import pyqtgraph as pg
 import tifffile as tf
@@ -36,33 +37,30 @@
     '''
     A class for viewing and interacting with SMLM localizations in a PyQt5 application.
     '''
 
     def __init__(
             self,
             path: str,
-            fittingResults: FittingResults = None,
-            threadpool: QThreadPool =None):
+            fittingResults: FittingResults = None):
         '''Initialize the StackView.
 
         Parameters
         ----------
         path : str
             The path to the image stack.
         fittingResults : FittingResults, optional
             Fitting results, by default None.
-        threadpool : QThreadPool, optional
-            Thread pool for concurrent processing, by default None.
         '''
         super().__init__()
 
         self.setWindowTitle(path.split('/')[-1])
 
         self.path = path
-        self._threadpool = threadpool
+        self._threadpool = QThreadPool.globalInstance()
         # Initialize variables
         self.fittingResults = fittingResults
 
         self.main_layout = QHBoxLayout()
         self.setLayout(self.main_layout)
 
         # Graphics layout
@@ -229,14 +227,17 @@
                 *self.fittingResults.toRender())
             # TODO: here
             self.image_items[0][0].setImage(img, autoLevels=True)
             return img
         else:
             return None
 
+    def render_tracks(self):
+        pass
+
     def setup_localization_tab(self):
         '''Set up the Localization tab.'''
         # Render tab layout
         self.localization_widget, self.localization_form = create_widget(
             QFormLayout)
         self.tab_widget.addTab(self.localization_widget, 'Localization')
 
@@ -786,18 +787,17 @@
                 dataFrame[exp_columns].to_hdf(
                     filename, key='microEye', index=False,
                     complevel=0)
 
             if 'Super-res image' in options:
                 sres_img = self.render_loc()
                 tf.imsave(
-                    filename.replace('.tsv', '_super_res.tif'),
+                    re.sub(r'(\.h5|\.tsv)$', '_super_res.tif', filename),
                     sres_img,
                     photometric='minisblack',
-                    append=True,
                     bigtiff=True,
                     ome=False)
 
     def import_loc(self):
         '''Import fitting results from a file.'''
         filename, _ = QFileDialog.getOpenFileName(
             self, 'Import localizations',
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/IR_Cam.py` & `microEye-2.0.0/src/microEye/hardware/cams/IR_Cam.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/__init__.py` & `microEye-2.0.0/src/microEye/hardware/cams/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from .micam import miCamera
-from .jobs import AcquisitionJob
-from .camera_panel import Camera_Panel
-from .camera_calibration import dark_calibration
-from .CameraListWidget import CameraListWidget
-from .IR_Cam import IR_Cam, ParallaxLineScanner
-from .thorlabs import CMD, thorlabs_camera
-from .thorlabs_panel import Thorlabs_Panel
-try:
-    from pyueye import ueye
-
-    from .ueye_camera import IDS_Camera
-    from .ueye_panel import IDS_Panel
-except Exception:
-    ueye = None
-    IDS_Camera = None
-    IDS_Panel = None
-try:
-    import vimba as vb
-
-    from .vimba_cam import vimba_cam
-    from .vimba_panel import Vimba_Panel
-except Exception:
-    vb = None
+from .camera_calibration import dark_calibration
+from .camera_list import CameraList
+from .camera_panel import Camera_Panel, CamParams
+from .IR_Cam import IR_Cam, ParallaxLineScanner
+from .jobs import AcquisitionJob
+from .micam import miCamera, miDummy
+from .thorlabs import CMD, thorlabs_camera
+from .thorlabs_panel import Thorlabs_Panel
+
+try:
+    from pyueye import ueye
+
+    from .ueye_camera import IDS_Camera
+    from .ueye_panel import IDS_Panel
+except Exception:
+    ueye = None
+    IDS_Camera = None
+    IDS_Panel = None
+try:
+    import vimba as vb
+
+    from .vimba_cam import vimba_cam
+    from .vimba_panel import Vimba_Panel
+except Exception:
+    vb = None
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/camera_calibration.py` & `microEye-2.0.0/src/microEye/hardware/cams/camera_calibration.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/camera_options.py` & `microEye-2.0.0/src/microEye/hardware/lasers/io_matchbox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,682 +1,639 @@
-import json
 import os
+import sys
 from enum import Enum
-from typing import Any, Optional, Union
+from typing import Optional
 
-import ome_types.model as om
-from ome_types.model import *
-from ome_types.model.simple_types import PixelType, UnitsLength, UnitsTime
+import qdarkstyle
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
+from PyQt5.QtSerialPort import *
 from PyQt5.QtWidgets import *
-from pyqtgraph.parametertree import Parameter, ParameterTree
-from pyqtgraph.parametertree.parameterTypes import ActionParameter, GroupParameter
+from pyqtgraph.parametertree import Parameter
 
+from ...shared import StartGUI, Tree
+from .io_params import *
 
-class CamParams(Enum):
+
+class io_combiner(QSerialPort):
     '''
-    Enum class defining Camera parameters.
+    Class representing a laser combiner MatchBox device | Inherits QSerialPort
     '''
-    CAMERA_OPTIONS = 'Camera'
-    CAMERA_GPIO = 'GPIOs'
-    CAMERA_TIMERS = 'Timers'
-    EXPOSURE = 'Camera.Exposure Time'
-    EXPERIMENT_NAME = 'Options.Experiment Name'
-    FRAMES = 'Options.Number of Frames'
-    SAVE_DIRECTORY = 'Options.Save Directory'
-    SAVE_DATA = 'Options.Save Data'
-    DARK_CALIBRATION = 'Options.Dark Calibration'
-    IMAGE_FORMAT = 'Options.Image Format'
-    TIFF_FORMAT = 'Options.Tiff Format'
-    ZARR_FORMAT = 'Options.Zarr Format'
-    BIGG_TIFF_FORMAT = 'Options.BiggTiff Format'
-    FULL_METADATA = 'Options.Full Metadata'
-    CAPTURE_STATS = 'Stats.Capture'
-    DISPLAY_STATS = 'Stats.Display'
-    SAVE_STATS = 'Stats.Save'
-    TEMPERATURE = 'Stats.Temperature'
-    ROI_X = 'Region of Interest (ROI).X'
-    ROI_Y = 'Region of Interest (ROI).Y'
-    ROI_WIDTH = 'Region of Interest (ROI).Width'
-    ROI_HEIGHT = 'Region of Interest (ROI).Height'
-    SET_ROI = 'Region of Interest (ROI).Set ROI'
-    RESET_ROI = 'Region of Interest (ROI).Reset ROI'
-    CENTER_ROI = 'Region of Interest (ROI).Center ROI'
-    SELECT_ROI = 'Region of Interest (ROI).Select ROI'
-    EXPORT_ROIS = 'Region of Interest (ROI).Export ROIs'
-    SELECT_EXPORT_ROIS = 'Region of Interest (ROI).Export ROIs.Select ROIs'
-    EXPORTED_ROIS = 'Region of Interest (ROI).Export ROIs.ROIs'
-    EXPORT_ROIS_SEPERATE = 'Region of Interest (ROI).Export ROIs.Seperate Files'
-    EXPORT_ROIS_FLIPPED = 'Region of Interest (ROI).Export ROIs.Flip Horizontally'
-    PREVIEW = 'Display.Preview'
-    DISPLAY_STATS_OPTION = 'Display.Display Stats'
-    AUTO_STRETCH = 'Display.Auto Stretch'
-    VIEW_OPTIONS = 'Display.View Options'
-    SINGLE_VIEW = 'Display.View Options.Single View'
-    DUAL_SIDE = 'Display.View Options.Dual Channel (Side by Side)'
-    DUAL_OVERLAID = 'Display.View Options.Dual Channel (Overlapped)'
-    ROIS_VIEW = 'Display.View Options.Export ROIs'
-    LINE_PROFILER = 'Display.Line Profiler'
-    LUT = 'Display.LUT'
-    LUT_NUMPY = 'Display.LUT Numpy (12bit)'
-    LUT_OPENCV = 'Display.LUT Opencv (8bit)'
-    RESIZE_DISPLAY = 'Display.Resize Display'
-
-    EXPORT_STATE = 'Export State'
-    IMPORT_STATE = 'Import State'
-
-    def __str__(self):
-        '''
-        Return the last part of the enum value (Param name).
-        '''
-        return self.value.split('.')[-1]
-
-    def get_path(self):
-        '''
-        Return the full parameter path.
-        '''
-        return self.value.split('.')
-
-class CameraOptions(ParameterTree):
-    '''
-    Tree widget for editing camera parameters.
-
-    Attributes
-    ----------
-    paramsChanged : pyqtSignal
-        Signal for parameter changed event.
-    '''
-
-    paramsChanged = pyqtSignal(GroupParameter, list)
-    '''Signal emitted when parameters are changed.
-
-    Parameters
-    ----------
-    GroupParameter
-        The group parameter that was changed.
-    list
-        A list of changes made to the parameter.
-    '''
-    setROI = pyqtSignal()
-    resetROI = pyqtSignal()
-    centerROI = pyqtSignal()
-    selectROI = pyqtSignal()
-    selectROIs = pyqtSignal()
-    directoryChanged = pyqtSignal(str)
-    viewOptionChanged = pyqtSignal()
-
-
-
-    def __init__(self, parent: Optional['QWidget'] = None):
-        '''
-        Initialize the CameraOptions.
-
-        Parameters
-        ----------
-        parent : QWidget, optional
-            The parent widget, by default None.
-        '''
-        super().__init__()
-
-        self.setMinimumWidth(50)
-        self.create_parameters()
-        self.setParameters(self.param_tree, showTop=False)
-
-    def create_parameters(self):
-        '''
-        Create the parameter tree structure.
-        '''
-        params = [
-            {'name': str(CamParams.CAMERA_OPTIONS), 'type': 'group', 'children': [
-                {'name': str(CamParams.EXPOSURE), 'type': 'float',
-                 'value': 100.0, 'dec': False, 'decimals': 6,
-                 'suffixes': [' ns', ' us', ' ms', ' s']},
-            ]},
-            {'name': 'Options', 'type': 'group', 'children': [
-                {'name': str(CamParams.EXPERIMENT_NAME),
-                'type': 'str', 'value': 'Experiment_001'},
-                {'name': str(CamParams.FRAMES),
-                'type': 'int', 'value': 1e6, 'limits': [1, 1e9]},
-                {'name': str(CamParams.SAVE_DIRECTORY), 'type': 'file',
-                 'directory': os.path.dirname(os.path.realpath(__file__)),
-                 'fileMode': 'DirectoryOnly'},
-                {'name': str(CamParams.SAVE_DATA), 'type': 'bool', 'value': False},
-                {'name': str(CamParams.DARK_CALIBRATION),
-                 'type': 'bool', 'value': False},
-                {'name': str(CamParams.IMAGE_FORMAT), 'type': 'list', 'values': [
-                    str(CamParams.BIGG_TIFF_FORMAT), str(CamParams.TIFF_FORMAT),
-                    str(CamParams.ZARR_FORMAT)
-                ]},
-                {'name': str(CamParams.FULL_METADATA), 'type': 'bool', 'value': True},
-                ]},
-            {'name': 'Display', 'type': 'group', 'children': [
-                {'name': str(CamParams.PREVIEW), 'type': 'bool', 'value': True},
-                {'name': str(CamParams.DISPLAY_STATS_OPTION),
-                 'type': 'bool', 'value': False},
-                {'name': str(CamParams.AUTO_STRETCH), 'type': 'bool', 'value': True},
-                {'name': str(CamParams.LUT), 'type': 'list', 'values': [
-                    str(CamParams.LUT_NUMPY), str(CamParams.LUT_OPENCV)
-                ]},
-                {'name': str(CamParams.VIEW_OPTIONS), 'type': 'list', 'values': [
-                    str(CamParams.SINGLE_VIEW), str(CamParams.DUAL_SIDE),
-                    str(CamParams.DUAL_OVERLAID), str(CamParams.ROIS_VIEW)]},
-                {'name': str(CamParams.LINE_PROFILER), 'type': 'bool', 'value': False},
-                {'name': str(CamParams.RESIZE_DISPLAY),
-                'type': 'float', 'value': 0.5, 'limits': [0.1, 4.0],
-                'step': 0.02, 'dec': False},
-            ]},
-            {'name': 'Stats', 'type': 'group', 'children': [
-                {'name': str(CamParams.CAPTURE_STATS),
-                'type': 'str', 'value': '0 | 0.00 ms', 'readonly': True},
-                {'name': str(CamParams.DISPLAY_STATS),
-                'type': 'str', 'value': '0 | 0.00 ms', 'readonly': True},
-                {'name': str(CamParams.SAVE_STATS),
-                'type': 'str', 'value': '0 | 0.00 ms', 'readonly': True},
-                {'name': str(CamParams.TEMPERATURE),
-                'type': 'str', 'value': ' T -127.00 °C', 'readonly': True},
-            ]},
-            {'name': 'Region of Interest (ROI)', 'type': 'group', 'children': [
-                {'name': str(CamParams.ROI_X), 'type': 'int', 'value': 0},
-                {'name': str(CamParams.ROI_Y), 'type': 'int', 'value': 0},
-                {'name': str(CamParams.ROI_WIDTH), 'type': 'int', 'value': 0},
-                {'name': str(CamParams.ROI_HEIGHT), 'type': 'int', 'value': 0},
-                {'name': str(CamParams.SET_ROI), 'type': 'action'},
-                {'name': str(CamParams.RESET_ROI), 'type': 'action'},
-                {'name': str(CamParams.CENTER_ROI), 'type': 'action'},
-                {'name': str(CamParams.SELECT_ROI), 'type': 'action'},
-                {'name': str(CamParams.EXPORT_ROIS), 'type': 'group', 'children': [
-                    {'name': str(CamParams.SELECT_EXPORT_ROIS), 'type': 'action'},
-                    {'name': str(CamParams.EXPORTED_ROIS), 'type': 'group',
-                     'children': []},
-                    {'name': str(CamParams.EXPORT_ROIS_SEPERATE),
-                     'type': 'bool', 'value': False,
-                     'tip': 'Export each ROI as a seperate Tiff file. (Not for Zarr)'},
-                    {'name': str(CamParams.EXPORT_ROIS_FLIPPED),
-                     'type': 'bool', 'value': True,
-                     'tip': 'Flip n-th ROIs horizontally for n > 1.'},
-                ]},
-            ]},
-            {'name': str(CamParams.CAMERA_GPIO), 'type': 'group', 'children': [
-            ]},
-            {'name': str(CamParams.CAMERA_TIMERS), 'type': 'group', 'children': [
-            ]},
-            {'name': str(CamParams.EXPORT_STATE), 'type': 'action'},
-            {'name': str(CamParams.IMPORT_STATE), 'type': 'action'},
-        ]
+    INFO = b'r i'
+    '''Get MatchBox Info
+    '''
+    ON = b'e 1'
+    '''Enable the combiner
+    '''
+    OFF = b'e 0'
+    '''Disable the combiner
+    '''
+    READ = b'r r'
+    SETTINGS = b'r s'
 
-        self.param_tree = Parameter.create(name='root', type='group', children=params)
-        self.param_tree.sigTreeStateChanged.connect(self.change)
-        self.header().setSectionResizeMode(
-            QHeaderView.ResizeMode.Stretch)
+    ENABLE_1 = b'L1E'
+    '''Enable 1st Laser Diode
+    '''
+    ENABLE_2 = b'L2E'
+    '''Enable 2nd Laser Diode
+    '''
+    ENABLE_3 = b'L3E'
+    '''Enable 3rd Laser Diode
+    '''
+    ENABLE_4 = b'L4E'
+    '''Enable 4th Laser Diode
+    '''
+    DISABLE_1 = b'L1D'
+    '''Disable 1st Laser Diode
+    '''
+    DISABLE_2 = b'L2D'
+    '''Disable 2nd Laser Diode
+    '''
+    DISABLE_3 = b'L3D'
+    '''Disable 3rd Laser Diode
+    '''
+    DISABLE_4 = b'L4D'
+    '''Disable 4th Laser Diode
+    '''
 
-        self.get_param(
-            CamParams.SAVE_DIRECTORY).sigValueChanged.connect(
-                lambda: self.directoryChanged.emit(
-                    self.get_param_value(CamParams.SAVE_DIRECTORY)
-                    ))
+    GET_WAVELENGTHS = b'Ln?'
+    '''Get available wavelengths
+    '''
 
-        self.get_param(
-            CamParams.SET_ROI).sigActivated.connect(lambda: self.setROI.emit())
-        self.get_param(
-            CamParams.RESET_ROI).sigActivated.connect(lambda: self.resetROI.emit())
-        self.get_param(
-            CamParams.CENTER_ROI).sigActivated.connect(lambda: self.centerROI.emit())
-        self.get_param(
-            CamParams.SELECT_ROI).sigActivated.connect(lambda: self.selectROI.emit())
-        self.get_param(
-            CamParams.SELECT_EXPORT_ROIS).sigActivated.connect(
-                lambda: self.selectROIs.emit())
-        self.get_param(
-            CamParams.VIEW_OPTIONS).sigValueChanged.connect(
-                lambda: self.viewOptionChanged.emit())
+    MAX_CUR = b'Lm?'
+    '''Get maximum current
+    '''
+    CUR_SET = b'Lc?'
+    '''Get the current set value
+    '''
+    CUR_CUR = b'Lr'
+    '''Get the current reading
+    '''
+    STATUS = b'Le'
+    '''Get the laser diodes enabled(1)/disabled(0) states
+    '''
+    START = b'c u 2 35488'
+    '''TBA
+    '''
 
-        self.get_param(
-            CamParams.IMPORT_STATE).sigActivated.connect(self.load_json)
-        self.get_param(
-            CamParams.EXPORT_STATE).sigActivated.connect(self.export_json)
+    DataReady = pyqtSignal(str, bytes)
 
-    def get_param(
-            self, param: CamParams
-            ) -> Union[Parameter, ActionParameter]:
-        '''Get a parameter by name.
+    Max_Power = 0.0
 
-        Parameters
-        ----------
-        param : CamParams
-            Camera parameter.
+    R_Diode_Temp = 0.0
+    R_Crystal_Temp = 0.0
+    R_Body_Temp = 0.0
+
+    R_LD_Current = '0.0mA'
+
+    R_Crystal_TEC_Load = '0%'
+    R_LD_TEC_Load = '0%'
+
+    R_Status = 'OFF'
+
+    R_Fan_Load = '0%'
+
+    R_Input_Voltage = '5V'
+
+    S_Crystal_Temp = 0.0
+    S_Diode_Temp = 0.0
+
+    S_LD_Current = '0.0mA'
+    S_Feedback_DAC = 0
+
+    S_Power = 0.0
+
+    S_LD_MaxCurrent = 0.0
+
+    S_Autostart_Mode = 'OFF'
+
+    S_Access_Level = 1
+
+    S_Fan_Temp = 0.0
+
+    Firmware = ''
+    Serial = ''
+    Model = ''
+    Operation_Time = ''
+    ON_Times = ''
+
+    Current = [0, 0, 0, 0]
+    Setting = [0, 0, 0, 0]
+    Max = [0, 0, 0, 0]
+    Wavelengths = [0, 0, 0, 0]
+
+    def SendCommand(self, command, log_print: bool = True, delay: int = 1):
+        '''Sends a specific command to the device and waits for
+        the response then emits the DataReady signal.
+        The DataReady signal passes the response and command.
+
+        Parameters
+        ----------
+        command : [bytes]
+            command to be sent, please check the constants
+            implemented in the MatchBox class.
+        '''
+        if (self.isOpen()):
+            self.readAll()
+            self.write(command)
+            self.waitForBytesWritten(500)
+            QThread.msleep(delay)
+            while self.bytesAvailable() < 5:
+                self.waitForReadyRead(500)
+
+            response = str(self.readAll().replace(b'\xff', b''),
+                           encoding='utf-8',
+                           errors='replace').strip('\r\n').strip()
+            if log_print:
+                print(response, command)
+
+            self.DataReady.emit(response, command)
+
+            return response
+
+    def OpenCOM(self):
+        '''Opens the serial port and initializes the combiner.
+        '''
+        if not self.isOpen():
+            self.open(QIODevice.ReadWrite)
+            self.flush()
+
+            if (self.isOpen()):
+                self.SendCommand(io_combiner.ON)
+                self.SendCommand(io_combiner.START)
+                # self.SendCommand(io_single_laser.STATUS)
+                self.GetInfo()
+                self.GetWavelengths()
+                self.SetCurrent(1, 0)
+                self.SetCurrent(2, 0)
+                self.SetCurrent(3, 0)
+                self.SetCurrent(4, 0)
+                self.GetMaxCurrent()
+
+    def CloseCOM(self):
+        '''Closes the serial port.
+        '''
+        if (self.isOpen()):
+            self.SendCommand(io_combiner.OFF)
+            self.waitForBytesWritten(500)
+
+            self.close()
+
+    def GetMaxCurrent(self):
+        if (self.isOpen()):
+            res = self.SendCommand(io_combiner.MAX_CUR)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                values = res.strip('<').strip('>').split(' ')
+                if len(values) >= 4:
+                    self.Max = list(map(int, values))
+
+    def GetCurrent(self, log_print: bool = False):
+        if (self.isOpen()):
+            res = self.SendCommand(
+                io_combiner.CUR_CUR, log_print)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                values = res.strip('<').strip(' mA>').split(' ')
+                if len(values) >= 4:
+                    self.Current = list(map(float, values))
+
+    def GetSetCurrent(self, log_print: bool = False):
+        if (self.isOpen()):
+            res = self.SendCommand(
+                io_combiner.CUR_SET, log_print)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                values = res.strip('<').strip('>').split(' ')
+                if len(values) >= 4:
+                    self.Setting = list(map(int, values))
+
+    def GetWavelengths(self):
+        if (self.isOpen()):
+            res = self.SendCommand(io_combiner.GET_WAVELENGTHS)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                values = res.strip('<').strip(
+                    ' >').strip().split(' ')
+                self.Wavelengths = []
+                if len(values) == 3:
+                    self.Wavelengths.append(0)
+                for x in range(len(values)):
+                    if values[x].isdigit():
+                        self.Wavelengths.append(int(values[x]))
+                    else:
+                        self.Wavelengths.append(0)
+                # if len(values) >= 3:
+                #     self.Wavelengths = list(map(int, values))
+
+    def GetReadings(self, log_print: bool = True):
+        if (self.isOpen()):
+            res = self.SendCommand(
+                io_combiner.READ,
+                log_print)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                readings = res.split(' ')
+                if len(readings) >= 10:
+                    self.R_Diode_Temp = float(readings[1])
+                    self.R_Crystal_Temp = float(readings[2])
+                    self.R_Body_Temp = float(readings[3])
+                    self.R_LD_Current = readings[4]
+                    self.R_Crystal_TEC_Load = readings[5]
+                    self.R_LD_TEC_Load = readings[6]
+                    self.R_Status = readings[7]
+                    self.R_Fan_Load = readings[8]
+                    self.R_Input_Voltage = readings[9]
+
+                    return {
+                        MB_Params.LD_TEMP : self.R_Diode_Temp,
+                        MB_Params.CRYSTAL_TEMP : self.R_Crystal_Temp,
+                        MB_Params.BODY_TEMP : self.R_Body_Temp,
+                        MB_Params.LD_CURRENT : self.R_LD_Current,
+                        MB_Params.CRYSTAL_TEC_LOAD : self.R_Crystal_TEC_Load,
+                        MB_Params.LD_TEC_LOAD : self.R_LD_TEC_Load,
+                        MB_Params.STATUS : self.R_Status,
+                        MB_Params.FAN_LOAD : self.R_Fan_Load,
+                        MB_Params.IN_VOLTAGE : self.R_Input_Voltage,
+                    }
+
+        return {}
+
+    def GetSettings(self, log_print: bool = True):
+        if (self.isOpen()):
+            res = self.SendCommand(
+                io_combiner.SETTINGS,
+                log_print)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                readings = res.split(' ')
+                if len(readings) >= 10:
+                    self.S_Crystal_Temp = float(readings[1]) / 100
+                    self.S_Diode_Temp = float(readings[2]) / 100
+                    self.S_LD_Current = float(readings[3])
+                    self.S_Feedback_DAC = float(readings[4])
+                    self.S_Power = float(readings[5])
+                    self.S_LD_MaxCurrent = float(readings[6])
+                    self.S_Autostart_Mode = readings[7]
+                    self.S_Access_Level = int(readings[8])
+                    self.S_Fan_Temp = float(readings[9]) / 100
+
+                    return {
+                        MB_Params.CRYSTAL_TEMP_SET : self.S_Crystal_Temp,
+                        MB_Params.LD_TEMP_SET : self.S_Diode_Temp,
+                        MB_Params.LD_CURRENT_SET : self.S_LD_Current,
+                        MB_Params.FEEDBACK_DAC : self.S_Feedback_DAC,
+                        MB_Params.POWER_READ : self.S_Power,
+                        MB_Params.LD_CURRENT_MAX : self.S_LD_MaxCurrent,
+                        MB_Params.AUTO_MODE : self.S_Autostart_Mode,
+                        MB_Params.ACCESS_LEVEL : self.S_Access_Level,
+                        MB_Params.FAN_TEMP_SET : self.S_Fan_Temp,
+                    }
+
+        return {}
+
+    def SetCurrent(self, index: int, value: int) -> bool:
+        if (self.isOpen()):
+            if not isinstance(value, int):
+                raise TypeError('Current must be an int!')
+            if value < 0 or value > self.Max[index-1]:
+                raise ValueError(f'Current must be between 0 and {self.Max[index-1]}')
+
+            res = self.SendCommand(
+                f'Lc{index:.0f} {value:.0f}'.encode())
+
+            return '<ACK>' in res
+
+    def SetDisabled(self, index: int) -> bool:
+        if (self.isOpen()):
+            res = self.SendCommand(
+                f'L{index:.0f}D'.encode())
+
+            return '<ACK>' in res
+
+    def SetEnabled(self, index: int) -> bool:
+        if (self.isOpen()):
+            res = self.SendCommand(
+                f'L{index:.0f}E'.encode())
+
+            return '<ACK>' in res
+
+    def GetInfo(self):
+        if (self.isOpen()):
+            res = self.SendCommand(
+                io_combiner.INFO,
+                delay=50)
+
+            if not ('<ERR>' in res or '<ACK>' in res):
+                info = res.split('\r\n')
+
+                self.Firmware = info[0]
+                self.Serial = info[1].split(':')[1]
+                self.Model = info[2].split(':')[1]
+                self.Operation_Time = info[3]
+                self.ON_Times = info[4]
 
-        Returns
-        -------
-        Union[Parameter, ActionParameter]
-            Retrieved parameter.
-        '''
-        return self.param_tree.param(*param.value.split('.'))
 
-    def get_param_value(
-            self, param: CamParams):
-        '''Get a parameter value by name.
+class LaserSwitches:
+    def __init__(self, Laser: io_combiner, index=1, wavelength=638) -> None:
+        super().__init__()
 
-        Parameters
-        ----------
-        param : CamParams
-            Camera parameter.
+        self.Laser = Laser
+        self.index = index
+        self.wavelength = wavelength
+        self.state = LaserState.OFF
+        self.max_current = Laser.Max[index - 1]
 
-        Returns
-        -------
-        Any
-            The value of the parameter.
-        '''
-        return self.param_tree.param(*param.value.split('.')).value()
+        self.STATE = f'Options.{self.wavelength:d}nm State'
+        self.CURRENT = f'Options.{self.wavelength:d}nm Current [mA]'
 
-    def set_param_value(
-            self, param: CamParams, value, blockSignals: Union[Any, None]= None):
-        '''
-        Set a camera parameter value by name.
+    def laser_state_changed(self, param: Parameter, value):
+        '''Sends enable/disable signals to the
+        laser combiner according to selected setting
 
         Parameters
         ----------
-        param : CamParams
-            Camera parameter.
-        value : Any
-            The value to set.
-        blockSignals : Union[Any, None], optional
-            If provided, signals for parameter changes are blocked during the update.
-            The interpretation of the value is left to the implementation.
-
-        Returns
-        -------
-        bool
-            True if the value is set successfully, False otherwise.
+        object : [QRadioButton]
+            the radio button toggled
         '''
-        try:
-            parameter: Parameter = self.param_tree.param(*param.value.split('.'))
-            parameter.setValue(value, blockSignals)
-        except Exception:
-            import traceback
-            traceback.print_exc()
-            return False
+        self.state = value
+        if self.state == LaserState.OFF:
+            self.Laser.SetDisabled(self.index)
         else:
-            return True
-
-    def get_param_path(self, param: Parameter):
-        '''
-        Get the child path of a parameter in the parameter tree.
-
-        Parameters
-        ----------
-        param : Parameter
-            The parameter for which to retrieve the child path.
-
-        Returns
-        -------
-        list
-            The child path of the parameter.
-        '''
-        return self.param_tree.childPath(param)
-
-    def add_param_child(self, parent: CamParams, value: dict):
-        '''
-        Add a child parameter to the specified parent parameter.
-
-        Parameters
-        ----------
-        parent : CamParams
-            The parent parameter to which the child will be added.
-        value : dict
-            A dictionary representing the child parameter. It should contain at
-            least the following key-value pairs:
-            - 'name': str, the name of the parameter.
-            - 'type': str, the type of the parameter (e.g., 'int', 'float', 'str').
-            - 'value': Any, the initial value of the parameter.
-            Additional optional keys can be included based on the desired configuration.
-
-        Returns
-        -------
-        None
-        '''
-        parent = self.get_param(parent)
-        parent.addChild(value, autoIncrementName=True)
-
-    def get_children(self, param: CamParams):
-        '''
-        Get the values of all children of a specified parameter.
-
-        Parameters
-        ----------
-        param : CamParams
-            The parameter whose children's values will be retrieved.
-
-        Returns
-        -------
-        list
-            List of values of all children of the specified parameter.
-        '''
-        res = []
-        param = self.get_param(param)
-        if isinstance(param, GroupParameter):
-            for child in param.children():
-                res.append(child.value())
-        return res
-
-    def change(self, param: Parameter, changes: list):
-        '''
-        Handle parameter changes as needed.
-
-        Parameters
-        ----------
-        param : Parameter
-            The parameter that triggered the change.
-        changes : list
-            List of changes.
+            self.Laser.SetEnabled(self.index)
 
-        Returns
-        -------
-        None
-        '''
-        # Handle parameter changes as needed
-        pass
+    def SetCurrent(self, value):
+        self.Laser.SetCurrent(
+            self.index, value)
 
-    def export_json(self):
-        '''
-        Export parameters to a JSON file.
+    def GetRelayState(self):
+        return f'L{self.wavelength:d}{self.state}'
 
-        Returns
-        -------
-        None
-        '''
-        filename, _ = QFileDialog.getSaveFileName(
-            None,
-            'Save Parameters', '', 'JSON Files (*.json);;All Files (*)')
-        if not filename:
-            return  # User canceled the operation
-
-        state = self.param_tree.saveState()
-        with open(filename, 'w', encoding='utf8') as file:
-            json.dump(state, file, indent=2)
+    def add_params(self, parent: Tree):
+        params = [
+            {'name': self.STATE.split('.')[1], 'type': 'list',
+                'value': LaserState.OFF, 'values': LaserState.get_list()},
+            {'name': self.CURRENT.split('.')[1],
+            'type': 'int', 'value': 0, 'limits': [0, self.max_current]}]
+        for param in params:
+            parent.add_param_child(MB_Params.OPTIONS, param)
 
-    # Load parameters from JSON
-    def load_json(self):
-        '''
-        Load parameters from a JSON file.
+        parent.get_param(self.STATE).sigValueChanged.connect(
+            self.laser_state_changed)
 
-        Returns
-        -------
-        None
-        '''
-        filename, _ = QFileDialog.getOpenFileName(
-            None, 'Load Parameters',
-            '', 'JSON Files (*.json);;All Files (*)')
-        if not filename:
-            return  # User canceled the operation
 
-        with open(filename, encoding='utf8') as file:
-            state = json.load(file)
-        self.param_tree.restoreState(state, blockSignals=False)
+class CombinerLaserWidget(Tree):
 
-    def get_roi_info(self, vimba=False):
-        '''
-        Get the region of interest (ROI) information.
+    def __init__(self, parent: Optional['QWidget'] = None):
+        '''Initializes a new CombinerLaserWidget instance.
 
         Parameters
         ----------
-        vimba : bool, optional
-            If True, returns ROI information suitable for Vimba API.
-            If False (default), returns ROI information in the default order.
-
-        Returns
-        -------
-        tuple
-            Tuple containing ROI X, ROI Y, ROI width, and ROI height.
-            If vimba is True, the order is (width, height, x, y).
-            If vimba is False, the order is (x, y, width, height).
-        '''
-        if not vimba:
-            info = [
-                self.get_param_value(CamParams.ROI_X),
-                self.get_param_value(CamParams.ROI_Y),
-                self.get_param_value(CamParams.ROI_WIDTH),
-                self.get_param_value(CamParams.ROI_HEIGHT),
-            ]
-            return info
-        else:
-            info = [
-                self.get_param_value(CamParams.ROI_WIDTH),
-                self.get_param_value(CamParams.ROI_HEIGHT),
-                self.get_param_value(CamParams.ROI_X),
-                self.get_param_value(CamParams.ROI_Y),
-            ]
-            return info
+        parent : Optional[QWidget]
+            The parent widget for this CombinerLaserWidget instance.
 
-    def set_roi_info(self, x: int, y: int, w: int, h: int):
-        '''
-        Set the region of interest (ROI) information.
-
-        Parameters
+        Attributes
         ----------
-        x : int
-            X-coordinate of the ROI.
-        y : int
-            Y-coordinate of the ROI.
-        w : int
-            Width of the ROI.
-        h : int
-            Height of the ROI.
-
-        Returns
-        -------
-        None
+        Laser : io_combiner
+            The `io_combiner` instance used to communicate with the device.
         '''
-        self.set_param_value(CamParams.ROI_X, x)
-        self.set_param_value(CamParams.ROI_Y, y)
-        self.set_param_value(CamParams.ROI_WIDTH, w)
-        self.set_param_value(CamParams.ROI_HEIGHT, h)
-
-    def set_roi_limits(
-            self,
-            x: tuple[int, int], y: tuple[int, int],
-            w: tuple[int, int], h: tuple[int, int]):
-        '''
-        Set limits for the Region of Interest (ROI) parameters.
+        super().__init__()
 
-        This function sets limits for the X-coordinate, Y-coordinate, width,
-        and height parameters of the Region of Interest (ROI).
+        self.Laser = io_combiner()
 
-        Parameters
-        ----------
-        x : tuple[int, int]
-            Tuple representing the minimum and maximum limits for the X-coordinate.
-        y : tuple[int, int]
-            Tuple representing the minimum and maximum limits for the Y-coordinate.
-        w : tuple[int, int]
-            Tuple representing the minimum and maximum limits for the width.
-        h : tuple[int, int]
-            Tuple representing the minimum and maximum limits for the height.
+        self._laserSwitches: list[LaserSwitches] = []
 
-        Returns
-        -------
-        None
-        '''
-        self.get_param(CamParams.ROI_X).setLimits(x)
-        self.get_param(CamParams.ROI_Y).setLimits(y)
-        self.get_param(CamParams.ROI_WIDTH).setLimits(w)
-        self.get_param(CamParams.ROI_HEIGHT).setLimits(h)
-
-    def get_export_rois(self):
-        '''
-        Get the export regions of interest (ROIs) information.
-
-        Returns
-        -------
-        list[list[int]]
-            list or ROIs with each being a list[int] of [x, y, w, h].
-        '''
-        rois_param = self.get_param(
-            CamParams.EXPORTED_ROIS)
-        rois = []
-
-        if len(rois_param.children()) > 0:
-            for child in rois_param.children():
-                rois.append(
-                    list(
-                        map(int,
-                            child.value().split(', '))
-                            )
-                    )
-        return rois
+        # Statues Bar Timer
+        self.timer = QTimer()
+        self.timer.setInterval(500)
+        self.timer.timeout.connect(self.update_stats)
+        self.timer.start()
 
-    @property
-    def isTiff(self):
+    def create_parameters(self):
         '''
-        Check if the image format is TIFF.
-
-        Returns
-        -------
-        bool
-            True if the image format is TIFF, False otherwise.
+        Create the parameter tree structure.
         '''
-        return self.get_param_value(CamParams.IMAGE_FORMAT) in [
-            str(CamParams.TIFF_FORMAT), str(CamParams.BIGG_TIFF_FORMAT)
+        params = [
+            {'name': str(MB_Params.MODEL),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+            {'name': str(MB_Params.WAVELENGTHS),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+            {'name': str(MB_Params.SERIAL_PORT), 'type': 'group', 'children': [
+                {'name': str(MB_Params.PORT), 'type': 'list',
+                 'values': [
+                     info.portName() for info in QSerialPortInfo.availablePorts()]},
+                {'name': str(MB_Params.BAUDRATE), 'type': 'list', 'value': 115200,
+                 'values': [
+                     baudrate for baudrate in QSerialPortInfo.standardBaudRates()]},
+                {'name': str(MB_Params.SET_PORT), 'type': 'action'},
+                {'name': str(MB_Params.OPEN), 'type': 'action'},
+                {'name': str(MB_Params.CLOSE), 'type': 'action'},
+                {'name': str(MB_Params.PORT_STATE),
+                 'type': 'str', 'value': 'closed', 'readonly': True},
+            ]},
+            {'name': str(MB_Params.OPTIONS), 'type': 'group', 'children': [
+                {'name': str(MB_Params.SET_CURRENT), 'type': 'action'},
+            ]},
+            {'name': str(MB_Params.READINGS), 'type': 'group', 'children': [
+                {'name': str(MB_Params.POWER_READ),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_CURRENT),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_CURRENT_SET),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_CURRENT_MAX),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_TEMP),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_TEMP_SET),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.LD_TEC_LOAD),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.CRYSTAL_TEMP),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.CRYSTAL_TEMP_SET),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.CRYSTAL_TEC_LOAD),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.BODY_TEMP),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.FAN_TEMP_SET),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.FAN_LOAD),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.FEEDBACK_DAC),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.AUTO_MODE),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.ACCESS_LEVEL),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.STATUS),
+                'type': 'str', 'value': '0', 'readonly': True},
+                {'name': str(MB_Params.IN_VOLTAGE),
+                'type': 'str', 'value': '0', 'readonly': True},
+            ]},
+            {'name': str(MB_Params.INFO), 'type': 'group', 'children': [
+                {'name': str(MB_Params.FIRMWARE),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+                {'name': str(MB_Params.SERIAL),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+                {'name': str(MB_Params.OPERATION_TIME),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+                {'name': str(MB_Params.ON_TIMES),
+                'type': 'str', 'value': 'N/A', 'readonly': True},
+            ]},
+            {'name': str(MB_Params.REMOVE), 'type': 'action'},
         ]
 
-    @property
-    def isBiggTiff(self):
-        '''
-        Check if the image format is BigTIFF.
-
-        Returns
-        -------
-        bool
-            True if the image format is BigTIFF, False otherwise.
-        '''
-        return self.get_param_value(CamParams.IMAGE_FORMAT) in [
-            str(CamParams.BIGG_TIFF_FORMAT)]
-
-    @property
-    def isSingleView(self):
-        '''
-        Check if the view option is set to single view.
-
-        Returns
-        -------
-        bool
-            True if the view option is set to single view, False otherwise.
-        '''
-        return self.get_param_value(CamParams.VIEW_OPTIONS) in [
-            str(CamParams.SINGLE_VIEW)]
-
-    @property
-    def isROIsView(self):
-        '''
-        Check if the view option is set to export ROIs view.
+        self.param_tree = Parameter.create(name='root', type='group', children=params)
+        self.param_tree.sigTreeStateChanged.connect(self.change)
+        self.header().setSectionResizeMode(
+            QHeaderView.ResizeMode.ResizeToContents)
 
-        Returns
-        -------
-        bool
-            True if the view option is set to export ROIs view, False otherwise.
-        '''
-        return self.get_param_value(CamParams.VIEW_OPTIONS) in [
-            str(CamParams.ROIS_VIEW)]
 
-    @property
-    def isOverlaidView(self):
-        '''
-        Check if the view option is set to overlaid view.
+        self.get_param(
+            MB_Params.SET_PORT).sigActivated.connect(self.set_config)
+        self.get_param(
+            MB_Params.OPEN).sigActivated.connect(self.laser_connect)
+        self.get_param(
+            MB_Params.CLOSE).sigActivated.connect(lambda: self.Laser.CloseCOM())
+        self.get_param(
+            MB_Params.SET_CURRENT).sigActivated.connect(self.set_current)
 
-        Returns
-        -------
-        bool
-            True if the view option is set to overlaid view, False otherwise.
-        '''
-        return self.get_param_value(CamParams.VIEW_OPTIONS) in [
-            str(CamParams.DUAL_OVERLAID)]
+        self.get_param(
+            MB_Params.REMOVE).sigActivated.connect(self.remove_widget)
 
-    @property
-    def isFullMetadata(self):
-        '''
-        Check if the metadata option is set to full.
+    def laser_connect(self):
+        '''Connects to the MatchBox device.
 
-        Returns
-        -------
-        bool
-            True if the full metadata option is set, False otherwise.
+        This method opens the serial port and initializes the laser.
         '''
-        return self.get_param_value(CamParams.FULL_METADATA)
+        self.Laser.OpenCOM()
 
-    @property
-    def isDarkCalibration(self):
-        '''
-        Check if the dark calibration option is set.
+        self.set_param_value(MB_Params.MODEL, self.Laser.Model)
+        self.set_param_value(MB_Params.WAVELENGTHS, str(self.Laser.Wavelengths))
+        self.set_param_value(MB_Params.FIRMWARE, self.Laser.Firmware)
+        self.set_param_value(MB_Params.SERIAL, self.Laser.Serial)
+
+        if not self._laserSwitches:
+            for idx in range(len(self.Laser.Wavelengths)):
+                if self.Laser.Wavelengths[idx] > 0:
+                    switch = LaserSwitches(
+                        self.Laser, idx + 1,
+                        self.Laser.Wavelengths[idx])
+                    switch.add_params(self)
+                    self._laserSwitches.append(switch)
+
+    def set_config(self):
+        '''Sets the serial port configuration.
+
+        This method sets the serial port configuration based on the current
+        settings in the parameter tree.
+        '''
+        if not self.Laser.isOpen():
+            self.Laser.setPortName(
+                self.get_param_value(MB_Params.PORT))
+            self.Laser.setBaudRate(
+                self.get_param_value(MB_Params.BAUDRATE))
+
+    def set_current(self):
+        for switch in self._laserSwitches:
+            value = self.get_param(switch.CURRENT).value()
+            switch.SetCurrent(value)
+
+    def update_stats(self):
+        '''
+        Updates the statistics displayed in the MatchBox GUI.
+
+        This method retrieves the current readings and settings from the device, and
+        updates the corresponding parameter tree items with the new values. It also
+        sets the limits of the power parameter based on the maximum power that can be
+        set for the laser diode.
+
+        If the laser is not connected, the method sets the 'Port State' parameter to
+        'closed'.
+        '''
+        if self.Laser.isOpen():
+            readings = self.Laser.GetReadings(False)
+            settings = self.Laser.GetSettings(False)
+            self.Laser.GetCurrent()
+
+            for key, value in readings.items():
+                if isinstance(value, (int, float)):
+                    self.set_param_value(key, f'{value:.2f}')
+                elif isinstance(value, str):
+                    self.set_param_value(key, value)
+
+            for key, value in settings.items():
+                if isinstance(value, (int, float)):
+                    self.set_param_value(key, f'{value:.2f}')
+                elif isinstance(value, str):
+                    self.set_param_value(key, value)
+
+            self.set_param_value(
+                MB_Params.LD_CURRENT,
+                '{:.2f} mA, {:.2f} mA, {:.2f} mA, {:.2f} mA'.format(
+                    *self.Laser.Current))
+            self.set_param_value(
+                MB_Params.LD_CURRENT_MAX,
+                '{:.2f} mA, {:.2f} mA, {:.2f} mA, {:.2f} mA'.format(
+                    *self.Laser.Max))
+            self.set_param_value(
+                MB_Params.LD_CURRENT_SET,
+                '{:.2f} mA, {:.2f} mA, {:.2f} mA, {:.2f} mA'.format(
+                    *self.Laser.Setting))
 
-        Returns
-        -------
-        bool
-            True if the dark calibration option is set, False otherwise.
-        '''
-        return self.get_param_value(CamParams.DARK_CALIBRATION)
+            self.set_param_value(MB_Params.OPERATION_TIME, self.Laser.Operation_Time)
+            self.set_param_value(MB_Params.ON_TIMES, self.Laser.ON_Times)
 
-    @property
-    def isSaveData(self):
-        '''
-        Check if the save data option is set.
+            self.set_param_value(MB_Params.PORT_STATE, 'open')
+        else:
+            self.set_param_value(MB_Params.PORT_STATE, 'closed')
 
-        Returns
-        -------
-        bool
-            True if the save data option is set, False otherwise.
-        '''
-        return self.get_param_value(CamParams.SAVE_DATA)
+        self.RefreshPorts()
 
-    @property
-    def isPreview(self):
+    def RefreshPorts(self):
         '''
-        Check if the preview option is set.
+        Refreshes the available serial ports list in the GUI.
 
-        Returns
-        -------
-        bool
-            True if the preview option is set, False otherwise.
+        This method updates the list of available serial ports in the GUI by fetching
+        the current list of available ports and setting it as the options for the
+        'Serial Port' parameter in the parameter tree.
         '''
-        return self.get_param_value(CamParams.PREVIEW)
+        if not self.Laser.isOpen():
+            self.get_param(MB_Params.PORT).setLimits([
+                info.portName() for info in QSerialPortInfo.availablePorts()])
 
-    @property
-    def isAutostretch(self):
-        '''
-        Check if the auto-stretch option is set.
+    def GetRelayState(self):
+        states = ''
+        for switch in self._laserSwitches:
+            states += switch.GetRelayState()
+        return states
 
-        Returns
-        -------
-        bool
-            True if the auto-stretch option is set, False otherwise.
-        '''
-        return self.get_param_value(CamParams.AUTO_STRETCH)
+    def remove_widget(self):
+        if self.parent() and not self.Laser.isOpen():
+            self.parent().layout().removeWidget(self)
+            self.deleteLater()
+        else:
+            print(f'Disconnect device {self.Laser.Model} before removing!')
 
-    @property
-    def isLineProfiler(self):
-        '''
-        Check if the line profiler option is set.
+    def StartGUI():
+        '''Initializes a new QApplication and CombinerLaserWidget.
 
-        Returns
+        Use
         -------
-        bool
-            True if the line profiler option is set, False otherwise.
-        '''
-        return self.get_param_value(CamParams.LINE_PROFILER)
+        app, window = CombinerLaserWidget.StartGUI()
 
-    @property
-    def isNumpyLUT(self):
-        '''
-        Check if the LUT option is set to numpy lut.
+        app.exec_()
 
         Returns
         -------
-        bool
-            True if the LUT option is set to numpy lut, False otherwise.
+        tuple (QApplication, CombinerLaserWidget)
+            Returns a tuple with QApp and CombinerLaserWidget main window.
         '''
-        return self.get_param_value(CamParams.LUT) in [str(CamParams.LUT_NUMPY)]
+        return StartGUI(CombinerLaserWidget)
 
 
 if __name__ == '__main__':
-    app = QApplication(sys.argv)
-    window = CameraOptions()
-    window.show()
-    sys.exit(app.exec_())
+    app, widget = CombinerLaserWidget.StartGUI()
+
+    app.exec_()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/camera_panel.py` & `microEye-2.0.0/src/microEye/hardware/cams/camera_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,56 +29,76 @@
 
 class Camera_Panel(QGroupBox):
     '''
     A Qt Widget base class for controlling a camera | Inherits QGroupBox
     '''
 
     exposureChanged = pyqtSignal()
+    asyncFreerun = pyqtSignal(str, threading.Event)
+    updateStatsSignal = pyqtSignal(tuple)
+    updateRangeSignal = pyqtSignal(int, int)
 
-    def __init__(self, threadpool: QThreadPool, cam: miCamera, mini=False,
+    def __init__(self, cam: miCamera, mini=False,
                  *args, **kwargs):
         '''
-        Initializes a new Vimba_Panel Qt widget
-        | Inherits QGroupBox
+        Initializes a new Camera_Panel Qt widget.
+
+        Inherits QGroupBox.
 
         Parameters
         ----------
-        threadpool : QThreadPool
-            The threadpool for multithreading
         cam : miCamera
-            Camera python adapter
+            Camera python adapter.
+
+        mini : bool, optional
+            Flag indicating if this is a mini camera panel, by default False.
+
+        Other Parameters
+        ---------------
+        *args
+            Arguments to pass to the QGroupBox constructor.
+
+        **kwargs
+            Keyword arguments to pass to the QGroupBox constructor.
         '''
         super().__init__(*args, **kwargs)
         self._cam = cam  # miCamera
         # flag true if master (always the first added camera is master)
         self.master = False
 
         self.c_worker = None  # worker for capturing
         self.d_worker = None  # worker for display
         self.s_worker = None  # worker for saving
 
-        self.c_event = None
-        self.s_event = None
+        self.asyncFreerun.connect(
+            lambda prefix, event: self.start_free_run(
+                Prefix=prefix, Event=event))
 
         # number of bins for the histogram (4096 is set for 12bit mono-camera)
         self._nBins = 2**12
         self._hist = np.arange(0, self._nBins) * 0  # arrays for the Hist plot
         self._bins = np.arange(0, self._nBins)      # arrays for the Hist plot
 
-        self._threadpool = threadpool  # the threadpool for workers
+        self.__update_timer = time.time()
+        self.updateStatsSignal.connect(self.updateStats)
+        self.updateRangeSignal.connect(self.updateRange)
+
+        self._threadpool = QThreadPool.globalInstance()  # the threadpool for workers
 
         # flag true to close camera adapter and dispose it
         self._dispose_cam = False
         self._buffer = Queue()  # data memory stack
         self._temps = Queue()  # camera sensor temperature stack
         # stack of (frame, temperature) tuples (for saving)
         self.frame = None
         self._frames = Queue()
         # reserved for saving
-        self._directory = ''  # save directory
+        home = os.path.expanduser('~')
+
+        self._directory = os.path.join(home, 'Desktop')  # save directory
         self._save_path = ''  # save path
         self._save_prefix = ''  # save prefix
 
         # acquisition job info class
         self.acq_job = None
 
         self.mini = mini
@@ -134,19 +154,18 @@
             add_button(self.cam_exp_shortcuts, value)
 
         self.first_tab_Layout.addRow(self.cam_exp_shortcuts)
         self.first_tab_Layout.addRow(self.camera_options)
 
         self.camera_options.get_param(CamParams.EXPERIMENT_NAME).sigValueChanged.connect(
             lambda x: self.OME_tab.set_param_value(
-                MetaParams.EXPERIMENT_NAME, x))
+                MetaParams.EXPERIMENT_NAME, x.value()))
 
         self.save_dir_layout = QHBoxLayout()
 
-        self._directory = os.path.dirname(os.path.realpath(__file__))
         self.camera_options.set_param_value(
             CamParams.SAVE_DIRECTORY, self._directory)
         self.camera_options.directoryChanged.connect(
             lambda value: self.directory_changed(value))
 
         save_param = self.camera_options.get_param(CamParams.SAVE_DATA)
         save_param.setOpts(enabled=not self.mini)
@@ -344,18 +363,17 @@
     def select_ROIs(self):
         '''Selects the ROI for the camera
         '''
         raise NotImplementedError(
             'The select_ROIs function is not implemented yet.')
 
     def get_meta(self):
-        meta = dict[str, any]()
-        return meta
+        return self.camera_options.get_json()
 
-    def getAcquisitionJob(self) -> AcquisitionJob:
+    def getAcquisitionJob(self, event=None) -> AcquisitionJob:
         self._save_path = os.path.join(
             self._directory,
             self.camera_options.get_param_value(CamParams.EXPERIMENT_NAME) + '\\')
         return AcquisitionJob(
             self._temps, self._buffer, self._frames,
             self._save_path, self._cam.getHeight(),
             self._cam.getWidth(),
@@ -371,15 +389,16 @@
             name=self._cam.name, prefix=self._save_prefix,
             save=self.camera_options.isSaveData,
             Zarr=not self.camera_options.isTiff,
             rois=self.camera_options.get_export_rois(),
             seperate_rois=self.camera_options.get_param_value(
                 CamParams.EXPORT_ROIS_SEPERATE),
             flip_rois=self.camera_options.get_param_value(
-                CamParams.EXPORT_ROIS_FLIPPED)
+                CamParams.EXPORT_ROIS_FLIPPED),
+            s_event=event if event else threading.Event()
         )
 
     def view_toggled(self):
         if self.camera_options.isSingleView:
             self.lr_0.setSpan(0, 1)
             self.lr_1.setMovable(False)
             self.lr_1.setRegion((0, self._nBins))
@@ -391,53 +410,51 @@
 
     @pyqtSlot()
     def directory_changed(self, value: str):
         '''Slot for directory changed signal'''
         if len(value) > 0:
             self._directory = value
 
-    def start_free_run(self, param=None, Prefix=''):
+    def start_free_run(self, param=None, Prefix='', Event=None):
         '''
         Starts free run acquisition mode
 
         Parameters
         ----------
         param : Parameter
             the parameter that was activated.
         Prefix : str
             an extra prefix added to the image stack file name.
         '''
         if self._cam.acquisition:
             return  # if acquisition is already going on
 
         self._save_prefix = Prefix
-        self.acq_job = self.getAcquisitionJob()
+        self.acq_job = self.getAcquisitionJob(Event)
 
         self._cam.acquisition = True  # set acquisition flag to true
 
         # start both capture and display workers
         self.start_all_workers()
 
     def stop(self):
-        if self.c_event is not None:
-            self.c_event.set()
+        if self.acq_job is not None:
+            self.acq_job.c_event.set()
         # set stop acquisition workers flag to true
         if self.acq_job is not None:
             self.acq_job.stop_threads = True
 
     def start_all_workers(self):
         '''
         Starts all workers
         '''
 
         self._buffer.queue.clear()
         self._temps.queue.clear()
         self._frames.queue.clear()
-        self.c_event = threading.Event()
-        self.s_event = threading.Event()
         self.time = QDateTime.currentDateTime()
 
         # Pass the display function to be executed
         if self.d_worker is None or self.d_worker.done:
             self.d_worker = thread_worker(
                 cam_display,
                 self.acq_job, self,
@@ -478,23 +495,20 @@
     def updateInfo(self):
         if isinstance(self.acq_job, AcquisitionJob):
             self.camera_options.set_param_value(
                 CamParams.TEMPERATURE,
                 f'T {self._cam.temperature:.2f} °C')
             self.camera_options.set_param_value(
                 CamParams.CAPTURE_STATS,
-                'Capture {:d}/{:d} {:.2%} | {:.2f} ms '.format(
-                    self.acq_job.frames_captured,
-                    self.acq_job.frames,
-                    self.acq_job.frames_captured / self.acq_job.frames,
-                    self.acq_job.capture_time))
+                (f'Capture {self.acq_job.frames_captured}/{self.acq_job.frames} ' +
+                 f'{self.acq_job.frames_captured / self.acq_job.frames:.2%} ' +
+                 f'| {self.acq_job.capture_time:.2f} ms'))
             self.camera_options.set_param_value(
                 CamParams.DISPLAY_STATS,
-                'Display {:d} | {:.2f} ms '.format(
-                    self._buffer.qsize(), self.acq_job.display_time))
+                f'Display {self._buffer.qsize()} | {self.acq_job.display_time:.2f} ms')
             self.camera_options.set_param_value(
                 CamParams.SAVE_STATS,
                 f'Save {self._frames.qsize():d} | {self.acq_job.save_time:.2f} ms ')
 
     def getCaptureArgs(self) -> list:
         '''User specific arguments to be passed to the parallelized
         Camera_Panel.cam_capture function.
@@ -530,14 +544,46 @@
         ------
         NotImplementedError
             Has to be implemented by the use in child class.
         '''
         raise NotImplementedError(
             'The cam_capture function is not implemented yet.')
 
+    def updateStats(self, frames: tuple[uImage]):
+        now = time.time()
+        if now - self.__update_timer < 0.1:
+            return
+
+        self.__update_timer = now
+        for idx, frame in enumerate(frames):
+            if idx < 2:
+                _lr = self.lr_0 if idx == 0 else self.lr_1
+                _plot_ref = self._plot_ref if idx == 0 else self._plot_ref_2
+                _cdf_plot_ref = self._cdf_plot_ref if idx == 0 else self._cdf_plot_ref_2
+
+                if frame is not None:
+                    if self.camera_options.isAutostretch:
+                        _lr.setRegion((frame._min, frame._max))
+
+                    _plot_ref.setData(frame._hist)
+                    _cdf_plot_ref.setData(frame._cdf)
+                else:
+                    _plot_ref.setData(self._hist)
+                    _cdf_plot_ref.setData(self._hist)
+            else:
+                break
+
+    def updateRange(self, rmin: int, rmax: int):
+        if time.time() - self.__update_timer < 0.1:
+            return
+
+        if self.camera_options.isAutostretch:
+            self.histogram.setXRange(rmin, rmax)
+            self.hist_cdf.setXRange(rmin, rmax)
+
 
 def cam_save(params: AcquisitionJob):
     '''Save function executed by the save worker thread.
 
     Saves the acquired frames using the config in AcquisitionJob
     with a csv file containing the sensor temp for each frame.
 
@@ -576,17 +622,44 @@
             if params.save_queue.empty() and \
                     params.stop_threads and params.display_done:
                 print('Save thread break.')
                 break
     except Exception:
         traceback.print_exc()
     finally:
+        params.s_event.set()
         params.finalize()
         print('Save thread finally finished.')
 
+def drawStats(frame: uImage):
+    stats = \
+        f'min/max: {np.min(frame.image)}/{np.max(frame.image)}\n'
+    stats += f'mean: {np.mean(frame.image):.3f}\n'
+    stats += f'median: {np.median(frame.image):.3f}\n'
+    stats += f'std: {np.std(frame.image):.4f}'
+
+    # Font settings
+    font = cv2.FONT_HERSHEY_SIMPLEX
+    font_scale = 0.8
+    font_thickness = 2
+    font_color = 255  # White color for monochrome image
+
+    # Split the text into lines
+    lines = stats.split('\n')
+
+    # Position to start adding text
+    x, y = 50, 50
+
+    # Add each line of text to the image
+    for line in lines:
+        cv2.putText(
+            frame._view, line, (x, y),
+            font, font_scale, font_color, font_thickness)
+        y += int(2 * font_scale * 20)  # Adjust vertical spacing
+
 def update_histogram_and_display(params: AcquisitionJob, camp: Camera_Panel):
     '''
     Update histogram and display based on camera options.
 
     Parameters
     ----------
     params : AcquisitionJob
@@ -603,43 +676,39 @@
         if not camp.camera_options.isAutostretch:
             _range = tuple(
                 map(math.ceil, camp.lr_0.getRegion()))
 
         params.frame.equalizeLUT(
             _range, camp.camera_options.isNumpyLUT)
 
-        if camp.camera_options.isAutostretch:
-            camp.lr_0.setRegion(
-                (params.frame._min, params.frame._max))
-            camp.histogram.setXRange(
-                params.frame._min, params.frame._max)
-            camp.hist_cdf.setXRange(
-                params.frame._min, params.frame._max)
-
-        camp._plot_ref.setData(params.frame._hist)
-        camp._cdf_plot_ref.setData(params.frame._cdf)
-        camp._plot_ref_2.setData(camp._hist)
-        camp._cdf_plot_ref_2.setData(camp._hist)
+        camp.updateRangeSignal.emit(params.frame._min, params.frame._max)
+
+        camp.updateStatsSignal.emit(
+            (params.frame, None))
 
         # resizing the image
         zoom = camp.camera_options.get_param_value(
             CamParams.RESIZE_DISPLAY)
+
+        if camp.camera_options.isDisplayStats:
+            drawStats(params.frame)
+
         params.frame._view = cv2.resize(
             params.frame._view, (0, 0),
             fx=zoom,
             fy=zoom,
             interpolation=cv2.INTER_NEAREST)
 
         # display it
         cv2.imshow(params.name, params.frame._view)
     elif camp.camera_options.isROIsView:
         if len(params.rois) == 1:
             camp._plot_ref_2.setData(camp._hist)
             camp._cdf_plot_ref_2.setData(camp._hist)
-        mins, maxs = [], []
+        images, mins, maxs = [], []
         for idx, roi in enumerate(params.rois):
             uimage = uImage(
                 params.frame.image[
                     roi[1]: roi[1] + roi[3],
                     roi[0]: roi[0] + roi[2]])
 
             if idx > 0 and params.flip_rois:
@@ -650,42 +719,32 @@
             if not camp.camera_options.isAutostretch and idx < 2:
                 linear_region = camp.lr_0 if idx == 0 else camp.lr_1
                 _range = tuple(
                     map(math.ceil, linear_region.getRegion()))
 
             uimage.equalizeLUT(_range, camp.camera_options.isNumpyLUT)
 
-            if camp.camera_options.isAutostretch and idx < 2:
-                linear_region = camp.lr_0 if idx == 0 else camp.lr_1
-                linear_region.setRegion(
-                    (uimage._min, uimage._max))
-                mins.append(uimage._min)
-                maxs.append(uimage._max)
-
-            if idx < 2:
-                _plot_ref = camp._plot_ref if idx == 0 else camp._plot_ref_2
-                _cdf_plot_ref = camp._cdf_plot_ref if idx == 0 else camp._cdf_plot_ref_2
-                _plot_ref.setData(uimage._hist)
-                _cdf_plot_ref.setData(uimage._cdf)
+            mins.append(uimage._min)
+            maxs.append(uimage._max)
+            images.append(uimage)
 
             # resizing the image
             zoom = camp.camera_options.get_param_value(
                 CamParams.RESIZE_DISPLAY)
             uimage._view = cv2.resize(
                 uimage._view, (0, 0),
                 fx=zoom,
                 fy=zoom,
                 interpolation=cv2.INTER_NEAREST)
 
             # display it
             cv2.imshow(params.name + f' ROI {idx+1}', uimage._view)
 
-        if camp.camera_options.isAutostretch:
-            camp.histogram.setXRange(min(mins), max(maxs))
-            camp.hist_cdf.setXRange(min(mins), max(maxs))
+        camp.updateRangeSignal.emit(min(mins), max(maxs))
+        camp.updateStatsSignal.emit(images)
     else:
         _rang_left = None
         _rang_right = None
 
         # image stretching
         if not camp.camera_options.isAutostretch:
             _rang_left = tuple(
@@ -695,28 +754,20 @@
 
         left, right = params.frame.hsplitView()
 
         left.equalizeLUT(
             _rang_left, camp.camera_options.isNumpyLUT)
         right.equalizeLUT(
             _rang_right, camp.camera_options.isNumpyLUT)
-        if camp.camera_options.isAutostretch:
-            camp.lr_0.setRegion((left._min, left._max))
-            camp.lr_1.setRegion((right._min, right._max))
-            camp.histogram.setXRange(
-                min(left._min, right._min),
-                max(left._max, right._max))
-            camp.hist_cdf.setXRange(
-                min(left._min, right._min),
-                max(left._max, right._max))
-
-        camp._plot_ref.setData(left._hist)
-        camp._cdf_plot_ref.setData(left._cdf)
-        camp._plot_ref_2.setData(right._hist)
-        camp._cdf_plot_ref_2.setData(right._cdf)
+
+        camp.updateRangeSignal.emit(
+            min(left._min, right._min),
+            max(left._max, right._max))
+        camp.updateStatsSignal.emit(
+            (left, right))
 
         zoom = camp.camera_options.get_param_value(
             CamParams.RESIZE_DISPLAY)
         if camp.camera_options.isOverlaidView:
             _img = np.zeros(
                 left._view.shape[:2] + (3,),
                 dtype=np.uint8)
@@ -765,15 +816,15 @@
                 with params.lock:
                     params.display_time = time.msecsTo(
                         QDateTime.currentDateTime())
                     time = QDateTime.currentDateTime()
 
                     # reshape image into proper shape
                     # (height, width, bytes per pixel)
-                    params.frame: uImage = uImage.fromBuffer(
+                    params.frame = uImage.fromBuffer(
                         params.display_queue.get(),
                         params.cam_height, params.cam_width,
                         params.bytes_per_pixel)
 
                     # add to saving stack
                     if params.save:
                         if not camp.mini:
@@ -792,15 +843,15 @@
                         cv2.waitKey(1)
             else:
                 cv2.waitKey(1)
 
             QThread.usleep(100)
             # Flag that ends the loop
             if params.stop_threads and params.display_queue.empty() \
-                    and camp.c_worker.done:
+                    and params.capture_done:
                 print('Display thread break.')
                 break
     except Exception:
         traceback.print_exc()
     finally:
         try:
             if not camp.mini:
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/jobs.py` & `microEye-2.0.0/src/microEye/hardware/cams/jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,495 +1,500 @@
-import json
-import os
-import threading
-import time
-from queue import Queue
-from typing import Callable
-
-import numpy as np
-import ome_types.model as om
-import tifffile as tf
-import zarr
-from PyQt5.QtCore import *
-from PyQt5.QtGui import *
-from PyQt5.QtWidgets import *
-
-from .camera_calibration import dark_calibration
-
-
-class AcquisitionJob:
-    '''A class holding cross-thread info required for an Acquisition Job.
-
-    Attributes
-    ----------
-    temp_queue : Queue[float]
-        The queue for temporary data.
-    display_queue : Queue[np.ndarray]
-        The queue for display data.
-    save_queue : Queue[tuple[np.ndarray, float]]
-        The queue for data to be saved along with associated timestamps.
-    path : str
-        The base path where files will be saved.
-    height : int
-        The height of the image frames.
-    width : int
-        The width of the image frames.
-    biggTiff : bool, optional
-        Flag indicating whether to use big TIFF format, by default True.
-    bytes_per_pixel : int, optional
-        The number of bytes per pixel, by default 1.
-    exposure : float, optional
-        The exposure time in milliseconds, by default 50.0.
-    frames : int, optional
-        The number of frames, by default 100.
-    full_tif_meta : bool, optional
-        Flag indicating whether to include full TIFF metadata, by default True.
-    is_dark_cal : bool, optional
-        Flag indicating whether dark calibration is enabled, by default False.
-    meta_file : str, optional
-        Additional metadata file path, by default ''.
-    meta_func : Callable, optional
-        A function to generate metadata, by default a lambda function.
-    name : str, optional
-        The name of the acquisition job, by default 'Camera'.
-    prefix : str, optional
-        A prefix for filenames, by default ''.
-    save : bool, optional
-        Flag indicating whether to save data, by default False.
-    Zarr : bool, optional
-        Flag indicating whether to use Zarr format, by default False.
-    rois : list[list[int]], optional
-        List of regions of interest, by default empty list.
-    seperate_rois : bool, optional
-        Flag indicating whether to save ROIs into seperate files,
-        by default False.
-        (For Zarr format different ROIs are treated as channels)
-    flip_rois : bool, optional
-        Flag indicating whether to flip n-th ROIs horizontally for n > 1,
-        by default True.
-
-
-    Methods
-    -------
-    getExt()
-        Return the file extension based on the Zarr attribute.
-    getFilename()
-        Generate the filename based on the current state.
-    getTempFilename()
-        Generate the temperatures filename based on the current state.
-    addDarkFrame(frame)
-        Add a dark frame for calibration.
-    addFrame(frame)
-        Add a frame to the acquisition job.
-    addTemp(temp)
-        Add temperature data to the acquisition job.
-    getMetaFilename()
-        Return the metadata file path.
-    writeMetaFile()
-        Write metadata to a file.
-    getTiffWriter()
-        Return a TiffWriter instance for saving TIFF files.
-    getZarrArray()
-        Return the Zarr array for saving Zarr files.
-    saveMetadata()
-        Save metadata to the current file.
-    finalize()
-        Finalize and clean up resources.
-    setDone(index, value)
-        Set the completion status for a specific stage.
-    '''
-
-    def __init__(self, temp_queue: Queue[float], display_queue: Queue[np.ndarray],
-             save_queue: Queue[tuple[np.ndarray, float]], path: str,
-             height: int, width: int, **kwargs) -> None:
-        '''Initialize the AcquisitionJob instance.
-
-        Parameters
-        ----------
-        temp_queue : Queue[float]
-            The queue for temporary data.
-        display_queue : Queue[np.ndarray]
-            The queue for display data.
-        save_queue : Queue[tuple[np.ndarray, float]]
-            The queue for data to be saved along with associated timestamps.
-        path : str
-            The base path where files will be saved.
-        height : int
-            The height of the image frames.
-        width : int
-            The width of the image frames.
-        **kwargs
-            Optional keyword arguments for customization.
-
-            Optional Parameters
-            -------------------
-            biggTiff : bool, optional
-                Flag indicating whether to use big TIFF format, by default True.
-            bytes_per_pixel : int, optional
-                The number of bytes per pixel, by default 1.
-            exposure : float, optional
-                The exposure time in milliseconds, by default 50.0.
-            frames : int, optional
-                The number of frames, by default 100.
-            full_tif_meta : bool, optional
-                Flag indicating whether to include full TIFF metadata, by default True.
-            is_dark_cal : bool, optional
-                Flag indicating whether dark calibration is enabled, by default False.
-            meta_file : str, optional
-                Additional metadata file path, by default ''.
-            meta_func : Callable, optional
-                A function to generate metadata, by default a lambda function.
-            name : str, optional
-                The name of the acquisition job, by default 'Camera'.
-            prefix : str, optional
-                A prefix for filenames, by default ''.
-            save : bool, optional
-                Flag indicating whether to save data, by default False.
-            Zarr : bool, optional
-                Flag indicating whether to use Zarr format, by default False.
-            rois : list[list[int]], optional
-                List of regions of interest, by default empty list.
-            seperate_rois : bool, optional
-                Flag indicating whether to save ROIs into seperate files,
-                by default False.
-                (For Zarr format different ROIs are treated as channels)
-            flip_rois : bool, optional
-                Flag indicating whether to flip n-th ROIs horizontally for n > 1,
-                by default True.
-        '''
-        self.display_queue = display_queue
-        self.height = height
-        self.cam_height = height
-        self.index = 0
-        self.lock = threading.Lock()
-        self.major = 0
-        self.path = path
-        self.save_queue = save_queue
-        self.temp_queue = temp_queue
-        self.timestamp = time.strftime('_%Y_%m_%d_%H%M%S')
-        self.width = width
-        self.cam_width = width
-        self.channels = 1
-        self.zarr_array = None
-
-        self.biggTiff: bool = kwargs.get('biggTiff', True)
-        self.bytes_per_pixel: int = kwargs.get('bytes_per_pixel', 1)
-        self.exposure: float = kwargs.get('exposure', 50.0)
-        self.frames: int = kwargs.get('frames', 100)
-        self.full_tif_meta: bool = kwargs.get('full_tif_meta', True)
-        self.is_dark_cal: bool = kwargs.get('is_dark_cal', False)
-        self.meta_file: str = kwargs.get('meta_file', '')
-        self.meta_func: Callable = kwargs.get('meta_func', lambda *args: '')
-        self.name: str = kwargs.get('name', 'Camera')
-        self.prefix: str = kwargs.get('prefix', '')
-        self.save: bool = kwargs.get('save', False)
-        '''cross-thread attribute (use lock)'''
-        self.zarr: bool = kwargs.get('Zarr', False)
-        self.rois: list[list[int]] = kwargs.get('rois', [])
-        self.seperate_rois: bool = kwargs.get('seperate_rois', False)
-        self.flip_rois: bool = kwargs.get('flip_rois', True)
-
-        if self.rois:
-            same_width = all(
-                [self.rois[0][2] == roi[2] for roi in self.rois])
-            same_height = all(
-                [self.rois[0][3] == roi[3] for roi in self.rois])
-            if not same_width or not same_height:
-                self.rois = None
-            else:
-                self.width = self.rois[0][2]
-                self.height = self.rois[0][3]
-                self.channels = len(self.rois)
-
-        self.capture_done = False
-        '''cross-thread attribute (use lock)'''
-        self.capture_time = 0.0
-        '''cross-thread attribute (use lock)'''
-        self.display_done = False
-        '''cross-thread attribute (use lock)'''
-        self.display_time = 0.0
-        '''cross-thread attribute (use lock)'''
-        self.frame = None
-        '''cross-thread attribute (use lock)'''
-        self.frames_captured = 0
-        '''cross-thread attribute (use lock)'''
-        self.frames_saved = 0
-        '''cross-thread attribute (use lock)'''
-        self.save_time = 0.0
-        '''cross-thread attribute (use lock)'''
-        self.stop_threads = False
-        '''cross-thread attribute (use lock)'''
-
-        self.tiffWriter: list[tf.TiffWriter] = []
-        self.dark_cal = None
-
-
-        if self.save:
-            if not os.path.exists(self.path):
-                os.makedirs(self.path)
-
-            while os.path.exists(self.getFilename()):
-                self.major += 1
-
-            self.writeMetaFile()
-
-    def getExt(self):
-        '''Return the file extension based on the Zarr attribute.
-
-        Returns
-        -------
-        str
-            File extension ('ome.tif' or 'zarr').
-        '''
-        return 'ome.tif' if not self.zarr else 'zarr'
-
-    def getFilename(self, roi_index: int=None) -> str:
-        '''Generate the filename based on the current state.
-
-        Parameters
-        ----------
-        roi_index : int, optional
-            the roi index for file name suffix, if None then not added. Default is None.
-
-        Returns
-        -------
-        str
-            Generated filename.
-        '''
-        roi_suffix = '' if roi_index is None else f'_ROI_{roi_index:02d}'
-        return self.path + \
-            f'{self.major:02d}_{self.prefix}_image_{self.index:05d}{roi_suffix}.{self.getExt()}'
-
-    def getTempFilename(self) -> str:
-        '''Generate the temperature log filename based on the current state.
-
-        Returns
-        -------
-        str
-            Generated temperature log filename.
-        '''
-        return self.path + self.prefix + \
-            f'{self.major:02d}_{self.prefix}_temp_log.csv'
-
-    def addDarkFrame(self, frame: np.ndarray):
-        '''Add a dark frame for calibration.
-
-        Parameters
-        ----------
-        frame : np.ndarray
-            Dark frame data.
-        '''
-        if self.is_dark_cal:
-            if self.dark_cal is None:
-                self.dark_cal = dark_calibration(
-                    frame.shape, self.exposure)
-            self.dark_cal.addFrame(frame)
-
-    def addFrame(self, frame: np.ndarray):
-        '''Add a frame to the acquisition job.
-
-        Parameters
-        ----------
-        frame : np.ndarray
-            Image frame data.
-        '''
-        if self.zarr:
-            if self.rois:
-                for idx, roi in enumerate(self.rois):
-                    roi_data = frame[
-                            roi[1]: roi[1] + roi[3],
-                            roi[0]: roi[0] + roi[2]]
-                    if idx > 0 and self.flip_rois:
-                        roi_data = np.fliplr(roi_data)
-
-                    self.getZarrArray()[self.frames_saved, idx, 0] = roi_data
-            else:
-                self.getZarrArray()[self.frames_saved, 0, 0] = frame
-        else:
-            if not self.tiffWriter:
-                if self.rois:
-                    if self.seperate_rois:
-                        for idx in range(len(self.rois)):
-                            self.tiffWriter.append(
-                                self.getTiffWriter(idx))
-                    else:
-                        self.tiffWriter.append(self.getTiffWriter())
-                else:
-                    self.tiffWriter.append(self.getTiffWriter())
-            # append frame to tiff
-            if self.rois:
-                if self.seperate_rois:
-                    for idx, roi in enumerate(self.rois):
-                        roi_data = frame[
-                                roi[1]: roi[1] + roi[3],
-                                roi[0]: roi[0] + roi[2]]
-                        if idx > 0 and self.flip_rois:
-                            roi_data = np.fliplr(roi_data)
-
-                        self.tiffWriter[idx] = self.writeTiffFrame(
-                            self.tiffWriter[idx],
-                            roi_data, idx)
-                else:
-                    data = np.zeros(
-                        (len(self.rois),
-                         self.rois[0][3], self.rois[0][2]), dtype=frame.dtype)
-                    for idx, roi in enumerate(self.rois):
-                        data[idx] = frame[
-                                roi[1]: roi[1] + roi[3],
-                                roi[0]: roi[0] + roi[2]]
-                        if idx > 0 and self.flip_rois:
-                            data[idx] = np.fliplr(data[idx])
-
-                    self.tiffWriter[0] = self.writeTiffFrame(
-                        self.tiffWriter[0], data)
-            else:
-                self.tiffWriter[0] = self.writeTiffFrame(
-                    self.tiffWriter[0], frame)
-
-    def writeTiffFrame(
-            self,
-            writer: tf.TiffWriter, frame: np.ndarray, roi_index=None):
-        '''writes an image into a Tiff file.
-
-        Parameters
-        ----------
-        writer : tf.TiffWriter
-            the TiffWriter class of the Tiff file.
-        frame : np.ndarray
-            Image frame data.
-        roi_index : int, optional
-            the roi index for file name suffix, if None then not added. Default is None.
-        '''
-
-        try:
-            writer.write(
-                data=frame[np.newaxis, np.newaxis, np.newaxis, ...
-                           ] if frame.ndim == 2 else frame[
-                               np.newaxis, :, np.newaxis, ...],
-                photometric='minisblack')
-        except ValueError as ve:
-            if str(ve) == \
-                    'data too large for standard TIFF file':
-                writer.close()
-                self.saveMetadata(roi_index)
-                self.frames_saved = 0
-                self.index += 1
-                writer = self.getTiffWriter(roi_index)
-                writer.write(
-                    data=frame[np.newaxis, np.newaxis, np.newaxis, ...
-                               ] if frame.ndim == 2 else frame[
-                                   np.newaxis, :, np.newaxis, ...],
-                    photometric='minisblack')
-            else:
-                raise ve
-
-        return writer
-
-    def addTemp(self, temp: float):
-        '''Add temperature data to the log file.
-
-        Parameters
-        ----------
-        temp : float
-            Temperature data.
-        '''
-        # open csv file and append sensor temp and close
-        with open(self.getTempFilename(), 'ab') as f:
-            np.savetxt(f, [temp], delimiter=';')
-
-    def getMetaFilename(self) -> str:
-        '''Return the metadata file path.
-
-        Returns
-        -------
-        str
-            Metadata file path.
-        '''
-        return self.path + self.name + self.timestamp + '.txt'
-
-    def writeMetaFile(self):
-        '''Write metadata to a file.'''
-        with open(self.getMetaFilename(), 'w+') as metaFile:
-            json.dump(self.meta_file, metaFile)
-
-    def getTiffWriter(self, roi_index: int =None) -> tf.TiffWriter:
-        '''Return a TiffWriter instance for saving TIFF files.
-
-        Parameters
-        ----------
-        roi_index : int, optional
-            the roi index for file name suffix, if None then not added. Default is None.
-
-        Returns
-        -------
-        tf.TiffWriter
-            TiffWriter instance.
-        '''
-        return tf.TiffWriter(
-            self.getFilename(roi_index), append=False,
-            bigtiff=self.biggTiff, ome=False)
-
-    def getZarrArray(self) -> zarr.Array:
-        '''Return the Zarr array for saving Zarr files.
-
-        Returns
-        -------
-        zarr.Array
-            Zarr array.
-        '''
-        if self.zarr_array is None:
-            self.zarr_array = zarr.open_array(
-                self.getFilename(),
-                shape=(self.frames, self.channels, 1, self.height, self.width),
-                compressor=None,
-                chunks=(1, 1, 1, self.height, self.width),
-                dtype=np.uint16)
-        return self.zarr_array
-
-    def saveMetadata(self, roi_index: int =None):
-        '''
-        Save metadata to the current file.
-
-        Parameters
-        ----------
-        roi_index : int, optional
-            the roi index for file name suffix, if None then not added. Default is None.
-        '''
-        ome: om.OME = self.meta_func(
-            self.frames_saved, self.width, self.height,
-            1 if self.seperate_rois else self.channels)
-
-        tf.tiffcomment(self.getFilename(roi_index), ome.to_xml())
-
-    def finalize(self):
-        '''Finalize and clean up resources.'''
-        if self.dark_cal is not None:
-            if self.dark_cal._counter > 1:
-                self.dark_cal.saveResults(
-                    self.path,
-                    f'{self.major:02d}_{self.prefix}')
-
-        if self.tiffWriter:
-            if self.rois and self.seperate_rois:
-                for idx, writer in enumerate(self.tiffWriter):
-                    writer.close()
-                    if self.save and not self.zarr:
-                        self.saveMetadata(idx)
-            else:
-                self.tiffWriter[0].close()
-                if self.save and not self.zarr:
-                    self.saveMetadata()
-
-    def setDone(self, index: int, value: bool):
-        '''Set the completion status for a specific stage.
-
-        Parameters
-        ----------
-        index : int
-            The index representing the stage (0 for capture, 1 for display, etc.).
-        value : bool
-            The completion status.
-        '''
-        if index == 0:
-            self.capture_done = value
-        elif index == 1:
-            self.display_done = value
+import json
+import os
+import threading
+import time
+from queue import Queue
+from typing import Callable
+
+import numpy as np
+import ome_types.model as om
+import tifffile as tf
+import zarr
+from PyQt5.QtCore import *
+from PyQt5.QtGui import *
+from PyQt5.QtWidgets import *
+
+from .camera_calibration import dark_calibration
+
+
+class AcquisitionJob:
+    '''A class holding cross-thread info required for an Acquisition Job.
+
+    Attributes
+    ----------
+    temp_queue : Queue[float]
+        The queue for temporary data.
+    display_queue : Queue[np.ndarray]
+        The queue for display data.
+    save_queue : Queue[tuple[np.ndarray, float]]
+        The queue for data to be saved along with associated timestamps.
+    path : str
+        The base path where files will be saved.
+    height : int
+        The height of the image frames.
+    width : int
+        The width of the image frames.
+    biggTiff : bool, optional
+        Flag indicating whether to use big TIFF format, by default True.
+    bytes_per_pixel : int, optional
+        The number of bytes per pixel, by default 1.
+    exposure : float, optional
+        The exposure time in milliseconds, by default 50.0.
+    frames : int, optional
+        The number of frames, by default 100.
+    full_tif_meta : bool, optional
+        Flag indicating whether to include full TIFF metadata, by default True.
+    is_dark_cal : bool, optional
+        Flag indicating whether dark calibration is enabled, by default False.
+    meta_file : str, optional
+        Additional metadata file path, by default ''.
+    meta_func : Callable, optional
+        A function to generate metadata, by default a lambda function.
+    name : str, optional
+        The name of the acquisition job, by default 'Camera'.
+    prefix : str, optional
+        A prefix for filenames, by default ''.
+    save : bool, optional
+        Flag indicating whether to save data, by default False.
+    Zarr : bool, optional
+        Flag indicating whether to use Zarr format, by default False.
+    rois : list[list[int]], optional
+        List of regions of interest, by default empty list.
+    seperate_rois : bool, optional
+        Flag indicating whether to save ROIs into seperate files,
+        by default False.
+        (For Zarr format different ROIs are treated as channels)
+    flip_rois : bool, optional
+        Flag indicating whether to flip n-th ROIs horizontally for n > 1,
+        by default True.
+
+
+    Methods
+    -------
+    getExt()
+        Return the file extension based on the Zarr attribute.
+    getFilename()
+        Generate the filename based on the current state.
+    getTempFilename()
+        Generate the temperatures filename based on the current state.
+    addDarkFrame(frame)
+        Add a dark frame for calibration.
+    addFrame(frame)
+        Add a frame to the acquisition job.
+    addTemp(temp)
+        Add temperature data to the acquisition job.
+    getMetaFilename()
+        Return the metadata file path.
+    writeMetaFile()
+        Write metadata to a file.
+    getTiffWriter()
+        Return a TiffWriter instance for saving TIFF files.
+    getZarrArray()
+        Return the Zarr array for saving Zarr files.
+    saveMetadata()
+        Save metadata to the current file.
+    finalize()
+        Finalize and clean up resources.
+    setDone(index, value)
+        Set the completion status for a specific stage.
+    '''
+
+    def __init__(self, temp_queue: Queue[float], display_queue: Queue[np.ndarray],
+             save_queue: Queue[tuple[np.ndarray, float]], path: str,
+             height: int, width: int, **kwargs) -> None:
+        '''Initialize the AcquisitionJob instance.
+
+        Parameters
+        ----------
+        temp_queue : Queue[float]
+            The queue for temporary data.
+        display_queue : Queue[np.ndarray]
+            The queue for display data.
+        save_queue : Queue[tuple[np.ndarray, float]]
+            The queue for data to be saved along with associated timestamps.
+        path : str
+            The base path where files will be saved.
+        height : int
+            The height of the image frames.
+        width : int
+            The width of the image frames.
+        **kwargs
+            Optional keyword arguments for customization.
+
+            Optional Parameters
+            -------------------
+            biggTiff : bool, optional
+                Flag indicating whether to use big TIFF format, by default True.
+            bytes_per_pixel : int, optional
+                The number of bytes per pixel, by default 1.
+            exposure : float, optional
+                The exposure time in milliseconds, by default 50.0.
+            frames : int, optional
+                The number of frames, by default 100.
+            full_tif_meta : bool, optional
+                Flag indicating whether to include full TIFF metadata, by default True.
+            is_dark_cal : bool, optional
+                Flag indicating whether dark calibration is enabled, by default False.
+            meta_file : str, optional
+                Additional metadata file path, by default ''.
+            meta_func : Callable, optional
+                A function to generate metadata, by default a lambda function.
+            name : str, optional
+                The name of the acquisition job, by default 'Camera'.
+            prefix : str, optional
+                A prefix for filenames, by default ''.
+            save : bool, optional
+                Flag indicating whether to save data, by default False.
+            Zarr : bool, optional
+                Flag indicating whether to use Zarr format, by default False.
+            rois : list[list[int]], optional
+                List of regions of interest, by default empty list.
+            seperate_rois : bool, optional
+                Flag indicating whether to save ROIs into seperate files,
+                by default False.
+                (For Zarr format different ROIs are treated as channels)
+            flip_rois : bool, optional
+                Flag indicating whether to flip n-th ROIs horizontally for n > 1,
+                by default True.
+        '''
+        self.display_queue = display_queue
+        self.height = height
+        self.cam_height = height
+        self.index = 0
+        self.lock = threading.Lock()
+        self.major = 0
+        self.path = path
+        self.save_queue = save_queue
+        self.temp_queue = temp_queue
+        self.timestamp = time.strftime('_%Y_%m_%d_%H%M%S')
+        self.width = width
+        self.cam_width = width
+        self.channels = 1
+        self.zarr_array = None
+
+        self.biggTiff: bool = kwargs.get('biggTiff', True)
+        self.bytes_per_pixel: int = kwargs.get('bytes_per_pixel', 1)
+        self.exposure: float = kwargs.get('exposure', 50.0)
+        self.frames: int = kwargs.get('frames', 100)
+        self.full_tif_meta: bool = kwargs.get('full_tif_meta', True)
+        self.is_dark_cal: bool = kwargs.get('is_dark_cal', False)
+        self.meta_file: str = kwargs.get('meta_file', '')
+        self.meta_func: Callable = kwargs.get('meta_func', lambda *args: '')
+        self.name: str = kwargs.get('name', 'Camera')
+        self.prefix: str = kwargs.get('prefix', '')
+        self.save: bool = kwargs.get('save', False)
+        '''cross-thread attribute (use lock)'''
+        self.zarr: bool = kwargs.get('Zarr', False)
+        self.rois: list[list[int]] = kwargs.get('rois', [])
+        self.seperate_rois: bool = kwargs.get('seperate_rois', False)
+        self.flip_rois: bool = kwargs.get('flip_rois', True)
+
+        if self.rois:
+            same_width = all(
+                [self.rois[0][2] == roi[2] for roi in self.rois])
+            same_height = all(
+                [self.rois[0][3] == roi[3] for roi in self.rois])
+            if not same_width or not same_height:
+                self.rois = None
+            else:
+                self.width = self.rois[0][2]
+                self.height = self.rois[0][3]
+                self.channels = len(self.rois)
+
+        self.capture_done = False
+        '''cross-thread attribute (use lock)'''
+        self.capture_time = 0.0
+        '''cross-thread attribute (use lock)'''
+        self.display_done = False
+        '''cross-thread attribute (use lock)'''
+        self.display_time = 0.0
+        '''cross-thread attribute (use lock)'''
+        self.frame = None
+        '''cross-thread attribute (use lock)'''
+        self.frames_captured = 0
+        '''cross-thread attribute (use lock)'''
+        self.frames_saved = 0
+        '''cross-thread attribute (use lock)'''
+        self.save_time = 0.0
+        '''cross-thread attribute (use lock)'''
+        self.stop_threads = False
+        '''cross-thread attribute (use lock)'''
+
+        self.c_event = threading.Event()
+        self.s_event = kwargs.get('s_event', threading.Event())
+
+        self.tiffWriter: list[tf.TiffWriter] = []
+        self.dark_cal = None
+
+
+        if self.save:
+            if not os.path.exists(self.path):
+                os.makedirs(self.path)
+
+            while os.path.exists(self.getFilename()):
+                self.major += 1
+
+            self.writeMetaFile()
+
+    def getExt(self):
+        '''Return the file extension based on the Zarr attribute.
+
+        Returns
+        -------
+        str
+            File extension ('ome.tif' or 'zarr').
+        '''
+        return 'ome.tif' if not self.zarr else 'zarr'
+
+    def getFilename(self, roi_index: int=None) -> str:
+        '''Generate the filename based on the current state.
+
+        Parameters
+        ----------
+        roi_index : int, optional
+            the roi index for file name suffix, if None then not added. Default is None.
+
+        Returns
+        -------
+        str
+            Generated filename.
+        '''
+        roi_suffix = '' if roi_index is None else f'_ROI_{roi_index:02d}'
+        return self.path + \
+            f'{self.major:02d}_{self.prefix}_image_{self.index:05d}{roi_suffix}.{self.getExt()}'
+
+    def getTempFilename(self) -> str:
+        '''Generate the temperature log filename based on the current state.
+
+        Returns
+        -------
+        str
+            Generated temperature log filename.
+        '''
+        return self.path + \
+            f'{self.major:02d}_{self.prefix}_temp_log.csv'
+
+    def addDarkFrame(self, frame: np.ndarray):
+        '''Add a dark frame for calibration.
+
+        Parameters
+        ----------
+        frame : np.ndarray
+            Dark frame data.
+        '''
+        if self.is_dark_cal:
+            if self.dark_cal is None:
+                self.dark_cal = dark_calibration(
+                    frame.shape, self.exposure)
+            self.dark_cal.addFrame(frame)
+
+    def addFrame(self, frame: np.ndarray):
+        '''Add a frame to the acquisition job.
+
+        Parameters
+        ----------
+        frame : np.ndarray
+            Image frame data.
+        '''
+        if self.zarr:
+            if self.rois:
+                for idx, roi in enumerate(self.rois):
+                    roi_data = frame[
+                            roi[1]: roi[1] + roi[3],
+                            roi[0]: roi[0] + roi[2]]
+                    if idx > 0 and self.flip_rois:
+                        roi_data = np.fliplr(roi_data)
+
+                    self.getZarrArray()[self.frames_saved, idx, 0] = roi_data
+            else:
+                self.getZarrArray()[self.frames_saved, 0, 0] = frame
+        else:
+            if not self.tiffWriter:
+                if self.rois:
+                    if self.seperate_rois:
+                        for idx in range(len(self.rois)):
+                            self.tiffWriter.append(
+                                self.getTiffWriter(idx))
+                    else:
+                        self.tiffWriter.append(self.getTiffWriter())
+                else:
+                    self.tiffWriter.append(self.getTiffWriter())
+            # append frame to tiff
+            if self.rois:
+                if self.seperate_rois:
+                    for idx, roi in enumerate(self.rois):
+                        roi_data = frame[
+                                roi[1]: roi[1] + roi[3],
+                                roi[0]: roi[0] + roi[2]]
+                        if idx > 0 and self.flip_rois:
+                            roi_data = np.fliplr(roi_data)
+
+                        self.tiffWriter[idx] = self.writeTiffFrame(
+                            self.tiffWriter[idx],
+                            roi_data, idx)
+                else:
+                    data = np.zeros(
+                        (len(self.rois),
+                         self.rois[0][3], self.rois[0][2]), dtype=frame.dtype)
+                    for idx, roi in enumerate(self.rois):
+                        data[idx] = frame[
+                                roi[1]: roi[1] + roi[3],
+                                roi[0]: roi[0] + roi[2]]
+                        if idx > 0 and self.flip_rois:
+                            data[idx] = np.fliplr(data[idx])
+
+                    self.tiffWriter[0] = self.writeTiffFrame(
+                        self.tiffWriter[0], data)
+            else:
+                self.tiffWriter[0] = self.writeTiffFrame(
+                    self.tiffWriter[0], frame)
+
+    def writeTiffFrame(
+            self,
+            writer: tf.TiffWriter, frame: np.ndarray, roi_index=None):
+        '''writes an image into a Tiff file.
+
+        Parameters
+        ----------
+        writer : tf.TiffWriter
+            the TiffWriter class of the Tiff file.
+        frame : np.ndarray
+            Image frame data.
+        roi_index : int, optional
+            the roi index for file name suffix, if None then not added. Default is None.
+        '''
+
+        try:
+            writer.write(
+                data=frame[np.newaxis, np.newaxis, np.newaxis, ...
+                           ] if frame.ndim == 2 else frame[
+                               np.newaxis, :, np.newaxis, ...],
+                photometric='minisblack')
+        except ValueError as ve:
+            if str(ve) == \
+                    'data too large for standard TIFF file':
+                writer.close()
+                self.saveMetadata(roi_index)
+                self.frames_saved = 0
+                self.index += 1
+                writer = self.getTiffWriter(roi_index)
+                writer.write(
+                    data=frame[np.newaxis, np.newaxis, np.newaxis, ...
+                               ] if frame.ndim == 2 else frame[
+                                   np.newaxis, :, np.newaxis, ...],
+                    photometric='minisblack')
+            else:
+                raise ve
+
+        return writer
+
+    def addTemp(self, temp: float):
+        '''Add temperature data to the log file.
+
+        Parameters
+        ----------
+        temp : float
+            Temperature data.
+        '''
+        # open csv file and append sensor temp and close
+        with open(self.getTempFilename(), 'ab') as f:
+            np.savetxt(f, [temp], delimiter=';')
+
+    def getMetaFilename(self) -> str:
+        '''Return the metadata file path.
+
+        Returns
+        -------
+        str
+            Metadata file path.
+        '''
+        return self.path + \
+            f'{self.major:02d}_{self.prefix}' + self.name.replace(
+                ' ', '_') + self.timestamp + '.json'
+
+    def writeMetaFile(self):
+        '''Write metadata to a file.'''
+        with open(self.getMetaFilename(), 'w+') as metaFile:
+            json.dump(self.meta_file, metaFile, indent=2)
+
+    def getTiffWriter(self, roi_index: int =None) -> tf.TiffWriter:
+        '''Return a TiffWriter instance for saving TIFF files.
+
+        Parameters
+        ----------
+        roi_index : int, optional
+            the roi index for file name suffix, if None then not added. Default is None.
+
+        Returns
+        -------
+        tf.TiffWriter
+            TiffWriter instance.
+        '''
+        return tf.TiffWriter(
+            self.getFilename(roi_index), append=False,
+            bigtiff=self.biggTiff, ome=False)
+
+    def getZarrArray(self) -> zarr.Array:
+        '''Return the Zarr array for saving Zarr files.
+
+        Returns
+        -------
+        zarr.Array
+            Zarr array.
+        '''
+        if self.zarr_array is None:
+            self.zarr_array = zarr.open_array(
+                self.getFilename(),
+                shape=(self.frames, self.channels, 1, self.height, self.width),
+                compressor=None,
+                chunks=(1, 1, 1, self.height, self.width),
+                dtype=np.uint16)
+        return self.zarr_array
+
+    def saveMetadata(self, roi_index: int =None):
+        '''
+        Save metadata to the current file.
+
+        Parameters
+        ----------
+        roi_index : int, optional
+            the roi index for file name suffix, if None then not added. Default is None.
+        '''
+        ome: om.OME = self.meta_func(
+            self.frames_saved, self.width, self.height,
+            1 if self.seperate_rois else self.channels)
+
+        tf.tiffcomment(self.getFilename(roi_index), ome.to_xml())
+
+    def finalize(self):
+        '''Finalize and clean up resources.'''
+        if self.dark_cal is not None:
+            if self.dark_cal._counter > 1:
+                self.dark_cal.saveResults(
+                    self.path,
+                    f'{self.major:02d}_{self.prefix}')
+
+        if self.tiffWriter:
+            if self.rois and self.seperate_rois:
+                for idx, writer in enumerate(self.tiffWriter):
+                    writer.close()
+                    if self.save and not self.zarr:
+                        self.saveMetadata(idx)
+            else:
+                self.tiffWriter[0].close()
+                if self.save and not self.zarr:
+                    self.saveMetadata()
+
+    def setDone(self, index: int, value: bool):
+        '''Set the completion status for a specific stage.
+
+        Parameters
+        ----------
+        index : int
+            The index representing the stage (0 for capture, 1 for display, etc.).
+        value : bool
+            The completion status.
+        '''
+        if index == 0:
+            self.capture_done = value
+        elif index == 1:
+            self.display_done = value
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/line_profiler.py` & `microEye-2.0.0/src/microEye/hardware/cams/line_profiler.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/thorlabs.py` & `microEye-2.0.0/src/microEye/hardware/cams/thorlabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,30 +645,30 @@
         output : bool, optional
             print out camera list, by default False
 
         Returns
         -------
         dict[str, object]
             dictionary containing
-            {camID, devID, senID, Status, InUse, Model, Serial}
+            {Camera ID, Device ID, Sensor ID, Status, InUse, Model, Serial}
         '''
         uc480 = windll.LoadLibrary(thorlabs_camera.uc480_file)
         cam_list = []
         cam_count = c_int(0)
         nRet = uc480.is_GetNumberOfCameras(byref(cam_count))
         if nRet == CMD.IS_SUCCESS and cam_count.value > 0:
             pucl = UC480_CAMERA_LIST(
                 UC480_CAMERA_INFO * cam_count.value)
             pucl.dwCount = cam_count.value
             if (uc480.is_GetCameraList(byref(pucl)) == CMD.IS_SUCCESS):
                 for index in range(cam_count.value):
                     cam_list.append({
-                        'camID': pucl.uci[index].dwCameraID,
-                        'devID': pucl.uci[index].dwDeviceID,
-                        'senID': pucl.uci[index].dwSensorID,
+                        'Camera ID': pucl.uci[index].dwCameraID,
+                        'Device ID': pucl.uci[index].dwDeviceID,
+                        'Sensor ID': pucl.uci[index].dwSensorID,
                         'Status': pucl.uci[index].dwStatus,
                         'InUse': pucl.uci[index].dwInUse,
                         'Model': pucl.uci[index].Model.decode('utf-8'),
                         'Serial': pucl.uci[index].SerNo.decode('utf-8'),
                         'Driver': 'Thorlabs DCx UC480'})
                 if output:
                     print(cam_list)
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/thorlabs_panel.py` & `microEye-2.0.0/src/microEye/hardware/cams/thorlabs_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     convert_rois_to_pos_size,
 )
 from ...shared.gui_helper import get_scaling_factor
 from ...shared.metadata_tree import MetaParams
 from ...shared.thread_worker import thread_worker
 from ...shared.uImage import uImage
 from ..widgets.qlist_slider import *
-from . import Camera_Panel
 from .camera_options import CamParams
+from .camera_panel import Camera_Panel
 from .thorlabs import *
 
 
 class ThorCamParams(Enum):
     PIXEL_CLOCK = 'Camera.Pixel Clock (MHz)'
     FRAMERATE = 'Camera.Framerate Slider'
     FRAME_AVERAGING = 'Camera.Frame Averaging'
@@ -56,29 +56,39 @@
 
 
 class Thorlabs_Panel(Camera_Panel):
     '''
     A Qt Widget for controlling a Thorlabs Camera | Inherits Camera_Panel
     '''
 
-    def __init__(self, threadpool, cam: thorlabs_camera,
+    def __init__(self, cam: thorlabs_camera,
                  mini: bool = False, *args, **kwargs):
         '''
-        Initializes a new Thorlabs_Panel Qt widget
-        | Inherits Camera_Panel
+        Initializes a new Thorlabs_Panel Qt widget.
+
+        Inherits Camera_Panel.
 
         Parameters
         ----------
-        threadpool : QThreadPool
-            The threadpool for multithreading
         cam : thorlabs_camera
-            Thorlabs Camera python adapter
+            Thorlabs Camera python adapter.
+
+        mini : bool, optional
+            Flag indicating if this is a mini camera panel, by default False.
+
+        Other Parameters
+        ---------------
+        *args
+            Arguments to pass to the Camera_Panel constructor.
+
+        **kwargs
+            Keyword arguments to pass to the Camera_Panel constructor.
         '''
         super().__init__(
-            threadpool, cam, mini,
+            cam, mini,
             *args, **kwargs)
 
         # flag true to close camera adapter and dispose it
         self._dispose_cam = False
 
         self.OME_tab.set_param_value(MetaParams.CHANNEL_NAME, self._cam.name)
         self.OME_tab.set_param_value(MetaParams.DET_MANUFACTURER, 'Thorlabs')
@@ -214,14 +224,21 @@
         save = {'name': str(ThorCamParams.SAVE), 'type': 'action'}
         self.camera_options.add_param_child(
             CamParams.CAMERA_OPTIONS, save)
         self.camera_options.get_param(
             ThorCamParams.SAVE).sigActivated.connect(
                 lambda: self.save_config())
 
+        # ROI
+        self.camera_options.set_roi_limits(
+            (0, self.cam.rectROI.s32Width),
+            (0, self.cam.rectROI.s32Height),
+            (32, self.cam.rectROI.s32Width),
+            (32, self.cam.rectROI.s32Height))
+
     @property
     def cam(self):
         '''The thorlabs_camera property.
 
         Returns
         -------
         thorlabs_camera
@@ -692,34 +709,14 @@
         ------
         NotImplementedError
             Has to be implemented by the use in child class.
         '''
         args = []
         return args
 
-    def get_meta(self):
-        meta = {
-            'Frames': self.camera_options.get_param_value(CamParams.FRAMES),
-            'model': self.cam.sInfo.strSensorName.decode('utf-8'),
-            'serial': self.cam.cInfo.SerNo.decode('utf-8'),
-            'clock speed': self.cam.pixel_clock.value,
-            'trigger': self.camera_options.get_param_value(ThorCamParams.TRIGGER_MODE),
-            'flash mode': self.camera_options.get_param_value(ThorCamParams.FLASH_MODE),
-            'framerate': self.cam.currentFrameRate.value,
-            'exposure': self.cam.exposure_current.value,
-            'flash duration': self.cam.flash_cur.u32Duration,
-            'flash delay': self.cam.flash_cur.s32Delay,
-            'ROI w': self.cam.set_rectROI.s32Width,
-            'ROI h': self.cam.set_rectROI.s32Height,
-            'ROI x': self.cam.set_rectROI.s32X,
-            'ROI y': self.cam.set_rectROI.s32Y,
-            'Zoom': self.camera_options.get_param_value(CamParams.RESIZE_DISPLAY),
-        }
-        return meta
-
     def save_config(self):
         filename, _ = QFileDialog.getSaveFileName(
             self, 'Save config', filter='JSON Files (*.json);;')
 
         if len(filename) > 0:
 
             config = {
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/ueye_camera.py` & `microEye-2.0.0/src/microEye/hardware/cams/ueye_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,29 +239,29 @@
         output : bool, optional
             print out camera list, by default False
 
         Returns
         -------
         dict[str, object]
             dictionary containing
-            {camID, devID, senID, Status, InUse, Model, Serial}
+            {Camera ID, Device ID, Sensor ID, Status, InUse, Model, Serial}
         '''
         cam_list = []
         cam_count = ueye.c_int(0)
         nRet = ueye.is_GetNumberOfCameras(cam_count)
         if nRet == ueye.IS_SUCCESS and cam_count > 0:
             pucl = ueye.UEYE_CAMERA_LIST(
                 ueye.UEYE_CAMERA_INFO * cam_count.value)
             pucl.dwCount = cam_count.value
             if (ueye.is_GetCameraList(pucl) == ueye.IS_SUCCESS):
                 for index in range(cam_count.value):
                     cam_list.append({
-                        'camID': pucl.uci[index].dwCameraID.value,
-                        'devID': pucl.uci[index].dwDeviceID.value,
-                        'senID': pucl.uci[index].dwSensorID.value,
+                        'Camera ID': pucl.uci[index].dwCameraID.value,
+                        'Device ID': pucl.uci[index].dwDeviceID.value,
+                        'Sensor ID': pucl.uci[index].dwSensorID.value,
                         'Status': pucl.uci[index].dwStatus.value,
                         'InUse': pucl.uci[index].dwInUse.value,
                         'Model': pucl.uci[index].Model.decode('utf-8'),
                         'Serial': pucl.uci[index].SerNo.decode('utf-8'),
                         'Driver': 'uEye'})
                 if output:
                     print(cam_list)
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/ueye_panel.py` & `microEye-2.0.0/src/microEye/hardware/cams/ueye_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     convert_rois_to_pos_size,
 )
 from ...shared.gui_helper import get_scaling_factor
 from ...shared.metadata_tree import MetaParams
 from ...shared.thread_worker import thread_worker
 from ...shared.uImage import uImage
 from ..widgets.qlist_slider import *
-from . import Camera_Panel, IDS_Camera
 from .camera_options import CamParams
+from .camera_panel import Camera_Panel
+from .ueye_camera import IDS_Camera
 
 try:
     from pyueye import ueye
 except Exception:
     ueye = None
 
 
@@ -55,29 +56,39 @@
         return self.value.split('.')
 
 class IDS_Panel(Camera_Panel):
     '''
     A Qt Widget for controlling an IDS Camera | Inherits Camera_Panel
     '''
 
-    def __init__(self, threadpool: QThreadPool, cam: IDS_Camera, mini=False,
+    def __init__(self, cam: IDS_Camera, mini=False,
                  *args, **kwargs):
         '''
-        Initializes a new IDS_Panel Qt widget
-        | Inherits Camera_Panel
+        Initializes a new IDS_Panel Qt widget.
+
+        Inherits Camera_Panel.
 
         Parameters
         ----------
-        threadpool : QThreadPool
-            The threadpool for multithreading
         cam : IDS_Camera
-            IDS Camera python adapter
+            IDS Camera python adapter.
+
+        mini : bool, optional
+            Flag indicating if this is a mini camera panel, by default False.
+
+        Other Parameters
+        ---------------
+        *args
+            Arguments to pass to the Camera_Panel constructor.
+
+        **kwargs
+            Keyword arguments to pass to the Camera_Panel constructor.
         '''
         super().__init__(
-            threadpool, cam, mini,
+            cam, mini,
             *args, **kwargs)
 
         # flag true to close camera adapter and dispose it
         self._dispose_cam = False
 
         self.OME_tab.set_param_value(MetaParams.CHANNEL_NAME, self._cam.name)
         self.OME_tab.set_param_value(MetaParams.DET_MANUFACTURER, 'IDS uEye')
@@ -222,14 +233,21 @@
         save = {'name': str(uEyeParams.SAVE), 'type': 'action'}
         self.camera_options.add_param_child(
             CamParams.CAMERA_OPTIONS, save)
         self.camera_options.get_param(
             uEyeParams.SAVE).sigActivated.connect(
                 lambda: self.save_config())
 
+        # ROI
+        self.camera_options.set_roi_limits(
+            (0, self.cam.rectROI.s32Width.value),
+            (0, self.cam.rectROI.s32Height.value),
+            (32, self.cam.rectROI.s32Width.value),
+            (32, self.cam.rectROI.s32Height.value))
+
     @property
     def cam(self):
         '''The IDS_Camera property.
 
         Returns
         -------
         IDS_Camera
@@ -660,15 +678,15 @@
                     self._buffer.put(data.copy())
                     # add sensor temperature to the stack
                     self._temps.put(self._cam.get_temperature())
                     self.acq_job.frames_captured = \
                         self.acq_job.frames_captured + 1
                     if self.acq_job.frames_captured >= self.acq_job.frames \
                             and not self.mini:
-                        self.c_event.set()
+                        self.acq_job.c_event.set()
                         self.acq_job.stop_threads = True
                         logging.debug('Stop')
                     self._cam.unlock_buffer()
 
                 QThread.usleep(100)  # sleep 100us
 
                 if self.acq_job.stop_threads:
@@ -704,34 +722,14 @@
         ------
         NotImplementedError
             Has to be implemented by the use in child class.
         '''
         args = []
         return args
 
-    def get_meta(self):
-        meta = {
-            'Frames': self.camera_options.get_param_value(CamParams.FRAMES),
-            'model': self.cam.sInfo.strSensorName.decode('utf-8'),
-            'serial': self.cam.cInfo.SerNo.decode('utf-8'),
-            'clock speed': self.cam.pixel_clock.value,
-            'trigger': self.camera_options.get_param_value(uEyeParams.TRIGGER_MODE),
-            'flash mode': self.camera_options.get_param_value(uEyeParams.FLASH_MODE),
-            'framerate': self.cam.currentFrameRate.value,
-            'exposure': self.cam.exposure_current.value,
-            'flash duration': self.cam.flash_cur.u32Duration.value,
-            'flash delay': self.cam.flash_cur.s32Delay.value,
-            'ROI w': self.cam.set_rectROI.s32Width.value,
-            'ROI h': self.cam.set_rectROI.s32Height.value,
-            'ROI x': self.cam.set_rectROI.s32X.value,
-            'ROI y': self.cam.set_rectROI.s32Y.value,
-            'Zoom': self.camera_options.get_param_value(CamParams.RESIZE_DISPLAY),
-        }
-        return meta
-
     def save_config(self):
         filename, _ = QFileDialog.getSaveFileName(
             self, 'Save config', filter='JSON Files (*.json);;')
 
         if len(filename) > 0:
 
             config = {
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/vimba_cam.py` & `microEye-2.0.0/src/microEye/hardware/cams/vimba_cam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-
 import contextlib
 from typing import Optional
 
 import numpy as np
+from tabulate import tabulate
 
 from .micam import miCamera
 
 try:
     import vimba as vb
 
     def get_camera_list():
         cam_list = []
         with vb.Vimba.get_instance() as vimba:
             cams = vimba.get_all_cameras()
             for cam in cams:
                 cam_list.append({
-                            'camID': cam.get_id(),
-                            'devID': cam.get_interface_id(),
-                            'senID': 'NA',
+                            'Camera ID': cam.get_id(),
+                            'Device ID': cam.get_interface_id(),
+                            'Sensor ID': 'NA',
                             'Status': 'NA',
                             'InUse': 0,
                             'Model': cam.get_model(),
                             'Serial': cam.get_serial(),
                             'Driver': 'Vimba',
                             'Name': cam.get_name()})
         return cam_list
 
-    def get_camera(camera_id: Optional[str]) -> vb.Camera:
+    def get_camera(camera_id: Optional[str]) -> vb.Camera: # type: ignore
         with vb.Vimba.get_instance() as vimba:
             if camera_id:
                 try:
                     return vimba.get_camera_by_id(camera_id)
                 except vb.VimbaCameraError:
                     print(
                         f"Failed to access Camera '{camera_id}'. Abort.")
             else:
                 cams = vimba.get_all_cameras()
                 if not cams:
                     print('No Cameras accessible. Abort.')
                     return None
 
                 return cams[0]
-
 except Exception:
     vb = None
 
     def get_camera_list():
         return []
 
     def get_camera(camera_id: Optional[str]):
@@ -123,39 +122,100 @@
         self.pixel_formats = []
 
         self.initialize()
 
     def initialize(self):
         with self.cam:
             self.default()
-            self.getAcquisitionFrameRateEnable()
-            self.getFrameRate()
-            self.get_exposure()
-            self.get_exposure_mode()
-            self.get_exposure_auto()
-            self.get_trigger_source()
-            self.get_trigger_selector()
-            self.get_trigger_mode()
-            self.get_trigger_activation()
-            self.get_acquisition_mode()
-            self.get_pixel_format()
-            self.get_pixel_size()
-            self.get_roi()
+            self.getAcquisitionFrameRateEnable(False)
+            self.getFrameRate(False)
+            self.get_exposure(False)
+            self.get_exposure_mode(False)
+            self.get_exposure_auto(False)
+            self.get_trigger_source(False)
+            self.get_trigger_selector(False)
+            self.get_trigger_mode(False)
+            self.get_trigger_activation(False)
+            self.get_acquisition_mode(False)
+            self.get_pixel_format(False)
+            self.get_pixel_size(False)
+            self.get_roi(False)
             self.get_temperature()
 
             self.trigger_modes = self.get_trigger_modes()
             self.trigger_sources = self.get_trigger_sources()
             self.trigger_selectors = self.get_trigger_selectors()
             self.trigger_activations = self.get_trigger_activations()
 
             self.exposure_modes = self.get_exposure_modes()
             self.exposure_auto_entries = self.get_exposure_auto_entries()
 
             self.pixel_formats = self.get_pixel_formats()
 
+            self.print_status()
+
+    def populate_status(self):
+        self.status['Camera'] = {
+            'Name': self.name
+        }
+
+        self.status['Temperature'] = {
+            'Value': self.temperature,
+            'Unit': 'Celsius'
+        }
+
+        self.status['Exposure'] = {
+            'Mode': self.exposure_mode,
+            'Value': self.exposure_current,
+            'Unit': self.exposure_unit,
+            'Increment': self.exposure_increment,
+            'Auto': self.exposure_auto
+        }
+
+        self.status['Framerate'] = {
+            'Value': self.frameRate,
+            'Unit': self.frameRate_unit,
+            'Range': self.frameRate_range,
+            'Increment': self.frameRate_increment,
+            'Enabled': self.frameRateEnabled
+        }
+
+        self.status['Acquisition'] = {
+            'Mode': self.acquisition_mode,
+            'Enabled': self.acquisition
+        }
+
+        # self.status['Trigger'] = {
+        #     'source': self.trigger_source,
+        #     'selector': self.trigger_selector,
+        #     'activation': self.trigger_activation,
+        # }
+        self.status['Image Format'] = {
+            'Pixel Format': self.pixel_format,
+            'Pixel Size': self.pixel_size,
+            'Bytes per Pixel': self.bytes_per_pixel
+        }
+
+        self.status['Image Size'] = {
+            'Width': self.width,
+            'Width_max': self.width_max,
+            'Width_range': self.width_range,
+            'Width_inc': self.width_inc,
+            'Height': self.height,
+            'Height_max': self.height_max,
+            'Height_range': self.height_range,
+            'Height_inc': self.height_inc,
+            'Offset_x': self.offsetX,
+            'Offset_x_range': self.offsetX_range,
+            'Offset_x_inc': self.offsetX_inc,
+            'Offset_y': self.offsetY,
+            'Offset_y_range': self.offsetY_range,
+            'Offset_y_inc': self.offsetY_inc
+        }
+
     def default(self):
         # with self.cam:
         # Restore settings to initial value.
         try:
             self.cam.UserSetSelector.set('Default')
 
         except (AttributeError, vb.VimbaFeatureError):
@@ -262,20 +322,21 @@
             if value in entries:
                 ExposureMode.set(value)
             return 1
         except Exception:
             print('ExposureMode Set ERROR')
             return 0
 
-    def get_exposure_mode(self):
+    def get_exposure_mode(self, output=True):
         try:
             # with self.cam:
             ExposureMode = self.cam.ExposureMode
             self.exposure_mode = ExposureMode.get()
-            print('Exposure mode ', self.exposure_mode)
+            if output:
+                print('Exposure mode ', self.exposure_mode)
             return self.exposure_mode
         except Exception:
             print('ExposureMode get ERROR')
             return 'NA'
 
     def get_exposure_modes(self):
         modes = []
@@ -306,20 +367,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('ExposureAuto Set ERROR')
             return 0
 
-    def get_exposure_auto(self):
+    def get_exposure_auto(self, output=True):
         try:
             # with self.cam:
             ExposureAuto = self.cam.ExposureAuto
             self.exposure_auto = ExposureAuto.get()
-            print('Exposure Auto ', self.exposure_auto)
+            if output:
+                print('Exposure Auto ', self.exposure_auto)
             return self.exposure_auto
         except Exception:
             print('ExposureAuto get ERROR')
             return 'NA'
 
     def get_exposure_auto_entries(self):
         modes = []
@@ -406,20 +468,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('trigger Set ERROR')
             return 0
 
-    def get_trigger_mode(self):
+    def get_trigger_mode(self, output=True):
         try:
             # with self.cam:
             TriggerMode = self.cam.TriggerMode
             self.trigger_mode = TriggerMode.get()
-            print('Trigger mode ', self.trigger_mode)
+            if output:
+                print('Trigger mode ', self.trigger_mode)
             return self.trigger_mode
         except Exception:
             print('trigger get ERROR')
             return 'NA'
 
     def get_trigger_modes(self):
         modes = []
@@ -450,20 +513,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('trigger source Set ERROR')
             return 0
 
-    def get_trigger_source(self):
+    def get_trigger_source(self, output=True):
         try:
             # with self.cam:
             TriggerSource = self.cam.TriggerSource
             self.trigger_source = TriggerSource.get()
-            print('Trigger source ', self.trigger_source)
+            if output:
+                print('Trigger source ', self.trigger_source)
             return self.trigger_source
         except Exception:
             print('trigger source get ERROR')
             return 'NA'
 
     def get_trigger_sources(self):
         sources = []
@@ -494,20 +558,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('trigger selector Set ERROR')
             return 0
 
-    def get_trigger_selector(self):
+    def get_trigger_selector(self, output=True):
         try:
             # with self.cam:
             TriggerSelector = self.cam.TriggerSelector
             self.trigger_selector = TriggerSelector.get()
-            print('Trigger selector ', self.trigger_selector)
+            if output:
+                print('Trigger selector ', self.trigger_selector)
             return self.trigger_selector
         except Exception:
             print('trigger selector get ERROR')
             return 'NA'
 
     def get_trigger_selectors(self):
         selectors = []
@@ -537,20 +602,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('TriggerActivation Set ERROR')
             return 0
 
-    def get_trigger_activation(self):
+    def get_trigger_activation(self, output=True):
         try:
             # with self.cam:
             TriggerActivation = self.cam.TriggerActivation
             self.trigger_activation = TriggerActivation.get()
-            print('Trigger activation ', self.trigger_activation)
+            if output:
+                print('Trigger activation ', self.trigger_activation)
             return self.trigger_activation
         except Exception:
             print('TriggerActivation get ERROR')
             return 'NA'
 
     def get_trigger_activations(self):
         activations = []
@@ -580,20 +646,21 @@
                 return 1
             else:
                 return 0
         except Exception:
             print('AcquisitionMode Set ERROR')
             return 0
 
-    def get_acquisition_mode(self):
+    def get_acquisition_mode(self, output=True):
         try:
             # with self.cam:
             AcquisitionMode = self.cam.AcquisitionMode
             self.acquisition_mode = AcquisitionMode.get()
-            print('Acquisition mode ', self.acquisition_mode)
+            if output:
+                print('Acquisition mode ', self.acquisition_mode)
             return self.acquisition_mode
         except Exception:
             print('AcquisitionMode get ERROR')
             return 'NA'
 
     def get_acquisition_modes(self):
         modes = []
@@ -620,20 +687,21 @@
             fmts = self.cam.get_pixel_formats()
             formats += map(str, fmts)
         except Exception:
             print('Pixel Formats Get ERROR')
 
         return formats
 
-    def get_pixel_format(self):
+    def get_pixel_format(self, output=True):
         formats = []
         try:
             # with self.cam:
             self.pixel_format = self.cam.get_pixel_format()
-            print('Pixel Format', self.pixel_format)
+            if output:
+                print('Pixel Format', self.pixel_format)
             return self.pixel_format
         except Exception:
             print('Pixel Format Get ERROR')
             return 'NA'
 
     def set_pixel_format(self, value: str):
         try:
@@ -659,20 +727,21 @@
                 return self.pixel_size
             else:
                 print('Pixel Format Not supported.')
                 return 'NA'
         finally:
             self.set_black_level(5.0)
 
-    def get_pixel_size(self):
+    def get_pixel_size(self, output=True):
         try:
             # with self.cam:
             self.pixel_size = self.cam.PixelSize.get()
             self.bytes_per_pixel = int(np.ceil(int(self.pixel_size)/8))
-            print('Pixel Format', self.pixel_size)
+            if output:
+                print('Pixel Size', self.pixel_size)
             return self.pixel_size
         except Exception:
             print('Pixel Size Get ERROR')
             return 'NA'
 
     def get_io_lines(self):
         try:
```

### Comparing `microEye-1.0.5/src/microEye/hardware/cams/vimba_panel.py` & `microEye-2.0.0/src/microEye/hardware/cams/vimba_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     convert_rois_to_pos_size,
 )
 from ...shared.gui_helper import get_scaling_factor
 from ...shared.metadata_tree import MetaParams
 from ...shared.thread_worker import thread_worker
 from ...shared.uImage import uImage
 from ..widgets.qlist_slider import *
-from . import Camera_Panel, vimba_cam
 from .camera_options import CamParams
+from .camera_panel import Camera_Panel
+from .vimba_cam import vimba_cam
 
 try:
     import vimba as vb
 except Exception:
     vb = None
 
 class VimbaParams(Enum):
@@ -69,30 +70,38 @@
 
 class Vimba_Panel(Camera_Panel):
     '''
     A Qt Widget for controlling an Allied Vision Camera through Vimba
      | Inherits Camera_Panel
     '''
 
-    def __init__(self, threadpool: QThreadPool, cam: vimba_cam, mini=False,
+    def __init__(self, cam: vimba_cam, mini=False,
                  *args, **kwargs):
         '''
-        Initializes a new Vimba_Panel Qt widget
-        | Inherits Camera_Panel
+        Initializes a new Vimba_Panel Qt widget.
+
+        Inherits Camera_Panel.
 
         Parameters
         ----------
-        threadpool : QThreadPool
-            The threadpool for multithreading
         cam : vimba_cam
-            Vimba Camera python adapter
+            Vimba Camera python adapter.
+
+        mini : bool, optional
+            Flag indicating if this is a mini camera panel, by default False.
+
+        Other Parameters
+        ---------------
+        *args
+            Arguments to pass to the Camera_Panel constructor.
+
+        **kwargs
+            Keyword arguments to pass to the Camera_Panel constructor.
         '''
-        super().__init__(
-            threadpool, cam, mini,
-            *args, **kwargs)
+        super().__init__(cam, mini, *args, **kwargs)
 
         self.OME_tab.set_param_value(MetaParams.CHANNEL_NAME, self._cam.name)
         self.OME_tab.set_param_value(MetaParams.DET_MANUFACTURER, 'Allied Vision')
         self.OME_tab.set_param_value(MetaParams.DET_MODEL, self._cam.cam.get_model())
         self.OME_tab.set_param_value(MetaParams.DET_SERIAL,
             self._cam.cam.get_serial())
         self.OME_tab.set_param_value(MetaParams.DET_TYPE,
@@ -370,19 +379,19 @@
         self.camera_options.get_param(
             VimbaParams.TIMER_RESET).sigActivated.connect(reset_timer)
         self.camera_options.get_param(
             VimbaParams.SET_TIMER_CONFIG).sigActivated.connect(set_timer)
 
     @property
     def cam(self):
-        '''The IDS_Camera property.
+        '''The vimba_cam property.
 
         Returns
         -------
-        IDS_Camera
+        vimba_cam
             the cam property value
         '''
         return self._cam
 
     @cam.setter
     def cam(self, cam: vimba_cam):
         '''The vimba_cam property.
@@ -682,17 +691,18 @@
             self._buffer.put(frame.as_numpy_ndarray()[..., 0])
             cam.queue_frame(frame)
             # add sensor temperature to the stack
             self._temps.put(self.cam.get_temperature())
             self.acq_job.frames_captured = self.acq_job.frames_captured + 1
         if self.acq_job.frames_captured > self.acq_job.frames - 1 and \
                 not self.mini:
-            self.c_event.set()
+            self.acq_job.c_event.set()
             self.acq_job.stop_threads = True
             logging.debug('Stop')
+            print('Capture Stopped!')
 
     def cam_capture(self, *args):
         '''Capture function executed by the capture worker.
 
         Sends software trigger signals and transfers the
         acquired frame to the display processing stack.
 
@@ -702,15 +712,15 @@
             the vimba_cam used to acquire frames.
         '''
         try:
             # Continuous image capture
             with self._cam.cam:
                 self._cam.cam.start_streaming(self._capture_handler)
 
-                self.c_event.wait()
+                self.acq_job.c_event.wait()
         except Exception:
             traceback.print_exc()
         finally:
             # reset flags and release resources
             with self._cam.cam:
                 self._cam.cam.stop_streaming()
             self._cam.acquisition = False
@@ -735,23 +745,14 @@
         ------
         NotImplementedError
             Has to be implemented by the use in child class.
         '''
         args = []
         return args
 
-    def get_meta(self):
-        with self._cam.cam:
-            meta = {
-                'Exposure': self._cam.exposure_current,
-                'ROI': self._cam.get_roi(False),
-                'Frames': self.camera_options.get_param_value(CamParams.FRAMES)
-            }
-        return meta
-
     def save_config(self):
         filename, _ = QFileDialog.getSaveFileName(
             self, 'Save config', filter='XML Files (*.xml);;')
 
         if len(filename) > 0:
 
             with self.cam.cam:
```

### Comparing `microEye-1.0.5/src/microEye/hardware/misc/acquisition_view.py` & `microEye-2.0.0/src/microEye/hardware/misc/acquisition_view.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/misc/reglo.py` & `microEye-2.0.0/src/microEye/hardware/misc/reglo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import qdarkstyle
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtSerialPort import *
 from PyQt5.QtWidgets import *
 
+from ...shared import StartGUI
+
 
 class RegloDigital(QSerialPort):
 
     _ACK_ = '*'
     _ERR_ = '#'
     _YES_ = '+'
     _NO_ = '-'
@@ -372,15 +374,15 @@
         # Statues Bar Timer
         self.timer = QTimer()
         self.timer.setInterval(10)
         self.timer.timeout.connect(self.update_gui)
         self.timer.start()
 
         # Threading
-        self._threadpool = QThreadPool()
+        self._threadpool = QThreadPool.globalInstance()
         print('Multithreading with maximum %d threads'
               % self._threadpool.maxThreadCount())
 
         self.show()
 
         # centered
         self.center()
@@ -728,52 +730,16 @@
         -------
         app, window = reglo_digital_module.StartGUI()
 
         app.exec_()
 
         Returns
         -------
-        tuple (QApplication, microEye.reglo_digital_module)
+        tuple (QApplication, reglo_digital_module)
             Returns a tuple with QApp and reglo_digital_module main window.
         '''
-        # create a QApp
-        app = QApplication(sys.argv)
-        # set darkmode from *qdarkstyle* (not compatible with pyqt6)
-        app.setStyleSheet(qdarkstyle.load_stylesheet(qt_api='pyqt5'))
-        font = app.font()
-        font.setPointSize(12)
-        app.setFont(font)
-        # sets the app icon
-        dirname = os.path.dirname(os.path.abspath(__file__))
-        app_icon = QIcon()
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/16.png'), QSize(16, 16))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/24.png'), QSize(24, 24))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/32.png'), QSize(32, 32))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/48.png'), QSize(48, 48))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/64.png'), QSize(64, 64))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/128.png'), QSize(128, 128))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/256.png'), QSize(256, 256))
-        app_icon.addFile(
-            os.path.join(dirname, '../icons/512.png'), QSize(512, 512))
-
-        app.setWindowIcon(app_icon)
-
-        if sys.platform.startswith('win'):
-            import ctypes
-            myappid = 'samhitech.mircoEye.reglo_digital_module'  # appid
-            ctypes.windll.shell32.\
-                SetCurrentProcessExplicitAppUserModelID(myappid)
-
-        window = reglo_digital_module()
-        return app, window
+        return StartGUI(reglo_digital_module)
 
 
 if __name__ == '__main__':
     app, window = reglo_digital_module.StartGUI()
     app.exec_()
```

### Comparing `microEye-1.0.5/src/microEye/hardware/protocols/actions.py` & `microEye-2.0.0/src/microEye/hardware/protocols/actions.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/stages/elliptec.py` & `microEye-2.0.0/src/microEye/hardware/stages/elliptec.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/hardware/stages/kinesis.py` & `microEye-2.0.0/src/microEye/hardware/stages/kinesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,22 @@
         '''Closes the supplied serial port.'''
         self.serial.close()
 
 
 class KinesisXY:
     '''Class for controlling Two Kinesis Devices as an XY Stage'''
 
-    def __init__(self, x_port='COM12', y_port='COM11',
-                 threadpool: QThreadPool = None):
+    def __init__(self, x_port='COM12', y_port='COM11'):
         self.X_Kinesis = KinesisDevice(x_port)
         self.Y_Kinesis = KinesisDevice(y_port)
         self.position = [0, 0]
         self.min = [0, 0]
         self.max = [25, 25]
         self.prec = 4
-        self.threadpool = threadpool
+        self.threadpool = QThreadPool.globalInstance()
 
     def home(self):
         self.X_Kinesis.home()
         self.Y_Kinesis.home()
         self.position = [0, 0]
         return self.X_Kinesis.wait(), self.Y_Kinesis.wait()
 
@@ -374,21 +373,21 @@
                 self.move_relative,
                 0,
                 self.jump_spin.value()
             )
         )
 
         self.n_x_step_btn.setStyleSheet(
-            'background-color: green')
+            'background-color: #004CB6')
         self.n_y_step_btn.setStyleSheet(
-            'background-color: green')
+            'background-color: #004CB6')
         self.p_x_step_btn.setStyleSheet(
-            'background-color: green')
+            'background-color: #004CB6')
         self.p_y_step_btn.setStyleSheet(
-            'background-color: green')
+            'background-color: #004CB6')
 
         grid = QGridLayout()
         grid.addWidget(self.n_x_jump_btn, 2, 0)
         grid.addWidget(self.n_x_step_btn, 2, 1)
         grid.addWidget(self.p_x_step_btn, 2, 3)
         grid.addWidget(self.p_x_jump_btn, 2, 4)
```

### Comparing `microEye-1.0.5/src/microEye/hardware/widgets/qlist_slider.py` & `microEye-2.0.0/src/microEye/hardware/widgets/qlist_slider.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/1024.png` & `microEye-2.0.0/src/microEye/icons/1024.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/128.png` & `microEye-2.0.0/src/microEye/icons/128.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/16.png` & `microEye-2.0.0/src/microEye/icons/16.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/256.png` & `microEye-2.0.0/src/microEye/icons/256.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/32.png` & `microEye-2.0.0/src/microEye/icons/32.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/512.png` & `microEye-2.0.0/src/microEye/icons/512.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/icons/64.png` & `microEye-2.0.0/src/microEye/icons/64.png`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/expandable_groupbox.py` & `microEye-2.0.0/src/microEye/shared/expandable_groupbox.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/gui_helper.py` & `microEye-2.0.0/src/microEye/shared/gui_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, overload
+from typing import Union
 
 import numpy as np
 from PyQt5.QtWidgets import (
     QApplication,
     QCheckBox,
     QComboBox,
     QDoubleSpinBox,
```

### Comparing `microEye-1.0.5/src/microEye/shared/labelled_slider.py` & `microEye-2.0.0/src/microEye/shared/labelled_slider.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/metadata.py` & `microEye-2.0.0/src/microEye/shared/metadata.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/metadata_tree.py` & `microEye-2.0.0/src/microEye/shared/metadata_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from ome_types.model.simple_types import PixelType, UnitsLength, UnitsTime
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 from pyqtgraph.parametertree import Parameter, ParameterTree
 from pyqtgraph.parametertree.parameterTypes import ActionParameter, GroupParameter
 
+from .parameter_tree import Tree
+
 
 class MetaParams(Enum):
     '''
     Enum class defining metadata parameters.
     '''
     EXPERIMENT_NAME = 'Experiment.Name'
     EXP_DESC = 'Experiment.Description'
@@ -71,15 +73,15 @@
 
     def get_path(self):
         '''
         Return the full parameter path.
         '''
         return self.value.split('.')
 
-class MetadataEditorTree(ParameterTree):
+class MetadataEditorTree(Tree):
     '''
     Tree widget for editing metadata parameters.
 
     Attributes
     ----------
     paramsChanged : pyqtSignal
         Signal for parameter changed event.
@@ -88,25 +90,14 @@
         List of dichroic suggestions, adjust to fit your setup.
     EMISSION_FILTERS : list
         List of emission filter suggestions, adjust to fit your setup.
     EXCITATION_FILTERS : list
         List of excitation filter suggestions, adjust to fit your setup.
     '''
 
-    paramsChanged = pyqtSignal(GroupParameter, list)
-    '''Signal emitted when parameters are changed.
-
-    Parameters
-    ----------
-    GroupParameter
-        The group parameter that was changed.
-    list
-        A list of changes made to the parameter.
-    '''
-
     DICHROIC_SUGGESTIONS = [
         'EM 550 Longpass',
         'EM 640 Longpass',
         'EX 405/488/532/640 2mm MultiBand',
         'EX 405/488/561/635 3mm MultiBand',
         'EX 488/640 2mm MultiBand',
         'EX 405/514/647 2mm MultiBand',
@@ -150,19 +141,15 @@
         Initialize the MetadataEditorTree.
 
         Parameters
         ----------
         parent : QWidget, optional
             The parent widget, by default None.
         '''
-        super().__init__()
-
-        self.setMinimumWidth(50)
-        self.create_parameters()
-        self.setParameters(self.param_tree, showTop=False)
+        super().__init__(parent=parent)
 
     def create_parameters(self):
         '''
         Create the parameter tree structure.
         '''
         params = [
             {'name': 'Experiment', 'type': 'group', 'children': [
@@ -259,15 +246,15 @@
                 {'name': str(MetaParams.IMPORT_XML), 'type': 'action'},
             ]},
         ]
 
         self.param_tree = Parameter.create(name='root', type='group', children=params)
         self.param_tree.sigTreeStateChanged.connect(self.change)
         self.header().setSectionResizeMode(
-            QHeaderView.ResizeMode.Stretch)
+            QHeaderView.ResizeMode.ResizeToContents)
 
         self.get_param(
             MetaParams.DICHROIC_MODEL_BTN).sigActivated.connect(
                 lambda: self.add_param_child(
                     MetaParams.DICHROIC_MODEL_LIST,
                     MetaParams.DICHROIC_MODEL))
         self.get_param(
@@ -286,88 +273,14 @@
         self.get_param(
             MetaParams.EXPORT_STATE).sigActivated.connect(self.export_json)
         self.get_param(
             MetaParams.IMPORT_XML).sigActivated.connect(self.load_xml)
         self.get_param(
             MetaParams.EXPORT_XML).sigActivated.connect(self.save)
 
-    def get_param(
-            self, param: MetaParams
-            ) -> Union[Parameter, ActionParameter]:
-        '''Get a parameter by name.
-
-        Parameters
-        ----------
-        param : MetaParams
-            Metadata parameter.
-
-        Returns
-        -------
-        Union[Parameter, ActionParameter]
-            Retrieved parameter.
-        '''
-        return self.param_tree.param(*param.value.split('.'))
-
-    def get_param_value(
-            self, param: MetaParams):
-        '''Get a parameter value by name.
-
-        Parameters
-        ----------
-        param : MetaParams
-            Metadata parameter.
-
-        Returns
-        -------
-        Any
-            The value of the parameter.
-        '''
-        return self.param_tree.param(*param.value.split('.')).value()
-
-    def set_param_value(
-            self, param: MetaParams, value):
-        '''Set a parameter value by name.
-
-        Parameters
-        ----------
-        param : MetaParams
-            Metadata parameter.
-        value : Any
-            The value to set.
-
-        Returns
-        -------
-        bool
-            True if the value is set successfully, False otherwise.
-        '''
-        try:
-            self.param_tree.param(*param.value.split('.')).setValue(value)
-        except Exception:
-            import traceback
-            traceback.print_exc()
-            return False
-        else:
-            return True
-
-    def get_param_path(self, param: Parameter):
-        '''
-        Get the child path of a parameter in the parameter tree.
-
-        Parameters
-        ----------
-        param : Parameter
-            The parameter for which to retrieve the child path.
-
-        Returns
-        -------
-        list
-            The child path of the parameter.
-        '''
-        return self.param_tree.childPath(param)
-
     def add_param_child(self, parent: MetaParams, value: Union[MetaParams, Any]):
         '''
         Add a child parameter to the specified parent parameter.
 
         Parameters
         ----------
         parent : MetaParams
@@ -382,35 +295,14 @@
         parent = self.get_param(parent)
         parent.addChild(
             {'name' : 'Item 1', 'type': 'str',
              'value': self.get_param_value(value) if \
                 isinstance(value, MetaParams) else value, 'removable': True},
             True)
 
-    def get_children(self, param: MetaParams):
-        '''
-        Get the values of all children of a specified parameter.
-
-        Parameters
-        ----------
-        param : MetaParams
-            The parameter whose children's values will be retrieved.
-
-        Returns
-        -------
-        list
-            List of values of all children of the specified parameter.
-        '''
-        res = []
-        param = self.get_param(param)
-        if isinstance(param, GroupParameter):
-            for child in param.children():
-                res.append(child.value())
-        return res
-
     def change(self, param: Parameter, changes: list):
         '''
         Handle parameter changes as needed.
 
         Parameters
         ----------
         param : Parameter
@@ -421,51 +313,14 @@
         Returns
         -------
         None
         '''
         # Handle parameter changes as needed
         pass
 
-    def export_json(self):
-        '''
-        Export parameters to a JSON file.
-
-        Returns
-        -------
-        None
-        '''
-        filename, _ = QFileDialog.getSaveFileName(
-            None,
-            'Save Parameters', '', 'JSON Files (*.json);;All Files (*)')
-        if not filename:
-            return  # User canceled the operation
-
-        state = self.param_tree.saveState()
-        with open(filename, 'w', encoding='utf8') as file:
-            json.dump(state, file, indent=2)
-
-    # Load parameters from JSON
-    def load_json(self):
-        '''
-        Load parameters from a JSON file.
-
-        Returns
-        -------
-        None
-        '''
-        filename, _ = QFileDialog.getOpenFileName(
-            None, 'Load Parameters',
-            '', 'JSON Files (*.json);;All Files (*)')
-        if not filename:
-            return  # User canceled the operation
-
-        with open(filename, encoding='utf8') as file:
-            state = json.load(file)
-        self.param_tree.restoreState(state)
-
     def save(self):
         '''
         Save metadata to an OME-XML file.
 
         Returns
         -------
         None
```

### Comparing `microEye-1.0.5/src/microEye/shared/pyscripting.py` & `microEye-2.0.0/src/microEye/shared/pyscripting.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/thread_worker.py` & `microEye-2.0.0/src/microEye/shared/thread_worker.py`

 * *Files identical despite different names*

### Comparing `microEye-1.0.5/src/microEye/shared/uImage.py` & `microEye-2.0.0/src/microEye/shared/uImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1091,15 +1091,15 @@
         '''
         if self.data is None:
             return None
         return zarr.open(self.path, 'r').__getitem__(i)
 
     def getSlice(
             self, timeSlice=None, channelSlice=None,
-            zSlice=None, ySlice=None, xSlice=None,
+            zSlice=None, ySlice=None, xSlice=None, squeezed=True,
             four='TCYX', three='TYX'):
         '''
         Retrieves a slice from the Zarr array based on specified indices.
 
         Parameters
         ----------
         timeSlice : slice or None
@@ -1108,14 +1108,16 @@
             Slice for the channel dimension.
         zSlice : slice or None
             Slice for the z dimension.
         ySlice : slice or None
             Slice for the y dimension.
         xSlice : slice or None
             Slice for the x dimension.
+        squeezed : bool (optional)
+            Squeeze returned slice, default is True.
         four : str
             String representing the axis configuration for four dimensions.
         three : str
             String representing the axis configuration for three dimensions.
 
         Returns
         -------
@@ -1128,38 +1130,43 @@
         timeSlice = ifnone(timeSlice, slice(None))
         channelSlice = ifnone(channelSlice, slice(None))
         zSlice = ifnone(zSlice, slice(None))
         ySlice = ifnone(ySlice, slice(None))
         xSlice = ifnone(xSlice, slice(None))
 
         if len(za.shape) == 5:
-            return za[timeSlice, channelSlice, zSlice, ySlice, xSlice]
+            data = za[timeSlice, channelSlice, zSlice, ySlice, xSlice]
         elif len(za.shape) == 4:
             if four == 'TCYX':
-                return za[timeSlice, channelSlice, ySlice, xSlice]
+                data = za[timeSlice, channelSlice, ySlice, xSlice]
             elif four == 'CZYX':
-                return za[channelSlice, zSlice, ySlice, xSlice]
+                data = za[channelSlice, zSlice, ySlice, xSlice]
             elif four == 'TZYX':
-                return za[timeSlice, zSlice, ySlice, xSlice]
+                data = za[timeSlice, zSlice, ySlice, xSlice]
             else:
                 raise ValueError(f'Unsupported dimensions format: {four}')
         elif len(za.shape) == 3:
             if three == 'TYX':
-                return za[timeSlice, ySlice, xSlice]
+                data = za[timeSlice, ySlice, xSlice]
             elif three == 'CYX':
-                return za[channelSlice, ySlice, xSlice]
+                data = za[channelSlice, ySlice, xSlice]
             elif three == 'ZYX':
-                return za[zSlice, ySlice, xSlice]
+                data = za[zSlice, ySlice, xSlice]
             else:
                 raise ValueError(f'Unsupported dimensions format: {three}')
         elif len(za.shape) == 2:
-            return za[ySlice, xSlice]
+            data = za[ySlice, xSlice]
         else:
             raise ValueError(f'Unsupported number of dimensions: {len(za.shape)}')
 
+        if squeezed:
+            return data.squeeze()
+        else:
+            return data
+
     def open(self):
         """
         Opens the Zarr array and assigns it to the 'data' attribute.
         """
         self.data = zarr.open(self.path, 'r')
 
     def close(self):
```

### Comparing `microEye-1.0.5/src/microEye.egg-info/SOURCES.txt` & `microEye-2.0.0/src/microEye.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 src/microEye/__init__.py
 src/microEye.egg-info/PKG-INFO
 src/microEye.egg-info/SOURCES.txt
 src/microEye.egg-info/dependency_links.txt
+src/microEye.egg-info/requires.txt
 src/microEye.egg-info/top_level.txt
 src/microEye/analysis/__init__.py
 src/microEye/analysis/checklist_dialog.py
 src/microEye/analysis/cmosMaps.py
 src/microEye/analysis/file_sys.py
 src/microEye/analysis/filters.py
 src/microEye/analysis/multi_viewer.py
@@ -40,47 +41,51 @@
 src/microEye/analysis/tools/roi_selectors.py
 src/microEye/analysis/viewer/__init__.py
 src/microEye/analysis/viewer/image_options_widget.py
 src/microEye/analysis/viewer/images.py
 src/microEye/analysis/viewer/layers_widget.py
 src/microEye/analysis/viewer/localizations.py
 src/microEye/hardware/__init__.py
-src/microEye/hardware/acquisition_module.py
-src/microEye/hardware/control_module.py
+src/microEye/hardware/device.py
 src/microEye/hardware/miEye.py
 src/microEye/hardware/port_config.py
-src/microEye/hardware/cams/CameraListWidget.py
 src/microEye/hardware/cams/IR_Cam.py
 src/microEye/hardware/cams/__init__.py
 src/microEye/hardware/cams/camera_calibration.py
+src/microEye/hardware/cams/camera_list.py
 src/microEye/hardware/cams/camera_options.py
 src/microEye/hardware/cams/camera_panel.py
+src/microEye/hardware/cams/dummy_panel.py
 src/microEye/hardware/cams/jobs.py
 src/microEye/hardware/cams/line_profiler.py
 src/microEye/hardware/cams/micam.py
 src/microEye/hardware/cams/thorlabs.py
 src/microEye/hardware/cams/thorlabs_panel.py
 src/microEye/hardware/cams/ueye_camera.py
 src/microEye/hardware/cams/ueye_panel.py
 src/microEye/hardware/cams/vimba_cam.py
 src/microEye/hardware/cams/vimba_panel.py
 src/microEye/hardware/lasers/__init__.py
 src/microEye/hardware/lasers/io_matchbox.py
+src/microEye/hardware/lasers/io_params.py
 src/microEye/hardware/lasers/io_single_laser.py
+src/microEye/hardware/lasers/laser_relay.py
 src/microEye/hardware/misc/__init__.py
 src/microEye/hardware/misc/acquisition_view.py
 src/microEye/hardware/misc/reglo.py
 src/microEye/hardware/misc/temp.py
 src/microEye/hardware/protocols/__init__.py
 src/microEye/hardware/protocols/actions.py
 src/microEye/hardware/stages/__init__.py
 src/microEye/hardware/stages/elliptec.py
 src/microEye/hardware/stages/kinesis.py
 src/microEye/hardware/stages/piezo_concept.py
+src/microEye/hardware/stages/stabilizer.py
 src/microEye/hardware/widgets/__init__.py
+src/microEye/hardware/widgets/devices.py
 src/microEye/hardware/widgets/focusWidget.py
 src/microEye/hardware/widgets/qlist_slider.py
 src/microEye/hardware/widgets/scan_acquisition.py
 src/microEye/icons/1024.png
 src/microEye/icons/128.png
 src/microEye/icons/16.png
 src/microEye/icons/256.png
@@ -90,10 +95,12 @@
 src/microEye/shared/__init__.py
 src/microEye/shared/expandable_groupbox.py
 src/microEye/shared/gui_helper.py
 src/microEye/shared/hid_controller.py
 src/microEye/shared/labelled_slider.py
 src/microEye/shared/metadata.py
 src/microEye/shared/metadata_tree.py
+src/microEye/shared/parameter_tree.py
 src/microEye/shared/pyscripting.py
+src/microEye/shared/start_gui.py
 src/microEye/shared/thread_worker.py
 src/microEye/shared/uImage.py
```

