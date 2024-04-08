# Comparing `tmp/tcxreader-0.4.8.tar.gz` & `tmp/tcxreader-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcxreader-0.4.8.tar", max compression
+gzip compressed data, was "tcxreader-0.4.9.tar", max compression
```

## Comparing `tcxreader-0.4.8.tar` & `tcxreader-0.4.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1087 2022-07-25 18:44:57.356225 tcxreader-0.4.8/LICENSE
--rw-r--r--   0        0        0      995 2024-01-31 15:31:33.643375 tcxreader-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    13167 2024-01-31 15:32:17.941039 tcxreader-0.4.8/README.md
--rw-r--r--   0        0        0      253 2023-11-24 11:07:47.714609 tcxreader-0.4.8/tcxreader/__init__.py
--rw-r--r--   0        0        0      939 2023-11-30 14:48:37.293981 tcxreader-0.4.8/tcxreader/tcx_author.py
--rw-r--r--   0        0        0     3450 2023-11-30 14:46:47.001576 tcxreader-0.4.8/tcxreader/tcx_exercise.py
--rw-r--r--   0        0        0     3138 2023-11-28 15:57:08.338024 tcxreader-0.4.8/tcxreader/tcx_lap.py
--rw-r--r--   0        0        0     1813 2023-11-30 14:50:12.499687 tcxreader-0.4.8/tcxreader/tcx_track_point.py
--rw-r--r--   0        0        0    17579 2024-01-31 15:27:34.887159 tcxreader-0.4.8/tcxreader/tcxreader.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 tcxreader-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-07-25 18:44:57.356225 tcxreader-0.4.9/LICENSE
+-rw-r--r--   0        0        0      995 2024-01-31 15:41:10.325746 tcxreader-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    13167 2024-01-31 15:32:17.941039 tcxreader-0.4.9/README.md
+-rw-r--r--   0        0        0      253 2023-11-24 11:07:47.714609 tcxreader-0.4.9/tcxreader/__init__.py
+-rw-r--r--   0        0        0      939 2023-11-30 14:48:37.293981 tcxreader-0.4.9/tcxreader/tcx_author.py
+-rw-r--r--   0        0        0     3450 2023-11-30 14:46:47.001576 tcxreader-0.4.9/tcxreader/tcx_exercise.py
+-rw-r--r--   0        0        0     3138 2023-11-28 15:57:08.338024 tcxreader-0.4.9/tcxreader/tcx_lap.py
+-rw-r--r--   0        0        0     1813 2023-11-30 14:50:12.499687 tcxreader-0.4.9/tcxreader/tcx_track_point.py
+-rw-r--r--   0        0        0    17552 2024-01-31 15:40:58.612111 tcxreader-0.4.9/tcxreader/tcxreader.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 tcxreader-0.4.9/PKG-INFO
```

### Comparing `tcxreader-0.4.8/LICENSE` & `tcxreader-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/pyproject.toml` & `tcxreader-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcxreader"
-version = "0.4.8"
+version = "0.4.9"
 description = "tcxreader is a reader for Garmin’s TCX file format. It also works well with missing data!"
 authors = ["Alen Rajšp <alen.rajsp@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/alenrajsp/tcxreader"
 repository = "https://github.com/alenrajsp/tcxreader"
 classifiers = [
     "Programming Language :: Python :: 3.6",
```

### Comparing `tcxreader-0.4.8/README.md` & `tcxreader-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/tcxreader/tcx_author.py` & `tcxreader-0.4.9/tcxreader/tcx_author.py`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/tcxreader/tcx_exercise.py` & `tcxreader-0.4.9/tcxreader/tcx_exercise.py`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/tcxreader/tcx_lap.py` & `tcxreader-0.4.9/tcxreader/tcx_lap.py`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/tcxreader/tcx_track_point.py` & `tcxreader-0.4.9/tcxreader/tcx_track_point.py`

 * *Files identical despite different names*

### Comparing `tcxreader-0.4.8/tcxreader/tcxreader.py` & `tcxreader-0.4.9/tcxreader/tcxreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     NONE = 1
     LINEAR_INTERPOLATION = 2
 
 class TCXReader:
     def __init__(self):
         pass
 
-    def read(self, fileLocation: str, only_gps: bool = True, null_value_handling: int | NullValueHandling = 1) -> TCXExercise:
+    def read(self, fileLocation: str, only_gps: bool = True, null_value_handling: int = 1) -> TCXExercise:
         """
         :param only_gps: If set to True erases any Trackpoints at the start and end of the exercise without GPS data.
         :param fileLocation: Location of the TCX file.
         :param null_value_handling: How to handle null values in TCX file. 1 = set to None, 2 = linear interpolation.
         :returns: A list of TCXTrackPoint objects.
         """
 
@@ -252,15 +252,15 @@
                 tpx_ext=new_tpx_ext,
                 time=trackpoints[i].time
             )
             new_trackpoints.append(new_trackpoint)
 
         return new_trackpoints
 
-    def __find_hi_lo_avg(self, tcx: TCXExercise|TCXLap, only_gps: bool) -> TCXExercise:
+    def __find_hi_lo_avg(self, tcx: TCXExercise, only_gps: bool) -> TCXExercise:
         trackpoints = tcx.trackpoints
 
         if only_gps == True:
             removalList = []
             for index in range(len(trackpoints)):
                 if trackpoints[index].longitude == None:
                     removalList.append(index)
```

### Comparing `tcxreader-0.4.8/PKG-INFO` & `tcxreader-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcxreader
-Version: 0.4.8
+Version: 0.4.9
 Summary: tcxreader is a reader for Garmin’s TCX file format. It also works well with missing data!
 Home-page: https://github.com/alenrajsp/tcxreader
 License: MIT
 Author: Alen Rajšp
 Author-email: alen.rajsp@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
```

