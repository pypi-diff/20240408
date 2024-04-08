# Comparing `tmp/ok-script-0.0.7.tar.gz` & `tmp/ok-script-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ok-script-0.0.7.tar", last modified: Mon Apr  8 13:41:39 2024, max compression
+gzip compressed data, was "ok-script-0.0.8.tar", last modified: Mon Apr  8 16:53:20 2024, max compression
```

## Comparing `ok-script-0.0.7.tar` & `ok-script-0.0.8.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.791394 ok-script-0.0.7/
--rw-rw-rw-   0        0        0     2196 2024-04-08 13:41:39.791394 ok-script-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2024-02-09 15:31:41.000000 ok-script-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.539278 ok-script-0.0.7/autohelper/
--rw-rw-rw-   0        0        0     5167 2024-04-07 13:02:23.000000 ok-script-0.0.7/autohelper/AutoHelper.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.7/autohelper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.543654 ok-script-0.0.7/autohelper/capture/
--rw-rw-rw-   0        0        0      602 2024-04-05 09:34:11.000000 ok-script-0.0.7/autohelper/capture/BaseCaptureMethod.py
--rw-rw-rw-   0        0        0     5371 2024-04-05 09:41:17.000000 ok-script-0.0.7/autohelper/capture/HwndWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 ok-script-0.0.7/autohelper/capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.556359 ok-script-0.0.7/autohelper/capture/adb/
--rw-rw-rw-   0        0        0      924 2024-04-05 03:42:41.000000 ok-script-0.0.7/autohelper/capture/adb/ADBCaptureMethod.py
--rw-rw-rw-   0        0        0     8505 2024-04-07 16:42:21.000000 ok-script-0.0.7/autohelper/capture/adb/DeviceManager.py
--rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 ok-script-0.0.7/autohelper/capture/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.557332 ok-script-0.0.7/autohelper/capture/adb/bin/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/capture/adb/bin/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 ok-script-0.0.7/autohelper/capture/adb/targets.py
--rw-rw-rw-   0        0        0     5808 2024-04-02 12:02:15.000000 ok-script-0.0.7/autohelper/capture/adb/vbox.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.570057 ok-script-0.0.7/autohelper/capture/windows/
--rw-rw-rw-   0        0        0     9246 2024-04-03 01:37:12.000000 ok-script-0.0.7/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py
--rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 ok-script-0.0.7/autohelper/capture/windows/__init__.py
--rw-rw-rw-   0        0        0     2689 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/capture/windows/d3d11.py
--rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 ok-script-0.0.7/autohelper/capture/windows/utils.py
--rw-rw-rw-   0        0        0     1320 2024-04-01 01:55:20.000000 ok-script-0.0.7/autohelper/capture/windows/window.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.573532 ok-script-0.0.7/autohelper/color/
--rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 ok-script-0.0.7/autohelper/color/Color.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/color/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.577426 ok-script-0.0.7/autohelper/config/
--rw-rw-rw-   0        0        0     2211 2024-04-02 04:15:06.000000 ok-script-0.0.7/autohelper/config/Config.py
--rw-rw-rw-   0        0        0      394 2024-04-03 09:47:40.000000 ok-script-0.0.7/autohelper/config/InfoDict.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.595590 ok-script-0.0.7/autohelper/feature/
--rw-rw-rw-   0        0        0     7181 2024-03-24 13:07:51.000000 ok-script-0.0.7/autohelper/feature/Box.py
--rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 ok-script-0.0.7/autohelper/feature/Feature.py
--rw-rw-rw-   0        0        0     9084 2024-04-02 17:38:24.000000 ok-script-0.0.7/autohelper/feature/FeatureSet.py
--rw-rw-rw-   0        0        0     2112 2024-03-18 00:55:14.000000 ok-script-0.0.7/autohelper/feature/FindFeature.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.609421 ok-script-0.0.7/autohelper/gui/
--rw-rw-rw-   0        0        0     4581 2024-04-04 16:24:15.000000 ok-script-0.0.7/autohelper/gui/App.py
--rw-rw-rw-   0        0        0      604 2024-04-03 09:22:41.000000 ok-script-0.0.7/autohelper/gui/Communicate.py
--rw-rw-rw-   0        0        0     2565 2024-04-03 02:56:02.000000 ok-script-0.0.7/autohelper/gui/MainWindow.py
--rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 ok-script-0.0.7/autohelper/gui/TabTitles.py
--rw-rw-rw-   0        0        0      140 2024-04-02 11:24:03.000000 ok-script-0.0.7/autohelper/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.618248 ok-script-0.0.7/autohelper/gui/debug/
--rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 ok-script-0.0.7/autohelper/gui/debug/AspectRatioWidget.py
--rw-rw-rw-   0        0        0     1358 2024-03-16 10:12:34.000000 ok-script-0.0.7/autohelper/gui/debug/DebugTab.py
--rw-rw-rw-   0        0        0     5111 2024-03-18 10:58:13.000000 ok-script-0.0.7/autohelper/gui/debug/FrameWidget.py
--rw-rw-rw-   0        0        0     1219 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/gui/debug/InfoWidget.py
--rw-rw-rw-   0        0        0     2698 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/gui/debug/LoggerWidget.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/debug/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.620503 ok-script-0.0.7/autohelper/gui/i18n/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/i18n/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-01 11:14:15.000000 ok-script-0.0.7/autohelper/gui/i18n/path.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.622505 ok-script-0.0.7/autohelper/gui/icon/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/icon/__init__.py
--rw-rw-rw-   0        0        0      174 2024-03-26 17:34:24.000000 ok-script-0.0.7/autohelper/gui/icon/icon.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.625424 ok-script-0.0.7/autohelper/gui/loading/
--rw-rw-rw-   0        0        0     6236 2024-04-05 09:39:36.000000 ok-script-0.0.7/autohelper/gui/loading/LoadingWindow.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.7/autohelper/gui/loading/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.627370 ok-script-0.0.7/autohelper/gui/overlay/
--rw-rw-rw-   0        0        0     1434 2024-03-23 15:09:36.000000 ok-script-0.0.7/autohelper/gui/overlay/OverlayWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/overlay/__init__.py
--rw-rw-rw-   0        0        0    22185 2024-04-04 16:18:48.000000 ok-script-0.0.7/autohelper/gui/resources.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.641600 ok-script-0.0.7/autohelper/gui/tasks/
--rw-rw-rw-   0        0        0      692 2024-03-25 16:13:40.000000 ok-script-0.0.7/autohelper/gui/tasks/ConfigItemFactory.py
--rw-rw-rw-   0        0        0     1615 2024-04-03 02:52:44.000000 ok-script-0.0.7/autohelper/gui/tasks/StartButton.py
--rw-rw-rw-   0        0        0      919 2024-04-03 04:00:06.000000 ok-script-0.0.7/autohelper/gui/tasks/TaskOpButton.py
--rw-rw-rw-   0        0        0     6041 2024-04-03 15:23:26.000000 ok-script-0.0.7/autohelper/gui/tasks/TaskTab.py
--rw-rw-rw-   0        0        0     1546 2024-04-03 14:53:01.000000 ok-script-0.0.7/autohelper/gui/tasks/TooltipTableWidget.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.649406 ok-script-0.0.7/autohelper/gui/util/
--rw-rw-rw-   0        0        0      416 2024-03-30 15:38:52.000000 ok-script-0.0.7/autohelper/gui/util/Alert.py
--rw-rw-rw-   0        0        0      372 2024-04-02 10:49:06.000000 ok-script-0.0.7/autohelper/gui/util/InitWorker.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.659736 ok-script-0.0.7/autohelper/gui/widget/
--rw-rw-rw-   0        0        0      951 2024-03-25 16:12:19.000000 ok-script-0.0.7/autohelper/gui/widget/ListTableWidgetItem.py
--rw-rw-rw-   0        0        0     1324 2024-03-26 06:35:12.000000 ok-script-0.0.7/autohelper/gui/widget/NumericTableWidgetItem.py
--rw-rw-rw-   0        0        0     2126 2024-04-02 12:32:43.000000 ok-script-0.0.7/autohelper/gui/widget/RoundCornerContainer.py
--rw-rw-rw-   0        0        0      830 2024-03-25 08:54:00.000000 ok-script-0.0.7/autohelper/gui/widget/TabWidget.py
--rw-rw-rw-   0        0        0      399 2024-03-25 14:18:22.000000 ok-script-0.0.7/autohelper/gui/widget/UpdateConfigWidgetItem.py
--rw-rw-rw-   0        0        0      693 2024-03-25 14:39:29.000000 ok-script-0.0.7/autohelper/gui/widget/YesNonWidgetItem.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/gui/widget/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.664464 ok-script-0.0.7/autohelper/interaction/
--rw-rw-rw-   0        0        0     1169 2024-04-02 04:25:35.000000 ok-script-0.0.7/autohelper/interaction/ADBInteraction.py
--rw-rw-rw-   0        0        0     1074 2024-04-02 17:41:04.000000 ok-script-0.0.7/autohelper/interaction/BaseInteraction.py
--rw-rw-rw-   0        0        0     1717 2024-04-03 01:37:12.000000 ok-script-0.0.7/autohelper/interaction/Win32Interaction.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/interaction/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.666410 ok-script-0.0.7/autohelper/logging/
--rw-rw-rw-   0        0        0     3642 2024-04-02 02:22:11.000000 ok-script-0.0.7/autohelper/logging/Logger.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.669330 ok-script-0.0.7/autohelper/ocr/
--rw-rw-rw-   0        0        0     2123 2024-04-03 02:48:38.000000 ok-script-0.0.7/autohelper/ocr/OCR.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.7/autohelper/ocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.671309 ok-script-0.0.7/autohelper/predict/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/predict/__init__.py
--rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 ok-script-0.0.7/autohelper/predict/predict.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.698360 ok-script-0.0.7/autohelper/rotypes/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.699327 ok-script-0.0.7/autohelper/rotypes/Windows/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.702305 ok-script-0.0.7/autohelper/rotypes/Windows/Foundation/
--rw-rw-rw-   0        0        0     2039 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Foundation/Collections.py
--rw-rw-rw-   0        0        0     5409 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Foundation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.704444 ok-script-0.0.7/autohelper/rotypes/Windows/Globalization/
--rw-rw-rw-   0        0        0      933 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Globalization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.706391 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.708370 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Capture/
--rw-rw-rw-   0        0        0     4731 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.709373 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.711354 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/
--rw-rw-rw-   0        0        0     1266 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
--rw-rw-rw-   0        0        0     4189 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.712354 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Imaging/
--rw-rw-rw-   0        0        0     1093 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py
--rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.713416 ok-script-0.0.7/autohelper/rotypes/Windows/Media/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.719260 ok-script-0.0.7/autohelper/rotypes/Windows/Media/Ocr/
--rw-rw-rw-   0        0        0     3095 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Media/Ocr/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Media/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.720232 ok-script-0.0.7/autohelper/rotypes/Windows/Security/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.722234 ok-script-0.0.7/autohelper/rotypes/Windows/Security/Cryptography/
--rw-rw-rw-   0        0        0      691 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Security/Cryptography/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Security/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.723522 ok-script-0.0.7/autohelper/rotypes/Windows/Storage/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.724500 ok-script-0.0.7/autohelper/rotypes/Windows/Storage/Streams/
--rw-rw-rw-   0        0        0      853 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Storage/Streams/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/Windows/Storage/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/Windows/__init__.py
--rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/__init__.py
--rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/delegate.py
--rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/export.py
--rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/idldsl.py
--rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/inspectable.py
--rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 ok-script-0.0.7/autohelper/rotypes/roapi.py
--rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/types.py
--rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 ok-script-0.0.7/autohelper/rotypes/winstring.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.738208 ok-script-0.0.7/autohelper/save/
--rw-rw-rw-   0        0        0      804 2024-03-16 12:48:02.000000 ok-script-0.0.7/autohelper/save/BlackBarProcessor.py
--rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 ok-script-0.0.7/autohelper/save/PostProcessor.py
--rw-rw-rw-   0        0        0      836 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/save/SaveByInterval.py
--rw-rw-rw-   0        0        0     1043 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/save/SaveByKeyPress.py
--rw-rw-rw-   0        0        0     1471 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/save/SaveMethodBase.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/save/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.741655 ok-script-0.0.7/autohelper/scene/
--rw-rw-rw-   0        0        0      344 2024-03-18 15:05:37.000000 ok-script-0.0.7/autohelper/scene/FeatureScene.py
--rw-rw-rw-   0        0        0      600 2024-04-02 18:02:38.000000 ok-script-0.0.7/autohelper/scene/Scene.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/scene/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.743626 ok-script-0.0.7/autohelper/stats/
--rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 ok-script-0.0.7/autohelper/stats/StreamStats.py
--rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 ok-script-0.0.7/autohelper/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.757453 ok-script-0.0.7/autohelper/task/
--rw-rw-rw-   0        0        0     3136 2024-04-03 13:39:04.000000 ok-script-0.0.7/autohelper/task/BaseTask.py
--rw-rw-rw-   0        0        0     4812 2024-04-02 18:06:06.000000 ok-script-0.0.7/autohelper/task/ExecutorOperation.py
--rw-rw-rw-   0        0        0      164 2024-03-12 10:11:44.000000 ok-script-0.0.7/autohelper/task/FindFeatureTask.py
--rw-rw-rw-   0        0        0     9495 2024-04-06 02:19:14.000000 ok-script-0.0.7/autohelper/task/TaskExecutor.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.7/autohelper/task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.767242 ok-script-0.0.7/autohelper/util/
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.7/autohelper/util/__init__.py
--rw-rw-rw-   0        0        0      707 2024-04-02 04:07:38.000000 ok-script-0.0.7/autohelper/util/json.py
--rw-rw-rw-   0        0        0      109 2024-04-02 11:28:23.000000 ok-script-0.0.7/autohelper/util/list.py
--rw-rw-rw-   0        0        0     1127 2024-04-04 17:00:56.000000 ok-script-0.0.7/autohelper/util/path.py
--rw-rw-rw-   0        0        0      246 2024-03-26 05:25:09.000000 ok-script-0.0.7/autohelper/util/thread.py
--rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 ok-script-0.0.7/autohelper/util/win32_process.py
--rw-rw-rw-   0        0        0      735 2024-03-26 06:27:07.000000 ok-script-0.0.7/autohelper/util/yaml.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:41:39.790386 ok-script-0.0.7/ok_script.egg-info/
--rw-rw-rw-   0        0        0     2196 2024-04-08 13:41:39.000000 ok-script-0.0.7/ok_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4374 2024-04-08 13:41:39.000000 ok-script-0.0.7/ok_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:41:39.000000 ok-script-0.0.7/ok_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-08 13:41:39.000000 ok-script-0.0.7/ok_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 13:41:39.000000 ok-script-0.0.7/ok_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 13:41:39.791394 ok-script-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-04-08 10:36:14.000000 ok-script-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.822513 ok-script-0.0.8/
+-rw-rw-rw-   0        0        0     2196 2024-04-08 16:53:20.821519 ok-script-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1513 2024-02-09 15:31:41.000000 ok-script-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.324413 ok-script-0.0.8/ok/
+-rw-rw-rw-   0        0        0     5055 2024-04-08 14:20:09.000000 ok-script-0.0.8/ok/OK.py
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.8/ok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.333496 ok-script-0.0.8/ok/capture/
+-rw-rw-rw-   0        0        0      602 2024-04-05 09:34:11.000000 ok-script-0.0.8/ok/capture/BaseCaptureMethod.py
+-rw-rw-rw-   0        0        0     5347 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/HwndWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 ok-script-0.0.8/ok/capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.360165 ok-script-0.0.8/ok/capture/adb/
+-rw-rw-rw-   0        0        0      908 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/ADBCaptureMethod.py
+-rw-rw-rw-   0        0        0     8433 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/DeviceManager.py
+-rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 ok-script-0.0.8/ok/capture/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.361671 ok-script-0.0.8/ok/capture/adb/bin/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/capture/adb/bin/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 ok-script-0.0.8/ok/capture/adb/targets.py
+-rw-rw-rw-   0        0        0     5784 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/vbox.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.399565 ok-script-0.0.8/ok/capture/windows/
+-rw-rw-rw-   0        0        0     9158 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/windows/WindowsGraphicsCaptureMethod.py
+-rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 ok-script-0.0.8/ok/capture/windows/__init__.py
+-rw-rw-rw-   0        0        0     2673 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/windows/d3d11.py
+-rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 ok-script-0.0.8/ok/capture/windows/utils.py
+-rw-rw-rw-   0        0        0     1320 2024-04-01 01:55:20.000000 ok-script-0.0.8/ok/capture/windows/window.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.405474 ok-script-0.0.8/ok/color/
+-rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 ok-script-0.0.8/ok/color/Color.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/color/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.414804 ok-script-0.0.8/ok/config/
+-rw-rw-rw-   0        0        0     2195 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/config/Config.py
+-rw-rw-rw-   0        0        0      386 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/config/InfoDict.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.443530 ok-script-0.0.8/ok/feature/
+-rw-rw-rw-   0        0        0     7181 2024-03-24 13:07:51.000000 ok-script-0.0.8/ok/feature/Box.py
+-rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 ok-script-0.0.8/ok/feature/Feature.py
+-rw-rw-rw-   0        0        0     9052 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/feature/FeatureSet.py
+-rw-rw-rw-   0        0        0     2104 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/feature/FindFeature.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.472314 ok-script-0.0.8/ok/gui/
+-rw-rw-rw-   0        0        0     4501 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/App.py
+-rw-rw-rw-   0        0        0      604 2024-04-03 09:22:41.000000 ok-script-0.0.8/ok/gui/Communicate.py
+-rw-rw-rw-   0        0        0     2541 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/MainWindow.py
+-rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 ok-script-0.0.8/ok/gui/TabTitles.py
+-rw-rw-rw-   0        0        0      132 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.502660 ok-script-0.0.8/ok/gui/debug/
+-rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 ok-script-0.0.8/ok/gui/debug/AspectRatioWidget.py
+-rw-rw-rw-   0        0        0     1334 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/DebugTab.py
+-rw-rw-rw-   0        0        0     5095 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/FrameWidget.py
+-rw-rw-rw-   0        0        0     1211 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/InfoWidget.py
+-rw-rw-rw-   0        0        0     2690 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/LoggerWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/debug/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.507527 ok-script-0.0.8/ok/gui/i18n/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/i18n/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-01 11:14:15.000000 ok-script-0.0.8/ok/gui/i18n/path.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.511455 ok-script-0.0.8/ok/gui/icon/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/icon/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-03-26 17:34:24.000000 ok-script-0.0.8/ok/gui/icon/icon.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.516384 ok-script-0.0.8/ok/gui/loading/
+-rw-rw-rw-   0        0        0     6156 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/loading/LoadingWindow.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.8/ok/gui/loading/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.522325 ok-script-0.0.8/ok/gui/overlay/
+-rw-rw-rw-   0        0        0     1402 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/overlay/OverlayWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/overlay/__init__.py
+-rw-rw-rw-   0        0        0    22185 2024-04-04 16:18:48.000000 ok-script-0.0.8/ok/gui/resources.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.550306 ok-script-0.0.8/ok/gui/tasks/
+-rw-rw-rw-   0        0        0      668 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/ConfigItemFactory.py
+-rw-rw-rw-   0        0        0     1567 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/StartButton.py
+-rw-rw-rw-   0        0        0      903 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/TaskOpButton.py
+-rw-rw-rw-   0        0        0     5969 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/TaskTab.py
+-rw-rw-rw-   0        0        0     1546 2024-04-03 14:53:01.000000 ok-script-0.0.8/ok/gui/tasks/TooltipTableWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/tasks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.565517 ok-script-0.0.8/ok/gui/util/
+-rw-rw-rw-   0        0        0      400 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/util/Alert.py
+-rw-rw-rw-   0        0        0      356 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/util/InitWorker.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.585979 ok-script-0.0.8/ok/gui/widget/
+-rw-rw-rw-   0        0        0      943 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/gui/widget/ListTableWidgetItem.py
+-rw-rw-rw-   0        0        0     1316 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/widget/NumericTableWidgetItem.py
+-rw-rw-rw-   0        0        0     2126 2024-04-02 12:32:43.000000 ok-script-0.0.8/ok/gui/widget/RoundCornerContainer.py
+-rw-rw-rw-   0        0        0      830 2024-03-25 08:54:00.000000 ok-script-0.0.8/ok/gui/widget/TabWidget.py
+-rw-rw-rw-   0        0        0      399 2024-03-25 14:18:22.000000 ok-script-0.0.8/ok/gui/widget/UpdateConfigWidgetItem.py
+-rw-rw-rw-   0        0        0      685 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/widget/YesNonWidgetItem.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/widget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.599219 ok-script-0.0.8/ok/interaction/
+-rw-rw-rw-   0        0        0     1153 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/ADBInteraction.py
+-rw-rw-rw-   0        0        0     1050 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/BaseInteraction.py
+-rw-rw-rw-   0        0        0     1693 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/Win32Interaction.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/interaction/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.604071 ok-script-0.0.8/ok/logging/
+-rw-rw-rw-   0        0        0     3618 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/logging/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.608960 ok-script-0.0.8/ok/ocr/
+-rw-rw-rw-   0        0        0     2099 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/ocr/OCR.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.8/ok/ocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.612463 ok-script-0.0.8/ok/predict/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/predict/__init__.py
+-rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 ok-script-0.0.8/ok/predict/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.662316 ok-script-0.0.8/ok/rotypes/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.664508 ok-script-0.0.8/ok/rotypes/Windows/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.668402 ok-script-0.0.8/ok/rotypes/Windows/Foundation/
+-rw-rw-rw-   0        0        0     2023 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Foundation/Collections.py
+-rw-rw-rw-   0        0        0     5385 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Foundation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.672366 ok-script-0.0.8/ok/rotypes/Windows/Globalization/
+-rw-rw-rw-   0        0        0      909 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Globalization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.674316 ok-script-0.0.8/ok/rotypes/Windows/Graphics/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.676262 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/
+-rw-rw-rw-   0        0        0     4675 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.679184 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.682674 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/
+-rw-rw-rw-   0        0        0     1234 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
+-rw-rw-rw-   0        0        0     4181 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.684620 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/
+-rw-rw-rw-   0        0        0     1053 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.687541 ok-script-0.0.8/ok/rotypes/Windows/Media/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.689487 ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/
+-rw-rw-rw-   0        0        0     3039 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Media/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.691468 ok-script-0.0.8/ok/rotypes/Windows/Security/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.694425 ok-script-0.0.8/ok/rotypes/Windows/Security/Cryptography/
+-rw-rw-rw-   0        0        0      675 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Security/Cryptography/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Security/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.695397 ok-script-0.0.8/ok/rotypes/Windows/Storage/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.697342 ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/
+-rw-rw-rw-   0        0        0      837 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Storage/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/__init__.py
+-rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/delegate.py
+-rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/export.py
+-rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/idldsl.py
+-rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/inspectable.py
+-rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 ok-script-0.0.8/ok/rotypes/roapi.py
+-rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/types.py
+-rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/winstring.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.715599 ok-script-0.0.8/ok/save/
+-rw-rw-rw-   0        0        0      796 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/BlackBarProcessor.py
+-rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 ok-script-0.0.8/ok/save/PostProcessor.py
+-rw-rw-rw-   0        0        0      828 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveByInterval.py
+-rw-rw-rw-   0        0        0     1019 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveByKeyPress.py
+-rw-rw-rw-   0        0        0     1455 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveMethodBase.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/save/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.724481 ok-script-0.0.8/ok/scene/
+-rw-rw-rw-   0        0        0      328 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/scene/FeatureScene.py
+-rw-rw-rw-   0        0        0      576 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/scene/Scene.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/scene/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.728376 ok-script-0.0.8/ok/stats/
+-rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 ok-script-0.0.8/ok/stats/StreamStats.py
+-rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 ok-script-0.0.8/ok/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.757717 ok-script-0.0.8/ok/task/
+-rw-rw-rw-   0        0        0     3096 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/BaseTask.py
+-rw-rw-rw-   0        0        0     4788 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/ExecutorOperation.py
+-rw-rw-rw-   0        0        0      148 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/FindFeatureTask.py
+-rw-rw-rw-   0        0        0     9455 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/TaskExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.779705 ok-script-0.0.8/ok/util/
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.8/ok/util/__init__.py
+-rw-rw-rw-   0        0        0      699 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/util/json.py
+-rw-rw-rw-   0        0        0      109 2024-04-02 11:28:23.000000 ok-script-0.0.8/ok/util/list.py
+-rw-rw-rw-   0        0        0     1127 2024-04-04 17:00:56.000000 ok-script-0.0.8/ok/util/path.py
+-rw-rw-rw-   0        0        0      246 2024-03-26 05:25:09.000000 ok-script-0.0.8/ok/util/thread.py
+-rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 ok-script-0.0.8/ok/util/win32_process.py
+-rw-rw-rw-   0        0        0      727 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/util/yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.816592 ok-script-0.0.8/ok_script.egg-info/
+-rw-rw-rw-   0        0        0     2196 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3422 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:53:20.823486 ok-script-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-04-08 16:52:53.000000 ok-script-0.0.8/setup.py
```

### Comparing `ok-script-0.0.7/PKG-INFO` & `ok-script-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ok-script
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automation with Computer Vision for Python
 Home-page: https://github.com/ok-oldking/ok-script
 Author: ok-oldking
 Author-email: firedcto@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ok-script-0.0.7/README.md` & `ok-script-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/AutoHelper.py` & `ok-script-0.0.8/ok/OK.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 import threading
 import time
 from typing import Dict, Any
 
 from PySide6.QtWidgets import QApplication
 
-import autohelper
-from autohelper.feature.FeatureSet import FeatureSet
-from autohelper.gui.App import App
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.overlay.OverlayWindow import OverlayWindow
-from autohelper.gui.util.InitWorker import InitWorker
-from autohelper.logging.Logger import get_logger, config_logger
-from autohelper.task.TaskExecutor import TaskExecutor
+import ok
+from ok.feature.FeatureSet import FeatureSet
+from ok.gui.App import App
+from ok.gui.Communicate import communicate
+from ok.gui.overlay.OverlayWindow import OverlayWindow
+from ok.gui.util.InitWorker import InitWorker
+from ok.logging.Logger import get_logger, config_logger
+from ok.task.TaskExecutor import TaskExecutor
 
 logger = get_logger(__name__)
 
 
-class AutoHelper:
+class OK:
     executor: TaskExecutor
     adb = None
     adb_device = None
     feature_set = None
     hwnd = None
     device_manager = None
     ocr = None
@@ -33,27 +33,27 @@
         self.debug = config.get("debug", False)
         self.exit_event = threading.Event()
         self.config = config
         self.init_device_manager()
         if config.get("use_gui"):
             self.app = App(self.config.get('gui_icon'), self.debug, self.config.get('gui_title'),
                            self.config['tasks'], self.exit_event)
-            autohelper.gui.app = self.app
+            ok.gui.app = self.app
             self.app.show_loading()
             self.worker = InitWorker(self.do_init)
             self.worker.start()
             self.app.exec()
         else:
             self.device_manager.set_preferred_device()
             self.device_manager.start()
             self.do_init()
             self.task_executor.start()
             if config.get("debug"):
                 self.app = QApplication(sys.argv)
-                self.overlay_window = OverlayWindow(autohelper.gui.device_manager.hwnd)
+                self.overlay_window = OverlayWindow(ok.gui.device_manager.hwnd)
                 self.app.exec()
             else:
                 try:
                     # Starting the task in a separate thread (optional)
                     # This allows the main thread to remain responsive to keyboard interrupts
                     task_thread = threading.Thread(target=self.wait_task())
                     task_thread.start()
@@ -97,20 +97,20 @@
         self.task_executor = TaskExecutor(self.device_manager, exit_event=self.exit_event,
                                           tasks=self.config['tasks'], scenes=self.config['scenes'],
                                           feature_set=self.feature_set,
                                           ocr=self.ocr, config_folder=self.config.get("config_folder") or "config")
         self.init_message("TaskExecutor init Done")
 
         if self.app:
-            autohelper.gui.executor = self.task_executor
+            ok.gui.executor = self.task_executor
 
     def wait_task(self):
         while not self.exit_event.is_set():
             time.sleep(1)
 
     def init_device_manager(self):
         if self.device_manager is None:
-            from autohelper.capture.adb.DeviceManager import DeviceManager
+            from ok.capture.adb.DeviceManager import DeviceManager
             self.device_manager = DeviceManager(self.config.get("config_folder") or "config",
                                                 self.config.get('capture_window_title'), self.config.get("debug"),
                                                 self.exit_event)
-            autohelper.gui.device_manager = self.device_manager
+            ok.gui.device_manager = self.device_manager
```

### Comparing `ok-script-0.0.7/autohelper/capture/BaseCaptureMethod.py` & `ok-script-0.0.8/ok/capture/BaseCaptureMethod.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/capture/HwndWindow.py` & `ok-script-0.0.8/ok/capture/HwndWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # original https://github.com/dantmnf & https://github.com/hakaboom/winAuto
 import re
 import threading
 
 from typing_extensions import override
 from win32 import win32gui
 
-from autohelper.capture.windows.window import is_foreground_window, get_window_bounds
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
+from ok.capture.windows.window import is_foreground_window, get_window_bounds
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class HwndWindow:
     visible = True
     x = 0
```

### Comparing `ok-script-0.0.7/autohelper/capture/adb/ADBCaptureMethod.py` & `ok-script-0.0.8/ok/capture/adb/ADBCaptureMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # original https://github.com/Toufool/AutoSplit/blob/master/src/capture_method/WindowsGraphicsCaptureMethod.py
 import numpy as np
 from typing_extensions import override
 
-from autohelper.capture.BaseCaptureMethod import BaseCaptureMethod
-from autohelper.logging.Logger import get_logger
+from ok.capture.BaseCaptureMethod import BaseCaptureMethod
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class ADBCaptureMethod(BaseCaptureMethod):
     name = "ADB command line Capture"
     description = "use the adb screencap command, slow but works when in background/minimized, takes 300ms per frame"
```

### Comparing `ok-script-0.0.7/autohelper/capture/adb/DeviceManager.py` & `ok-script-0.0.8/ok/capture/adb/DeviceManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import threading
 
 import adbutils
 import cv2
 import numpy as np
 
-from autohelper.capture.HwndWindow import HwndWindow
-from autohelper.capture.adb.ADBCaptureMethod import ADBCaptureMethod
-from autohelper.capture.adb.vbox import installed_emulator
-from autohelper.capture.windows.WindowsGraphicsCaptureMethod import WindowsGraphicsCaptureMethod
-from autohelper.config.Config import Config
-from autohelper.gui.Communicate import communicate
-from autohelper.interaction.ADBInteraction import ADBBaseInteraction
-from autohelper.interaction.Win32Interaction import Win32Interaction
-from autohelper.logging.Logger import get_logger
+from ok.capture.HwndWindow import HwndWindow
+from ok.capture.adb.ADBCaptureMethod import ADBCaptureMethod
+from ok.capture.adb.vbox import installed_emulator
+from ok.capture.windows.WindowsGraphicsCaptureMethod import WindowsGraphicsCaptureMethod
+from ok.config.Config import Config
+from ok.gui.Communicate import communicate
+from ok.interaction.ADBInteraction import ADBBaseInteraction
+from ok.interaction.Win32Interaction import Win32Interaction
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class DeviceManager:
 
     def __init__(self, config_folder, hwnd_title=None, debug=False, exit_event=None):
```

### Comparing `ok-script-0.0.7/autohelper/capture/adb/targets.py` & `ok-script-0.0.8/ok/capture/adb/targets.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/capture/adb/vbox.py` & `ok-script-0.0.8/ok/capture/adb/vbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import winreg
 from dataclasses import dataclass
 
 import adbutils
 import win32com.client
 
-from autohelper.capture.adb.targets import ADBControllerTarget
-from autohelper.logging.Logger import get_logger
-from autohelper.util import win32_process
+from ok.capture.adb.targets import ADBControllerTarget
+from ok.logging.Logger import get_logger
+from ok.util import win32_process
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class VBoxClass:
     clsid: str
```

### Comparing `ok-script-0.0.7/autohelper/capture/windows/WindowsGraphicsCaptureMethod.py` & `ok-script-0.0.8/ok/capture/windows/WindowsGraphicsCaptureMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import ctypes
 import ctypes.wintypes
 import time
 
 import numpy as np
 from typing_extensions import override
 
-from autohelper.capture.BaseCaptureMethod import BaseCaptureMethod
-from autohelper.capture.HwndWindow import HwndWindow
-from autohelper.capture.windows import d3d11
-from autohelper.capture.windows.utils import WINDOWS_BUILD_NUMBER
-from autohelper.logging.Logger import get_logger
-from autohelper.rotypes import IInspectable
-from autohelper.rotypes.Windows.Foundation import TypedEventHandler
-from autohelper.rotypes.Windows.Graphics.Capture import Direct3D11CaptureFramePool, IGraphicsCaptureItemInterop, \
+from ok.capture.BaseCaptureMethod import BaseCaptureMethod
+from ok.capture.HwndWindow import HwndWindow
+from ok.capture.windows import d3d11
+from ok.capture.windows.utils import WINDOWS_BUILD_NUMBER
+from ok.logging.Logger import get_logger
+from ok.rotypes import IInspectable
+from ok.rotypes.Windows.Foundation import TypedEventHandler
+from ok.rotypes.Windows.Graphics.Capture import Direct3D11CaptureFramePool, IGraphicsCaptureItemInterop, \
     IGraphicsCaptureItem, GraphicsCaptureItem
-from autohelper.rotypes.Windows.Graphics.DirectX import DirectXPixelFormat
-from autohelper.rotypes.Windows.Graphics.DirectX.Direct3D11 import IDirect3DDevice, \
+from ok.rotypes.Windows.Graphics.DirectX import DirectXPixelFormat
+from ok.rotypes.Windows.Graphics.DirectX.Direct3D11 import IDirect3DDevice, \
     CreateDirect3D11DeviceFromDXGIDevice, \
     IDirect3DDxgiInterfaceAccess
-from autohelper.rotypes.roapi import GetActivationFactory
+from ok.rotypes.roapi import GetActivationFactory
 
 PBYTE = ctypes.POINTER(ctypes.c_ubyte)
 WGC_NO_BORDER_MIN_BUILD = 20348
 
 logger = get_logger(__name__)
```

### Comparing `ok-script-0.0.7/autohelper/capture/windows/d3d11.py` & `ok-script-0.0.8/ok/capture/windows/d3d11.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ctypes.wintypes
 
-from autohelper.rotypes import IUnknown
-from autohelper.rotypes import idldsl
+from ok.rotypes import IUnknown
+from ok.rotypes import idldsl
 
 D3D11_SDK_VERSION = 7
 D3D_DRIVER_TYPE_HARDWARE = 1
 D3D11_CREATE_DEVICE_BGRA_SUPPORT = 0x20
 D3D11_USAGE_STAGING = 3
 D3D11_CPU_ACCESS_READ = 0x20000
 D3D11_MAP_READ = 1
```

### Comparing `ok-script-0.0.7/autohelper/capture/windows/utils.py` & `ok-script-0.0.8/ok/capture/windows/utils.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/capture/windows/window.py` & `ok-script-0.0.8/ok/capture/windows/window.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/color/Color.py` & `ok-script-0.0.8/ok/color/Color.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/config/Config.py` & `ok-script-0.0.8/ok/config/Config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from autohelper.util.json import read_json_file, write_json_file
-from autohelper.util.path import get_path_relative_to_exe
+from ok.util.json import read_json_file, write_json_file
+from ok.util.path import get_path_relative_to_exe
 
 
 class Config:
     def __init__(self, default, folder, name):
         super().__init__()
         self.config_file = get_path_relative_to_exe(folder, f"{name}.json")
         self.config = read_json_file(self.config_file)
```

### Comparing `ok-script-0.0.7/autohelper/feature/Box.py` & `ok-script-0.0.8/ok/feature/Box.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/feature/Feature.py` & `ok-script-0.0.8/ok/feature/Feature.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/feature/FeatureSet.py` & `ok-script-0.0.8/ok/feature/FeatureSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sys
 from typing import Dict
 from typing import List
 
 import cv2
 import numpy as np
 
-from autohelper.feature.Box import Box, sort_boxes
-from autohelper.feature.Feature import Feature
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
+from ok.feature.Box import Box, sort_boxes
+from ok.feature.Feature import Feature
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class FeatureSet:
     # Category_name to OpenCV Mat
     featureDict: Dict[str, Feature] = {}
```

### Comparing `ok-script-0.0.7/autohelper/feature/FindFeature.py` & `ok-script-0.0.8/ok/feature/FindFeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from typing import List
 
-from autohelper.feature.Box import Box
+from ok.feature.Box import Box
 
 
 class FindFeature:
 
     def __init__(self):
         self.feature_set = None
         self.executor = None
```

### Comparing `ok-script-0.0.7/autohelper/gui/App.py` & `ok-script-0.0.8/ok/gui/App.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 
 from PySide6.QtCore import QSize, QCoreApplication, QLocale, QTranslator
 from PySide6.QtGui import QIcon
 from PySide6.QtWidgets import QApplication, QStyleFactory, QMenu, QSystemTrayIcon
 
-import autohelper
-import autohelper.gui.resources
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.MainWindow import MainWindow
-from autohelper.gui.i18n.path import i18n_path
-from autohelper.gui.loading.LoadingWindow import LoadingWindow
-from autohelper.gui.overlay.OverlayWindow import OverlayWindow
-from autohelper.logging.Logger import get_logger
+import ok
+import ok.gui.resources
+from ok.gui.Communicate import communicate
+from ok.gui.MainWindow import MainWindow
+from ok.gui.i18n.path import i18n_path
+from ok.gui.loading.LoadingWindow import LoadingWindow
+from ok.gui.overlay.OverlayWindow import OverlayWindow
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class App:
     def __init__(self, icon=None, overlay=False, title="AutoUI", tasks=None,
                  exit_event=None):
@@ -85,16 +85,16 @@
             self.loading_window.update_progress(message)
 
     def show_main_window(self):
         self.loading_window.close()
         self.main_window = MainWindow(self.tasks, self.overlay, exit_event=self.exit_event)
         self.main_window.setWindowTitle(self.title)  # Set the window title here
         self.main_window.setWindowIcon(self.icon)
-        if self.overlay and autohelper.gui.device_manager.hwnd is not None:
-            self.overlay_window = OverlayWindow(autohelper.gui.device_manager.hwnd)
+        if self.overlay and ok.gui.device_manager.hwnd is not None:
+            self.overlay_window = OverlayWindow(ok.gui.device_manager.hwnd)
 
         size = self.size_relative_to_screen(width=0.5, height=0.6)
         self.main_window.resize(size)
         self.main_window.setMinimumSize(size)
 
         # Optional: Move the window to the center of the screen
```

### Comparing `ok-script-0.0.7/autohelper/gui/Communicate.py` & `ok-script-0.0.8/ok/gui/Communicate.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/MainWindow.py` & `ok-script-0.0.8/ok/gui/MainWindow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PySide6.QtCore import QObject, Signal, Slot
 from PySide6.QtWidgets import QMessageBox, QTabWidget
 
-from autohelper.gui.debug.DebugTab import DebugTab
-from autohelper.gui.tasks.TaskTab import TaskTab
-from autohelper.logging.Logger import get_logger
+from ok.gui.debug.DebugTab import DebugTab
+from ok.gui.tasks.TaskTab import TaskTab
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Communicate(QObject):
     speak = Signal(str)
```

### Comparing `ok-script-0.0.7/autohelper/gui/TabTitles.py` & `ok-script-0.0.8/ok/gui/TabTitles.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/debug/AspectRatioWidget.py` & `ok-script-0.0.8/ok/gui/debug/AspectRatioWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/debug/DebugTab.py` & `ok-script-0.0.8/ok/gui/debug/DebugTab.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QWidget, QGridLayout, QSplitter
 
-from autohelper.gui.debug.FrameWidget import FrameWidget
-from autohelper.gui.debug.InfoWidget import InfoWidget
-from autohelper.gui.debug.LoggerWidget import LoggerWidget
+from ok.gui.debug.FrameWidget import FrameWidget
+from ok.gui.debug.InfoWidget import InfoWidget
+from ok.gui.debug.LoggerWidget import LoggerWidget
 
 
 class DebugTab(QWidget):
     def __init__(self):
         super().__init__()
 
         self.mainLayout = QGridLayout()
```

### Comparing `ok-script-0.0.7/autohelper/gui/debug/FrameWidget.py` & `ok-script-0.0.8/ok/gui/debug/FrameWidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 
 import numpy as np
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QPainter, QImage, QPixmap, QColor, QPen
 from PySide6.QtWidgets import QWidget
 
-from autohelper.feature.Box import Box
-from autohelper.gui.Communicate import communicate
+from ok.feature.Box import Box
+from ok.gui.Communicate import communicate
 
 
 class FrameWidget(QWidget):
     def __init__(self, draw_frame=False, parent=None):
         super(FrameWidget, self).__init__(parent)
         self.cv_image = None
         self.color_map = {
```

### Comparing `ok-script-0.0.7/autohelper/gui/debug/InfoWidget.py` & `ok-script-0.0.8/ok/gui/debug/InfoWidget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QLabel
 
-from autohelper.gui.Communicate import communicate
+from ok.gui.Communicate import communicate
 
 
 class InfoWidget(QWidget):
 
     def __init__(self):
         super().__init__()
         self.init_ui()
```

### Comparing `ok-script-0.0.7/autohelper/gui/debug/LoggerWidget.py` & `ok-script-0.0.8/ok/gui/debug/LoggerWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from PySide6.QtWidgets import (QWidget, QVBoxLayout, QHBoxLayout, QComboBox, QLineEdit, QTextEdit)
 
-from autohelper.gui.Communicate import communicate
+from ok.gui.Communicate import communicate
 
 level_map = {'DEBUG': logging.DEBUG, 'INFO': logging.INFO, 'WARNING': logging.WARNING, 'ERROR': logging.ERROR,
              'CRITICAL': logging.CRITICAL}
 
 
 def get_colored_message(level, message):
     if level >= logging.ERROR:
```

### Comparing `ok-script-0.0.7/autohelper/gui/loading/LoadingWindow.py` & `ok-script-0.0.8/ok/gui/loading/LoadingWindow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QMessageBox, QHBoxLayout, QListWidget, QPushButton
 
-import autohelper
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.util.Alert import show_alert
-from autohelper.gui.widget.RoundCornerContainer import RoundCornerContainer
-from autohelper.interaction.Win32Interaction import is_admin
-from autohelper.logging.Logger import get_logger
+import ok
+from ok.gui.Communicate import communicate
+from ok.gui.util.Alert import show_alert
+from ok.gui.widget.RoundCornerContainer import RoundCornerContainer
+from ok.interaction.Win32Interaction import is_admin
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class LoadingWindow(QWidget):
     def __init__(self, app, exit_event):
         super().__init__()
@@ -46,39 +46,39 @@
         self.start_button = QPushButton(self.tr("Start"))
         self.start_button.setEnabled(False)
         self.start_button.clicked.connect(self.on_start_clicked)
         layout.addWidget(self.start_button, alignment=Qt.AlignCenter)
         self.update_capture()
 
     def refresh_clicked(self):
-        autohelper.gui.device_manager.refresh()
+        ok.gui.device_manager.refresh()
         self.refresh_button.setDisabled(True)
         self.refresh_button.setText(self.tr("Refreshing"))
 
     def on_start_clicked(self):
         i = self.capture_list.currentRow()
         connected = self.capture_list_data[i]["connected"]
         if not connected:
             show_alert(self.tr("Error"), self.tr("Game Window is not detected, Please open game and refresh!"))
             return
         method = self.capture_list_data[i]["method"]
         if method == "windows" and not is_admin():
             show_alert(self.tr("Error"),
                        self.tr(f"PC version requires admin privileges, Please restart this app with admin privileges!"))
             return
-        autohelper.gui.device_manager.start()
+        ok.gui.device_manager.start()
         self.app.show_main_window()
 
     def capture_index_changed(self):  # i is an index
         i = self.capture_list.currentRow()
         imei = self.capture_list_data[i]["imei"]
-        autohelper.gui.device_manager.set_preferred_device(imei)
+        ok.gui.device_manager.set_preferred_device(imei)
 
     def update_capture(self):
-        devices = autohelper.gui.device_manager.get_devices()
+        devices = ok.gui.device_manager.get_devices()
         selected = self.capture_list.currentRow()
         self.capture_list.clear()
         self.capture_list_data.clear()
         if len(devices) > 0:
             for row, device in enumerate(devices):
                 if device["preferred"]:
                     selected = row
```

### Comparing `ok-script-0.0.7/autohelper/gui/overlay/OverlayWindow.py` & `ok-script-0.0.8/ok/gui/overlay/OverlayWindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PySide6.QtCore import QObject, Signal, Qt
 
-from autohelper.capture.HwndWindow import HwndWindow
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.debug.FrameWidget import FrameWidget
-from autohelper.logging.Logger import get_logger
+from ok.capture.HwndWindow import HwndWindow
+from ok.gui.Communicate import communicate
+from ok.gui.debug.FrameWidget import FrameWidget
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Communicate(QObject):
     speak = Signal(str)
```

### Comparing `ok-script-0.0.7/autohelper/gui/resources.py` & `ok-script-0.0.8/ok/gui/resources.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/tasks/ConfigItemFactory.py` & `ok-script-0.0.8/ok/gui/tasks/ConfigItemFactory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from autohelper.gui.widget.ListTableWidgetItem import ListTableWidgetItem
-from autohelper.gui.widget.NumericTableWidgetItem import NumericTableWidgetItem
-from autohelper.gui.widget.YesNonWidgetItem import YesNonWidgetItem
+from ok.gui.widget.ListTableWidgetItem import ListTableWidgetItem
+from ok.gui.widget.NumericTableWidgetItem import NumericTableWidgetItem
+from ok.gui.widget.YesNonWidgetItem import YesNonWidgetItem
 
 
 def config_widget_item(table, row, col, config, key, value):
     if isinstance(value, bool):
         table.setCellWidget(row, 1, YesNonWidgetItem(config, key, value))
     elif isinstance(value, list):
         table.setItem(row, 1, ListTableWidgetItem(config, key, value))
```

### Comparing `ok-script-0.0.7/autohelper/gui/tasks/StartButton.py` & `ok-script-0.0.8/ok/gui/tasks/StartButton.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PySide6.QtCore import Slot, QPropertyAnimation
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QPushButton
 
-import autohelper
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.util.Alert import show_alert
-from autohelper.logging.Logger import get_logger
+import ok
+from ok.gui.Communicate import communicate
+from ok.gui.util.Alert import show_alert
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class StartButton(QPushButton):
     def __init__(self):
         super().__init__("Start")
@@ -29,19 +29,19 @@
             self.setChecked(True)
             self.start_animation()
 
     @Slot()
     def toggle_text(self):
         if self.isChecked():
             logger.info("Click Start Executor")
-            if not autohelper.gui.executor.start():
+            if not ok.gui.executor.start():
                 show_alert("Error", "No Task to Run, Please Enable Task First!")
                 self.setChecked(False)
         else:
             logger.info("Click Pause Executor")
-            autohelper.gui.executor.pause()
+            ok.gui.executor.pause()
 
     def start_animation(self):
         self.animation.setStartValue(QColor(0, 0, 0))
         self.animation.setEndValue(QColor(255, 255, 255))
         self.animation.setDuration(1000)
         self.animation.start()
```

### Comparing `ok-script-0.0.7/autohelper/gui/tasks/TaskTab.py` & `ok-script-0.0.8/ok/gui/tasks/TaskTab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List
 
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QTableWidget, QTableWidgetItem, QVBoxLayout, QWidget, QHBoxLayout
 
-from autohelper.gui.Communicate import communicate
-from autohelper.gui.tasks.ConfigItemFactory import config_widget_item
-from autohelper.gui.tasks.StartButton import StartButton
-from autohelper.gui.tasks.TaskOpButton import TaskOpButton
-from autohelper.gui.tasks.TooltipTableWidget import TooltipTableWidget
-from autohelper.gui.widget.RoundCornerContainer import RoundCornerContainer
-from autohelper.gui.widget.UpdateConfigWidgetItem import value_to_string
-from autohelper.logging.Logger import get_logger
-from autohelper.task.BaseTask import BaseTask
+from ok.gui.Communicate import communicate
+from ok.gui.tasks.ConfigItemFactory import config_widget_item
+from ok.gui.tasks.StartButton import StartButton
+from ok.gui.tasks.TaskOpButton import TaskOpButton
+from ok.gui.tasks.TooltipTableWidget import TooltipTableWidget
+from ok.gui.widget.RoundCornerContainer import RoundCornerContainer
+from ok.gui.widget.UpdateConfigWidgetItem import value_to_string
+from ok.logging.Logger import get_logger
+from ok.task.BaseTask import BaseTask
 
 logger = get_logger(__name__)
 
 
 class TaskTab(QWidget):
     def __init__(self, tasks: List[BaseTask]):
         super().__init__()
```

### Comparing `ok-script-0.0.7/autohelper/gui/tasks/TooltipTableWidget.py` & `ok-script-0.0.8/ok/gui/tasks/TooltipTableWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/widget/ListTableWidgetItem.py` & `ok-script-0.0.8/ok/gui/widget/ListTableWidgetItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QTableWidgetItem
 
-from autohelper.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem, value_to_string
+from ok.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem, value_to_string
 
 
 class ListTableWidgetItem(UpdateConfigWidgetItem, QTableWidgetItem):
 
     def __init__(self, config, key, value, parent=None):
         UpdateConfigWidgetItem.__init__(self, config, key, value)
         QTableWidgetItem.__init__(self)
```

### Comparing `ok-script-0.0.7/autohelper/gui/widget/NumericTableWidgetItem.py` & `ok-script-0.0.8/ok/gui/widget/NumericTableWidgetItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIntValidator, QDoubleValidator
 from PySide6.QtWidgets import QTableWidgetItem
 
-from autohelper.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem, value_to_string
+from ok.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem, value_to_string
 
 
 class NumericTableWidgetItem(UpdateConfigWidgetItem, QTableWidgetItem):
 
     def __init__(self, config, key, value, parent=None):
         UpdateConfigWidgetItem.__init__(self, config, key, value)
         QTableWidgetItem.__init__(self)
```

### Comparing `ok-script-0.0.7/autohelper/gui/widget/RoundCornerContainer.py` & `ok-script-0.0.8/ok/gui/widget/RoundCornerContainer.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/widget/TabWidget.py` & `ok-script-0.0.8/ok/gui/widget/TabWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/gui/widget/YesNonWidgetItem.py` & `ok-script-0.0.8/ok/gui/widget/YesNonWidgetItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PySide6.QtWidgets import QComboBox
 
-from autohelper.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem
+from ok.gui.widget.UpdateConfigWidgetItem import UpdateConfigWidgetItem
 
 
 class YesNonWidgetItem(UpdateConfigWidgetItem, QComboBox):
 
     def __init__(self, config, key, value):
         UpdateConfigWidgetItem.__init__(self, config, key, value)
         QComboBox.__init__(self)
```

### Comparing `ok-script-0.0.7/autohelper/interaction/ADBInteraction.py` & `ok-script-0.0.8/ok/interaction/ADBInteraction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from autohelper.interaction.BaseInteraction import BaseInteraction
-from autohelper.logging.Logger import get_logger
+from ok.interaction.BaseInteraction import BaseInteraction
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class ADBBaseInteraction(BaseInteraction):
 
     def __init__(self, device_manager, capture):
```

### Comparing `ok-script-0.0.7/autohelper/interaction/BaseInteraction.py` & `ok-script-0.0.8/ok/interaction/BaseInteraction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from autohelper.feature.Box import Box
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
+from ok.feature.Box import Box
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class BaseInteraction:
 
     def __init__(self, capture):
```

### Comparing `ok-script-0.0.7/autohelper/interaction/Win32Interaction.py` & `ok-script-0.0.8/ok/interaction/Win32Interaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ctypes
 import time
 
 import pydirectinput
 
-from autohelper.capture.BaseCaptureMethod import BaseCaptureMethod
-from autohelper.interaction.BaseInteraction import BaseInteraction
-from autohelper.logging.Logger import get_logger
+from ok.capture.BaseCaptureMethod import BaseCaptureMethod
+from ok.interaction.BaseInteraction import BaseInteraction
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Win32Interaction(BaseInteraction):
 
     def __init__(self, capture: BaseCaptureMethod):
```

### Comparing `ok-script-0.0.7/autohelper/logging/Logger.py` & `ok-script-0.0.8/ok/logging/Logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import traceback
 from logging.handlers import TimedRotatingFileHandler
 
-from autohelper.gui.Communicate import communicate
-from autohelper.util.path import get_path_relative_to_exe, ensure_dir_for_file
+from ok.gui.Communicate import communicate
+from ok.util.path import get_path_relative_to_exe, ensure_dir_for_file
 
 
 class CommunicateHandler(logging.Handler):
     def __init__(self):
         super().__init__()
 
     def emit(self, record):
@@ -27,15 +27,15 @@
     # If there's no ".", return an empty string or the original string based on your need
     if last_dot_index == -1:
         return ""  # or return s to return the whole string if there's no dot
     # Slice the string from just after the last "." to the end
     return s[last_dot_index + 1:]
 
 
-auto_helper_logger = logging.getLogger("autohelper")
+auto_helper_logger = logging.getLogger("ok")
 
 
 def config_logger(config):
     if config.get('debug'):
         auto_helper_logger.setLevel(logging.DEBUG)
     else:
         auto_helper_logger.setLevel(logging.INFO)
```

### Comparing `ok-script-0.0.7/autohelper/ocr/OCR.py` & `ok-script-0.0.8/ok/ocr/OCR.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
-from autohelper.feature.Box import Box, sort_boxes, find_boxes_by_name
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
+from ok.feature.Box import Box, sort_boxes, find_boxes_by_name
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class OCR:
     executor = None
     default_threshold = 0.6
```

### Comparing `ok-script-0.0.7/autohelper/predict/predict.py` & `ok-script-0.0.8/ok/predict/predict.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Foundation/Collections.py` & `ok-script-0.0.8/ok/rotypes/Windows/Foundation/Collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ctypes import c_uint, c_uint32, c_bool
 from functools import lru_cache
 
 from _ctypes import POINTER
 
-from autohelper.rotypes.idldsl import define_winrt_com_method, pinterface_type
-from autohelper.rotypes.inspectable import IInspectable
+from ok.rotypes.idldsl import define_winrt_com_method, pinterface_type
+from ok.rotypes.inspectable import IInspectable
 
 
 class IIterator_helpers:
     def __next__(self):
         if self.HasCurrent:
             value = self.Current
             self.MoveNext()
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Foundation/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Foundation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from ctypes import Structure, c_float, HRESULT, c_int, windll, c_uint32, c_int32, WinError
 
-from autohelper.rotypes import delegate, HSTRING
-from autohelper.rotypes.idldsl import define_winrt_com_method, generics_cache, define_winrt_com_delegate, pinterface_type, \
+from ok.rotypes import delegate, HSTRING
+from ok.rotypes.idldsl import define_winrt_com_method, generics_cache, define_winrt_com_delegate, pinterface_type, \
     GUID
-from autohelper.rotypes.inspectable import IInspectable, IUnknown
+from ok.rotypes.inspectable import IInspectable, IUnknown
 
 _kernel32 = windll.LoadLibrary('kernel32.dll')
 _CreateEvent = _kernel32.CreateEventW
 _SetEvent = _kernel32.SetEvent
 _WaitForSingleObject = _kernel32.WaitForSingleObject
 _CloseHandle = _kernel32.CloseHandle
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Globalization/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Globalization/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from autohelper.rotypes.idldsl import define_winrt_com_method, runtimeclass, _static_method, GUID
-from autohelper.rotypes.inspectable import IInspectable
-from autohelper.rotypes.winstring import HSTRING
+from ok.rotypes.idldsl import define_winrt_com_method, runtimeclass, _static_method, GUID
+from ok.rotypes.inspectable import IInspectable
+from ok.rotypes.winstring import HSTRING
 
 
 @GUID('EA79A752-F7C2-4265-B1BD-C4DEC4E4F080')
 class ILanguage(IInspectable):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Capture/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from ctypes import c_bool, c_int32, c_int64
 from ctypes.wintypes import HWND, HMONITOR
 
-from autohelper.rotypes.Windows.Foundation import IClosable, TypedEventHandler
-from autohelper.rotypes.Windows.Graphics import SizeInt32
-from autohelper.rotypes.Windows.Graphics.DirectX import DirectXPixelFormat
-from autohelper.rotypes.idldsl import define_winrt_com_method, runtimeclass, GUID, \
+from ok.rotypes.Windows.Foundation import IClosable, TypedEventHandler
+from ok.rotypes.Windows.Graphics import SizeInt32
+from ok.rotypes.Windows.Graphics.DirectX import DirectXPixelFormat
+from ok.rotypes.idldsl import define_winrt_com_method, runtimeclass, GUID, \
     runtimeclass_add_statics
-from autohelper.rotypes.inspectable import IInspectable, IUnknown
-from autohelper.rotypes.types import REFGUID
-from autohelper.rotypes.winstring import HSTRING
+from ok.rotypes.inspectable import IInspectable, IUnknown
+from ok.rotypes.types import REFGUID
+from ok.rotypes.winstring import HSTRING
 
 
 @GUID('FA50C623-38DA-4B32-ACF3-FA9734AD800E')
 class IDirect3D11CaptureFrame(IInspectable):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ctypes
 
-import autohelper.rotypes as rotypes
-import autohelper.rotypes.Windows.Foundation
-import autohelper.rotypes.idldsl
-from autohelper.rotypes.types import REFGUID
+import ok.rotypes as rotypes
+import ok.rotypes.Windows.Foundation
+import ok.rotypes.idldsl
+from ok.rotypes.types import REFGUID
 
 
 @rotypes.idldsl.GUID('A37624AB-8D5F-4650-9D3E-9EAE3D9BC670')
 class _IDirect3DDevice(rotypes.IInspectable):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/DirectX/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autohelper.rotypes.idldsl import CtypesEnum
+from ok.rotypes.idldsl import CtypesEnum
 
 
 class DirectXAlphaMode(CtypesEnum):
     Unspecified = 0
     Premultiplied = 1
     Straight = 2
     Ignore = 3
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Graphics/Imaging/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ctypes import c_int, c_int32
 
-import autohelper.rotypes.Windows.Storage.Streams
-from autohelper.rotypes.Windows.Foundation import IClosable
-from autohelper.rotypes.idldsl import define_winrt_com_method, _static_method, runtimeclass, GUID
-from autohelper.rotypes.inspectable import IInspectable
+import ok.rotypes.Windows.Storage.Streams
+from ok.rotypes.Windows.Foundation import IClosable
+from ok.rotypes.idldsl import define_winrt_com_method, _static_method, runtimeclass, GUID
+from ok.rotypes.inspectable import IInspectable
 
 
 @GUID('689e0708-7eef-483f-963f-da938818e073')
 class ISoftwareBitmap(IClosable, IInspectable):
     pass
 
 
@@ -25,10 +25,10 @@
 
 
 class SoftwareBitmap(runtimeclass, ISoftwareBitmap):
     CreateCopyWithAlphaFromBuffer = _static_method(ISoftwareBitmapStatics, 'CreateCopyWithAlphaFromBuffer')
 
 
 define_winrt_com_method(ISoftwareBitmapStatics, "CreateCopyWithAlphaFromBuffer",
-                        autohelper.rotypes.Windows.Storage.Streams.IBuffer, BitmapPixelFormat, c_int32, c_int32,
+                        ok.rotypes.Windows.Storage.Streams.IBuffer, BitmapPixelFormat, c_int32, c_int32,
                         BitmapAlphaMode,
                         retval=SoftwareBitmap, vtbl=10)
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Media/Ocr/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from ctypes import c_uint32, c_bool, c_double
 
-from autohelper.rotypes.Windows.Foundation import IReference, Rect, IAsyncOperation
-from autohelper.rotypes.Windows.Foundation.Collections import IVectorView
-from autohelper.rotypes.Windows.Globalization import Language
-from autohelper.rotypes.Windows.Graphics.Imaging import SoftwareBitmap
-from autohelper.rotypes.idldsl import define_winrt_com_method, _static_propget, _static_method, _non_activatable_init, \
+from ok.rotypes.Windows.Foundation import IReference, Rect, IAsyncOperation
+from ok.rotypes.Windows.Foundation.Collections import IVectorView
+from ok.rotypes.Windows.Globalization import Language
+from ok.rotypes.Windows.Graphics.Imaging import SoftwareBitmap
+from ok.rotypes.idldsl import define_winrt_com_method, _static_propget, _static_method, _non_activatable_init, \
     runtimeclass, GUID
-from autohelper.rotypes.inspectable import IInspectable
-from autohelper.rotypes.winstring import HSTRING
+from ok.rotypes.inspectable import IInspectable
+from ok.rotypes.winstring import HSTRING
 
 
 @GUID('3C2A477A-5CD9-3525-BA2A-23D1E0A68A1D')
 class IOcrWord(IInspectable):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/Windows/Storage/Streams/__init__.py` & `ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ctypes import c_uint32, c_void_p, string_at
 
-from autohelper.rotypes.idldsl import define_winrt_com_method, GUID
-from autohelper.rotypes.inspectable import IInspectable, IUnknown
+from ok.rotypes.idldsl import define_winrt_com_method, GUID
+from ok.rotypes.inspectable import IInspectable, IUnknown
 
 
 @GUID('905a0fef-bc53-11df-8c49-001e4fc686da')
 class IBufferByteAccess(IUnknown):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/rotypes/delegate.py` & `ok-script-0.0.8/ok/rotypes/delegate.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/export.py` & `ok-script-0.0.8/ok/rotypes/export.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/idldsl.py` & `ok-script-0.0.8/ok/rotypes/idldsl.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/inspectable.py` & `ok-script-0.0.8/ok/rotypes/inspectable.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/roapi.py` & `ok-script-0.0.8/ok/rotypes/roapi.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/types.py` & `ok-script-0.0.8/ok/rotypes/types.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/rotypes/winstring.py` & `ok-script-0.0.8/ok/rotypes/winstring.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/save/BlackBarProcessor.py` & `ok-script-0.0.8/ok/save/BlackBarProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cv2
 import numpy as np
 
-from autohelper.save.PostProcessor import PostProcessor
+from ok.save.PostProcessor import PostProcessor
 
 
 class BlackBarProcessor(PostProcessor):
     def __init__(self, x, y, width, height, color=(1, 1, 1)):
         self.x = x
         self.y = y
         self.width = width
```

### Comparing `ok-script-0.0.7/autohelper/save/SaveByInterval.py` & `ok-script-0.0.8/ok/save/SaveByInterval.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 
 import cv2
 
-from autohelper.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
+from ok.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
 
 
 class SaveByInterval:
 
     def __init__(self, method: "BaseCaptureMethod", interval=1):
         self.interval = interval
         self.method = method
```

### Comparing `ok-script-0.0.7/autohelper/save/SaveByKeyPress.py` & `ok-script-0.0.8/ok/save/SaveByKeyPress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pynput import keyboard
 
-from autohelper.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
-from autohelper.save.PostProcessor import PostProcessor
-from autohelper.save.SaveMethodBase import SaveMethodBase
+from ok.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
+from ok.save.PostProcessor import PostProcessor
+from ok.save.SaveMethodBase import SaveMethodBase
 
 
 class SaveByKeyPress(SaveMethodBase):
 
     def __init__(self, method: BaseCaptureMethod, image_processor: PostProcessor = None, capture_key="c", stop_key="x"):
         super().__init__(method, image_processor)
         self.capture_key = capture_key
```

### Comparing `ok-script-0.0.7/autohelper/save/SaveMethodBase.py` & `ok-script-0.0.8/ok/save/SaveMethodBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import threading
 
 import cv2
 
-from autohelper.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
-from autohelper.save.PostProcessor import PostProcessor
+from ok.capture.windows.WindowsGraphicsCaptureMethod import BaseCaptureMethod
+from ok.save.PostProcessor import PostProcessor
 
 
 class SaveMethodBase:
 
     def __init__(self, method: BaseCaptureMethod, image_processor: PostProcessor = None):
         self.method = method
         self.image_processor = image_processor
```

### Comparing `ok-script-0.0.7/autohelper/scene/Scene.py` & `ok-script-0.0.8/ok/scene/Scene.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
-from autohelper.task.ExecutorOperation import ExecutorOperation
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
+from ok.task.ExecutorOperation import ExecutorOperation
 
 
 class Scene(ExecutorOperation):
     name = None
 
     def __init__(self):
         self.name = self.__class__.__name__
```

### Comparing `ok-script-0.0.7/autohelper/stats/StreamStats.py` & `ok-script-0.0.8/ok/stats/StreamStats.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/task/BaseTask.py` & `ok-script-0.0.8/ok/task/BaseTask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 
-from autohelper.config.Config import Config
-from autohelper.config.InfoDict import InfoDict
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
-from autohelper.task.ExecutorOperation import ExecutorOperation
+from ok.config.Config import Config
+from ok.config.InfoDict import InfoDict
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
+from ok.task.ExecutorOperation import ExecutorOperation
 
 logger = get_logger(__name__)
 
 
 class BaseTask(ExecutorOperation):
     _done = False
```

### Comparing `ok-script-0.0.7/autohelper/task/ExecutorOperation.py` & `ok-script-0.0.8/ok/task/ExecutorOperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from autohelper.feature.Box import Box, find_box_by_name
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
+from ok.feature.Box import Box, find_box_by_name
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class ExecutorOperation:
     executor = None
```

### Comparing `ok-script-0.0.7/autohelper/task/TaskExecutor.py` & `ok-script-0.0.8/ok/task/TaskExecutor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import threading
 import time
 import traceback
 
-from autohelper.capture.adb.DeviceManager import DeviceManager
-from autohelper.gui.Communicate import communicate
-from autohelper.logging.Logger import get_logger
-from autohelper.scene.Scene import Scene
-from autohelper.stats.StreamStats import StreamStats
+from ok.capture.adb.DeviceManager import DeviceManager
+from ok.gui.Communicate import communicate
+from ok.logging.Logger import get_logger
+from ok.scene.Scene import Scene
+from ok.stats.StreamStats import StreamStats
 
 logger = get_logger(__name__)
 
 
 class TaskDisabledException(Exception):
     pass
```

### Comparing `ok-script-0.0.7/autohelper/util/json.py` & `ok-script-0.0.8/ok/util/json.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 
-from autohelper.util.path import ensure_dir_for_file
+from ok.util.path import ensure_dir_for_file
 
 
 def read_json_file(file_path) -> dict | None:
     if not os.path.exists(file_path):
         return None
 
     try:
```

### Comparing `ok-script-0.0.7/autohelper/util/path.py` & `ok-script-0.0.8/ok/util/path.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/util/win32_process.py` & `ok-script-0.0.8/ok/util/win32_process.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.7/autohelper/util/yaml.py` & `ok-script-0.0.8/ok/util/yaml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import yaml
 
-from autohelper.util.path import ensure_dir_for_file
+from ok.util.path import ensure_dir_for_file
 
 
 def read_yaml_file(file_path) -> dict | None:
     if not os.path.exists(file_path):
         return None
 
     try:
```

### Comparing `ok-script-0.0.7/ok_script.egg-info/PKG-INFO` & `ok-script-0.0.8/ok_script.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ok-script
-Version: 0.0.7
+Version: 0.0.8
 Summary: Automation with Computer Vision for Python
 Home-page: https://github.com/ok-oldking/ok-script
 Author: ok-oldking
 Author-email: firedcto@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ok-script-0.0.7/setup.py` & `ok-script-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ok-script",
-    version="0.0.7",
+    version="0.0.8",
     author="ok-oldking",
     author_email="firedcto@gmail.com",
     description="Automation with Computer Vision for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ok-oldking/ok-script",
     packages=setuptools.find_packages(),
```

