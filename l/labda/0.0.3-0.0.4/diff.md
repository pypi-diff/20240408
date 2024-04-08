# Comparing `tmp/labda-0.0.3.tar.gz` & `tmp/labda-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.3.tar", max compression
+gzip compressed data, was "labda-0.0.4.tar", max compression
```

## Comparing `labda-0.0.3.tar` & `labda-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,49 @@
--rw-r--r--   0        0        0      548 2024-02-06 17:52:16.166389 labda-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      570 2024-04-02 08:48:51.335892 labda-0.0.3/README.md
--rw-r--r--   0        0        0      151 2024-04-02 08:48:51.335892 labda-0.0.3/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.3/labda/assets/__init__.py
--rw-r--r--   0        0        0      329 2024-03-26 12:57:17.697713 labda-0.0.3/labda/assets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1080 2024-04-02 08:49:41.505981 labda-0.0.3/labda/assets/__pycache__/counts_cut_points.cpython-311.pyc
--rw-r--r--   0        0        0      630 2024-04-02 11:28:55.363245 labda-0.0.3/labda/assets/__pycache__/transportation_cut_points.cpython-311.pyc
--rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.3/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      459 2024-04-02 11:28:47.324035 labda-0.0.3/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.3/labda/expanders/__init__.py
--rw-r--r--   0        0        0      432 2024-02-06 18:20:13.138435 labda-0.0.3/labda/expanders/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1351 2024-03-26 08:50:45.871038 labda-0.0.3/labda/expanders/__pycache__/accelerometer.cpython-311.pyc
--rw-r--r--   0        0        0     1469 2024-03-26 08:50:44.271381 labda-0.0.3/labda/expanders/__pycache__/extras.cpython-311.pyc
--rw-r--r--   0        0        0     9044 2024-04-02 08:49:41.475981 labda-0.0.3/labda/expanders/__pycache__/spatial.cpython-311.pyc
--rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.3/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.3/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.3/labda/expanders/spatial.py
--rw-r--r--   0        0        0     1140 2024-04-02 08:51:28.536242 labda-0.0.3/labda/logging.py
--rw-r--r--   0        0        0     1073 2024-04-02 14:15:23.256237 labda-0.0.3/labda/parallel.py
--rw-r--r--   0        0        0      141 2024-03-05 08:22:02.089665 labda-0.0.3/labda/parsers/__init__.py
--rw-r--r--   0        0        0      394 2024-04-02 08:49:41.505981 labda-0.0.3/labda/parsers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11178 2024-04-02 08:52:02.746325 labda-0.0.3/labda/parsers/__pycache__/actigraph.cpython-311.pyc
--rw-r--r--   0        0        0     1802 2024-04-02 08:49:42.015982 labda-0.0.3/labda/parsers/__pycache__/bulk.cpython-311.pyc
--rw-r--r--   0        0        0    10001 2024-04-02 08:49:41.505981 labda-0.0.3/labda/parsers/__pycache__/gadgetbridge.cpython-311.pyc
--rw-r--r--   0        0        0    18382 2024-04-02 10:22:16.092741 labda-0.0.3/labda/parsers/__pycache__/qstarz.cpython-311.pyc
--rw-r--r--   0        0        0     2120 2024-04-02 10:56:34.978296 labda-0.0.3/labda/parsers/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      617 2024-02-06 18:20:13.168428 labda-0.0.3/labda/parsers/__pycache__/vendors.cpython-311.pyc
--rw-r--r--   0        0        0     6854 2024-04-02 08:51:54.456305 labda-0.0.3/labda/parsers/actigraph.py
--rw-r--r--   0        0        0      930 2024-04-02 08:48:51.335892 labda-0.0.3/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6765 2024-03-26 07:45:27.282975 labda-0.0.3/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.3/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10772 2024-04-02 10:20:55.340245 labda-0.0.3/labda/parsers/qstarz.py
--rw-r--r--   0        0        0     1157 2024-04-02 10:31:20.628801 labda-0.0.3/labda/parsers/utils.py
--rw-r--r--   0        0        0       36 2024-02-09 10:52:49.204568 labda-0.0.3/labda/processing/__init__.py
--rw-r--r--   0        0        0      224 2024-02-09 10:55:00.040194 labda-0.0.3/labda/processing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3222 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/__pycache__/bouts.cpython-311.pyc
--rw-r--r--   0        0        0     1222 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/__pycache__/domains.cpython-311.pyc
--rw-r--r--   0        0        0     1302 2024-03-26 08:50:45.881036 labda-0.0.3/labda/processing/__pycache__/manipulations.cpython-311.pyc
--rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.3/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0      316 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/accelerometer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2770 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/accelerometer/__pycache__/activity_intensity.cpython-311.pyc
--rw-r--r--   0        0        0     2754 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/accelerometer/__pycache__/cut_points.cpython-311.pyc
--rw-r--r--   0        0        0     1282 2024-02-09 11:45:26.255590 labda-0.0.3/labda/processing/accelerometer/__pycache__/steps.cpython-311.pyc
--rw-r--r--   0        0        0     1411 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/accelerometer/__pycache__/wear.cpython-311.pyc
--rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.3/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/bouts.py
--rw-r--r--   0        0        0      751 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/domains.py
--rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.3/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0      501 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/spatial/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7768 2024-04-02 09:40:11.576062 labda-0.0.3/labda/processing/spatial/__pycache__/manipulations.cpython-311.pyc
--rw-r--r--   0        0        0     5145 2024-04-02 12:07:44.826996 labda-0.0.3/labda/processing/spatial/__pycache__/timeline.cpython-311.pyc
--rw-r--r--   0        0        0     4487 2024-04-02 08:49:41.485981 labda-0.0.3/labda/processing/spatial/__pycache__/transportation.cpython-311.pyc
--rw-r--r--   0        0        0    27515 2024-04-02 13:47:45.136539 labda-0.0.3/labda/processing/spatial/__pycache__/trips.cpython-311.pyc
--rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.3/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     3061 2024-04-02 12:07:23.697246 labda-0.0.3/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     2198 2024-04-02 08:48:51.335892 labda-0.0.3/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    24216 2024-04-02 13:46:22.410849 labda-0.0.3/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.3/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      250 2024-03-12 09:04:33.383063 labda-0.0.3/labda/structure/__init__.py
--rw-r--r--   0        0        0      621 2024-03-26 08:50:43.151621 labda-0.0.3/labda/structure/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8409 2024-04-02 13:59:02.487227 labda-0.0.3/labda/structure/__pycache__/collection.cpython-311.pyc
--rw-r--r--   0        0        0     1158 2024-02-09 12:27:22.799138 labda-0.0.3/labda/structure/__pycache__/domains.cpython-311.pyc
--rw-r--r--   0        0        0     1186 2024-02-09 12:27:23.249118 labda-0.0.3/labda/structure/__pycache__/linkage.cpython-311.pyc
--rw-r--r--   0        0        0     6562 2024-04-02 08:49:41.495981 labda-0.0.3/labda/structure/__pycache__/merging.cpython-311.pyc
--rw-r--r--   0        0        0     3595 2024-03-26 08:50:45.881036 labda-0.0.3/labda/structure/__pycache__/resampling.cpython-311.pyc
--rw-r--r--   0        0        0    14577 2024-04-02 13:47:44.916549 labda-0.0.3/labda/structure/__pycache__/subject.cpython-311.pyc
--rw-r--r--   0        0        0     4586 2024-04-02 13:58:21.046661 labda-0.0.3/labda/structure/collection.py
--rw-r--r--   0        0        0      704 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/domains.py
--rw-r--r--   0        0        0      568 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/linkage.py
--rw-r--r--   0        0        0     5000 2024-04-02 08:48:51.335892 labda-0.0.3/labda/structure/merging.py
--rw-r--r--   0        0        0     2771 2024-03-26 07:45:27.282975 labda-0.0.3/labda/structure/resampling.py
--rw-r--r--   0        0        0     9043 2024-04-02 13:46:05.711935 labda-0.0.3/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.3/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0      174 2024-03-26 08:50:43.151621 labda-0.0.3/labda/structure/validation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      912 2024-02-09 12:27:22.809137 labda-0.0.3/labda/structure/validation/__pycache__/domains.cpython-311.pyc
--rw-r--r--   0        0        0      840 2024-02-09 20:01:56.329810 labda-0.0.3/labda/structure/validation/__pycache__/linkage.cpython-311.pyc
--rw-r--r--   0        0        0     8243 2024-04-02 11:44:31.779533 labda-0.0.3/labda/structure/validation/__pycache__/subject.cpython-311.pyc
--rw-r--r--   0        0        0      963 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/validation/domains.py
--rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.3/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0     9704 2024-04-02 11:44:21.091638 labda-0.0.3/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     8338 2024-04-02 08:48:51.335892 labda-0.0.3/labda/utils.py
--rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.3/labda/visualisation/__init__.py
--rw-r--r--   0        0        0      167 2024-04-02 13:25:04.160019 labda-0.0.3/labda/visualisation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3643 2024-04-02 14:25:41.270154 labda-0.0.3/labda/visualisation/__pycache__/spatial.cpython-311.pyc
--rw-r--r--   0        0        0     2510 2024-04-02 14:25:35.290436 labda-0.0.3/labda/visualisation/spatial.py
--rw-r--r--   0        0        0     1434 2024-04-02 14:29:13.641929 labda-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 labda-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      548 2024-02-06 17:52:16.166389 labda-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2024-04-02 08:48:51.335892 labda-0.0.4/README.md
+-rw-r--r--   0        0        0      151 2024-04-02 08:48:51.335892 labda-0.0.4/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.4/labda/assets/__init__.py
+-rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.4/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      459 2024-04-02 11:28:47.324035 labda-0.0.4/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.4/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.4/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.4/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.4/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1140 2024-04-02 08:51:28.536242 labda-0.0.4/labda/logging.py
+-rw-r--r--   0        0        0     1073 2024-04-02 14:15:23.256237 labda-0.0.4/labda/parallel.py
+-rw-r--r--   0        0        0      141 2024-03-05 08:22:02.089665 labda-0.0.4/labda/parsers/__init__.py
+-rw-r--r--   0        0        0     6854 2024-04-02 08:51:54.456305 labda-0.0.4/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0      930 2024-04-02 08:48:51.335892 labda-0.0.4/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6508 2024-04-08 08:01:34.897150 labda-0.0.4/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.4/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10928 2024-04-08 08:01:34.897150 labda-0.0.4/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     1739 2024-04-08 08:01:34.897150 labda-0.0.4/labda/parsers/utils.py
+-rw-r--r--   0        0        0       36 2024-02-09 10:52:49.204568 labda-0.0.4/labda/processing/__init__.py
+-rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.4/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.4/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.4/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.4/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.4/labda/processing/bouts.py
+-rw-r--r--   0        0        0      751 2024-03-26 07:45:27.282975 labda-0.0.4/labda/processing/domains.py
+-rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.4/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.4/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.4/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3277 2024-04-03 14:44:06.593954 labda-0.0.4/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     2311 2024-04-08 11:33:37.546595 labda-0.0.4/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    25472 2024-04-03 14:52:48.450963 labda-0.0.4/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.4/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      250 2024-03-12 09:04:33.383063 labda-0.0.4/labda/structure/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-02 13:58:21.046661 labda-0.0.4/labda/structure/collection.py
+-rw-r--r--   0        0        0      704 2024-04-08 08:01:34.897150 labda-0.0.4/labda/structure/domains.py
+-rw-r--r--   0        0        0      600 2024-04-08 08:01:34.897150 labda-0.0.4/labda/structure/linkage.py
+-rw-r--r--   0        0        0     5000 2024-04-02 08:48:51.335892 labda-0.0.4/labda/structure/merging.py
+-rw-r--r--   0        0        0     2771 2024-03-26 07:45:27.282975 labda-0.0.4/labda/structure/resampling.py
+-rw-r--r--   0        0        0     9046 2024-04-03 09:14:10.108474 labda-0.0.4/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.4/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0      963 2024-02-09 12:27:12.019606 labda-0.0.4/labda/structure/validation/domains.py
+-rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.4/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0     9704 2024-04-02 11:44:21.091638 labda-0.0.4/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     8338 2024-04-02 08:48:51.335892 labda-0.0.4/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.4/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0     3707 2024-04-08 11:46:48.951159 labda-0.0.4/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1434 2024-04-08 11:48:22.697238 labda-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 labda-0.0.4/PKG-INFO
```

### Comparing `labda-0.0.3/CHANGELOG.md` & `labda-0.0.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/README.md` & `labda-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/assets/counts_cut_points.py` & `labda-0.0.4/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/expanders/accelerometer.py` & `labda-0.0.4/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/expanders/extras.py` & `labda-0.0.4/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/expanders/spatial.py` & `labda-0.0.4/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/logging.py` & `labda-0.0.4/labda/logging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/parallel.py` & `labda-0.0.4/labda/parallel.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/parsers/actigraph.py` & `labda-0.0.4/labda/parsers/actigraph.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/parsers/bulk.py` & `labda-0.0.4/labda/parsers/bulk.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/parsers/gadgetbridge.py` & `labda-0.0.4/labda/parsers/gadgetbridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import secrets
 from datetime import datetime
 from pathlib import Path
 
 import pandas as pd
 import pytz
 from sqlalchemy import Engine, MetaData, Table, create_engine, select
 
@@ -108,28 +107,23 @@
         devices.drop(columns=["sensor_id"], inplace=True)
     else:
         devices[Column.SUBJECT_ID] = devices["serial_number"]
 
     return devices
 
 
-def _get_wear_by_hr(df: pd.DataFrame) -> pd.DataFrame:
-    # FIXME: Rework this function.
-    df = df.copy().reset_index(drop=True)
+def _get_wear_by_hr(df: pd.DataFrame, limit: int | None = None) -> pd.DataFrame:
+    df = df.copy()
     df[Column.WEAR] = pd.NA
-    indices = df[Column.HEART_RATE].dropna().index
-    intervals = indices.to_series().diff()
+    df.loc[df[Column.HEART_RATE].notna(), Column.WEAR] = True
 
-    if not intervals.isna().all():
-        interval = int(intervals.mode().iloc[0]) - 1
-        df.loc[df[Column.HEART_RATE].notna(), Column.WEAR] = True
-
-        if not interval == 0:
-            df[Column.WEAR] = df[Column.WEAR].bfill(limit=interval)
-        df.loc[df[Column.WEAR].isna(), Column.WEAR] = False
+    if limit:
+        df[Column.WEAR] = df[Column.WEAR].bfill(limit=limit)
+
+    df.loc[df[Column.WEAR].isna(), Column.WEAR] = False
 
     return df
 
 
 def _get_xiaomi(
     engine: Engine,
     *,
@@ -164,16 +158,16 @@
     # TODO: Add docstring.
     # TODO: Maybe force resampling for making sure that all records have the same frequency.
     records = records.groupby(Column.SUBJECT_ID, as_index=False)  # type: ignore
     objs = []
     for record in records:
         id = record[0]  # type: ignore
         df = record[1]  # type: ignore
-        df = _get_wear_by_hr(df)
         df.set_index(Column.DATETIME, inplace=True)
+        df = _get_wear_by_hr(df, 4)
         df = SCHEMA.validate(df)
 
         sampling_frequency = get_sampling_frequency(df)
 
         device = devices.loc[devices[Column.SUBJECT_ID] == id].iloc[0].to_dict()
         sensor = Sensor(id=device["serial_number"], **device, vendor=Vendor.XIAOMI)
         metadata = Metadata(
```

### Comparing `labda-0.0.3/labda/parsers/garmin.py` & `labda-0.0.4/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/parsers/qstarz.py` & `labda-0.0.4/labda/parsers/qstarz.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,19 @@
     df: pd.DataFrame,
     method: str,
     limit: int | float,
 ) -> pd.DataFrame:
     df = df.copy()
 
     methods = [
-        Column.SNR_VIEWED,  # 260
-        Column.NSAT_RATIO,  # 70
+        Column.SNR_USED,  # 225 (F1: 46,80)
+        Column.SNR_VIEWED,  # 260 (F1: 71,18)
+        Column.NSAT_USED,  # 7 (F1: 48,86)
+        Column.NSAT_VIEWED,  # 9 (F1: 42,93)
+        Column.NSAT_RATIO,  # 70 (F1: 46,40)
     ]
     if method not in methods:
         raise ValueError(f"Method muset be one of {methods}")
 
     if method not in df.columns:
         raise ValueError(f"Column '{method}' does not exist in dataframe")
```

### Comparing `labda-0.0.3/labda/parsers/utils.py` & `labda-0.0.4/labda/parsers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,58 @@
 import pandas as pd
 
 from ..logging import logger
 from ..utils import change_crs, change_timezone, get_crs, get_timezone
 
 DEFAULT_CRS_SENSOR = "EPSG:4326"
 
+# TODO: Maybe those functions should be refactored, i.e. if (None, timezone) -> timezone would be guessed from the data and then changed to the target timezone. Same for CRS.
+
 
 def set_timezone(
     df: pd.DataFrame,
     timezone: str | None | Tuple[str, str] = None,
-) -> Tuple[pd.DataFrame, str]:
-    if isinstance(timezone, tuple) and len(timezone) == 2:
+) -> Tuple[pd.DataFrame, str | None]:
+    if (
+        isinstance(timezone, tuple)
+        and len(timezone) == 2
+        and all(isinstance(tz, str) for tz in timezone)
+    ):
         source_tz = timezone[0]
         target_tz = timezone[1]
         df = change_timezone(df, source_tz, target_tz)
         timezone = target_tz
+    elif isinstance(timezone, str):
+        pass
     elif not timezone:
-        timezone = get_timezone(df)
+        if "latitude" in df.columns and "longitude" in df.columns:
+            timezone = get_timezone(df)
+        else:
+            timezone = None
+    else:
+        raise ValueError(f"Invalid value for timezone: {timezone}")
 
     return df, timezone
 
 
 def set_crs(
     df: pd.DataFrame,
     crs: str | None | Tuple[str, str] = None,
 ) -> Tuple[pd.DataFrame, str]:
-    if isinstance(crs, tuple) and len(crs) == 2:
+    if (
+        isinstance(crs, tuple)
+        and len(crs) == 2
+        and all(isinstance(tz, str) for tz in crs)
+    ):
         source_crs = crs[0]
         target_crs = crs[1]
         df = change_crs(df, source_crs, target_crs)
         crs = target_crs
     elif isinstance(crs, str):
         df = change_crs(df, DEFAULT_CRS_SENSOR, crs)
     elif not crs:
         crs = get_crs(df)
         df = change_crs(df, DEFAULT_CRS_SENSOR, crs)
     else:
-        logger.error(f"Invalid value for crs: {crs}")
+        raise ValueError(f"Invalid value for crs: {crs}")
 
     return df, crs
```

### Comparing `labda-0.0.3/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.4/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/accelerometer/steps.py` & `labda-0.0.4/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/accelerometer/wear.py` & `labda-0.0.4/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/bouts.py` & `labda-0.0.4/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/domains.py` & `labda-0.0.4/labda/processing/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/spatial/manipulations.py` & `labda-0.0.4/labda/processing/spatial/manipulations.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/processing/spatial/timeline.py` & `labda-0.0.4/labda/processing/spatial/timeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         .reset_index(drop=True)
     )
 
     return partial_trip_summaries
 
 
 def get_timeline(df: pd.DataFrame, crs: str) -> pd.DataFrame:
-    # TODO: Add a check for specific trip columns.
+    # TODO: Add a check for specific trip columns (that they are exists, so timeline can be calculated)
+    # TODO: Add indoor/outdoor trip detection, same one as in removal of indoor trips inside trips.py (it should mark whole trip if it was inside or not - maybe?)
     df = df.copy()
 
     trips = (
         df.groupby("trip_id")
         .apply(lambda x: get_transport_information(x, crs=crs))
         .reset_index(drop=True)
     )
```

### Comparing `labda-0.0.3/labda/processing/spatial/transportation.py` & `labda-0.0.4/labda/processing/spatial/transportation.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import pandas as pd
 from pandas.core.groupby import DataFrameGroupBy
 
 from ...expanders.spatial import add_speed
 from ...structure.validation.subject import Column
 from ...utils import columns_exists, columns_not_exists, get_unique_column_name
 
+# TODO: Add something, so even pause has a mode.
+# TODO: Option: pause_mode = True/False, before, after, mixed?
+
 
 def _set_trip_mode(df: pd.DataFrame, name: str):
     modes = df[name].value_counts()
     dominant_mode = modes.idxmax()
     df[name] = dominant_mode
```

### Comparing `labda-0.0.3/labda/processing/spatial/trips.py` & `labda-0.0.4/labda/processing/spatial/trips.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,30 @@
 
     # Unique ID for each stop.
     df["stop_id"] = (df["stop"].diff() != 0).cumsum()
 
     # Set the trip status to 'stationary' if the point is a stop, otherwise 'transport'.
     df["trip_status"] = np.where(df["stop"], "stationary", "transport")
 
-    return df.astype({"stop_id": "UInt16", "trip_status": "category"})
+    # Creating category column and setting the categories.
+    # FIXME: Import categories from Subject SCHEMA.
+    # TODO: Maybe move all the setting of categories to a separate function and as initialisation (start of the detect_trips function).
+    categories = [
+        "start",
+        "end",
+        "start-end",
+        "transport",
+        "pause",
+        "stationary",
+    ]
+    df["trip_status"] = pd.Categorical(
+        df["trip_status"], categories=categories, ordered=False
+    )
+
+    return df.astype({"stop_id": "UInt16"})
 
 
 def get_pauses(
     df: pd.DataFrame,
     *,
     crs: str,
     pause_radius: int | float,
@@ -129,15 +144,14 @@
         id_col (str): The name of the column in df that contains the unique ID for each trip.
         status_col (str): The name of the column in df that contains the trip status.
         extremities (bool): If True, the function will add 'start' and 'end' statuses to the first and last trips, respectively.
 
     Returns:
         None. The function modifies df in-place.
     """
-    df[status_col] = df[status_col].cat.add_categories(["start", "end", "start-end"])
 
     # If 'transport' is at the start or end of the DataFrame, change it to 'start' or 'end' respectively.
     if extremities:
         if df.iloc[0][status_col] == "transport":
             df.iloc[0, df.columns.get_loc(status_col)] = "start"
         if df.iloc[-1][status_col] == "transport":
             df.iloc[-1, df.columns.get_loc(status_col)] = "end"
@@ -223,15 +237,15 @@
         df.groupby("group", as_index=False)
         .apply(lambda x: adjust_group(x, df))
         .reset_index(level=0, drop=True)
     )  # type: ignore
 
     df.drop("group", axis=1, inplace=True)
 
-    return df.astype({"trip_status": "category"})
+    return df
 
 
 def add_ids(
     df: pd.DataFrame, column: str, target_values: list[str], id_column: str
 ) -> None:
     """
     Adds a new column to the DataFrame with unique IDs for each group of consecutive rows that match the target values.
@@ -264,38 +278,40 @@
     Args:
         df (pd.DataFrame): The DataFrame containing the trips.
         min_duration (timedelta): The minimum duration for a trip to be kept in the DataFrame.
 
     Returns:
         None: The function modifies the DataFrame in-place, and does not return anything.
     """
+
     trips = df[
         df["trip_id"].notna()
         & df["trip_status"].isin(["start", "transport", "end", "start-end"])
     ].copy()
 
     # Calculate the duration for each trip.
     trips = trips.groupby(["segment_id", "trip_id"], as_index=False).apply(
         lambda x: x.index.max() - x.index.min()
     )
     trips.rename(columns={None: "duration"}, inplace=True)  # type: ignore
 
     # Select only the trips that are shorter than the minimum duration.
     removed_trips = trips[trips["duration"] < min_duration][["segment_id", "trip_id"]]
 
-    # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
-    mask = df.set_index(["segment_id", "trip_id"]).index.isin(
-        removed_trips.set_index(["segment_id", "trip_id"]).index
-    )
-    df.loc[mask, "trip_id"] = pd.NA
-    # df.loc[mask, "trip_status"] = (
-    #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
-    # )
-    df.loc[mask, "trip_status"] = "stationary"
-    df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
+    if not removed_trips.empty:
+        # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
+        mask = df.set_index(["segment_id", "trip_id"]).index.isin(
+            removed_trips.set_index(["segment_id", "trip_id"]).index
+        )
+        df.loc[mask, "trip_id"] = pd.NA
+        # df.loc[mask, "trip_status"] = (
+        #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
+        # )
+        df.loc[mask, "trip_status"] = "stationary"
+        df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
 
 
 def remove_trips_by_length(df: pd.DataFrame, min_length: int | float, crs: str) -> None:
     """
     Removes trips from a DataFrame based on their length.
 
     Args:
@@ -317,24 +333,25 @@
         lambda x: add_distance(x, crs=crs)["distance"].sum()
     )
     trips.rename(columns={None: "length"}, inplace=True)  # type: ignore
 
     # Select only the trips that are shorter than the minimum length.
     removed_trips = trips[trips["length"] < min_length][["segment_id", "trip_id"]]
 
-    # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
-    mask = df.set_index(["segment_id", "trip_id"]).index.isin(
-        removed_trips.set_index(["segment_id", "trip_id"]).index
-    )
-    df.loc[mask, "trip_id"] = pd.NA
-    # df.loc[mask, "trip_status"] = (
-    #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
-    # )
-    df.loc[mask, "trip_status"] = "stationary"
-    df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
+    if not removed_trips.empty:
+        # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
+        mask = df.set_index(["segment_id", "trip_id"]).index.isin(
+            removed_trips.set_index(["segment_id", "trip_id"]).index
+        )
+        df.loc[mask, "trip_id"] = pd.NA
+        # df.loc[mask, "trip_status"] = (
+        #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
+        # )
+        df.loc[mask, "trip_status"] = "stationary"
+        df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
 
 
 def _change_indoor_trip_to_stationary(df: pd.DataFrame, limit: float) -> str | None:
     environment = df["environment"].value_counts()
     dominant_environment = environment.idxmax()
 
     if len(environment) >= 2 and dominant_environment == "indoor" and limit:
@@ -353,29 +370,33 @@
         df["trip_id"].notna()
         & df["trip_status"].isin(["start", "transport", "end", "start-end"])
     ].copy()
 
     trips = trips.groupby(["segment_id", "trip_id"], as_index=False).apply(
         lambda x: _change_indoor_trip_to_stationary(x, indoor_limit)  # type: ignore
     )
-    trips.rename(columns={None: "environment"}, inplace=True)  # type: ignore
-    trips = trips.astype({"environment": "category"})
-
-    removed_trips = trips[trips["environment"] == "indoor"][["segment_id", "trip_id"]]
 
-    # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
-    mask = df.set_index(["segment_id", "trip_id"]).index.isin(
-        removed_trips.set_index(["segment_id", "trip_id"]).index
-    )
-    df.loc[mask, "trip_id"] = pd.NA
-    # df.loc[mask, "trip_status"] = (
-    #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
-    # )
-    df.loc[mask, "trip_status"] = "stationary"
-    df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].bfill()
+    if not trips.empty:
+        trips.rename(columns={None: "environment"}, inplace=True)  # type: ignore
+        trips = trips.astype({"environment": "category"})
+
+        removed_trips = trips[trips["environment"] == "indoor"][
+            ["segment_id", "trip_id"]
+        ]
+
+        # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
+        mask = df.set_index(["segment_id", "trip_id"]).index.isin(
+            removed_trips.set_index(["segment_id", "trip_id"]).index
+        )
+        df.loc[mask, "trip_id"] = pd.NA
+        # df.loc[mask, "trip_status"] = (
+        #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
+        # )
+        df.loc[mask, "trip_status"] = "stationary"
+        df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].bfill()
 
 
 def get_segment_trips(
     df: pd.DataFrame,
     crs: str,
     sampling_frequency: float,
     stop_radius: int | float,
@@ -505,14 +526,21 @@
         min_distance (int | float | None, optional): The minimum distance between points. Points that are closer than this distance are filtered out. If None, filter is not applied.
         max_speed (int | float | None, optional): The maximum speed. Speed between points that are faster than this speed are filtered out. If None, filter is not applied.
 
     Returns:
         pd.DataFrame: The processed DataFrame with updated 'trip_id' and 'trip_status' columns.
     """
 
+    # TODO: Check sampling frequency against some parameters, e.g. if sampling frequency is 2 minute, we can't have a gap_duration of 1 minute etc. Check what happens if some parameters are the same as sampling frequency.
+    if (not min_duration or min_duration == 0) and (not min_length or min_length == 0):
+        raise ValueError("Both 'min_duration' and 'min_length' cannot be None or zero.")
+
+    if df.empty:
+        raise ValueError("The input DataFrame is empty.")
+
     columns_not_exists(
         df,
         ["segment_id", "trip_id", "trip_status", "stationary_id"],
         overwrite=overwrite,
     )
 
     working_cols = ["latitude", "longitude"]
@@ -557,14 +585,15 @@
         remove_trips_by_duration(temp_df, min_duration=min_duration)
 
     # Remove trips that are too short (length).
     if min_length:
         remove_trips_by_length(temp_df, min_length=min_length, crs=crs)
 
     if "environment" in temp_df.columns and indoor_limit:
+        # TODO: Should be this set outside of the function? And maybe just annotated if the trip is indoor or not, so researchers can exclude indoor trips and say that they are stationary.
         remove_indoor_trips(temp_df, indoor_limit)
 
     temp_df = temp_df[temp_df["trip_status"].notna()]
     trip_mask = temp_df["trip_id"].notna()
     stationary_mask = temp_df["stationary_id"].notna()
 
     # Renumbers the trip IDs to be unique across all segments.
```

### Comparing `labda-0.0.3/labda/processing/wear_validity.py` & `labda-0.0.4/labda/processing/wear_validity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/collection.py` & `labda-0.0.4/labda/structure/collection.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/domains.py` & `labda-0.0.4/labda/structure/domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
         dtype={
             "subject_id": "string",
             "domain": "string",
             "geometry": "string",
         },
         delimiter=";",
         parse_dates=["start", "end"],
-        date_format="%d-%m-%Y %H:%M:%S",
+        date_format="%Y-%m-%d %H:%M:%S",
     )
 
     domains["geometry"] = domains["geometry"].apply(wkt.loads)
 
     return SCHEMA.validate(domains)
```

### Comparing `labda-0.0.3/labda/structure/linkage.py` & `labda-0.0.4/labda/structure/linkage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 
 import pandas as pd
-from shapely import wkt
 
 from .validation.linkage import SCHEMA
 
 
 def from_csv(path: str | Path) -> pd.DataFrame:
     if isinstance(path, str):
         path = Path(path)
@@ -16,13 +15,13 @@
             "subject_id": "string",
             "sensor_id": "string",
         },
         delimiter=";",
     )
 
     if "start" in df.columns:
-        df["start"] = pd.to_datetime(df["start"])
+        df["start"] = pd.to_datetime(df["start"], format="%Y-%m-%d %H:%M:%S")
 
     if "end" in df.columns:
-        df["end"] = pd.to_datetime(df["end"])
+        df["end"] = pd.to_datetime(df["end"], format="%Y-%m-%d %H:%M:%S")
 
     return SCHEMA.validate(df)
```

### Comparing `labda-0.0.3/labda/structure/merging.py` & `labda-0.0.4/labda/structure/merging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/resampling.py` & `labda-0.0.4/labda/structure/resampling.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/subject.py` & `labda-0.0.4/labda/structure/subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     def detect_trips(
         self,
         cut_points: dict[str, Any] | None = None,
         *,
         gap_duration: timedelta,
         stop_radius: int | float,
         stop_duration: timedelta,
-        window: int | None = 3,
+        window: int | None = None,
         pause_radius: int | float | None = None,
         pause_duration: timedelta | None = None,
         min_duration: timedelta | None = None,
         min_length: int | float | None = None,
         min_distance: int | float | None = None,
         max_speed: int | float | None = None,
         indoor_limit: float | None = None,
```

### Comparing `labda-0.0.3/labda/structure/validation/domains.py` & `labda-0.0.4/labda/structure/validation/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/validation/linkage.py` & `labda-0.0.4/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/structure/validation/subject.py` & `labda-0.0.4/labda/structure/validation/subject.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/utils.py` & `labda-0.0.4/labda/utils.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.3/labda/visualisation/spatial.py` & `labda-0.0.4/labda/visualisation/spatial.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,90 +4,124 @@
 import pandas as pd
 import pydeck as pdk
 from shapely.geometry import Point
 
 from ..utils import convert_to_geodataframe
 
 
-def timeline_layer(df: pd.DataFrame, crs: str | None = None) -> Tuple[pdk.Layer, Point]:
+def get_status(row):
+    if row["status"] == "stationary":
+        return f"Stationary {row['stationary_id']}"
+    elif row["status"] == "transport":
+        return f"Trip {row['trip_id']}"
+    elif row["status"] == "pause":
+        return f"Trip {row['trip_id']} (Pause {row['stationary_id']})"
+
+
+def get_color(row):
+    if row["status"] == "stationary":
+        return [255, 0, 0]
+    elif row["status"] == "transport":
+        return [0, 255, 0]
+    elif row["status"] == "pause":
+        return [50, 205, 50]
+
+
+def timeline_layer(
+    df: pd.DataFrame, crs: str | None = None
+) -> Tuple[pdk.Layer, Dict[str, Any], Point]:
     gdf = gpd.GeoDataFrame(df, geometry="geometry", crs=crs)  # type: ignore
     center = gdf.geometry.centroid.to_crs(epsg=4326).unary_union.centroid
 
-    gdf["duration"] = gdf["duration"].dt.total_seconds()
+    gdf["duration"] = gdf["duration"].astype(str)
     gdf["start"] = gdf["start"].dt.strftime("%Y-%m-%d %H:%M:%S")
     gdf["end"] = gdf["end"].dt.strftime("%Y-%m-%d %H:%M:%S")
+    gdf["distance"] = gdf["distance"].round(2)
+    gdf["status_text"] = gdf.apply(get_status, axis=1)
+    gdf["mode"] = gdf["mode"].cat.add_categories(["Stationary"])
+    gdf["mode"] = gdf["mode"].fillna("Stationary")
+    gdf["color"] = gdf.apply(get_color, axis=1)
 
     gdf.to_crs(epsg=4326, inplace=True)
-    gdf = gdf.astype(
-        {
-            "trip_id": "float64",
-            "stationary_id": "float64",
-            "status": "object",
-            "mode": "object",
-        }
-    )  # type: ignore
-
-    geojson = gdf.__geo_interface__  # type: ignore
 
     layer = pdk.Layer(
         "GeoJsonLayer",
-        geojson,
-        stroked=False,
-        filled=True,
+        gdf,
         get_position="geometry.coordinates",
         get_radius=10,  # Radius is in meters
-        get_fill_color=[255, 0, 0],
-        get_line_color=[127, 0, 0],
-        get_line_width=5,
+        get_fill_color="color",
+        get_line_color="color",
+        get_line_width=7.5,
         pickable=True,
         auto_highlight=True,
     )
 
-    return layer, center
+    tooltip = {
+        "html": """<strong>Status:</strong> {status_text}<br/>
+        <strong>Start:</strong> {start}<br/>
+        <strong>End:</strong> {end}<br/>
+        <strong>Duration:</strong> {duration}<br/>
+        <strong>Distance:</strong> {distance}<br/>
+        <strong>Mode:</strong> {mode}<br/>
+        """,
+    }
+
+    return layer, tooltip, center
 
 
 def gps_layer(
     df: pd.DataFrame,
     crs: str | None = None,
-) -> Tuple[pdk.Layer, Point]:
+) -> Tuple[pdk.Layer, Dict[str, Any], Point]:
     gdf = convert_to_geodataframe(df, crs=crs)
     gdf.to_crs(epsg=4326, inplace=True)
     center = gdf.geometry.unary_union.centroid
-    geojson = gdf.__geo_interface__  # type: ignore
+
+    gdf["latitude"] = gdf.geometry.y
+    gdf["longitude"] = gdf.geometry.x
+    gdf.reset_index(inplace=True)
+    gdf["datetime"] = gdf["datetime"].dt.strftime("%Y-%m-%d %H:%M:%S")
+
     layer = pdk.Layer(
         "GeoJsonLayer",
-        geojson,
+        gdf,
         stroked=False,
         filled=True,
         get_position="geometry.coordinates",
-        get_radius=10,  # Radius is in meters
+        get_radius=7.5,  # Radius is in meters
         get_fill_color=[255, 0, 0],
-        get_line_color=[127, 0, 0],
         get_line_width=5,
         pickable=True,
         auto_highlight=True,
     )
 
-    return layer, center
+    tooltip = {
+        "html": """<strong>Datetime:</strong> {datetime}<br/>
+        <strong>Latitude:</strong> {latitude}<br/>
+        <strong>Longitude:</strong> {longitude}<br/>
+        """,
+    }
+
+    return layer, tooltip, center
 
 
 def plot(
     df: pd.DataFrame,
     kind: str,
     *,
     crs: str | None = None,
 ) -> str:
     match kind:
         case "timeline":
-            layer, center = timeline_layer(df, crs)
+            layer, tooltip, center = timeline_layer(df, crs)
         case "gps":
-            layer, center = gps_layer(df, crs)
+            layer, tooltip, center = gps_layer(df, crs)
         case _:
             raise ValueError(f"Kind '{kind}' not supported.")
 
     # Set the viewport location
     view_state = pdk.ViewState(longitude=center.x, latitude=center.y, zoom=10)
 
     # Render
-    r = pdk.Deck(layers=[layer], initial_view_state=view_state)
+    r = pdk.Deck(layers=[layer], initial_view_state=view_state, tooltip=tooltip)  # type: ignore
 
     return r.to_html()  # type: ignore
```

### Comparing `labda-0.0.3/pyproject.toml` & `labda-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.3"
+version = "0.0.4"
 description = "Library for Advanced Behavioural Data Analysis"
 authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
 maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
```

### Comparing `labda-0.0.3/PKG-INFO` & `labda-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labda
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for Advanced Behavioural Data Analysis
 Home-page: https://labda.josefheidler.cz
 License: 	CC-BY-SA-4.0
 Keywords: analysis,health,behaviour,data,spatial,temporal
 Author: Josef Heidler
 Author-email: jheidler@health.sdu.dk
 Maintainer: Josef Heidler
```

