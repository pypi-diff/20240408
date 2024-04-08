# Comparing `tmp/libsrg-3.8.6-py3-none-any.whl.zip` & `tmp/libsrg-4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 37457 bytes, number of entries: 27
+Zip file size: 49098 bytes, number of entries: 41
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
+-rw-r--r--  2.0 unx     5445 b- defN 24-Apr-08 17:25 libsrg/Config.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
 -rw-r--r--  2.0 unx     6536 b- defN 24-Apr-02 16:28 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6093 b- defN 24-Apr-02 15:52 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
@@ -12,18 +13,31 @@
 -rw-r--r--  2.0 unx    15682 b- defN 24-Feb-24 19:36 libsrg/ReZFS.py
 -rw-r--r--  2.0 unx     5865 b- defN 24-Apr-02 15:44 libsrg/Runner.py
 -rw-r--r--  2.0 unx     4035 b- defN 23-May-22 23:46 libsrg/Runner2.py
 -rw-r--r--  2.0 unx     7024 b- defN 23-Oct-05 17:56 libsrg/Stage0.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 16:52 libsrg/__init__.py
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:35 libsrg/template.py
 -rw-r--r--  2.0 unx    26527 b- defN 24-Jan-08 17:22 libsrg/ztool.py
+-rw-r--r--  2.0 unx     2000 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsBase.py
+-rw-r--r--  2.0 unx     1436 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsCumulative.py
+-rw-r--r--  2.0 unx     2300 b- defN 24-Apr-08 17:02 libsrg/Statistics/AnalogStatsFading.py
+-rw-r--r--  2.0 unx     1175 b- defN 24-Apr-08 17:02 libsrg/Statistics/DiscreteStatsBase.py
+-rw-r--r--  2.0 unx      774 b- defN 24-Apr-08 17:02 libsrg/Statistics/DiscreteStatsCumulative.py
+-rw-r--r--  2.0 unx     3644 b- defN 24-Apr-07 19:48 libsrg/Statistics/RunStatsBase.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/__init__.py
+-rw-r--r--  2.0 unx     2525 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+-rw-r--r--  2.0 unx     3884 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+-rw-r--r--  2.0 unx     1604 b- defN 24-Apr-08 17:25 libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+-rw-r--r--  2.0 unx     1391 b- defN 24-Apr-08 17:02 libsrg/Statistics/UnitTests/RunStatsBase_test.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-07 19:48 libsrg/Statistics/UnitTests/__init__.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-02 16:28 libsrg-3.8.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-02 16:28 libsrg-3.8.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 16:28 libsrg-3.8.6.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-02 16:28 libsrg-3.8.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2092 b- defN 24-Apr-02 16:28 libsrg-3.8.6.dist-info/RECORD
-27 files, 114447 bytes uncompressed, 34149 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3358 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3460 b- defN 24-Apr-08 17:30 libsrg-4.0.0.dist-info/RECORD
+41 files, 144308 bytes uncompressed, 43572 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: libsrg/AppTemplate.py
 Comment: 
 
+Filename: libsrg/Config.py
+Comment: 
+
 Filename: libsrg/ElapsedTime.py
 Comment: 
 
 Filename: libsrg/Info.py
 Comment: 
 
 Filename: libsrg/LevelBanner.py
@@ -45,14 +48,53 @@
 
 Filename: libsrg/template.py
 Comment: 
 
 Filename: libsrg/ztool.py
 Comment: 
 
+Filename: libsrg/Statistics/AnalogStatsBase.py
+Comment: 
+
+Filename: libsrg/Statistics/AnalogStatsCumulative.py
+Comment: 
+
+Filename: libsrg/Statistics/AnalogStatsFading.py
+Comment: 
+
+Filename: libsrg/Statistics/DiscreteStatsBase.py
+Comment: 
+
+Filename: libsrg/Statistics/DiscreteStatsCumulative.py
+Comment: 
+
+Filename: libsrg/Statistics/RunStatsBase.py
+Comment: 
+
+Filename: libsrg/Statistics/__init__.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/AnalogStatsBase_test.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/AnalogStatsCumulative_test.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/AnalogStatsFading_test.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/DiscteteStatsBase_test.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/RunStatsBase_test.py
+Comment: 
+
+Filename: libsrg/Statistics/UnitTests/__init__.py
+Comment: 
+
 Filename: libsrg/TKGUI/GuiBase.py
 Comment: 
 
 Filename: libsrg/TKGUI/GuiRequest.py
 Comment: 
 
 Filename: libsrg/TKGUI/GuiRequestQueue.py
@@ -60,23 +102,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-3.8.6.dist-info/LICENSE.txt
+Filename: libsrg-4.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-3.8.6.dist-info/METADATA
+Filename: libsrg-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-3.8.6.dist-info/WHEEL
+Filename: libsrg-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-3.8.6.dist-info/top_level.txt
+Filename: libsrg-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-3.8.6.dist-info/RECORD
+Filename: libsrg-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libsrg-3.8.6.dist-info/LICENSE.txt` & `libsrg-4.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-3.8.6.dist-info/METADATA` & `libsrg-4.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 3.8.6
+Version: 4.0.0
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ## Name
 libsrg -- count calls to python logging at each logging severity level
 
 ## Description
```

